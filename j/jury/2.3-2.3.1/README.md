# Comparing `tmp/jury-2.3.tar.gz` & `tmp/jury-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jury-2.3.tar", last modified: Sun Oct  8 19:02:39 2023, max compression
+gzip compressed data, was "jury-2.3.1.tar", last modified: Mon May 20 08:28:09 2024, max compression
```

## Comparing `jury-2.3.tar` & `jury-2.3.1.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.833930 jury-2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2023-10-08 19:02:29.000000 jury-2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14973 2023-10-08 19:02:39.833930 jury-2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13826 2023-10-08 19:02:29.000000 jury-2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.821930 jury-2.3/jury/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-10-08 19:02:29.000000 jury-2.3/jury/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2023-10-08 19:02:29.000000 jury-2.3/jury/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2023-10-08 19:02:29.000000 jury-2.3/jury/collator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8247 2023-10-08 19:02:29.000000 jury-2.3/jury/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-10-08 19:02:29.000000 jury-2.3/jury/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.821930 jury-2.3/jury/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.821930 jury-2.3/jury/metrics/_core/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5761 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/_core/auto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4140 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/_core/auxiliary.py
--rw-r--r--   0 runner    (1001) docker     (127)    23361 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/_core/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.825930 jury-2.3/jury/metrics/accuracy/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/accuracy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/accuracy/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/accuracy/accuracy_for_language_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/accuracy/accuracy_for_sequence_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.825930 jury-2.3/jury/metrics/bartscore/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/bartscore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/bartscore/bartscore.py
--rw-r--r--   0 runner    (1001) docker     (127)    11740 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/bartscore/bartscore_for_language_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.825930 jury-2.3/jury/metrics/bertscore/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/bertscore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/bertscore/bertscore.py
--rw-r--r--   0 runner    (1001) docker     (127)    12887 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/bertscore/bertscore_for_language_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.825930 jury-2.3/jury/metrics/bleu/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/bleu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/bleu/bleu.py
--rw-r--r--   0 runner    (1001) docker     (127)    12432 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/bleu/bleu_for_language_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.829930 jury-2.3/jury/metrics/bleurt/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/bleurt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/bleurt/bleurt.py
--rw-r--r--   0 runner    (1001) docker     (127)     8609 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/bleurt/bleurt_for_language_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.829930 jury-2.3/jury/metrics/cer/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/cer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/cer/cer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9839 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/cer/cer_for_language_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.829930 jury-2.3/jury/metrics/chrf/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/chrf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/chrf/chrf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10872 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/chrf/chrf_for_language_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.829930 jury-2.3/jury/metrics/comet/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/comet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/comet/comet.py
--rw-r--r--   0 runner    (1001) docker     (127)    11253 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/comet/comet_for_language_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.829930 jury-2.3/jury/metrics/f1/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/f1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/f1/f1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/f1/f1_for_language_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6925 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/f1/f1_for_sequence_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.829930 jury-2.3/jury/metrics/meteor/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/meteor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/meteor/meteor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6973 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/meteor/meteor_for_language_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.829930 jury-2.3/jury/metrics/precision/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/precision/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/precision/precision_for_language_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7072 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/precision/precision_for_sequence_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.829930 jury-2.3/jury/metrics/prism/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/prism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/prism/prism.py
--rw-r--r--   0 runner    (1001) docker     (127)    12281 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/prism/prism_for_language_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.829930 jury-2.3/jury/metrics/recall/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/recall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/recall/recall.py
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/recall/recall_for_language_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6692 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/recall/recall_for_sequence_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.829930 jury-2.3/jury/metrics/rouge/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/rouge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/rouge/rouge.py
--rw-r--r--   0 runner    (1001) docker     (127)    10228 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/rouge/rouge_for_language_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.829930 jury-2.3/jury/metrics/sacrebleu/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/sacrebleu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/sacrebleu/sacrebleu.py
--rw-r--r--   0 runner    (1001) docker     (127)    11101 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/sacrebleu/sacrebleu_for_language_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.829930 jury-2.3/jury/metrics/seqeval/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/seqeval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/seqeval/seqeval.py
--rw-r--r--   0 runner    (1001) docker     (127)     8399 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/seqeval/seqeval_for_sequence_labeling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.829930 jury-2.3/jury/metrics/squad/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/squad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/squad/squad.py
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/squad/squad_for_language_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.833930 jury-2.3/jury/metrics/ter/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/ter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/ter/ter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9679 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/ter/ter_for_language_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.833930 jury-2.3/jury/metrics/wer/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/wer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/wer/wer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9927 2023-10-08 19:02:29.000000 jury-2.3/jury/metrics/wer/wer_for_language_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-10-08 19:02:29.000000 jury-2.3/jury/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.833930 jury-2.3/jury/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:29.000000 jury-2.3/jury/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2023-10-08 19:02:29.000000 jury-2.3/jury/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2023-10-08 19:02:29.000000 jury-2.3/jury/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2023-10-08 19:02:29.000000 jury-2.3/jury/utils/nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.821930 jury-2.3/jury.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14973 2023-10-08 19:02:39.000000 jury-2.3/jury.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2023-10-08 19:02:39.000000 jury-2.3/jury.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-08 19:02:39.000000 jury-2.3/jury.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-08 19:02:39.000000 jury-2.3/jury.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      638 2023-10-08 19:02:39.000000 jury-2.3/jury.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-10-08 19:02:39.000000 jury-2.3/jury.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2023-10-08 19:02:29.000000 jury-2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-10-08 19:02:39.833930 jury-2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2023-10-08 19:02:29.000000 jury-2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.817930 jury-2.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.833930 jury-2.3/tests/jury/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-10-08 19:02:29.000000 jury-2.3/tests/jury/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2023-10-08 19:02:29.000000 jury-2.3/tests/jury/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:39.833930 jury-2.3/tests/jury/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-08 19:02:29.000000 jury-2.3/tests/jury/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2023-10-08 19:02:29.000000 jury-2.3/tests/jury/metrics/test_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2023-10-08 19:02:29.000000 jury-2.3/tests/jury/metrics/test_bartscore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2023-10-08 19:02:29.000000 jury-2.3/tests/jury/metrics/test_bertscore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2023-10-08 19:02:29.000000 jury-2.3/tests/jury/metrics/test_bleu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2023-10-08 19:02:29.000000 jury-2.3/tests/jury/metrics/test_bleurt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2023-10-08 19:02:29.000000 jury-2.3/tests/jury/metrics/test_cer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2023-10-08 19:02:29.000000 jury-2.3/tests/jury/metrics/test_chrf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2023-10-08 19:02:29.000000 jury-2.3/tests/jury/metrics/test_comet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2023-10-08 19:02:29.000000 jury-2.3/tests/jury/metrics/test_custom_bleu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2023-10-08 19:02:29.000000 jury-2.3/tests/jury/metrics/test_f1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2023-10-08 19:02:29.000000 jury-2.3/tests/jury/metrics/test_meteor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2023-10-08 19:02:29.000000 jury-2.3/tests/jury/metrics/test_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2023-10-08 19:02:29.000000 jury-2.3/tests/jury/metrics/test_prism.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2023-10-08 19:02:29.000000 jury-2.3/tests/jury/metrics/test_recall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2023-10-08 19:02:29.000000 jury-2.3/tests/jury/metrics/test_rouge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2023-10-08 19:02:29.000000 jury-2.3/tests/jury/metrics/test_sacrebleu.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2023-10-08 19:02:29.000000 jury-2.3/tests/jury/metrics/test_seqeval.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2023-10-08 19:02:29.000000 jury-2.3/tests/jury/metrics/test_squad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2023-10-08 19:02:29.000000 jury-2.3/tests/jury/metrics/test_ter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2023-10-08 19:02:29.000000 jury-2.3/tests/jury/metrics/test_wer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2023-10-08 19:02:29.000000 jury-2.3/tests/jury/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-10-08 19:02:29.000000 jury-2.3/tests/jury/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     6208 2023-10-08 19:02:29.000000 jury-2.3/tests/jury/test_jury.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2023-10-08 19:02:29.000000 jury-2.3/tests/jury/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.887881 jury-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-20 08:27:56.000000 jury-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17593 2024-05-20 08:28:09.887881 jury-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14821 2024-05-20 08:27:56.000000 jury-2.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.871881 jury-2.3.1/jury/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-20 08:27:56.000000 jury-2.3.1/jury/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-05-20 08:27:56.000000 jury-2.3.1/jury/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-20 08:27:56.000000 jury-2.3.1/jury/collator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-05-20 08:27:56.000000 jury-2.3.1/jury/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-20 08:27:56.000000 jury-2.3.1/jury/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.871881 jury-2.3.1/jury/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.871881 jury-2.3.1/jury/metrics/_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/_core/auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4140 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/_core/auxiliary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23361 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/_core/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.871881 jury-2.3.1/jury/metrics/accuracy/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/accuracy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/accuracy/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/accuracy/accuracy_for_language_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/accuracy/accuracy_for_sequence_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.875881 jury-2.3.1/jury/metrics/bartscore/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/bartscore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/bartscore/bartscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11740 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/bartscore/bartscore_for_language_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.875881 jury-2.3.1/jury/metrics/bertscore/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/bertscore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/bertscore/bertscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/bertscore/bertscore_for_language_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.875881 jury-2.3.1/jury/metrics/bleu/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/bleu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/bleu/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12432 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/bleu/bleu_for_language_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.875881 jury-2.3.1/jury/metrics/bleurt/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/bleurt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/bleurt/bleurt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8609 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/bleurt/bleurt_for_language_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.875881 jury-2.3.1/jury/metrics/cer/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/cer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/cer/cer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9839 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/cer/cer_for_language_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.875881 jury-2.3.1/jury/metrics/chrf/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/chrf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/chrf/chrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/chrf/chrf_for_language_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.875881 jury-2.3.1/jury/metrics/comet/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/comet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/comet/comet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11253 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/comet/comet_for_language_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.875881 jury-2.3.1/jury/metrics/f1/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/f1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/f1/f1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/f1/f1_for_language_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/f1/f1_for_sequence_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.875881 jury-2.3.1/jury/metrics/meteor/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/meteor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/meteor/meteor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/meteor/meteor_for_language_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.879881 jury-2.3.1/jury/metrics/precision/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/precision/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/precision/precision_for_language_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7072 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/precision/precision_for_sequence_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.879881 jury-2.3.1/jury/metrics/prism/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/prism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/prism/prism.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12281 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/prism/prism_for_language_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.879881 jury-2.3.1/jury/metrics/recall/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/recall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/recall/recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/recall/recall_for_language_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/recall/recall_for_sequence_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.879881 jury-2.3.1/jury/metrics/rouge/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/rouge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/rouge/rouge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/rouge/rouge_for_language_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.879881 jury-2.3.1/jury/metrics/sacrebleu/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/sacrebleu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/sacrebleu/sacrebleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11101 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/sacrebleu/sacrebleu_for_language_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.879881 jury-2.3.1/jury/metrics/seqeval/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/seqeval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/seqeval/seqeval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/seqeval/seqeval_for_sequence_labeling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.879881 jury-2.3.1/jury/metrics/squad/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/squad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/squad/squad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/squad/squad_for_language_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.879881 jury-2.3.1/jury/metrics/ter/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/ter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/ter/ter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/ter/ter_for_language_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.879881 jury-2.3.1/jury/metrics/wer/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/wer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/wer/wer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9927 2024-05-20 08:27:56.000000 jury-2.3.1/jury/metrics/wer/wer_for_language_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-20 08:27:56.000000 jury-2.3.1/jury/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.883880 jury-2.3.1/jury/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 08:27:56.000000 jury-2.3.1/jury/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-20 08:27:56.000000 jury-2.3.1/jury/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-20 08:27:56.000000 jury-2.3.1/jury/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-20 08:27:56.000000 jury-2.3.1/jury/utils/nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.883880 jury-2.3.1/jury.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17593 2024-05-20 08:28:09.000000 jury-2.3.1/jury.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-05-20 08:28:09.000000 jury-2.3.1/jury.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 08:28:09.000000 jury-2.3.1/jury.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 08:28:09.000000 jury-2.3.1/jury.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-20 08:28:09.000000 jury-2.3.1/jury.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-20 08:28:09.000000 jury-2.3.1/jury.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-20 08:27:56.000000 jury-2.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-20 08:28:09.887881 jury-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-20 08:27:56.000000 jury-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.871881 jury-2.3.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.883880 jury-2.3.1/tests/jury/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-20 08:27:56.000000 jury-2.3.1/tests/jury/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-05-20 08:27:56.000000 jury-2.3.1/tests/jury/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:28:09.883880 jury-2.3.1/tests/jury/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 08:27:56.000000 jury-2.3.1/tests/jury/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-20 08:27:56.000000 jury-2.3.1/tests/jury/metrics/test_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-20 08:27:56.000000 jury-2.3.1/tests/jury/metrics/test_bartscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-20 08:27:56.000000 jury-2.3.1/tests/jury/metrics/test_bertscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-20 08:27:56.000000 jury-2.3.1/tests/jury/metrics/test_bleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-20 08:27:56.000000 jury-2.3.1/tests/jury/metrics/test_bleurt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-20 08:27:56.000000 jury-2.3.1/tests/jury/metrics/test_cer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-20 08:27:56.000000 jury-2.3.1/tests/jury/metrics/test_chrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-20 08:27:56.000000 jury-2.3.1/tests/jury/metrics/test_comet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-20 08:27:56.000000 jury-2.3.1/tests/jury/metrics/test_custom_bleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-05-20 08:27:56.000000 jury-2.3.1/tests/jury/metrics/test_f1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-20 08:27:56.000000 jury-2.3.1/tests/jury/metrics/test_meteor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-05-20 08:27:56.000000 jury-2.3.1/tests/jury/metrics/test_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-20 08:27:56.000000 jury-2.3.1/tests/jury/metrics/test_prism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-20 08:27:56.000000 jury-2.3.1/tests/jury/metrics/test_recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-20 08:27:56.000000 jury-2.3.1/tests/jury/metrics/test_rouge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-20 08:27:56.000000 jury-2.3.1/tests/jury/metrics/test_sacrebleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-20 08:27:56.000000 jury-2.3.1/tests/jury/metrics/test_seqeval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-20 08:27:56.000000 jury-2.3.1/tests/jury/metrics/test_squad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-20 08:27:56.000000 jury-2.3.1/tests/jury/metrics/test_ter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-20 08:27:56.000000 jury-2.3.1/tests/jury/metrics/test_wer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-20 08:27:56.000000 jury-2.3.1/tests/jury/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-20 08:27:56.000000 jury-2.3.1/tests/jury/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-05-20 08:27:56.000000 jury-2.3.1/tests/jury/test_jury.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-20 08:27:56.000000 jury-2.3.1/tests/jury/test_utils.py
```

### Comparing `jury-2.3/LICENSE` & `jury-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jury-2.3/PKG-INFO` & `jury-2.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: jury
-Version: 2.3
-Summary: Evaluation toolkit for neural language generation.
-Home-page: https://github.com/obss/jury
-Author: 
-License: MIT
-Keywords: machine-learning,deep-learning,ml,pytorch,NLP,evaluation,question-answering,question-generation
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Education
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: prism
-Provides-Extra: metrics
-Provides-Extra: dev
-License-File: LICENSE
-
 <h1 align="center">Jury</h1>
 
 <p align="center">
 <a href="https://pypi.org/project/jury"><img src="https://img.shields.io/pypi/pyversions/jury" alt="Python versions"></a>
 <a href="https://pepy.tech/project/jury"><img src="https://pepy.tech/badge/jury" alt="downloads"></a>
 <a href="https://pypi.org/project/jury"><img src="https://img.shields.io/pypi/v/jury?color=blue" alt="PyPI version"></a>
 <a href="https://github.com/obss/jury/releases/latest"><img alt="Latest Release" src="https://img.shields.io/github/release-date/obss/jury"></a>
@@ -260,15 +231,15 @@
 
 PRs are welcomed as always :)
 
 ### Installation
 
     git clone https://github.com/obss/jury.git
     cd jury
-    pip install -e .[dev]
+    pip install -e ".[dev]"
 
 Also, you need to install the packages which are available through a git source separately with the following command. 
 For the folks who are curious about "why?"; a short explaination is that PYPI does not allow indexing a package which 
 are directly dependent on non-pypi packages due to security reasons. The file `requirements-dev.txt` includes packages 
 which are currently only available through a git source, or they are PYPI packages with no recent release or 
 incompatible with Jury, so that they are added as git sources or pointing to specific commits.
 
@@ -301,10 +272,20 @@
       year={2023},
       eprint={2310.02040},
       archivePrefix={arXiv},
       primaryClass={cs.CL},
       doi={10.48550/arXiv.2310.02040}
     }
 
+## Community Interaction
+
+We use the GitHub Issue Tracker to track issues in general. Issues can be bug reports, feature requests or implementation of a new metric type. Please refer to the related issue template for opening new issues.
+
+|                                | Location                                                                                           |
+|--------------------------------|----------------------------------------------------------------------------------------------------|
+| Bug Report                     | [Bug Report Template](https://github.com/obss/jury/issues/new?assignees=&labels=&projects=&template=bug_report.md&title=) |
+| New Metric Request             | [Request Metric Implementation](https://github.com/obss/jury/issues/new?assignees=&labels=&projects=&template=new-metric.md&title=) |
+| All other issues and questions | [General Issues](https://github.com/obss/jury/issues/new)                                                            |
+
 ## <div align="center"> License </div>
 
 Licensed under the [MIT](LICENSE) License.
```

#### html2text {}

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1 Name: jury Version: 2.3 Summary: Evaluation toolkit for
-neural language generation. Home-page: https://github.com/obss/jury Author:
-License: MIT Keywords: machine-learning,deep-
-learning,ml,pytorch,NLP,evaluation,question-answering,question-generation
-Classifier: Development Status :: 5 - Production/Stable Classifier: Operating
-System :: OS Independent Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Classifier: Topic ::
-Education Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
-Description-Content-Type: text/markdown Provides-Extra: prism Provides-Extra:
-metrics Provides-Extra: dev License-File: LICENSE
                               ************ JJuurryy ************
    _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_d_o_w_n_l_o_a_d_s_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_L_a_t_e_s_t_ _R_e_l_e_a_s_e_]_[_O_p_e_n_ _i_n_ _C_o_l_a_b_]
          _[_B_u_i_l_d_ _s_t_a_t_u_s_]_[_D_e_p_e_n_d_e_n_c_i_e_s_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_L_i_c_e_n_s_e_:_ _M_I_T_]
                                      _[_D_O_I_]
 A comprehensive toolkit for evaluating NLP experiments offering various
 automated metrics. Jury offers a smooth and easy-to-use interface. It uses a
 more advanced version of [evaluate](https://github.com/huggingface/evaluate/
@@ -136,15 +120,15 @@
 _compute_single_pred_multi_ref( self, predictions, references, reduce_fn =
 None, **kwargs ): raise NotImplementedError def _compute_multi_pred_multi_ref
 ( self, predictions, references, reduce_fn = None, **kwargs ): raise
 NotImplementedError ``` For more details, have a look at base metric
 implementation [jury.metrics.Metric](./jury/metrics/_base.py) ##
                                  Contributing
 PRs are welcomed as always :) ### Installation git clone https://github.com/
-obss/jury.git cd jury pip install -e .[dev] Also, you need to install the
+obss/jury.git cd jury pip install -e ".[dev]" Also, you need to install the
 packages which are available through a git source separately with the following
 command. For the folks who are curious about "why?"; a short explaination is
 that PYPI does not allow indexing a package which are directly dependent on
 non-pypi packages due to security reasons. The file `requirements-dev.txt`
 includes packages which are currently only available through a git source, or
 they are PYPI packages with no recent release or incompatible with Jury, so
 that they are added as git sources or pointing to specific commits. pip install
@@ -152,10 +136,21 @@
 run_tests.py ### Code Style To check code style, python tests/run_code_style.py
 check To format codebase, python tests/run_code_style.py format ##
                                    Citation
 If you use this package in your work, please cite it as: @misc
 {cavusoglu2023jury, title={Jury: A Comprehensive Evaluation Toolkit}, author=
 {Devrim Cavusoglu and Ulas Sert and Secil Sen and Sinan Altinuc}, year={2023},
 eprint={2310.02040}, archivePrefix={arXiv}, primaryClass={cs.CL}, doi=
-{10.48550/arXiv.2310.02040} } ##
+{10.48550/arXiv.2310.02040} } ## Community Interaction We use the GitHub Issue
+Tracker to track issues in general. Issues can be bug reports, feature requests
+or implementation of a new metric type. Please refer to the related issue
+template for opening new issues. | | Location | |------------------------------
+--|----------------------------------------------------------------------------
+------------------------| | Bug Report | [Bug Report Template](https://
+github.com/obss/jury/issues/
+new?assignees=&labels=&projects=&template=bug_report.md&title=) | | New Metric
+Request | [Request Metric Implementation](https://github.com/obss/jury/issues/
+new?assignees=&labels=&projects=&template=new-metric.md&title=) | | All other
+issues and questions | [General Issues](https://github.com/obss/jury/issues/
+new) | ##
                                     License
 Licensed under the [MIT](LICENSE) License.
```

### Comparing `jury-2.3/README.md` & `jury-2.3.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,72 @@
+Metadata-Version: 2.1
+Name: jury
+Version: 2.3.1
+Summary: Evaluation toolkit for neural language generation.
+Home-page: https://github.com/obss/jury
+Author: 
+License: MIT
+Keywords: machine-learning,deep-learning,ml,pytorch,NLP,evaluation,question-answering,question-generation
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Education
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: click==8.0.4
+Requires-Dist: evaluate<0.5,>=0.4
+Requires-Dist: datasets<2.10,>=2.9
+Requires-Dist: fire>=0.4.0
+Requires-Dist: nltk<3.7.1,>=3.6.6
+Requires-Dist: rouge-score==0.0.4
+Requires-Dist: scikit-learn
+Requires-Dist: tqdm
+Requires-Dist: validators
+Provides-Extra: prism
+Requires-Dist: fairseq==0.9.0; extra == "prism"
+Requires-Dist: numpy<1.24,>=1.23; extra == "prism"
+Provides-Extra: metrics
+Requires-Dist: sacrebleu>=2.0.0; extra == "metrics"
+Requires-Dist: bert_score==0.3.11; extra == "metrics"
+Requires-Dist: jiwer>=2.3.0; extra == "metrics"
+Requires-Dist: seqeval==1.2.2; extra == "metrics"
+Requires-Dist: sentencepiece<0.2,>=0.1.99; extra == "metrics"
+Requires-Dist: unbabel-comet==2.0.1; extra == "metrics"
+Requires-Dist: protobuf<3.21,>=3.20.3; extra == "metrics"
+Requires-Dist: fairseq==0.9.0; extra == "metrics"
+Requires-Dist: numpy<1.24,>=1.23; extra == "metrics"
+Provides-Extra: dev
+Requires-Dist: black==21.7b0; extra == "dev"
+Requires-Dist: deepdiff==5.5.0; extra == "dev"
+Requires-Dist: flake8==3.9.2; extra == "dev"
+Requires-Dist: isort==5.9.2; extra == "dev"
+Requires-Dist: pytest>=7.0.1; extra == "dev"
+Requires-Dist: pytest-cov>=3.0.0; extra == "dev"
+Requires-Dist: pytest-timeout>=2.1.0; extra == "dev"
+Requires-Dist: sacrebleu>=2.0.0; extra == "dev"
+Requires-Dist: bert_score==0.3.11; extra == "dev"
+Requires-Dist: jiwer>=2.3.0; extra == "dev"
+Requires-Dist: seqeval==1.2.2; extra == "dev"
+Requires-Dist: sentencepiece<0.2,>=0.1.99; extra == "dev"
+Requires-Dist: unbabel-comet==2.0.1; extra == "dev"
+Requires-Dist: protobuf<3.21,>=3.20.3; extra == "dev"
+Requires-Dist: fairseq==0.9.0; extra == "dev"
+Requires-Dist: numpy<1.24,>=1.23; extra == "dev"
+
 <h1 align="center">Jury</h1>
 
 <p align="center">
 <a href="https://pypi.org/project/jury"><img src="https://img.shields.io/pypi/pyversions/jury" alt="Python versions"></a>
 <a href="https://pepy.tech/project/jury"><img src="https://pepy.tech/badge/jury" alt="downloads"></a>
 <a href="https://pypi.org/project/jury"><img src="https://img.shields.io/pypi/v/jury?color=blue" alt="PyPI version"></a>
 <a href="https://github.com/obss/jury/releases/latest"><img alt="Latest Release" src="https://img.shields.io/github/release-date/obss/jury"></a>
@@ -231,15 +296,15 @@
 
 PRs are welcomed as always :)
 
 ### Installation
 
     git clone https://github.com/obss/jury.git
     cd jury
-    pip install -e .[dev]
+    pip install -e ".[dev]"
 
 Also, you need to install the packages which are available through a git source separately with the following command. 
 For the folks who are curious about "why?"; a short explaination is that PYPI does not allow indexing a package which 
 are directly dependent on non-pypi packages due to security reasons. The file `requirements-dev.txt` includes packages 
 which are currently only available through a git source, or they are PYPI packages with no recent release or 
 incompatible with Jury, so that they are added as git sources or pointing to specific commits.
 
@@ -272,10 +337,20 @@
       year={2023},
       eprint={2310.02040},
       archivePrefix={arXiv},
       primaryClass={cs.CL},
       doi={10.48550/arXiv.2310.02040}
     }
 
+## Community Interaction
+
+We use the GitHub Issue Tracker to track issues in general. Issues can be bug reports, feature requests or implementation of a new metric type. Please refer to the related issue template for opening new issues.
+
+|                                | Location                                                                                           |
+|--------------------------------|----------------------------------------------------------------------------------------------------|
+| Bug Report                     | [Bug Report Template](https://github.com/obss/jury/issues/new?assignees=&labels=&projects=&template=bug_report.md&title=) |
+| New Metric Request             | [Request Metric Implementation](https://github.com/obss/jury/issues/new?assignees=&labels=&projects=&template=new-metric.md&title=) |
+| All other issues and questions | [General Issues](https://github.com/obss/jury/issues/new)                                                            |
+
 ## <div align="center"> License </div>
 
 Licensed under the [MIT](LICENSE) License.
```

#### html2text {}

```diff
@@ -1,7 +1,45 @@
+Metadata-Version: 2.1 Name: jury Version: 2.3.1 Summary: Evaluation toolkit for
+neural language generation. Home-page: https://github.com/obss/jury Author:
+License: MIT Keywords: machine-learning,deep-
+learning,ml,pytorch,NLP,evaluation,question-answering,question-generation
+Classifier: Development Status :: 5 - Production/Stable Classifier: Operating
+System :: OS Independent Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Classifier: Topic ::
+Education Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+click==8.0.4 Requires-Dist: evaluate<0.5,>=0.4 Requires-Dist:
+datasets<2.10,>=2.9 Requires-Dist: fire>=0.4.0 Requires-Dist:
+nltk<3.7.1,>=3.6.6 Requires-Dist: rouge-score==0.0.4 Requires-Dist: scikit-
+learn Requires-Dist: tqdm Requires-Dist: validators Provides-Extra: prism
+Requires-Dist: fairseq==0.9.0; extra == "prism" Requires-Dist:
+numpy<1.24,>=1.23; extra == "prism" Provides-Extra: metrics Requires-Dist:
+sacrebleu>=2.0.0; extra == "metrics" Requires-Dist: bert_score==0.3.11; extra
+== "metrics" Requires-Dist: jiwer>=2.3.0; extra == "metrics" Requires-Dist:
+seqeval==1.2.2; extra == "metrics" Requires-Dist: sentencepiece<0.2,>=0.1.99;
+extra == "metrics" Requires-Dist: unbabel-comet==2.0.1; extra == "metrics"
+Requires-Dist: protobuf<3.21,>=3.20.3; extra == "metrics" Requires-Dist:
+fairseq==0.9.0; extra == "metrics" Requires-Dist: numpy<1.24,>=1.23; extra ==
+"metrics" Provides-Extra: dev Requires-Dist: black==21.7b0; extra == "dev"
+Requires-Dist: deepdiff==5.5.0; extra == "dev" Requires-Dist: flake8==3.9.2;
+extra == "dev" Requires-Dist: isort==5.9.2; extra == "dev" Requires-Dist:
+pytest>=7.0.1; extra == "dev" Requires-Dist: pytest-cov>=3.0.0; extra == "dev"
+Requires-Dist: pytest-timeout>=2.1.0; extra == "dev" Requires-Dist:
+sacrebleu>=2.0.0; extra == "dev" Requires-Dist: bert_score==0.3.11; extra ==
+"dev" Requires-Dist: jiwer>=2.3.0; extra == "dev" Requires-Dist:
+seqeval==1.2.2; extra == "dev" Requires-Dist: sentencepiece<0.2,>=0.1.99; extra
+== "dev" Requires-Dist: unbabel-comet==2.0.1; extra == "dev" Requires-Dist:
+protobuf<3.21,>=3.20.3; extra == "dev" Requires-Dist: fairseq==0.9.0; extra ==
+"dev" Requires-Dist: numpy<1.24,>=1.23; extra == "dev"
                               ************ JJuurryy ************
    _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_d_o_w_n_l_o_a_d_s_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_L_a_t_e_s_t_ _R_e_l_e_a_s_e_]_[_O_p_e_n_ _i_n_ _C_o_l_a_b_]
          _[_B_u_i_l_d_ _s_t_a_t_u_s_]_[_D_e_p_e_n_d_e_n_c_i_e_s_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_L_i_c_e_n_s_e_:_ _M_I_T_]
                                      _[_D_O_I_]
 A comprehensive toolkit for evaluating NLP experiments offering various
 automated metrics. Jury offers a smooth and easy-to-use interface. It uses a
 more advanced version of [evaluate](https://github.com/huggingface/evaluate/
@@ -120,15 +158,15 @@
 _compute_single_pred_multi_ref( self, predictions, references, reduce_fn =
 None, **kwargs ): raise NotImplementedError def _compute_multi_pred_multi_ref
 ( self, predictions, references, reduce_fn = None, **kwargs ): raise
 NotImplementedError ``` For more details, have a look at base metric
 implementation [jury.metrics.Metric](./jury/metrics/_base.py) ##
                                  Contributing
 PRs are welcomed as always :) ### Installation git clone https://github.com/
-obss/jury.git cd jury pip install -e .[dev] Also, you need to install the
+obss/jury.git cd jury pip install -e ".[dev]" Also, you need to install the
 packages which are available through a git source separately with the following
 command. For the folks who are curious about "why?"; a short explaination is
 that PYPI does not allow indexing a package which are directly dependent on
 non-pypi packages due to security reasons. The file `requirements-dev.txt`
 includes packages which are currently only available through a git source, or
 they are PYPI packages with no recent release or incompatible with Jury, so
 that they are added as git sources or pointing to specific commits. pip install
@@ -136,10 +174,21 @@
 run_tests.py ### Code Style To check code style, python tests/run_code_style.py
 check To format codebase, python tests/run_code_style.py format ##
                                    Citation
 If you use this package in your work, please cite it as: @misc
 {cavusoglu2023jury, title={Jury: A Comprehensive Evaluation Toolkit}, author=
 {Devrim Cavusoglu and Ulas Sert and Secil Sen and Sinan Altinuc}, year={2023},
 eprint={2310.02040}, archivePrefix={arXiv}, primaryClass={cs.CL}, doi=
-{10.48550/arXiv.2310.02040} } ##
+{10.48550/arXiv.2310.02040} } ## Community Interaction We use the GitHub Issue
+Tracker to track issues in general. Issues can be bug reports, feature requests
+or implementation of a new metric type. Please refer to the related issue
+template for opening new issues. | | Location | |------------------------------
+--|----------------------------------------------------------------------------
+------------------------| | Bug Report | [Bug Report Template](https://
+github.com/obss/jury/issues/
+new?assignees=&labels=&projects=&template=bug_report.md&title=) | | New Metric
+Request | [Request Metric Implementation](https://github.com/obss/jury/issues/
+new?assignees=&labels=&projects=&template=new-metric.md&title=) | | All other
+issues and questions | [General Issues](https://github.com/obss/jury/issues/
+new) | ##
                                     License
 Licensed under the [MIT](LICENSE) License.
```

### Comparing `jury-2.3/jury/cli.py` & `jury-2.3.1/jury/cli.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/collator.py` & `jury-2.3.1/jury/collator.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/core.py` & `jury-2.3.1/jury/core.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/__init__.py` & `jury-2.3.1/jury/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/_core/__init__.py` & `jury-2.3.1/jury/metrics/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/_core/auto.py` & `jury-2.3.1/jury/metrics/_core/auto.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/_core/auxiliary.py` & `jury-2.3.1/jury/metrics/_core/auxiliary.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/_core/base.py` & `jury-2.3.1/jury/metrics/_core/base.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/_core/utils.py` & `jury-2.3.1/jury/metrics/_core/utils.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/accuracy/accuracy_for_language_generation.py` & `jury-2.3.1/jury/metrics/accuracy/accuracy_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/accuracy/accuracy_for_sequence_classification.py` & `jury-2.3.1/jury/metrics/accuracy/accuracy_for_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/bartscore/bartscore_for_language_generation.py` & `jury-2.3.1/jury/metrics/bartscore/bartscore_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/bertscore/bertscore_for_language_generation.py` & `jury-2.3.1/jury/metrics/bertscore/bertscore_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/bleu/bleu.py` & `jury-2.3.1/jury/metrics/bleu/bleu.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/bleu/bleu_for_language_generation.py` & `jury-2.3.1/jury/metrics/bleu/bleu_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/bleurt/bleurt_for_language_generation.py` & `jury-2.3.1/jury/metrics/bleurt/bleurt_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/cer/cer_for_language_generation.py` & `jury-2.3.1/jury/metrics/cer/cer_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/chrf/chrf_for_language_generation.py` & `jury-2.3.1/jury/metrics/chrf/chrf_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/comet/comet_for_language_generation.py` & `jury-2.3.1/jury/metrics/comet/comet_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/f1/f1_for_language_generation.py` & `jury-2.3.1/jury/metrics/f1/f1_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/f1/f1_for_sequence_classification.py` & `jury-2.3.1/jury/metrics/f1/f1_for_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/meteor/meteor_for_language_generation.py` & `jury-2.3.1/jury/metrics/meteor/meteor_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/precision/precision_for_language_generation.py` & `jury-2.3.1/jury/metrics/precision/precision_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/precision/precision_for_sequence_classification.py` & `jury-2.3.1/jury/metrics/precision/precision_for_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/prism/prism_for_language_generation.py` & `jury-2.3.1/jury/metrics/prism/prism_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/recall/recall_for_language_generation.py` & `jury-2.3.1/jury/metrics/recall/recall_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/recall/recall_for_sequence_classification.py` & `jury-2.3.1/jury/metrics/recall/recall_for_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/rouge/rouge_for_language_generation.py` & `jury-2.3.1/jury/metrics/rouge/rouge_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/sacrebleu/sacrebleu_for_language_generation.py` & `jury-2.3.1/jury/metrics/sacrebleu/sacrebleu_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/seqeval/seqeval_for_sequence_labeling.py` & `jury-2.3.1/jury/metrics/seqeval/seqeval_for_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/squad/squad_for_language_generation.py` & `jury-2.3.1/jury/metrics/squad/squad_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/ter/ter_for_language_generation.py` & `jury-2.3.1/jury/metrics/ter/ter_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/metrics/wer/wer_for_language_generation.py` & `jury-2.3.1/jury/metrics/wer/wer_for_language_generation.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/tokenizer.py` & `jury-2.3.1/jury/tokenizer.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/utils/common.py` & `jury-2.3.1/jury/utils/common.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury/utils/io.py` & `jury-2.3.1/jury/utils/io.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury.egg-info/PKG-INFO` & `jury-2.3.1/jury.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jury
-Version: 2.3
+Version: 2.3.1
 Summary: Evaluation toolkit for neural language generation.
 Home-page: https://github.com/obss/jury
 Author: 
 License: MIT
 Keywords: machine-learning,deep-learning,ml,pytorch,NLP,evaluation,question-answering,question-generation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -18,18 +18,54 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: click==8.0.4
+Requires-Dist: evaluate<0.5,>=0.4
+Requires-Dist: datasets<2.10,>=2.9
+Requires-Dist: fire>=0.4.0
+Requires-Dist: nltk<3.7.1,>=3.6.6
+Requires-Dist: rouge-score==0.0.4
+Requires-Dist: scikit-learn
+Requires-Dist: tqdm
+Requires-Dist: validators
 Provides-Extra: prism
+Requires-Dist: fairseq==0.9.0; extra == "prism"
+Requires-Dist: numpy<1.24,>=1.23; extra == "prism"
 Provides-Extra: metrics
+Requires-Dist: sacrebleu>=2.0.0; extra == "metrics"
+Requires-Dist: bert_score==0.3.11; extra == "metrics"
+Requires-Dist: jiwer>=2.3.0; extra == "metrics"
+Requires-Dist: seqeval==1.2.2; extra == "metrics"
+Requires-Dist: sentencepiece<0.2,>=0.1.99; extra == "metrics"
+Requires-Dist: unbabel-comet==2.0.1; extra == "metrics"
+Requires-Dist: protobuf<3.21,>=3.20.3; extra == "metrics"
+Requires-Dist: fairseq==0.9.0; extra == "metrics"
+Requires-Dist: numpy<1.24,>=1.23; extra == "metrics"
 Provides-Extra: dev
-License-File: LICENSE
+Requires-Dist: black==21.7b0; extra == "dev"
+Requires-Dist: deepdiff==5.5.0; extra == "dev"
+Requires-Dist: flake8==3.9.2; extra == "dev"
+Requires-Dist: isort==5.9.2; extra == "dev"
+Requires-Dist: pytest>=7.0.1; extra == "dev"
+Requires-Dist: pytest-cov>=3.0.0; extra == "dev"
+Requires-Dist: pytest-timeout>=2.1.0; extra == "dev"
+Requires-Dist: sacrebleu>=2.0.0; extra == "dev"
+Requires-Dist: bert_score==0.3.11; extra == "dev"
+Requires-Dist: jiwer>=2.3.0; extra == "dev"
+Requires-Dist: seqeval==1.2.2; extra == "dev"
+Requires-Dist: sentencepiece<0.2,>=0.1.99; extra == "dev"
+Requires-Dist: unbabel-comet==2.0.1; extra == "dev"
+Requires-Dist: protobuf<3.21,>=3.20.3; extra == "dev"
+Requires-Dist: fairseq==0.9.0; extra == "dev"
+Requires-Dist: numpy<1.24,>=1.23; extra == "dev"
 
 <h1 align="center">Jury</h1>
 
 <p align="center">
 <a href="https://pypi.org/project/jury"><img src="https://img.shields.io/pypi/pyversions/jury" alt="Python versions"></a>
 <a href="https://pepy.tech/project/jury"><img src="https://pepy.tech/badge/jury" alt="downloads"></a>
 <a href="https://pypi.org/project/jury"><img src="https://img.shields.io/pypi/v/jury?color=blue" alt="PyPI version"></a>
@@ -260,15 +296,15 @@
 
 PRs are welcomed as always :)
 
 ### Installation
 
     git clone https://github.com/obss/jury.git
     cd jury
-    pip install -e .[dev]
+    pip install -e ".[dev]"
 
 Also, you need to install the packages which are available through a git source separately with the following command. 
 For the folks who are curious about "why?"; a short explaination is that PYPI does not allow indexing a package which 
 are directly dependent on non-pypi packages due to security reasons. The file `requirements-dev.txt` includes packages 
 which are currently only available through a git source, or they are PYPI packages with no recent release or 
 incompatible with Jury, so that they are added as git sources or pointing to specific commits.
 
@@ -301,10 +337,20 @@
       year={2023},
       eprint={2310.02040},
       archivePrefix={arXiv},
       primaryClass={cs.CL},
       doi={10.48550/arXiv.2310.02040}
     }
 
+## Community Interaction
+
+We use the GitHub Issue Tracker to track issues in general. Issues can be bug reports, feature requests or implementation of a new metric type. Please refer to the related issue template for opening new issues.
+
+|                                | Location                                                                                           |
+|--------------------------------|----------------------------------------------------------------------------------------------------|
+| Bug Report                     | [Bug Report Template](https://github.com/obss/jury/issues/new?assignees=&labels=&projects=&template=bug_report.md&title=) |
+| New Metric Request             | [Request Metric Implementation](https://github.com/obss/jury/issues/new?assignees=&labels=&projects=&template=new-metric.md&title=) |
+| All other issues and questions | [General Issues](https://github.com/obss/jury/issues/new)                                                            |
+
 ## <div align="center"> License </div>
 
 Licensed under the [MIT](LICENSE) License.
```

#### html2text {}

```diff
@@ -1,23 +1,45 @@
-Metadata-Version: 2.1 Name: jury Version: 2.3 Summary: Evaluation toolkit for
+Metadata-Version: 2.1 Name: jury Version: 2.3.1 Summary: Evaluation toolkit for
 neural language generation. Home-page: https://github.com/obss/jury Author:
 License: MIT Keywords: machine-learning,deep-
 learning,ml,pytorch,NLP,evaluation,question-answering,question-generation
 Classifier: Development Status :: 5 - Production/Stable Classifier: Operating
 System :: OS Independent Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Classifier: Topic ::
 Education Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
-Description-Content-Type: text/markdown Provides-Extra: prism Provides-Extra:
-metrics Provides-Extra: dev License-File: LICENSE
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+click==8.0.4 Requires-Dist: evaluate<0.5,>=0.4 Requires-Dist:
+datasets<2.10,>=2.9 Requires-Dist: fire>=0.4.0 Requires-Dist:
+nltk<3.7.1,>=3.6.6 Requires-Dist: rouge-score==0.0.4 Requires-Dist: scikit-
+learn Requires-Dist: tqdm Requires-Dist: validators Provides-Extra: prism
+Requires-Dist: fairseq==0.9.0; extra == "prism" Requires-Dist:
+numpy<1.24,>=1.23; extra == "prism" Provides-Extra: metrics Requires-Dist:
+sacrebleu>=2.0.0; extra == "metrics" Requires-Dist: bert_score==0.3.11; extra
+== "metrics" Requires-Dist: jiwer>=2.3.0; extra == "metrics" Requires-Dist:
+seqeval==1.2.2; extra == "metrics" Requires-Dist: sentencepiece<0.2,>=0.1.99;
+extra == "metrics" Requires-Dist: unbabel-comet==2.0.1; extra == "metrics"
+Requires-Dist: protobuf<3.21,>=3.20.3; extra == "metrics" Requires-Dist:
+fairseq==0.9.0; extra == "metrics" Requires-Dist: numpy<1.24,>=1.23; extra ==
+"metrics" Provides-Extra: dev Requires-Dist: black==21.7b0; extra == "dev"
+Requires-Dist: deepdiff==5.5.0; extra == "dev" Requires-Dist: flake8==3.9.2;
+extra == "dev" Requires-Dist: isort==5.9.2; extra == "dev" Requires-Dist:
+pytest>=7.0.1; extra == "dev" Requires-Dist: pytest-cov>=3.0.0; extra == "dev"
+Requires-Dist: pytest-timeout>=2.1.0; extra == "dev" Requires-Dist:
+sacrebleu>=2.0.0; extra == "dev" Requires-Dist: bert_score==0.3.11; extra ==
+"dev" Requires-Dist: jiwer>=2.3.0; extra == "dev" Requires-Dist:
+seqeval==1.2.2; extra == "dev" Requires-Dist: sentencepiece<0.2,>=0.1.99; extra
+== "dev" Requires-Dist: unbabel-comet==2.0.1; extra == "dev" Requires-Dist:
+protobuf<3.21,>=3.20.3; extra == "dev" Requires-Dist: fairseq==0.9.0; extra ==
+"dev" Requires-Dist: numpy<1.24,>=1.23; extra == "dev"
                               ************ JJuurryy ************
    _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_d_o_w_n_l_o_a_d_s_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_L_a_t_e_s_t_ _R_e_l_e_a_s_e_]_[_O_p_e_n_ _i_n_ _C_o_l_a_b_]
          _[_B_u_i_l_d_ _s_t_a_t_u_s_]_[_D_e_p_e_n_d_e_n_c_i_e_s_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_L_i_c_e_n_s_e_:_ _M_I_T_]
                                      _[_D_O_I_]
 A comprehensive toolkit for evaluating NLP experiments offering various
 automated metrics. Jury offers a smooth and easy-to-use interface. It uses a
 more advanced version of [evaluate](https://github.com/huggingface/evaluate/
@@ -136,15 +158,15 @@
 _compute_single_pred_multi_ref( self, predictions, references, reduce_fn =
 None, **kwargs ): raise NotImplementedError def _compute_multi_pred_multi_ref
 ( self, predictions, references, reduce_fn = None, **kwargs ): raise
 NotImplementedError ``` For more details, have a look at base metric
 implementation [jury.metrics.Metric](./jury/metrics/_base.py) ##
                                  Contributing
 PRs are welcomed as always :) ### Installation git clone https://github.com/
-obss/jury.git cd jury pip install -e .[dev] Also, you need to install the
+obss/jury.git cd jury pip install -e ".[dev]" Also, you need to install the
 packages which are available through a git source separately with the following
 command. For the folks who are curious about "why?"; a short explaination is
 that PYPI does not allow indexing a package which are directly dependent on
 non-pypi packages due to security reasons. The file `requirements-dev.txt`
 includes packages which are currently only available through a git source, or
 they are PYPI packages with no recent release or incompatible with Jury, so
 that they are added as git sources or pointing to specific commits. pip install
@@ -152,10 +174,21 @@
 run_tests.py ### Code Style To check code style, python tests/run_code_style.py
 check To format codebase, python tests/run_code_style.py format ##
                                    Citation
 If you use this package in your work, please cite it as: @misc
 {cavusoglu2023jury, title={Jury: A Comprehensive Evaluation Toolkit}, author=
 {Devrim Cavusoglu and Ulas Sert and Secil Sen and Sinan Altinuc}, year={2023},
 eprint={2310.02040}, archivePrefix={arXiv}, primaryClass={cs.CL}, doi=
-{10.48550/arXiv.2310.02040} } ##
+{10.48550/arXiv.2310.02040} } ## Community Interaction We use the GitHub Issue
+Tracker to track issues in general. Issues can be bug reports, feature requests
+or implementation of a new metric type. Please refer to the related issue
+template for opening new issues. | | Location | |------------------------------
+--|----------------------------------------------------------------------------
+------------------------| | Bug Report | [Bug Report Template](https://
+github.com/obss/jury/issues/
+new?assignees=&labels=&projects=&template=bug_report.md&title=) | | New Metric
+Request | [Request Metric Implementation](https://github.com/obss/jury/issues/
+new?assignees=&labels=&projects=&template=new-metric.md&title=) | | All other
+issues and questions | [General Issues](https://github.com/obss/jury/issues/
+new) | ##
                                     License
 Licensed under the [MIT](LICENSE) License.
```

### Comparing `jury-2.3/jury.egg-info/SOURCES.txt` & `jury-2.3.1/jury.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jury-2.3/jury.egg-info/requires.txt` & `jury-2.3.1/jury.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `jury-2.3/setup.py` & `jury-2.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/tests/jury/conftest.py` & `jury-2.3.1/tests/jury/conftest.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/tests/jury/metrics/test_accuracy.py` & `jury-2.3.1/tests/jury/metrics/test_accuracy.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/tests/jury/metrics/test_bartscore.py` & `jury-2.3.1/tests/jury/metrics/test_bartscore.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/tests/jury/metrics/test_bertscore.py` & `jury-2.3.1/tests/jury/metrics/test_bertscore.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/tests/jury/metrics/test_bleu.py` & `jury-2.3.1/tests/jury/metrics/test_bleu.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/tests/jury/metrics/test_bleurt.py` & `jury-2.3.1/tests/jury/metrics/test_bleurt.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/tests/jury/metrics/test_cer.py` & `jury-2.3.1/tests/jury/metrics/test_cer.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/tests/jury/metrics/test_chrf.py` & `jury-2.3.1/tests/jury/metrics/test_chrf.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/tests/jury/metrics/test_comet.py` & `jury-2.3.1/tests/jury/metrics/test_comet.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/tests/jury/metrics/test_custom_bleu.py` & `jury-2.3.1/tests/jury/metrics/test_custom_bleu.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/tests/jury/metrics/test_f1.py` & `jury-2.3.1/tests/jury/metrics/test_f1.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/tests/jury/metrics/test_meteor.py` & `jury-2.3.1/tests/jury/metrics/test_meteor.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/tests/jury/metrics/test_precision.py` & `jury-2.3.1/tests/jury/metrics/test_precision.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/tests/jury/metrics/test_prism.py` & `jury-2.3.1/tests/jury/metrics/test_prism.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/tests/jury/metrics/test_recall.py` & `jury-2.3.1/tests/jury/metrics/test_recall.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/tests/jury/metrics/test_rouge.py` & `jury-2.3.1/tests/jury/metrics/test_rouge.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/tests/jury/metrics/test_sacrebleu.py` & `jury-2.3.1/tests/jury/metrics/test_sacrebleu.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/tests/jury/metrics/test_seqeval.py` & `jury-2.3.1/tests/jury/metrics/test_seqeval.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/tests/jury/metrics/test_squad.py` & `jury-2.3.1/tests/jury/metrics/test_squad.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/tests/jury/metrics/test_ter.py` & `jury-2.3.1/tests/jury/metrics/test_ter.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/tests/jury/metrics/test_wer.py` & `jury-2.3.1/tests/jury/metrics/test_wer.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/tests/jury/test_cli.py` & `jury-2.3.1/tests/jury/test_cli.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/tests/jury/test_jury.py` & `jury-2.3.1/tests/jury/test_jury.py`

 * *Files identical despite different names*

### Comparing `jury-2.3/tests/jury/test_utils.py` & `jury-2.3.1/tests/jury/test_utils.py`

 * *Files identical despite different names*

