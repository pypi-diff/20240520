# Comparing `tmp/BioSAK-1.88.8.tar.gz` & `tmp/BioSAK-1.88.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BioSAK-1.88.8.tar", last modified: Wed May  8 15:08:14 2024, max compression
+gzip compressed data, was "BioSAK-1.88.9.tar", last modified: Thu May  9 03:17:50 2024, max compression
```

## Comparing `BioSAK-1.88.8.tar` & `BioSAK-1.88.9.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-08 15:08:14.003649 BioSAK-1.88.8/
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-08 15:08:14.001546 BioSAK-1.88.8/BioSAK/
--rw-r--r--   0 songweizhi   (501) staff       (20)     3653 2024-01-16 05:10:59.000000 BioSAK-1.88.8/BioSAK/BLCA_op_parser.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2031 2023-05-31 05:26:00.000000 BioSAK-1.88.8/BioSAK/BioSAK_config.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)    39300 2024-03-22 00:45:31.000000 BioSAK-1.88.8/BioSAK/COG2020.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3615 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/COG_boxplot_last1row.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     6974 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/COG_boxplot_last2row.R
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     6067 2024-01-16 05:00:13.000000 BioSAK-1.88.8/BioSAK/CheckM.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5891 2024-01-16 05:10:59.000000 BioSAK-1.88.8/BioSAK/ConvertMSA.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    16671 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/DnaFeaturesViewer.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2292 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/FastaSplitler_by_num.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2485 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/FastaSplitler_by_size.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2190 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/GTDB_for_BLCA.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1321 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/Gene2Ctg.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    45147 2024-03-23 14:54:03.000000 BioSAK-1.88.8/BioSAK/KEGG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3484 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/KEGG_boxplot_last1row.R
--rw-r--r--   0 songweizhi   (501) staff       (20)      269 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/KEGG_get_eukaryotic_kos.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3077 2023-08-22 09:31:28.000000 BioSAK-1.88.8/BioSAK/KeepRemovingTmp.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2620 2024-01-16 05:10:59.000000 BioSAK-1.88.8/BioSAK/MeanMappingDepth.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3682 2024-01-16 12:39:58.000000 BioSAK-1.88.8/BioSAK/MetaBiosample.py
--rw-r--r--   0 songweizhi   (501) staff       (20)  3297822 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/MetaCHIP_phylo.hmm
--rw-r--r--   0 songweizhi   (501) staff       (20)  1206805 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/MetaCyc_reactions_with_ec.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)    16960 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/NetEnzymes.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3713 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/Newick_tree_plotter.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1659 2024-01-16 05:10:59.000000 BioSAK-1.88.8/BioSAK/OneLineAln.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    10448 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/Prodigal.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6048 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/Reads_simulator.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3573 2024-01-16 05:10:59.000000 BioSAK-1.88.8/BioSAK/RunGraphMB.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3833 2024-01-16 05:10:59.000000 BioSAK-1.88.8/BioSAK/SILVA_for_BLCA.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     6255 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/SankeyTaxon.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5678 2024-01-16 05:10:59.000000 BioSAK-1.88.8/BioSAK/SliceMSA.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3173 2024-01-16 05:10:59.000000 BioSAK-1.88.8/BioSAK/SubsampleLongReads.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     1696 2024-01-16 05:10:59.000000 BioSAK-1.88.8/BioSAK/Tax4Fun2IndOTU.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3700 2024-05-08 15:08:11.000000 BioSAK-1.88.8/BioSAK/VERSION
--rw-r--r--   0 songweizhi   (501) staff       (20)      467 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/VisBlastOp.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     9944 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/VisGeneFlk.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/__init__.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2526 2024-03-25 14:00:14.000000 BioSAK-1.88.8/BioSAK/add_desc.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)    38573 2024-05-08 05:20:42.000000 BioSAK-1.88.8/BioSAK/arCOG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6985 2024-01-16 05:00:13.000000 BioSAK-1.88.8/BioSAK/bam2reads.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     2630 2024-03-22 13:23:45.000000 BioSAK-1.88.8/BioSAK/boxplot.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3312 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/boxplot_last1row.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     6104 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/boxplot_matrix_COG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5403 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/boxplot_matrix_COG_backup.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6984 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/boxplot_matrix_KEGG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5747 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/boxplot_matrix_dbCAN.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1695 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/cat_fa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    13440 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/cdd2cog.pl
--rw-r--r--   0 songweizhi   (501) staff       (20)     1186 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/checkm_marker.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1485 2024-05-02 15:52:56.000000 BioSAK-1.88.8/BioSAK/compare_sets.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1076 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/compare_trees.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     9745 2024-01-16 05:10:59.000000 BioSAK-1.88.8/BioSAK/compare_trees.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      814 2024-05-04 12:52:07.000000 BioSAK-1.88.8/BioSAK/count_num.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6592 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/cross_link_seqs.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    24033 2024-03-22 00:45:31.000000 BioSAK-1.88.8/BioSAK/dbCAN.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1936 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/download_GenBank_genome_subset_prokaryotes_csv.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      767 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/dwnld_sra_reads.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)    14081 2024-05-08 15:08:11.000000 BioSAK-1.88.8/BioSAK/enrich.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      929 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/exe_cmds.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1508 2023-12-05 01:06:39.000000 BioSAK-1.88.8/BioSAK/ezaai2mat.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1396 2023-12-05 01:02:55.000000 BioSAK-1.88.8/BioSAK/fa2id.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1195 2023-05-17 06:14:50.000000 BioSAK-1.88.8/BioSAK/fa2phy.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1363 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/fa2tree.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6280 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/format_converter.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     2861 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/format_leaf_name.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      639 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/fq2fa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3204 2024-04-19 15:04:59.000000 BioSAK-1.88.8/BioSAK/gapseq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2846 2023-06-14 10:08:30.000000 BioSAK-1.88.8/BioSAK/gbk2faa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3342 2023-06-14 10:14:13.000000 BioSAK-1.88.8/BioSAK/gbk2ffn.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2528 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/gbk2fna.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6886 2024-04-29 03:23:48.000000 BioSAK-1.88.8/BioSAK/gbk2gff.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3726 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/gbk_to_ffn_faa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1887 2024-04-15 02:59:40.000000 BioSAK-1.88.8/BioSAK/gc.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      813 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/get_EC_from_ko_stats_D.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7477 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/get_GTDB_taxon_gnm.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5428 2023-06-15 03:03:02.000000 BioSAK-1.88.8/BioSAK/get_MAG_reads_long.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3991 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/get_Pfam_hmms.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    29246 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/get_SCG_tree.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1784 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/get_TopHits_taxonomy.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2247 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/get_aa_composition.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    12066 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/get_bin_abundance copy.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2139 2024-01-23 11:57:14.000000 BioSAK-1.88.8/BioSAK/get_data_matrix.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5523 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/get_gene_depth.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3591 2024-01-16 05:10:59.000000 BioSAK-1.88.8/BioSAK/get_genome_GTDB.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6070 2024-01-16 04:57:23.000000 BioSAK-1.88.8/BioSAK/get_genome_NCBI.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    11209 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/get_genome_NCBI_v1.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    12620 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/get_genome_NCBI_v2.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3048 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/get_gnm_size.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4834 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/get_ko_gene_seqs.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1192 2023-09-21 08:44:42.000000 BioSAK-1.88.8/BioSAK/get_krona_plot.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1559 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/get_reads_from_sam.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      792 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/get_reads_id_in_sam.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2386 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/get_sankey_plot.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     4242 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/get_top_hit.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      820 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/get_total_length.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1834 2024-04-29 04:11:58.000000 BioSAK-1.88.8/BioSAK/gff2chrom.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4643 2023-05-18 01:37:58.000000 BioSAK-1.88.8/BioSAK/global_functions.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     2910 2024-03-11 00:57:02.000000 BioSAK-1.88.8/BioSAK/hpc3.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    26876 2024-05-06 12:18:36.000000 BioSAK-1.88.8/BioSAK/iTOL.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3337 2024-03-07 03:01:35.000000 BioSAK-1.88.8/BioSAK/js_cmds.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3281 2024-04-08 09:48:49.000000 BioSAK-1.88.8/BioSAK/js_hpc3.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1643 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/keep_best_hit.py
--rw-r--r--   0 songweizhi   (501) staff       (20)  3361029 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/ko00001.keg
--rw-r--r--   0 songweizhi   (501) staff       (20)     1848 2024-03-10 15:18:30.000000 BioSAK-1.88.8/BioSAK/koala.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2772 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/label_tree.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     4788 2024-01-16 05:10:59.000000 BioSAK-1.88.8/BioSAK/label_tree.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    35857 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/link_16S_MAG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    12349 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/magabund.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    19855 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/magabund2.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1224 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/manipulator_fasta.py
--rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/manipulator_msa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3659 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/manipulator_newick.py
--rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/manipulator_sam.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      903 2024-04-17 08:12:49.000000 BioSAK-1.88.8/BioSAK/mannwhitneyu.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2433 2023-05-30 01:59:44.000000 BioSAK-1.88.8/BioSAK/mean_MAG_cov.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1880 2024-03-25 06:45:20.000000 BioSAK-1.88.8/BioSAK/merge_df.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2405 2024-01-16 05:10:59.000000 BioSAK-1.88.8/BioSAK/merge_seq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     8826 2024-05-06 06:13:20.000000 BioSAK-1.88.8/BioSAK/metaAssembly.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1327 2023-06-11 13:56:21.000000 BioSAK-1.88.8/BioSAK/metabat2concoct.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1612 2023-06-11 16:00:51.000000 BioSAK-1.88.8/BioSAK/metabat2maxbin.py
--rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/msa_to_distance_matrix.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1759 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/ncbi_dataset.py
--rw-r--r--   0 songweizhi   (501) staff       (20)        0 2024-03-03 11:00:02.000000 BioSAK-1.88.8/BioSAK/odp.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2820 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/parse_MetaCyc_RxnDB.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1460 2023-09-18 14:42:31.000000 BioSAK-1.88.8/BioSAK/parse_mmseqs_tsv.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     8633 2024-01-16 05:10:59.000000 BioSAK-1.88.8/BioSAK/plot_mag.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7332 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/plot_sam_depth.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1638 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/plot_tree.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     2256 2023-07-22 00:36:16.000000 BioSAK-1.88.8/BioSAK/prefix_file.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4221 2024-01-16 05:10:59.000000 BioSAK-1.88.8/BioSAK/prokka.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5057 2023-08-03 02:58:56.000000 BioSAK-1.88.8/BioSAK/reads2bam.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     2534 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/rename_leaves.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2005 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/rename_reads_for_Reago.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6801 2023-10-26 11:55:44.000000 BioSAK-1.88.8/BioSAK/rename_seq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2210 2024-01-16 05:10:59.000000 BioSAK-1.88.8/BioSAK/rename_seqs.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    15703 2024-04-29 07:37:26.000000 BioSAK-1.88.8/BioSAK/ribbon.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1996 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/sam2bam.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6877 2023-05-13 11:01:19.000000 BioSAK-1.88.8/BioSAK/sampling_GTDB_gnms.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3603 2024-01-16 05:10:59.000000 BioSAK-1.88.8/BioSAK/select_seq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3167 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/sep_reads_by_barcode.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2671 2024-01-16 05:10:59.000000 BioSAK-1.88.8/BioSAK/slice_seq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3788 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/split_fasta.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1998 2024-01-16 05:10:59.000000 BioSAK-1.88.8/BioSAK/split_folder.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4561 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/split_sam.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     1204 2024-01-16 05:10:59.000000 BioSAK-1.88.8/BioSAK/submitHPC.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2011 2024-01-16 05:10:59.000000 BioSAK-1.88.8/BioSAK/subset_GTDB_meta.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4585 2024-04-09 03:15:33.000000 BioSAK-1.88.8/BioSAK/subset_df.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7296 2024-01-16 05:10:59.000000 BioSAK-1.88.8/BioSAK/subset_tree.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1912 2024-05-06 05:46:35.000000 BioSAK-1.88.8/BioSAK/tmp_1.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7844 2024-01-16 05:10:59.000000 BioSAK-1.88.8/BioSAK/top_16S_hits.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2106 2023-05-09 01:09:35.000000 BioSAK-1.88.8/BioSAK/top_hits_in_a_group.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      831 2024-04-09 06:05:51.000000 BioSAK-1.88.8/BioSAK/transpose.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2252 2024-01-16 05:10:59.000000 BioSAK-1.88.8/BioSAK/usearch_uc.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      962 2024-04-17 08:12:49.000000 BioSAK-1.88.8/BioSAK/wilcox.py
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-08 15:08:14.003191 BioSAK-1.88.8/BioSAK.egg-info/
--rw-r--r--   0 songweizhi   (501) staff       (20)      508 2024-05-08 15:08:13.000000 BioSAK-1.88.8/BioSAK.egg-info/PKG-INFO
--rw-r--r--   0 songweizhi   (501) staff       (20)     3763 2024-05-08 15:08:13.000000 BioSAK-1.88.8/BioSAK.egg-info/SOURCES.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)        1 2024-05-08 15:08:13.000000 BioSAK-1.88.8/BioSAK.egg-info/dependency_links.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)       95 2024-05-08 15:08:13.000000 BioSAK-1.88.8/BioSAK.egg-info/requires.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)        7 2024-05-08 15:08:13.000000 BioSAK-1.88.8/BioSAK.egg-info/top_level.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)    35141 2023-05-09 01:09:36.000000 BioSAK-1.88.8/LICENSE
--rwxr-xr-x   0 songweizhi   (501) staff       (20)      300 2023-05-09 01:09:36.000000 BioSAK-1.88.8/MANIFEST.in
--rw-r--r--   0 songweizhi   (501) staff       (20)      508 2024-05-08 15:08:14.003439 BioSAK-1.88.8/PKG-INFO
--rw-r--r--   0 songweizhi   (501) staff       (20)     1533 2024-01-23 07:37:01.000000 BioSAK-1.88.8/README.md
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-08 15:08:14.002334 BioSAK-1.88.8/bin/
--rwxr-xr-x   0 songweizhi   (501) staff       (20)    78626 2024-05-08 15:03:16.000000 BioSAK-1.88.8/bin/BioSAK
--rw-r--r--   0 songweizhi   (501) staff       (20)       38 2024-05-08 15:08:14.003689 BioSAK-1.88.8/setup.cfg
--rw-r--r--   0 songweizhi   (501) staff       (20)      915 2024-01-15 11:41:11.000000 BioSAK-1.88.8/setup.py
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-09 03:17:50.961209 BioSAK-1.88.9/
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-09 03:17:50.958698 BioSAK-1.88.9/BioSAK/
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3653 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/BLCA_op_parser.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2031 2023-05-31 05:26:00.000000 BioSAK-1.88.9/BioSAK/BioSAK_config.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)    39300 2024-03-22 00:45:31.000000 BioSAK-1.88.9/BioSAK/COG2020.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3615 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/COG_boxplot_last1row.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6974 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/COG_boxplot_last2row.R
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     6067 2024-01-16 05:00:13.000000 BioSAK-1.88.9/BioSAK/CheckM.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5891 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/ConvertMSA.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    16671 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/DnaFeaturesViewer.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2292 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/FastaSplitler_by_num.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2485 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/FastaSplitler_by_size.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2190 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/GTDB_for_BLCA.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1321 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/Gene2Ctg.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    45147 2024-03-23 14:54:03.000000 BioSAK-1.88.9/BioSAK/KEGG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3484 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/KEGG_boxplot_last1row.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)      269 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/KEGG_get_eukaryotic_kos.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3077 2023-08-22 09:31:28.000000 BioSAK-1.88.9/BioSAK/KeepRemovingTmp.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2620 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/MeanMappingDepth.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3682 2024-01-16 12:39:58.000000 BioSAK-1.88.9/BioSAK/MetaBiosample.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)  3297822 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/MetaCHIP_phylo.hmm
+-rw-r--r--   0 songweizhi   (501) staff       (20)  1206805 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/MetaCyc_reactions_with_ec.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)    16960 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/NetEnzymes.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3713 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/Newick_tree_plotter.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1659 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/OneLineAln.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    10448 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/Prodigal.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6048 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/Reads_simulator.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3573 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/RunGraphMB.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3833 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/SILVA_for_BLCA.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     6255 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/SankeyTaxon.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5678 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/SliceMSA.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3173 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/SubsampleLongReads.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     1696 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/Tax4Fun2IndOTU.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3700 2024-05-09 03:17:49.000000 BioSAK-1.88.9/BioSAK/VERSION
+-rw-r--r--   0 songweizhi   (501) staff       (20)      467 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/VisBlastOp.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     9944 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/VisGeneFlk.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/__init__.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2526 2024-03-25 14:00:14.000000 BioSAK-1.88.9/BioSAK/add_desc.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)    38573 2024-05-08 05:20:42.000000 BioSAK-1.88.9/BioSAK/arCOG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6985 2024-01-16 05:00:13.000000 BioSAK-1.88.9/BioSAK/bam2reads.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     2630 2024-03-22 13:23:45.000000 BioSAK-1.88.9/BioSAK/boxplot.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3312 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/boxplot_last1row.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6104 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/boxplot_matrix_COG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5403 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/boxplot_matrix_COG_backup.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6984 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/boxplot_matrix_KEGG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5747 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/boxplot_matrix_dbCAN.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1695 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/cat_fa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    13440 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/cdd2cog.pl
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1186 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/checkm_marker.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1485 2024-05-02 15:52:56.000000 BioSAK-1.88.9/BioSAK/compare_sets.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1076 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/compare_trees.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     9745 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/compare_trees.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      814 2024-05-04 12:52:07.000000 BioSAK-1.88.9/BioSAK/count_num.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6592 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/cross_link_seqs.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    24033 2024-03-22 00:45:31.000000 BioSAK-1.88.9/BioSAK/dbCAN.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1936 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/download_GenBank_genome_subset_prokaryotes_csv.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      767 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/dwnld_sra_reads.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)    14152 2024-05-08 15:09:54.000000 BioSAK-1.88.9/BioSAK/enrich.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      929 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/exe_cmds.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1508 2023-12-05 01:06:39.000000 BioSAK-1.88.9/BioSAK/ezaai2mat.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1396 2023-12-05 01:02:55.000000 BioSAK-1.88.9/BioSAK/fa2id.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1195 2023-05-17 06:14:50.000000 BioSAK-1.88.9/BioSAK/fa2phy.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1363 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/fa2tree.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6280 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/format_converter.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     2861 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/format_leaf_name.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      639 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/fq2fa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4404 2024-05-09 03:17:49.000000 BioSAK-1.88.9/BioSAK/gapseq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2846 2023-06-14 10:08:30.000000 BioSAK-1.88.9/BioSAK/gbk2faa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3342 2023-06-14 10:14:13.000000 BioSAK-1.88.9/BioSAK/gbk2ffn.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2528 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/gbk2fna.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6886 2024-04-29 03:23:48.000000 BioSAK-1.88.9/BioSAK/gbk2gff.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3726 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/gbk_to_ffn_faa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1887 2024-04-15 02:59:40.000000 BioSAK-1.88.9/BioSAK/gc.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      813 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_EC_from_ko_stats_D.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7477 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_GTDB_taxon_gnm.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5428 2023-06-15 03:03:02.000000 BioSAK-1.88.9/BioSAK/get_MAG_reads_long.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3991 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_Pfam_hmms.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    29246 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_SCG_tree.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1784 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_TopHits_taxonomy.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2247 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_aa_composition.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    12066 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_bin_abundance copy.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2139 2024-01-23 11:57:14.000000 BioSAK-1.88.9/BioSAK/get_data_matrix.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5523 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_gene_depth.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3591 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/get_genome_GTDB.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6070 2024-01-16 04:57:23.000000 BioSAK-1.88.9/BioSAK/get_genome_NCBI.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    11209 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_genome_NCBI_v1.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    12620 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_genome_NCBI_v2.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3048 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_gnm_size.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4834 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_ko_gene_seqs.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1192 2023-09-21 08:44:42.000000 BioSAK-1.88.9/BioSAK/get_krona_plot.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1559 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_reads_from_sam.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      792 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_reads_id_in_sam.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2386 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_sankey_plot.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4242 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_top_hit.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      820 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/get_total_length.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1834 2024-04-29 04:11:58.000000 BioSAK-1.88.9/BioSAK/gff2chrom.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4643 2023-05-18 01:37:58.000000 BioSAK-1.88.9/BioSAK/global_functions.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     2910 2024-03-11 00:57:02.000000 BioSAK-1.88.9/BioSAK/hpc3.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    26876 2024-05-06 12:18:36.000000 BioSAK-1.88.9/BioSAK/iTOL.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3337 2024-03-07 03:01:35.000000 BioSAK-1.88.9/BioSAK/js_cmds.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3281 2024-04-08 09:48:49.000000 BioSAK-1.88.9/BioSAK/js_hpc3.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1643 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/keep_best_hit.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)  3361029 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/ko00001.keg
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1848 2024-03-10 15:18:30.000000 BioSAK-1.88.9/BioSAK/koala.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2772 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/label_tree.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4788 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/label_tree.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    35857 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/link_16S_MAG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    12349 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/magabund.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    19855 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/magabund2.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1224 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/manipulator_fasta.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/manipulator_msa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3659 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/manipulator_newick.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/manipulator_sam.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      903 2024-04-17 08:12:49.000000 BioSAK-1.88.9/BioSAK/mannwhitneyu.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2433 2023-05-30 01:59:44.000000 BioSAK-1.88.9/BioSAK/mean_MAG_cov.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1880 2024-03-25 06:45:20.000000 BioSAK-1.88.9/BioSAK/merge_df.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2405 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/merge_seq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     8826 2024-05-06 06:13:20.000000 BioSAK-1.88.9/BioSAK/metaAssembly.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1327 2023-06-11 13:56:21.000000 BioSAK-1.88.9/BioSAK/metabat2concoct.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1612 2023-06-11 16:00:51.000000 BioSAK-1.88.9/BioSAK/metabat2maxbin.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/msa_to_distance_matrix.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1759 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/ncbi_dataset.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)        0 2024-03-03 11:00:02.000000 BioSAK-1.88.9/BioSAK/odp.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2820 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/parse_MetaCyc_RxnDB.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1460 2023-09-18 14:42:31.000000 BioSAK-1.88.9/BioSAK/parse_mmseqs_tsv.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     8633 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/plot_mag.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7332 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/plot_sam_depth.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1638 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/plot_tree.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2256 2023-07-22 00:36:16.000000 BioSAK-1.88.9/BioSAK/prefix_file.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4221 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/prokka.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5057 2023-08-03 02:58:56.000000 BioSAK-1.88.9/BioSAK/reads2bam.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     2534 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/rename_leaves.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2005 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/rename_reads_for_Reago.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6801 2023-10-26 11:55:44.000000 BioSAK-1.88.9/BioSAK/rename_seq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2210 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/rename_seqs.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    15703 2024-04-29 07:37:26.000000 BioSAK-1.88.9/BioSAK/ribbon.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1996 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/sam2bam.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6877 2023-05-13 11:01:19.000000 BioSAK-1.88.9/BioSAK/sampling_GTDB_gnms.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3603 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/select_seq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3167 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/sep_reads_by_barcode.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2671 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/slice_seq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3788 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/split_fasta.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1998 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/split_folder.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4561 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/split_sam.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     1204 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/submitHPC.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2011 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/subset_GTDB_meta.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4585 2024-04-09 03:15:33.000000 BioSAK-1.88.9/BioSAK/subset_df.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7296 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/subset_tree.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1912 2024-05-06 05:46:35.000000 BioSAK-1.88.9/BioSAK/tmp_1.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7844 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/top_16S_hits.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2106 2023-05-09 01:09:35.000000 BioSAK-1.88.9/BioSAK/top_hits_in_a_group.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      831 2024-04-09 06:05:51.000000 BioSAK-1.88.9/BioSAK/transpose.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2252 2024-01-16 05:10:59.000000 BioSAK-1.88.9/BioSAK/usearch_uc.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      962 2024-04-17 08:12:49.000000 BioSAK-1.88.9/BioSAK/wilcox.py
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-09 03:17:50.960678 BioSAK-1.88.9/BioSAK.egg-info/
+-rw-r--r--   0 songweizhi   (501) staff       (20)      508 2024-05-09 03:17:50.000000 BioSAK-1.88.9/BioSAK.egg-info/PKG-INFO
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3763 2024-05-09 03:17:50.000000 BioSAK-1.88.9/BioSAK.egg-info/SOURCES.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)        1 2024-05-09 03:17:50.000000 BioSAK-1.88.9/BioSAK.egg-info/dependency_links.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)       95 2024-05-09 03:17:50.000000 BioSAK-1.88.9/BioSAK.egg-info/requires.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)        7 2024-05-09 03:17:50.000000 BioSAK-1.88.9/BioSAK.egg-info/top_level.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)    35141 2023-05-09 01:09:36.000000 BioSAK-1.88.9/LICENSE
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)      300 2023-05-09 01:09:36.000000 BioSAK-1.88.9/MANIFEST.in
+-rw-r--r--   0 songweizhi   (501) staff       (20)      508 2024-05-09 03:17:50.960985 BioSAK-1.88.9/PKG-INFO
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1533 2024-01-23 07:37:01.000000 BioSAK-1.88.9/README.md
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-09 03:17:50.959668 BioSAK-1.88.9/bin/
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)    78626 2024-05-08 15:03:16.000000 BioSAK-1.88.9/bin/BioSAK
+-rw-r--r--   0 songweizhi   (501) staff       (20)       38 2024-05-09 03:17:50.961255 BioSAK-1.88.9/setup.cfg
+-rw-r--r--   0 songweizhi   (501) staff       (20)      915 2024-01-15 11:41:11.000000 BioSAK-1.88.9/setup.py
```

### Comparing `BioSAK-1.88.8/BioSAK/BLCA_op_parser.py` & `BioSAK-1.88.9/BioSAK/BLCA_op_parser.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/BioSAK_config.py` & `BioSAK-1.88.9/BioSAK/BioSAK_config.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/COG2020.py` & `BioSAK-1.88.9/BioSAK/COG2020.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/COG_boxplot_last1row.R` & `BioSAK-1.88.9/BioSAK/COG_boxplot_last1row.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/COG_boxplot_last2row.R` & `BioSAK-1.88.9/BioSAK/COG_boxplot_last2row.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/CheckM.py` & `BioSAK-1.88.9/BioSAK/CheckM.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/ConvertMSA.py` & `BioSAK-1.88.9/BioSAK/ConvertMSA.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/DnaFeaturesViewer.py` & `BioSAK-1.88.9/BioSAK/DnaFeaturesViewer.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/FastaSplitler_by_num.py` & `BioSAK-1.88.9/BioSAK/FastaSplitler_by_num.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/FastaSplitler_by_size.py` & `BioSAK-1.88.9/BioSAK/FastaSplitler_by_size.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/GTDB_for_BLCA.py` & `BioSAK-1.88.9/BioSAK/GTDB_for_BLCA.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/Gene2Ctg.py` & `BioSAK-1.88.9/BioSAK/Gene2Ctg.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/KEGG.py` & `BioSAK-1.88.9/BioSAK/KEGG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/KEGG_boxplot_last1row.R` & `BioSAK-1.88.9/BioSAK/KEGG_boxplot_last1row.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/KeepRemovingTmp.py` & `BioSAK-1.88.9/BioSAK/KeepRemovingTmp.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/MeanMappingDepth.py` & `BioSAK-1.88.9/BioSAK/MeanMappingDepth.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/MetaBiosample.py` & `BioSAK-1.88.9/BioSAK/MetaBiosample.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/MetaCHIP_phylo.hmm` & `BioSAK-1.88.9/BioSAK/MetaCHIP_phylo.hmm`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/MetaCyc_reactions_with_ec.txt` & `BioSAK-1.88.9/BioSAK/MetaCyc_reactions_with_ec.txt`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/NetEnzymes.py` & `BioSAK-1.88.9/BioSAK/NetEnzymes.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/Newick_tree_plotter.py` & `BioSAK-1.88.9/BioSAK/Newick_tree_plotter.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/OneLineAln.py` & `BioSAK-1.88.9/BioSAK/OneLineAln.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/Prodigal.py` & `BioSAK-1.88.9/BioSAK/Prodigal.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/Reads_simulator.py` & `BioSAK-1.88.9/BioSAK/Reads_simulator.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/RunGraphMB.py` & `BioSAK-1.88.9/BioSAK/RunGraphMB.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/SILVA_for_BLCA.py` & `BioSAK-1.88.9/BioSAK/SILVA_for_BLCA.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/SankeyTaxon.py` & `BioSAK-1.88.9/BioSAK/SankeyTaxon.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/SliceMSA.py` & `BioSAK-1.88.9/BioSAK/SliceMSA.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/SubsampleLongReads.py` & `BioSAK-1.88.9/BioSAK/SubsampleLongReads.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/Tax4Fun2IndOTU.py` & `BioSAK-1.88.9/BioSAK/Tax4Fun2IndOTU.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/VERSION` & `BioSAK-1.88.9/BioSAK/VERSION`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-1.88.8
+1.88.9
 - fixed bugs
 
 1.88.0
 - new modules added: count_num
 
 1.87.0
 - new modules added: compare_sets
```

### Comparing `BioSAK-1.88.8/BioSAK/VisGeneFlk.py` & `BioSAK-1.88.9/BioSAK/VisGeneFlk.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/add_desc.py` & `BioSAK-1.88.9/BioSAK/add_desc.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/arCOG.py` & `BioSAK-1.88.9/BioSAK/arCOG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/bam2reads.py` & `BioSAK-1.88.9/BioSAK/bam2reads.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/boxplot.py` & `BioSAK-1.88.9/BioSAK/boxplot.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/boxplot_last1row.R` & `BioSAK-1.88.9/BioSAK/boxplot_last1row.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/boxplot_matrix_COG.py` & `BioSAK-1.88.9/BioSAK/boxplot_matrix_COG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/boxplot_matrix_COG_backup.py` & `BioSAK-1.88.9/BioSAK/boxplot_matrix_COG_backup.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/boxplot_matrix_KEGG.py` & `BioSAK-1.88.9/BioSAK/boxplot_matrix_KEGG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/boxplot_matrix_dbCAN.py` & `BioSAK-1.88.9/BioSAK/boxplot_matrix_dbCAN.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/cat_fa.py` & `BioSAK-1.88.9/BioSAK/cat_fa.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/cdd2cog.pl` & `BioSAK-1.88.9/BioSAK/cdd2cog.pl`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/checkm_marker.py` & `BioSAK-1.88.9/BioSAK/checkm_marker.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/compare_sets.py` & `BioSAK-1.88.9/BioSAK/compare_sets.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/compare_trees.R` & `BioSAK-1.88.9/BioSAK/compare_trees.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/compare_trees.py` & `BioSAK-1.88.9/BioSAK/compare_trees.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/count_num.py` & `BioSAK-1.88.9/BioSAK/count_num.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/cross_link_seqs.py` & `BioSAK-1.88.9/BioSAK/cross_link_seqs.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/dbCAN.py` & `BioSAK-1.88.9/BioSAK/dbCAN.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/download_GenBank_genome_subset_prokaryotes_csv.py` & `BioSAK-1.88.9/BioSAK/download_GenBank_genome_subset_prokaryotes_csv.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/dwnld_sra_reads.py` & `BioSAK-1.88.9/BioSAK/dwnld_sra_reads.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/enrich.py` & `BioSAK-1.88.9/BioSAK/enrich.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from scipy import stats
 from statsmodels.stats.multitest import multipletests
 
 
 enrich_usage = '''
 =================================== enrich example commands ===================================
 
+BioSAK enrich -i annotation_files -x txt -g grouping.txt -o output_dir
 BioSAK enrich -i annotation_files -x txt -g grouping.txt -o output_dir -bc
 
 # Note:
 1. The number of genome groups has to be TWO!!!
 2. Group name should NOT be 1 and 0. use some alphabet or words instead.
 
 # Example input files:
```

### Comparing `BioSAK-1.88.8/BioSAK/exe_cmds.py` & `BioSAK-1.88.9/BioSAK/exe_cmds.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/ezaai2mat.py` & `BioSAK-1.88.9/BioSAK/ezaai2mat.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/fa2id.py` & `BioSAK-1.88.9/BioSAK/fa2id.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/fa2phy.py` & `BioSAK-1.88.9/BioSAK/fa2phy.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/fa2tree.py` & `BioSAK-1.88.9/BioSAK/fa2tree.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/format_converter.py` & `BioSAK-1.88.9/BioSAK/format_converter.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/format_leaf_name.py` & `BioSAK-1.88.9/BioSAK/format_leaf_name.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/fq2fa.py` & `BioSAK-1.88.9/BioSAK/fq2fa.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/gapseq.py` & `BioSAK-1.88.9/BioSAK/js_cmds.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,90 +1,93 @@
 import os
-import glob
 import argparse
 
 
-gapseq_usage = '''
-============ gapseq example commands ============
+js_cmds_usage = '''
+====================== js_cmds example commands ======================
 
-BioSAK gapseq -i gapseq_op_dir -o df.txt
-BioSAK gapseq -i gapseq_op_dir -o df.txt -name
+BioSAK js_cmds -p Demo -cmd cmds.txt -hd js_header.txt -n 3 -force
 
-=================================================
+======================================================================
 '''
 
 
-def sep_path_basename_ext(file_in):
+def js_cmds(args):
 
-    f_path, file_name = os.path.split(file_in)
-    if f_path == '':
-        f_path = '.'
-    f_base, f_ext = os.path.splitext(file_name)
-    return f_path, f_base, f_ext
-
-
-def gapseq(args):
-
-    dir_in       = args['i']
-    df_out       = args['o']
-    include_desc = args['name']
-
-    file_re   = '%s/*-Pathways.tbl' % dir_in
-    file_list = glob.glob(file_re)
-
-    # read in annotation results
-    gnm_id_set = set()
-    detected_pwy_set = set()
-    pwy_to_gnm_dict = dict()
-    pwy_id_to_name_dict = dict()
-    annotation_results_dict = dict()
-    for each_file in sorted(file_list):
-        _, f_base, _ = sep_path_basename_ext(each_file)
-        gnm_id = '-'.join(f_base.split('-')[:-2])
-        gnm_id_set.add(gnm_id)
-        encoded_pwy_set = set()
-        for each_line in open(each_file):
-            if not each_line.startswith('#'):
-                if not each_line.startswith('ID\tName'):
-                    each_line_split = each_line.strip().split('\t')
-                    pwy_id = each_line_split[0]
-                    if (pwy_id[0] == '|') and (pwy_id[-1] == '|'):
-                        pwy_id = pwy_id[1:-1]
-                    pwy_name = each_line_split[1]
-                    pwy_id_to_name_dict[pwy_id] = pwy_name
-                    pa = each_line_split[2]
-                    if pa == 'true':
-                        detected_pwy_set.add(pwy_id)
-                        encoded_pwy_set.add(pwy_id)
-                        if pwy_id not in pwy_to_gnm_dict:
-                            pwy_to_gnm_dict[pwy_id] = set()
-                        pwy_to_gnm_dict[pwy_id].add(gnm_id)
-        annotation_results_dict[gnm_id] = encoded_pwy_set
-
-    pwy_id_list_sorted = sorted(list(detected_pwy_set))
-    pwy_id_list_sorted_desc = [('%s__%s' % (i, pwy_id_to_name_dict[i])) for i in pwy_id_list_sorted]
-
-    df_out_handle = open(df_out, 'w')
-    if include_desc is False:
-        df_out_handle.write('\t' + '\t'.join(pwy_id_list_sorted) + '\n')
+    js_prefix       = args['p']
+    cmd_file        = args['cmd']
+    js_header_file  = args['hd']
+    cmd_num_per_js  = args['n']
+    auto_submit     = args['auto']
+    js_folder_hpc   = args['js_hpc']
+    force_overwrite = args['force']
+    use_sbatch      = args['sbatch']
+
+    pwd_js_folder       = '%s/%s_js' % (os.getcwd(), js_prefix)
+
+    if js_folder_hpc is None:
+        js_folder_hpc = pwd_js_folder
+
+
+    if (os.path.isdir(pwd_js_folder) is True) and (force_overwrite is False):
+        print('Output folder detected, program exited: %s' % pwd_js_folder)
+        exit()
     else:
-        df_out_handle.write('\t' + '\t'.join(pwy_id_list_sorted_desc) + '\n')
-    for each_gnm in sorted(list(gnm_id_set)):
-        encoded_pwys = annotation_results_dict[each_gnm]
-        value_list = [each_gnm]
-        for each_pwy in pwy_id_list_sorted:
-            if each_pwy in encoded_pwys:
-                value_list.append('1')
-            else:
-                value_list.append('0')
-        df_out_handle.write('\t'.join(value_list) + '\n')
-    df_out_handle.close()
+        if os.path.isdir(pwd_js_folder) is True:
+            os.system('rm -r %s' % pwd_js_folder)
+            os.mkdir(pwd_js_folder)
+        else:
+            os.mkdir(pwd_js_folder)
+
+    # read in js header
+    js_header_str = ''
+    for each_line in open(js_header_file):
+        js_header_str += each_line
+
+    js_index = 1
+    n = 1
+    for each_cmd in open(cmd_file):
+
+        pwd_js_previous = '%s/%s_%s.sh' % (pwd_js_folder, js_prefix, (js_index - 1))
+        pwd_js          = '%s/%s_%s.sh' % (pwd_js_folder, js_prefix, js_index)
+        pwd_js_hpc      = '%s/%s_%s.sh' % (js_folder_hpc, js_prefix, js_index)
+
+        if os.path.isfile(pwd_js) is False:
+
+            if js_index > 1:
+
+                if auto_submit is True:
+                    pwd_js_previous_handle = open(pwd_js_previous, 'a')
+                    if use_sbatch is True:
+                        pwd_js_previous_handle.write('sbatch %s\n' % pwd_js_hpc)
+                    else:
+                        pwd_js_previous_handle.write('qsub %s\n' % pwd_js_hpc)
+                    pwd_js_previous_handle.close()
+
+            pwd_js_handle = open(pwd_js, 'w')
+            pwd_js_handle.write(js_header_str)
+            pwd_js_handle.write('\n')
+            pwd_js_handle.write(each_cmd)
+            pwd_js_handle.close()
+        else:
+            pwd_js_handle = open(pwd_js, 'a')
+            pwd_js_handle.write(each_cmd)
+            pwd_js_handle.close()
+
+        if n % cmd_num_per_js == 0:
+            js_index += 1
+        n += 1
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
 
     parser = argparse.ArgumentParser()
-    parser.add_argument('-i',       required=True,                        help='folder holds the *Pathways.tbl files')
-    parser.add_argument('-o',       required=True,                        help='output file')
-    parser.add_argument('-name',    required=False, action="store_true",  help='include pathway name in the output dataframe')
+    parser.add_argument('-p',      required=True,                       help='js prefix')
+    parser.add_argument('-cmd',    required=True,                       help='cmds file')
+    parser.add_argument('-hd',     required=True,                       help='js header')
+    parser.add_argument('-n',      required=True, type=int,             help='number of cmds per job script')
+    parser.add_argument('-auto',   required=False, action="store_true", help='automatically submit next job script')
+    parser.add_argument('-sbatch', required=False, action="store_true", help='use sbatch, instead of qsub')
+    parser.add_argument('-js_hpc', required=False, default=None,        help='Full path to js folder on HPC')
+    parser.add_argument('-force',  required=False, action="store_true", help='force overwrite existing results')
     args = vars(parser.parse_args())
-    gapseq(args)
+    js_cmds(args)
```

### Comparing `BioSAK-1.88.8/BioSAK/gbk2faa.py` & `BioSAK-1.88.9/BioSAK/gbk2faa.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/gbk2ffn.py` & `BioSAK-1.88.9/BioSAK/gbk2ffn.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/gbk2fna.py` & `BioSAK-1.88.9/BioSAK/gbk2fna.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/gbk2gff.py` & `BioSAK-1.88.9/BioSAK/gbk2gff.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/gbk_to_ffn_faa.py` & `BioSAK-1.88.9/BioSAK/gbk_to_ffn_faa.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/gc.py` & `BioSAK-1.88.9/BioSAK/gc.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/get_EC_from_ko_stats_D.py` & `BioSAK-1.88.9/BioSAK/get_EC_from_ko_stats_D.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/get_GTDB_taxon_gnm.py` & `BioSAK-1.88.9/BioSAK/get_GTDB_taxon_gnm.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/get_MAG_reads_long.py` & `BioSAK-1.88.9/BioSAK/get_MAG_reads_long.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/get_Pfam_hmms.py` & `BioSAK-1.88.9/BioSAK/get_Pfam_hmms.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/get_SCG_tree.py` & `BioSAK-1.88.9/BioSAK/get_SCG_tree.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/get_TopHits_taxonomy.py` & `BioSAK-1.88.9/BioSAK/get_TopHits_taxonomy.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/get_aa_composition.py` & `BioSAK-1.88.9/BioSAK/get_aa_composition.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/get_bin_abundance copy.py` & `BioSAK-1.88.9/BioSAK/get_bin_abundance copy.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/get_data_matrix.py` & `BioSAK-1.88.9/BioSAK/get_data_matrix.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/get_gene_depth.py` & `BioSAK-1.88.9/BioSAK/get_gene_depth.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/get_genome_GTDB.py` & `BioSAK-1.88.9/BioSAK/get_genome_GTDB.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/get_genome_NCBI.py` & `BioSAK-1.88.9/BioSAK/get_genome_NCBI.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/get_genome_NCBI_v1.py` & `BioSAK-1.88.9/BioSAK/get_genome_NCBI_v1.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/get_genome_NCBI_v2.py` & `BioSAK-1.88.9/BioSAK/get_genome_NCBI_v2.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/get_gnm_size.py` & `BioSAK-1.88.9/BioSAK/get_gnm_size.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/get_ko_gene_seqs.py` & `BioSAK-1.88.9/BioSAK/get_ko_gene_seqs.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/get_krona_plot.py` & `BioSAK-1.88.9/BioSAK/get_krona_plot.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/get_reads_from_sam.py` & `BioSAK-1.88.9/BioSAK/get_reads_from_sam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/get_reads_id_in_sam.py` & `BioSAK-1.88.9/BioSAK/get_reads_id_in_sam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/get_sankey_plot.R` & `BioSAK-1.88.9/BioSAK/get_sankey_plot.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/get_top_hit.py` & `BioSAK-1.88.9/BioSAK/get_top_hit.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/get_total_length.py` & `BioSAK-1.88.9/BioSAK/get_total_length.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/gff2chrom.py` & `BioSAK-1.88.9/BioSAK/gff2chrom.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/global_functions.py` & `BioSAK-1.88.9/BioSAK/global_functions.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/hpc3.py` & `BioSAK-1.88.9/BioSAK/hpc3.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/iTOL.py` & `BioSAK-1.88.9/BioSAK/iTOL.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/js_cmds.py` & `BioSAK-1.88.9/BioSAK/js_hpc3.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 import os
+import math
 import argparse
 
 
-js_cmds_usage = '''
-====================== js_cmds example commands ======================
+js_hpc3_usage = '''
+==================== js_hpc3 example commands ====================
 
-BioSAK js_cmds -p Demo -cmd cmds.txt -hd js_header.txt -n 3 -force
+BioSAK js_hpc3 -p Demo -c cmds.txt -hd js_header.sh -n 3 -force
 
-======================================================================
+==================================================================
 '''
 
 
-def js_cmds(args):
+def js_hpc3(args):
 
     js_prefix       = args['p']
-    cmd_file        = args['cmd']
+    cmd_file        = args['c']
     js_header_file  = args['hd']
     cmd_num_per_js  = args['n']
-    auto_submit     = args['auto']
-    js_folder_hpc   = args['js_hpc']
-    force_overwrite = args['force']
-    use_sbatch      = args['sbatch']
-
-    pwd_js_folder       = '%s/%s_js' % (os.getcwd(), js_prefix)
-
-    if js_folder_hpc is None:
-        js_folder_hpc = pwd_js_folder
+    force_overwrite = args['f']
+    cmd_t           = args['t']
 
+    pwd_js_folder = '%s_job_scripts' % js_prefix
 
     if (os.path.isdir(pwd_js_folder) is True) and (force_overwrite is False):
         print('Output folder detected, program exited: %s' % pwd_js_folder)
         exit()
     else:
         if os.path.isdir(pwd_js_folder) is True:
             os.system('rm -r %s' % pwd_js_folder)
@@ -39,55 +34,53 @@
             os.mkdir(pwd_js_folder)
 
     # read in js header
     js_header_str = ''
     for each_line in open(js_header_file):
         js_header_str += each_line
 
-    js_index = 1
-    n = 1
+    # get the total number of commands
+    cmd_num = 0
     for each_cmd in open(cmd_file):
+        if len(each_cmd.strip()) > 0:
+            cmd_num += 1
 
-        pwd_js_previous = '%s/%s_%s.sh' % (pwd_js_folder, js_prefix, (js_index - 1))
-        pwd_js          = '%s/%s_%s.sh' % (pwd_js_folder, js_prefix, js_index)
-        pwd_js_hpc      = '%s/%s_%s.sh' % (js_folder_hpc, js_prefix, js_index)
-
-        if os.path.isfile(pwd_js) is False:
-
-            if js_index > 1:
-
-                if auto_submit is True:
-                    pwd_js_previous_handle = open(pwd_js_previous, 'a')
-                    if use_sbatch is True:
-                        pwd_js_previous_handle.write('sbatch %s\n' % pwd_js_hpc)
+    n = 1
+    for each_cmd in open(cmd_file):
+        if len(each_cmd.strip()) > 0:
+            js_index = math.ceil((n-1)//cmd_num_per_js) + 1
+            pwd_js = '%s/%s_%s.sh' % (pwd_js_folder, js_prefix, js_index)
+            if os.path.isfile(pwd_js) is False:
+                pwd_js_handle = open(pwd_js, 'w')
+                pwd_js_handle.write(js_header_str)
+                pwd_js_handle.write('\n')
+                if n < cmd_num:
+                    pwd_js_handle.write('srun -n %s %s &\n' % (cmd_t, each_cmd.strip()))
+                else:
+                    pwd_js_handle.write('%s\n' % each_cmd.strip())
+                pwd_js_handle.close()
+            else:
+                pwd_js_handle = open(pwd_js, 'a')
+                if (math.ceil((n-1)//cmd_num_per_js) + 1) == (math.ceil((n)//cmd_num_per_js) + 1):
+                    if n < cmd_num:
+                        pwd_js_handle.write('srun -n %s %s &\n' % (cmd_t, each_cmd.strip()))
                     else:
-                        pwd_js_previous_handle.write('qsub %s\n' % pwd_js_hpc)
-                    pwd_js_previous_handle.close()
-
-            pwd_js_handle = open(pwd_js, 'w')
-            pwd_js_handle.write(js_header_str)
-            pwd_js_handle.write('\n')
-            pwd_js_handle.write(each_cmd)
-            pwd_js_handle.close()
-        else:
-            pwd_js_handle = open(pwd_js, 'a')
-            pwd_js_handle.write(each_cmd)
-            pwd_js_handle.close()
-
-        if n % cmd_num_per_js == 0:
-            js_index += 1
-        n += 1
+                        pwd_js_handle.write('srun -n %s %s\n' % (cmd_t, each_cmd.strip()))
+                        pwd_js_handle.write('wait\n')
+                else:
+                    pwd_js_handle.write('srun -n %s %s\n' % (cmd_t, each_cmd.strip()))
+                    pwd_js_handle.write('wait\n')
+                pwd_js_handle.close()
+            n += 1
 
 
 if __name__ == '__main__':
 
     parser = argparse.ArgumentParser()
-    parser.add_argument('-p',      required=True,                       help='js prefix')
-    parser.add_argument('-cmd',    required=True,                       help='cmds file')
-    parser.add_argument('-hd',     required=True,                       help='js header')
-    parser.add_argument('-n',      required=True, type=int,             help='number of cmds per job script')
-    parser.add_argument('-auto',   required=False, action="store_true", help='automatically submit next job script')
-    parser.add_argument('-sbatch', required=False, action="store_true", help='use sbatch, instead of qsub')
-    parser.add_argument('-js_hpc', required=False, default=None,        help='Full path to js folder on HPC')
-    parser.add_argument('-force',  required=False, action="store_true", help='force overwrite existing results')
+    parser.add_argument('-p',       required=True,                          help='js prefix')
+    parser.add_argument('-c',       required=True,                          help='cmds file')
+    parser.add_argument('-hd',      required=True,                          help='js header')
+    parser.add_argument('-n',       required=True,  type=int,               help='number of cmds per job script')
+    parser.add_argument('-t',       required=False, type=int, default=1,    help='number of threads specified in the commands')
+    parser.add_argument('-f',       required=False, action="store_true",    help='force overwrite existing results')
     args = vars(parser.parse_args())
-    js_cmds(args)
+    js_hpc3(args)
```

### Comparing `BioSAK-1.88.8/BioSAK/keep_best_hit.py` & `BioSAK-1.88.9/BioSAK/keep_best_hit.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/ko00001.keg` & `BioSAK-1.88.9/BioSAK/ko00001.keg`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/koala.py` & `BioSAK-1.88.9/BioSAK/koala.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/label_tree.R` & `BioSAK-1.88.9/BioSAK/label_tree.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/label_tree.py` & `BioSAK-1.88.9/BioSAK/label_tree.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/link_16S_MAG.py` & `BioSAK-1.88.9/BioSAK/link_16S_MAG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/magabund.py` & `BioSAK-1.88.9/BioSAK/magabund.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/magabund2.py` & `BioSAK-1.88.9/BioSAK/magabund2.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/manipulator_fasta.py` & `BioSAK-1.88.9/BioSAK/manipulator_fasta.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/manipulator_newick.py` & `BioSAK-1.88.9/BioSAK/manipulator_newick.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/mannwhitneyu.py` & `BioSAK-1.88.9/BioSAK/mannwhitneyu.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/mean_MAG_cov.py` & `BioSAK-1.88.9/BioSAK/mean_MAG_cov.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/merge_df.py` & `BioSAK-1.88.9/BioSAK/merge_df.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/merge_seq.py` & `BioSAK-1.88.9/BioSAK/merge_seq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/metaAssembly.py` & `BioSAK-1.88.9/BioSAK/metaAssembly.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/metabat2concoct.py` & `BioSAK-1.88.9/BioSAK/metabat2concoct.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/metabat2maxbin.py` & `BioSAK-1.88.9/BioSAK/metabat2maxbin.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/ncbi_dataset.py` & `BioSAK-1.88.9/BioSAK/ncbi_dataset.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/parse_MetaCyc_RxnDB.py` & `BioSAK-1.88.9/BioSAK/parse_MetaCyc_RxnDB.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/parse_mmseqs_tsv.py` & `BioSAK-1.88.9/BioSAK/parse_mmseqs_tsv.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/plot_mag.py` & `BioSAK-1.88.9/BioSAK/plot_mag.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/plot_sam_depth.py` & `BioSAK-1.88.9/BioSAK/plot_sam_depth.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/plot_tree.R` & `BioSAK-1.88.9/BioSAK/plot_tree.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/prefix_file.py` & `BioSAK-1.88.9/BioSAK/prefix_file.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/prokka.py` & `BioSAK-1.88.9/BioSAK/prokka.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/reads2bam.py` & `BioSAK-1.88.9/BioSAK/reads2bam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/rename_leaves.py` & `BioSAK-1.88.9/BioSAK/rename_leaves.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/rename_reads_for_Reago.py` & `BioSAK-1.88.9/BioSAK/rename_reads_for_Reago.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/rename_seq.py` & `BioSAK-1.88.9/BioSAK/rename_seq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/rename_seqs.py` & `BioSAK-1.88.9/BioSAK/rename_seqs.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/ribbon.py` & `BioSAK-1.88.9/BioSAK/ribbon.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/sam2bam.py` & `BioSAK-1.88.9/BioSAK/sam2bam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/sampling_GTDB_gnms.py` & `BioSAK-1.88.9/BioSAK/sampling_GTDB_gnms.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/select_seq.py` & `BioSAK-1.88.9/BioSAK/select_seq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/sep_reads_by_barcode.py` & `BioSAK-1.88.9/BioSAK/sep_reads_by_barcode.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/slice_seq.py` & `BioSAK-1.88.9/BioSAK/slice_seq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/split_fasta.py` & `BioSAK-1.88.9/BioSAK/split_fasta.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/split_folder.py` & `BioSAK-1.88.9/BioSAK/split_folder.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/split_sam.py` & `BioSAK-1.88.9/BioSAK/split_sam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/submitHPC.py` & `BioSAK-1.88.9/BioSAK/submitHPC.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/subset_GTDB_meta.py` & `BioSAK-1.88.9/BioSAK/subset_GTDB_meta.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/subset_df.py` & `BioSAK-1.88.9/BioSAK/subset_df.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/subset_tree.py` & `BioSAK-1.88.9/BioSAK/subset_tree.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/tmp_1.py` & `BioSAK-1.88.9/BioSAK/tmp_1.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/top_16S_hits.py` & `BioSAK-1.88.9/BioSAK/top_16S_hits.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/top_hits_in_a_group.py` & `BioSAK-1.88.9/BioSAK/top_hits_in_a_group.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/transpose.py` & `BioSAK-1.88.9/BioSAK/transpose.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/usearch_uc.py` & `BioSAK-1.88.9/BioSAK/usearch_uc.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK/wilcox.py` & `BioSAK-1.88.9/BioSAK/wilcox.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/BioSAK.egg-info/SOURCES.txt` & `BioSAK-1.88.9/BioSAK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/LICENSE` & `BioSAK-1.88.9/LICENSE`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/README.md` & `BioSAK-1.88.9/README.md`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/bin/BioSAK` & `BioSAK-1.88.9/bin/BioSAK`

 * *Files identical despite different names*

### Comparing `BioSAK-1.88.8/setup.py` & `BioSAK-1.88.9/setup.py`

 * *Files identical despite different names*

