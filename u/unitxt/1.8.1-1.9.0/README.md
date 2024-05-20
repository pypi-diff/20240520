# Comparing `tmp/unitxt-1.8.1.tar.gz` & `tmp/unitxt-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitxt-1.8.1.tar", last modified: Mon May  6 07:52:59 2024, max compression
+gzip compressed data, was "unitxt-1.9.0.tar", last modified: Mon May 20 12:21:07 2024, max compression
```

## Comparing `unitxt-1.8.1.tar` & `unitxt-1.9.0.tar`

### file list

```diff
@@ -1,1107 +1,1179 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.913401 unitxt-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-06 07:52:56.000000 unitxt-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-06 07:52:56.000000 unitxt-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-05-06 07:52:59.913401 unitxt-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-05-06 07:52:56.000000 unitxt-1.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-06 07:52:56.000000 unitxt-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 07:52:59.913401 unitxt-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-06 07:52:56.000000 unitxt-1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.717401 unitxt-1.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.737401 unitxt-1.8.1/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.745401 unitxt-1.8.1/src/unitxt/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/card.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.729401 unitxt-1.8.1/src/unitxt/catalog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.749401 unitxt-1.8.1/src/unitxt/catalog/augmentors/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/augmentors/augment_whitespace_model_input.json
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/augmentors/augment_whitespace_prefix_and_suffix_task_input.json
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/augmentors/augment_whitespace_task_input.json
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/augmentors/no_augmentation.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.757401 unitxt-1.8.1/src/unitxt/catalog/cards/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.757401 unitxt-1.8.1/src/unitxt/catalog/cards/20_newsgroups/
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/20_newsgroups/sklearn.json
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/20_newsgroups.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.717401 unitxt-1.8.1/src/unitxt/catalog/cards/CFPB/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.761401 unitxt-1.8.1/src/unitxt/catalog/cards/CFPB/product/
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/CFPB/product/2023.json
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/CFPB/product/watsonx.json
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/ag_news.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.761401 unitxt-1.8.1/src/unitxt/catalog/cards/ai2_arc/
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/ai2_arc/arc_challenge.json
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/ai2_arc/arc_easy.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.761401 unitxt-1.8.1/src/unitxt/catalog/cards/almost_evil/
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/almost_evil/de.json
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/almost_evil/en.json
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/almost_evil/es.json
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/almost_evil/fr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/almost_evil/it.json
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/almost_evil/nl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/almost_evil/pt.json
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/almost_evil/ru.json
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/almost_evil.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.773401 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/af_ZA.json
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.773401 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/all_1/
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/all_1/1.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/am_ET.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/ar_SA.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/az_AZ.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/bn_BD.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/ca_ES.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/cy_GB.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/da_DK.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/de_DE.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/el_GR.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/en_US.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/es_ES.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/fa_IR.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/fi_FI.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/fr_FR.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/he_IL.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/hi_IN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/hu_HU.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/hy_AM.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/id_ID.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/is_IS.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/it_IT.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/ja_JP.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/jv_ID.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/ka_GE.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/km_KH.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/kn_IN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/ko_KR.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/lv_LV.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/ml_IN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/mn_MN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/ms_MY.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/my_MM.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/nb_NO.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/nl_NL.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/pl_PL.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/pt_PT.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/ro_RO.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/ru_RU.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/sl_SL.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/sq_AL.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/sv_SE.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/sw_KE.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/ta_IN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/te_IN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/th_TH.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/tl_PH.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/tr_TR.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/ur_PK.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/vi_VN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/zh_CN.json
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/amazon_mass/zh_TW.json
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/argument_topic.json
--rw-r--r--   0 runner    (1001) docker     (127)    13266 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/atis.json
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/atta_q.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.773401 unitxt-1.8.1/src/unitxt/catalog/cards/babi/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/babi/qa.json
--rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/banking77.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.793401 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/acm_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/afr_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/als_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/amh_ethi.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/apc_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/arb_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/arb_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/ars_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/ary_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/arz_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/asm_beng.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/azj_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/bam_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/ben_beng.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/ben_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/bod_tibt.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/bul_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/cat_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/ceb_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/ces_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/ckb_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/dan_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/deu_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/ell_grek.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/eng_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/est_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/eus_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/fin_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/fra_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/fuv_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/gaz_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/grn_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/guj_gujr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/hat_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/hau_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/heb_hebr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/hin_deva.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/hin_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/hrv_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/hun_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/hye_armn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/ibo_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/ilo_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/ind_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/isl_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/ita_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/jav_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/jpn_jpan.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/kac_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/kan_knda.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/kat_geor.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/kaz_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/kea_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/khk_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/khm_khmr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/kin_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/kir_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/kor_hang.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/lao_laoo.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/lin_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/lit_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/lug_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/luo_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/lvs_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/mal_mlym.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/mar_deva.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/mkd_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/mlt_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/mri_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/mya_mymr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/nld_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/nob_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/npi_deva.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/npi_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/nso_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/nya_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/ory_orya.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/pan_guru.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/pbt_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/pes_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/plt_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/pol_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/por_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/ron_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/rus_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/shn_mymr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/sin_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/sin_sinh.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/slk_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/slv_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/sna_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/snd_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/som_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/sot_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/spa_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/srp_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/ssw_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/sun_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/swe_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/swh_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/tam_taml.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/tel_telu.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/tgk_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/tgl_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/tha_thai.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/tir_ethi.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/tsn_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/tso_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/tur_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/ukr_cyrl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/urd_arab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/urd_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/uzn_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/vie_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/war_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/wol_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/xho_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/yor_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/zho_hans.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/zho_hant.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/zsm_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/belebele/zul_latn.json
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/bold.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.793401 unitxt-1.8.1/src/unitxt/catalog/cards/boolq/
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/boolq/classification.json
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/boolq/multiple_choice.json
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/claim_stance_topic.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.797401 unitxt-1.8.1/src/unitxt/catalog/cards/clinc_oos/
--rw-r--r--   0 runner    (1001) docker     (127)    12619 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/clinc_oos/imbalanced.json
--rw-r--r--   0 runner    (1001) docker     (127)    12613 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/clinc_oos/plus.json
--rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/clinc_oos/small.json
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/cnn_dailymail.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.797401 unitxt-1.8.1/src/unitxt/catalog/cards/coedit/
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/coedit/paraphrase.json
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/coedit/preference.json
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/coedit/rewriting.json
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/coedit/selection.json
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/coedit_error_detection.json
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/coedit_gec.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.717401 unitxt-1.8.1/src/unitxt/catalog/cards/cohere_for_ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.797401 unitxt-1.8.1/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/arb.json
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/eng.json
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/por.json
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tel.json
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tur.json
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/yor.json
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/zho.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.797401 unitxt-1.8.1/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/fra.json
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/spa.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.801401 unitxt-1.8.1/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/deu.json
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/eng.json
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/fra.json
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/jpn.json
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/por.json
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/spa.json
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/cola.json
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/copa.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.801401 unitxt-1.8.1/src/unitxt/catalog/cards/coqa/
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/coqa/completion.json
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/coqa/qa.json
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/dart.json
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/dbpedia_14.json
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/ethos_binary.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.801401 unitxt-1.8.1/src/unitxt/catalog/cards/ffqa_filtered/
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/ffqa_filtered/16k.json
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/ffqa_filtered/2k.json
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/ffqa_filtered/4k.json
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/ffqa_filtered/8k.json
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/financial_tweets.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.801401 unitxt-1.8.1/src/unitxt/catalog/cards/head_qa/
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/head_qa/en.json
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/head_qa/es.json
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/hellaswag.json
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/hh_rlhf.json
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/human_eval.json
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/law_stack_exchange.json
--rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/ledgar.json
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mbpp.json
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/medical_abstracts.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.801401 unitxt-1.8.1/src/unitxt/catalog/cards/mlsum/
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mlsum/de.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mlsum/es.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mlsum/fr.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mlsum/ru.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mlsum/tu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.813401 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/abstract_algebra.json
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/anatomy.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/astronomy.json
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/business_ethics.json
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/clinical_knowledge.json
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/college_biology.json
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/college_chemistry.json
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/college_computer_science.json
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/college_mathematics.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/college_medicine.json
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/college_physics.json
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/computer_security.json
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/conceptual_physics.json
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/econometrics.json
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/electrical_engineering.json
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/elementary_mathematics.json
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/formal_logic.json
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/global_facts.json
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/high_school_biology.json
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/high_school_chemistry.json
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/high_school_computer_science.json
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/high_school_european_history.json
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/high_school_geography.json
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/high_school_government_and_politics.json
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/high_school_macroeconomics.json
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/high_school_mathematics.json
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/high_school_microeconomics.json
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/high_school_physics.json
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/high_school_psychology.json
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/high_school_statistics.json
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/high_school_us_history.json
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/high_school_world_history.json
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/human_aging.json
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/human_sexuality.json
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/international_law.json
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/jurisprudence.json
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/logical_fallacies.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/machine_learning.json
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/management.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/marketing.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/medical_genetics.json
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/miscellaneous.json
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/moral_disputes.json
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/moral_scenarios.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/nutrition.json
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/philosophy.json
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/prehistory.json
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/professional_accounting.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/professional_law.json
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/professional_medicine.json
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/professional_psychology.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/public_relations.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/security_studies.json
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/sociology.json
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/us_foreign_policy.json
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/virology.json
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/world_religions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mnli.json
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/mrpc.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.813401 unitxt-1.8.1/src/unitxt/catalog/cards/multidoc2dial/
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/multidoc2dial/abstractive.json
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/multidoc2dial/extractive.json
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/news_category_classification_headline.json
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/openbook_qa.json
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/piqa.json
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/pop_qa.json
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/qnli.json
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/qqp.json
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/race_all.json
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/race_high.json
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/race_middle.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.721401 unitxt-1.8.1/src/unitxt/catalog/cards/rag/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.813401 unitxt-1.8.1/src/unitxt/catalog/cards/rag/model_response_assessment/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/rag/model_response_assessment/llm_as_judge_using_mt_bench_template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.813401 unitxt-1.8.1/src/unitxt/catalog/cards/reuters21578/
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/reuters21578/ModApte.json
--rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/reuters21578/ModHayes.json
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/reuters21578/ModLewis.json
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/rte.json
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/sciq.json
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/squad.json
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/sst2.json
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/stsb.json
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/summarize_from_human_feedback.json
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/tab_fact.json
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/tablerow_classify.json
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/toxigen.json
--rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/trec.json
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/unfair_tos.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.721401 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.813401 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/ceb/
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/ceb/gja.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.813401 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/da/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/da/ddt.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.813401 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/de/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/de/pud.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.813401 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/en/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/en/ewt.json
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/en/pud.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.813401 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/hr/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/hr/set.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.813401 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/pt/
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/pt/bosque.json
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/pt/pud.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.813401 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/ru/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/ru/pud.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.813401 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/sk/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/sk/snk.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.813401 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/sr/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/sr/set.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.817401 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/sv/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/sv/pud.json
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/sv/talbanken.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.817401 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/tl/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/tl/trg.json
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/tl/ugnayan.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.817401 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/zh/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/zh/gsd.json
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/zh/gsdsimp.json
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/zh/pud.json
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/wiki_bio.json
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/wikitq.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.817401 unitxt-1.8.1/src/unitxt/catalog/cards/winogrande/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/winogrande/debiased.json
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/winogrande/l.json
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/winogrande/m.json
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/winogrande/s.json
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/winogrande/xl.json
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/winogrande/xs.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.817401 unitxt-1.8.1/src/unitxt/catalog/cards/wmt/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/wmt/en_de.json
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/wmt/en_fr.json
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/wmt/en_ro.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.817401 unitxt-1.8.1/src/unitxt/catalog/cards/wnli/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/wnli/truthfulness.json
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/wnli.json
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/wsc.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.825401 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/amharic.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/arabic.json
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/azerbaijani.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/bengali.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/burmese.json
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/chinese_simplified.json
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/chinese_traditional.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/english.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/french.json
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/gujarati.json
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/hausa.json
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/hindi.json
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/igbo.json
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/indonesian.json
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/japanese.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/kirundi.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/korean.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/kyrgyz.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/marathi.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/nepali.json
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/oromo.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/pashto.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/persian.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/pidgin.json
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/portuguese.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/punjabi.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/russian.json
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/scottish_gaelic.json
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/serbian_cyrillic.json
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/serbian_latin.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/sinhala.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/somali.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/spanish.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/swahili.json
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/tamil.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/telugu.json
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/thai.json
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/tigrinya.json
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/turkish.json
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/ukrainian.json
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/urdu.json
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/uzbek.json
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/vietnamese.json
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/welsh.json
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/yoruba.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.829401 unitxt-1.8.1/src/unitxt/catalog/cards/xnli/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xnli/ar.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xnli/bg.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xnli/de.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xnli/el.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xnli/en.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xnli/es.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xnli/fr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xnli/hi.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xnli/ru.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xnli/sw.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xnli/th.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xnli/tr.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xnli/ur.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xnli/vi.json
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xnli/zh.json
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xsum.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.829401 unitxt-1.8.1/src/unitxt/catalog/cards/xwinogrande/
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xwinogrande/en.json
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xwinogrande/jp.json
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xwinogrande/pt.json
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xwinogrande/ru.json
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/xwinogrande/zh.json
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/cards/yahoo_answers_topics.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.833401 unitxt-1.8.1/src/unitxt/catalog/formats/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/formats/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/formats/empty_input_output_separator.json
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/formats/human_assistant.json
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/formats/llama.json
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/formats/llama2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.833401 unitxt-1.8.1/src/unitxt/catalog/formats/models/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/formats/models/alpaca_instruct.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.833401 unitxt-1.8.1/src/unitxt/catalog/formats/models/flan/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/formats/models/flan/exq_exa.json
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/formats/models/flan/few_shot.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.833401 unitxt-1.8.1/src/unitxt/catalog/formats/models/labradorite/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/formats/models/labradorite/few_shot.json
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/formats/models/labradorite/zero_shot.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.833401 unitxt-1.8.1/src/unitxt/catalog/formats/models/mistral/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.833401 unitxt-1.8.1/src/unitxt/catalog/formats/models/mistral/instruction/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/formats/models/mistral/instruction/with_system_prompt.json
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/formats/models/mistral/instruction.json
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/formats/textual_assistant.json
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/formats/user_agent.json
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/formats/user_assistant.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.841401 unitxt-1.8.1/src/unitxt/catalog/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/accuracy_binary.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.841401 unitxt-1.8.1/src/unitxt/catalog/metrics/bert_score/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/bert_score/deberta_base_mnli.json
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/bert_score/deberta_large_mnli.json
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/bert_score/deberta_v3_base_mnli_xnli_ml.json
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/bert_score/deberta_xlarge_mnli.json
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/bert_score/distilbert_base_uncased.json
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/bleu.json
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/char_edit_dist_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/char_edit_distance.json
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/f1_binary.json
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/f1_macro.json
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/f1_macro_multi_label.json
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/f1_micro.json
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/f1_micro_multi_label.json
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/f1_weighted.json
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/kendalltau_b.json
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/kpa.json
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/map.json
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/matthews_correlation.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/max_accuracy_binary.json
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/max_f1_binary.json
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/mrr.json
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/ndcg.json
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/ner.json
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/normalized_sacrebleu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.841401 unitxt-1.8.1/src/unitxt/catalog/metrics/perplexity/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/perplexity/flan_t5_small.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.841401 unitxt-1.8.1/src/unitxt/catalog/metrics/perplexity_a/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/perplexity_a/flan_t5_small.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.841401 unitxt-1.8.1/src/unitxt/catalog/metrics/perplexity_chat/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/perplexity_chat/flan_t5_small.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.841401 unitxt-1.8.1/src/unitxt/catalog/metrics/perplexity_nli/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/perplexity_nli/t5_nli_mixture.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.841401 unitxt-1.8.1/src/unitxt/catalog/metrics/perplexity_q/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/perplexity_q/flan_t5_small.json
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/precision_binary.json
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/precision_macro_multi_label.json
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/precision_micro_multi_label.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.845401 unitxt-1.8.1/src/unitxt/catalog/metrics/rag/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/rag/answer_correctness.json
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/rag/answer_inference.json
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/rag/answer_reward.json
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/rag/bert_k_precision.json
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/rag/bert_k_precision_ml.json
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/rag/bert_recall.json
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/rag/bert_recall_ml.json
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/rag/context_correctness.json
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/rag/context_perplexity.json
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/rag/context_relevance.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.845401 unitxt-1.8.1/src/unitxt/catalog/metrics/rag/correctness/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/rag/correctness/llama_index_by_gpt_3_5_turbo.json
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/rag/correctness/llama_index_by_mock.json
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/rag/faithfulness.json
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/rag/k_precision.json
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/rag/map.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.845401 unitxt-1.8.1/src/unitxt/catalog/metrics/rag/model_response_assessment/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/rag/model_response_assessment/llm_as_judge_by_flan_t5_large_on_hf_pipeline_using_mt_bench_template.json
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/rag/mrr.json
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/rag/recall.json
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/recall_binary.json
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/recall_macro_multi_label.json
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/recall_micro_multi_label.json
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/regard.json
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/rerank_recall.json
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/retrieval_at_k.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.845401 unitxt-1.8.1/src/unitxt/catalog/metrics/reward/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/reward/deberta_v3_large_v2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.849401 unitxt-1.8.1/src/unitxt/catalog/metrics/robustness/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_cohens_h_paraphrase_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_cohens_h_paraphrase_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_hedges_g_paraphrase_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_hedges_g_paraphrase_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/robustness/fixed_group_mean_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/robustness/fixed_group_mean_baseline_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/robustness/fixed_group_mean_baseline_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/robustness/fixed_group_mean_paraphrase_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/robustness/fixed_group_mean_paraphrase_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/robustness/fixed_group_mean_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/robustness/fixed_group_norm_cohens_h_paraphrase_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/robustness/fixed_group_norm_cohens_h_paraphrase_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/robustness/fixed_group_norm_hedges_g_paraphrase_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/robustness/fixed_group_norm_hedges_g_paraphrase_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/robustness/fixed_group_pdr_paraphrase_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/robustness/fixed_group_pdr_paraphrase_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/robustness/group_mean_accuracy.json
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/robustness/group_mean_string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/robustness/group_mean_token_overlap.json
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/roc_auc.json
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/rouge.json
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/rouge_with_confidence_intervals.json
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/sacrebleu.json
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/safety.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.849401 unitxt-1.8.1/src/unitxt/catalog/metrics/sentence_bert/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/sentence_bert/mpnet_base_v2.json
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/spearman.json
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/squad.json
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/string_containment.json
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/token_overlap.json
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/token_overlap_with_context.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/unsorted_list_exact_match.json
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/metrics/wer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.725401 unitxt-1.8.1/src/unitxt/catalog/operators/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.725401 unitxt-1.8.1/src/unitxt/catalog/operators/balancers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.849401 unitxt-1.8.1/src/unitxt/catalog/operators/balancers/classification/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/operators/balancers/classification/by_label.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.849401 unitxt-1.8.1/src/unitxt/catalog/operators/balancers/multi_label/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/operators/balancers/multi_label/zero_vs_many_labels.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.849401 unitxt-1.8.1/src/unitxt/catalog/operators/balancers/ner/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/operators/balancers/ner/zero_vs_many_entities.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.849401 unitxt-1.8.1/src/unitxt/catalog/operators/balancers/qa/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/operators/balancers/qa/by_answer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.853401 unitxt-1.8.1/src/unitxt/catalog/processors/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/capitalize.json
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/cast_to_float_return_nan_if_failed.json
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/cast_to_float_return_zero_if_failed.json
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/convert_to_boolean.json
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/dict_of_lists_to_value_key_pairs.json
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/extract_from_double_brackets.json
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/extract_mt_bench_judgment.json
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/first_character.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/get_string_after_colon.json
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/hate_speech_or_not_hate_speech.json
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/list_to_empty_entity_tuples.json
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/load_json.json
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/load_json_from_predictions.json
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/lower_case.json
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/lower_case_till_punc.json
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/match_closest_option.json
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/predictions_yes_1_else_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/remove_none_from_list.json
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/stance_to_pro_con.json
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/str_to_float_format.json
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/substring.json
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/take_first_non_empty_line.json
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/take_first_word.json
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/to_list_by_comma.json
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/to_span_label_pairs.json
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/to_span_label_pairs_surface_only.json
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/to_string.json
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/to_string_stripped.json
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/to_yes_or_none.json
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/toxic_or_not_toxic.json
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/processors/yes_no_to_int.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.857401 unitxt-1.8.1/src/unitxt/catalog/splitters/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/splitters/default.json
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/splitters/diverse_labels_sampler.json
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/splitters/large_no_dev.json
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/splitters/large_no_test.json
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/splitters/small_no_dev.json
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/splitters/small_no_test.json
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/splitters/test_only.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.725401 unitxt-1.8.1/src/unitxt/catalog/system_prompt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.857401 unitxt-1.8.1/src/unitxt/catalog/system_prompt/models/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/system_prompt/models/japanese_llama.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.857401 unitxt-1.8.1/src/unitxt/catalog/system_prompts/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/system_prompts/empty.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.857401 unitxt-1.8.1/src/unitxt/catalog/system_prompts/models/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/system_prompts/models/alpaca.json
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/system_prompts/models/labradorite.json
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/system_prompts/models/llama.json
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/system_prompts/models/llama2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.857401 unitxt-1.8.1/src/unitxt/catalog/tasks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.857401 unitxt-1.8.1/src/unitxt/catalog/tasks/classification/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.857401 unitxt-1.8.1/src/unitxt/catalog/tasks/classification/binary/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/classification/binary/zero_or_one.json
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/classification/binary.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.857401 unitxt-1.8.1/src/unitxt/catalog/tasks/classification/multi_class/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/classification/multi_class/relation.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/classification/multi_class.json
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/classification/multi_label.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.857401 unitxt-1.8.1/src/unitxt/catalog/tasks/completion/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/completion/abstractive.json
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/completion/extractive.json
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/completion/multiple_choice.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.857401 unitxt-1.8.1/src/unitxt/catalog/tasks/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/evaluation/preference.json
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/generation.json
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/grammatical_error_correction.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.857401 unitxt-1.8.1/src/unitxt/catalog/tasks/ner/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/ner/all_entity_types.json
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/ner/single_entity_type.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.857401 unitxt-1.8.1/src/unitxt/catalog/tasks/qa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.861401 unitxt-1.8.1/src/unitxt/catalog/tasks/qa/multiple_choice/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/qa/multiple_choice/open.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.861401 unitxt-1.8.1/src/unitxt/catalog/tasks/qa/multiple_choice/with_context/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/qa/multiple_choice/with_context/with_topic.json
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/qa/multiple_choice/with_context.json
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/qa/multiple_choice/with_topic.json
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/qa/open.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.861401 unitxt-1.8.1/src/unitxt/catalog/tasks/qa/with_context/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/qa/with_context/abstractive.json
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/qa/with_context/extractive.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.861401 unitxt-1.8.1/src/unitxt/catalog/tasks/rag/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/rag/model_response_assessment.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.861401 unitxt-1.8.1/src/unitxt/catalog/tasks/regression/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/regression/single_text.json
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/regression/two_texts.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.861401 unitxt-1.8.1/src/unitxt/catalog/tasks/rewriting/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/rewriting/by_attribute.json
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/rewriting/paraphrase.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.861401 unitxt-1.8.1/src/unitxt/catalog/tasks/selection/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/selection/by_attribute.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.861401 unitxt-1.8.1/src/unitxt/catalog/tasks/span_labeling/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/span_labeling/extraction.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.861401 unitxt-1.8.1/src/unitxt/catalog/tasks/summarization/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/summarization/abstractive.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.861401 unitxt-1.8.1/src/unitxt/catalog/tasks/targeted_sentiment_extraction/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/targeted_sentiment_extraction/all_sentiment_classes.json
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/targeted_sentiment_extraction/single_sentiment_class.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.861401 unitxt-1.8.1/src/unitxt/catalog/tasks/translation/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/tasks/translation/directed.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.861401 unitxt-1.8.1/src/unitxt/catalog/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.729401 unitxt-1.8.1/src/unitxt/catalog/templates/classification/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.865401 unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_class/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_class/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_class/default.json
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_class/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_class/instruction.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.865401 unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_class/relation/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_class/relation/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_class/relation/default.json
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_class/relation/simple.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.865401 unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_1.json
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_2.json
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_3.json
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_4.json
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_5.json
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_6.json
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_7.json
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_class/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.865401 unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_label/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_label/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_label/default.json
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_label/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_label/instruction.json
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_label/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.729401 unitxt-1.8.1/src/unitxt/catalog/templates/completion/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.865401 unitxt-1.8.1/src/unitxt/catalog/templates/completion/abstractive/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/completion/abstractive/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/completion/abstractive/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/completion/abstractive/standard.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.869401 unitxt-1.8.1/src/unitxt/catalog/templates/completion/multiple_choice/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/completion/multiple_choice/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/completion/multiple_choice/enumerated.json
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/completion/multiple_choice/simple.json
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/completion/multiple_choice/standard.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/completion/multiple_choice/title.json
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/empty.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.729401 unitxt-1.8.1/src/unitxt/catalog/templates/evaluation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.869401 unitxt-1.8.1/src/unitxt/catalog/templates/evaluation/preference/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/evaluation/preference/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/evaluation/preference/default.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.869401 unitxt-1.8.1/src/unitxt/catalog/templates/generation/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/generation/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/generation/default.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.869401 unitxt-1.8.1/src/unitxt/catalog/templates/grammatical_error_correction/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/grammatical_error_correction/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/grammatical_error_correction/simple.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.869401 unitxt-1.8.1/src/unitxt/catalog/templates/grammatical_error_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/grammatical_error_detection/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/grammatical_error_detection/yes_no.json
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/key_val.json
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/key_val_with_new_lines.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.733401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.869401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/match.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.869401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.869401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/de/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/de/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/de/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/de/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/de/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.873401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/es/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/es/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/es/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/es/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/es/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.873401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/helm.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.873401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.873401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.873401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/match.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.873401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.877401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.877401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.877401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/helm.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.877401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.877401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.881401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.881401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.881401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fm_eval.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.881401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/helm.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.881401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/match.json
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.885401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.885401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.885401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.885401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fm_eval.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.885401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/helm.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.889401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/match.json
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/mmlu.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.889401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/helm.json
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/lm_eval_harness.json
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/mmlu.json
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.889401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/open/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/open/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/open/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/open/simple.json
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/open/simple2.json
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/open/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.889401 unitxt-1.8.1/src/unitxt/catalog/templates/qa/with_context/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/with_context/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/with_context/ffqa.json
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/with_context/question_first.json
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/with_context/simple.json
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/with_context/simple2.json
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/with_context/title.json
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/qa/with_context/with_type.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.733401 unitxt-1.8.1/src/unitxt/catalog/templates/rag/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.889401 unitxt-1.8.1/src/unitxt/catalog/templates/rag/model_response_assessment/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/rag/model_response_assessment/llm_as_judge_using_mt_bench_template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.733401 unitxt-1.8.1/src/unitxt/catalog/templates/regression/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.889401 unitxt-1.8.1/src/unitxt/catalog/templates/regression/single_text/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/regression/single_text/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/regression/single_text/simple.json
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/regression/single_text/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.893401 unitxt-1.8.1/src/unitxt/catalog/templates/regression/two_texts/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/regression/two_texts/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.893401 unitxt-1.8.1/src/unitxt/catalog/templates/regression/two_texts/similarity/
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/regression/two_texts/similarity/flan.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/regression/two_texts/simple.json
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/regression/two_texts/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.733401 unitxt-1.8.1/src/unitxt/catalog/templates/rewriting/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.893401 unitxt-1.8.1/src/unitxt/catalog/templates/rewriting/by_attribute/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/rewriting/by_attribute/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/rewriting/by_attribute/default.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.893401 unitxt-1.8.1/src/unitxt/catalog/templates/rewriting/paraphrase/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/rewriting/paraphrase/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/rewriting/paraphrase/default.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.733401 unitxt-1.8.1/src/unitxt/catalog/templates/selection/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.893401 unitxt-1.8.1/src/unitxt/catalog/templates/selection/by_attribute/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/selection/by_attribute/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/selection/by_attribute/default.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.733401 unitxt-1.8.1/src/unitxt/catalog/templates/span_labeling/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.893401 unitxt-1.8.1/src/unitxt/catalog/templates/span_labeling/extraction/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/span_labeling/extraction/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/span_labeling/extraction/carry.json
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/span_labeling/extraction/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/span_labeling/extraction/extract.json
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/span_labeling/extraction/having.json
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/span_labeling/extraction/identify.json
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/span_labeling/extraction/title.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.733401 unitxt-1.8.1/src/unitxt/catalog/templates/summarization/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.897401 unitxt-1.8.1/src/unitxt/catalog/templates/summarization/abstractive/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/summarization/abstractive/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/summarization/abstractive/casual.json
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/summarization/abstractive/formal.json
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/summarization/abstractive/formal_without_label.json
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/summarization/abstractive/full.json
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/summarization/abstractive/instructive.json
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/summarization/abstractive/one_sentence.json
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/summarization/abstractive/passive.json
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/summarization/abstractive/professional.json
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/summarization/abstractive/title.json
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/summarization/abstractive/write_succinct.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.897401 unitxt-1.8.1/src/unitxt/catalog/templates/targeted_sentiment_extraction/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/targeted_sentiment_extraction/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.897401 unitxt-1.8.1/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/convert_with_explicit_keys.json
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/convert_with_implicit_keys.json
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/targeted_sentiment_extraction/carry_sentiment.json
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/targeted_sentiment_extraction/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/targeted_sentiment_extraction/entities_sentiment.json
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/targeted_sentiment_extraction/extract_sentiment.json
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/targeted_sentiment_extraction/having_sentiment.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.897401 unitxt-1.8.1/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/having_sentiment.json
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/sentiment_extracted.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.897401 unitxt-1.8.1/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/having_sentiment.json
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/sentiment_extracted.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.901401 unitxt-1.8.1/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/empty.json
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/having_sentiment.json
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/sentiment_extracted.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.733401 unitxt-1.8.1/src/unitxt/catalog/templates/translation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.901401 unitxt-1.8.1/src/unitxt/catalog/templates/translation/directed/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/translation/directed/all.json
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/translation/directed/casual.json
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/translation/directed/formal.json
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/translation/directed/instructional.json
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/translation/directed/playful.json
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/translation/directed/simple.json
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog/templates/translation/directed/title.json
--rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/collections_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    17311 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/deprecation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/dialog_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    23755 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/dict_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/eval_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8209 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/fusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/generator_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/hf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/instructions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/llm_as_judge.py
--rw-r--r--   0 runner    (1001) docker     (127)    17915 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/metric_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   137698 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/normalizers.py
--rw-r--r--   0 runner    (1001) docker     (127)    21477 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)    80904 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/parsing_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.901401 unitxt-1.8.1/src/unitxt/prepare_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/prepare_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/prepare_utils/card_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/prepare_utils/instructions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/random_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/recipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.901401 unitxt-1.8.1/src/unitxt/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.901401 unitxt-1.8.1/src/unitxt/service/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/service/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/service/metrics/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/service/metrics/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/settings_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/span_lableing_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    12229 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/split_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11430 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/splitters.py
--rw-r--r--   0 runner    (1001) docker     (127)    14272 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/standard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/string_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    17231 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/struct_data_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/system_prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/task.py
--rw-r--r--   0 runner    (1001) docker     (127)    20531 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.905401 unitxt-1.8.1/src/unitxt/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/test_utils/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/test_utils/card.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/test_utils/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/test_utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/test_utils/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/test_utils/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/text_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    31413 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/type_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.905401 unitxt-1.8.1/src/unitxt/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    56810 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/ui/banner.png
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/ui/gradio_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/ui/load_catalog_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    14100 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/ui/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/ui/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/ui/ui_tester.py
--rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/ui/ui_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-06 07:52:56.000000 unitxt-1.8.1/src/unitxt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:52:59.905401 unitxt-1.8.1/src/unitxt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-05-06 07:52:59.000000 unitxt-1.8.1/src/unitxt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    50258 2024-05-06 07:52:59.000000 unitxt-1.8.1/src/unitxt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 07:52:59.000000 unitxt-1.8.1/src/unitxt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-06 07:52:59.000000 unitxt-1.8.1/src/unitxt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-06 07:52:59.000000 unitxt-1.8.1/src/unitxt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-06 07:52:59.000000 unitxt-1.8.1/src/unitxt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.349566 unitxt-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-20 12:20:59.000000 unitxt-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-20 12:20:59.000000 unitxt-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9053 2024-05-20 12:21:07.349566 unitxt-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-05-20 12:20:59.000000 unitxt-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-20 12:20:59.000000 unitxt-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 12:21:07.349566 unitxt-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-20 12:20:59.000000 unitxt-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.153567 unitxt-1.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.177567 unitxt-1.9.0/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.189567 unitxt-1.9.0/src/unitxt/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11722 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/card.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.169567 unitxt-1.9.0/src/unitxt/catalog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.189567 unitxt-1.9.0/src/unitxt/catalog/augmentors/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/augmentors/augment_whitespace_model_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/augmentors/augment_whitespace_prefix_and_suffix_task_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/augmentors/augment_whitespace_task_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/augmentors/no_augmentation.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.197567 unitxt-1.9.0/src/unitxt/catalog/cards/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.197567 unitxt-1.9.0/src/unitxt/catalog/cards/20_newsgroups/
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/20_newsgroups/sklearn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/20_newsgroups.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.157567 unitxt-1.9.0/src/unitxt/catalog/cards/CFPB/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.197567 unitxt-1.9.0/src/unitxt/catalog/cards/CFPB/product/
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/CFPB/product/2023.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/CFPB/product/watsonx.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/ag_news.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.197567 unitxt-1.9.0/src/unitxt/catalog/cards/ai2_arc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/ai2_arc/arc_challenge.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/ai2_arc/arc_easy.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.201567 unitxt-1.9.0/src/unitxt/catalog/cards/almost_evil/
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/almost_evil/de.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/almost_evil/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/almost_evil/es.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/almost_evil/fr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/almost_evil/it.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/almost_evil/nl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/almost_evil/pt.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/almost_evil/ru.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/almost_evil.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.209567 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/af_ZA.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7734 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.209567 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/all_1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/all_1/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/am_ET.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/ar_SA.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/az_AZ.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/bn_BD.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/ca_ES.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/cy_GB.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/da_DK.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/de_DE.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/el_GR.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/en_US.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/es_ES.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/fa_IR.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/fi_FI.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/fr_FR.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/he_IL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/hi_IN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/hu_HU.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/hy_AM.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/id_ID.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/is_IS.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/it_IT.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/ja_JP.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/jv_ID.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/ka_GE.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/km_KH.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/kn_IN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/ko_KR.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/lv_LV.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/ml_IN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/mn_MN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/ms_MY.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/my_MM.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/nb_NO.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/nl_NL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/pl_PL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/pt_PT.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/ro_RO.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/ru_RU.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/sl_SL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/sq_AL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/sv_SE.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/sw_KE.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/ta_IN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/te_IN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/th_TH.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/tl_PH.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/tr_TR.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/ur_PK.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/vi_VN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/zh_CN.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/amazon_mass/zh_TW.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/argument_topic.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13341 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/atis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/atta_q.json
+-rw-r--r--   0 runner    (1001) docker     (127)    71437 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/attaq_500.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.209567 unitxt-1.9.0/src/unitxt/catalog/cards/babi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/babi/qa.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/banking77.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.229567 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/acm_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/afr_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/als_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/amh_ethi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/apc_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/arb_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/arb_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/ars_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/ary_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/arz_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/asm_beng.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/azj_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/bam_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/ben_beng.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/ben_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/bod_tibt.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/bul_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/cat_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/ceb_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/ces_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/ckb_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/dan_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/deu_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/ell_grek.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/eng_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/est_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/eus_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/fin_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/fra_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/fuv_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/gaz_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/grn_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/guj_gujr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/hat_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/hau_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/heb_hebr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/hin_deva.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/hin_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/hrv_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/hun_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/hye_armn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/ibo_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/ilo_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/ind_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/isl_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/ita_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/jav_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/jpn_jpan.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/kac_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/kan_knda.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/kat_geor.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/kaz_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/kea_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/khk_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/khm_khmr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/kin_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/kir_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/kor_hang.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/lao_laoo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/lin_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/lit_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/lug_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/luo_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/lvs_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/mal_mlym.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/mar_deva.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/mkd_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/mlt_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/mri_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/mya_mymr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/nld_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/nob_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/npi_deva.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/npi_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/nso_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/nya_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/ory_orya.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/pan_guru.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/pbt_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/pes_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/plt_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/pol_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/por_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/ron_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/rus_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/shn_mymr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/sin_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/sin_sinh.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/slk_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/slv_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/sna_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/snd_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/som_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/sot_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/spa_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/srp_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/ssw_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/sun_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/swe_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/swh_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/tam_taml.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/tel_telu.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/tgk_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/tgl_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/tha_thai.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/tir_ethi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/tsn_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/tso_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/tur_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/ukr_cyrl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/urd_arab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/urd_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/uzn_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/vie_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/war_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/wol_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/xho_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/yor_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/zho_hans.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/zho_hant.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/zsm_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/belebele/zul_latn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/billsum.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/bold.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.229567 unitxt-1.9.0/src/unitxt/catalog/cards/boolq/
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/boolq/classification.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/boolq/multiple_choice.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/claim_stance_topic.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.229567 unitxt-1.9.0/src/unitxt/catalog/cards/clinc_oos/
+-rw-r--r--   0 runner    (1001) docker     (127)    13649 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/clinc_oos/imbalanced.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13643 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/clinc_oos/plus.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13644 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/clinc_oos/small.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/cnn_dailymail.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.229567 unitxt-1.9.0/src/unitxt/catalog/cards/coedit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/coedit/paraphrase.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/coedit/preference.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/coedit/rewriting.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/coedit/selection.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/coedit_error_detection.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/coedit_gec.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.157567 unitxt-1.9.0/src/unitxt/catalog/cards/cohere_for_ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.229567 unitxt-1.9.0/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/arb.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/eng.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/por.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tel.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/tur.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/yor.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/zho.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.229567 unitxt-1.9.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/fra.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/spa.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.233567 unitxt-1.9.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/deu.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/eng.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/fra.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/jpn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/por.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/spa.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/cola.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/copa.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.233567 unitxt-1.9.0/src/unitxt/catalog/cards/coqa/
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/coqa/completion.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/coqa/qa.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/dart.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/dbpedia_14.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.157567 unitxt-1.9.0/src/unitxt/catalog/cards/dynamic_cards_for_llm_judges/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.233567 unitxt-1.9.0/src/unitxt/catalog/cards/dynamic_cards_for_llm_judges/rating/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/dynamic_cards_for_llm_judges/rating/single_turn.json
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/dynamic_cards_for_llm_judges/rating/single_turn_with_reference.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/ethos_binary.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.233567 unitxt-1.9.0/src/unitxt/catalog/cards/ffqa_filtered/
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/ffqa_filtered/16k.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/ffqa_filtered/2k.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/ffqa_filtered/4k.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/ffqa_filtered/8k.json
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/financebench.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/financial_tweets.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.233567 unitxt-1.9.0/src/unitxt/catalog/cards/head_qa/
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/head_qa/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/head_qa/es.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/hellaswag.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/hh_rlhf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/human_eval.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/law_stack_exchange.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9686 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/ledgar.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.233567 unitxt-1.9.0/src/unitxt/catalog/cards/legalbench/
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/legalbench/abercrombie.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/legalbench/corporate_lobbying.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/legalbench/function_of_decision_section.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/legalbench/international_citizenship_questions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/legalbench/proa.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mbpp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/medical_abstracts.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.233567 unitxt-1.9.0/src/unitxt/catalog/cards/mlsum/
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mlsum/de.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mlsum/es.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mlsum/fr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mlsum/ru.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mlsum/tu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.245567 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/abstract_algebra.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/anatomy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/astronomy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/business_ethics.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/clinical_knowledge.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/college_biology.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/college_chemistry.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/college_computer_science.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/college_mathematics.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/college_medicine.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/college_physics.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/computer_security.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/conceptual_physics.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/econometrics.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/electrical_engineering.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/elementary_mathematics.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/formal_logic.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/global_facts.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/high_school_biology.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/high_school_chemistry.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/high_school_computer_science.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/high_school_european_history.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/high_school_geography.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/high_school_government_and_politics.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/high_school_macroeconomics.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/high_school_mathematics.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/high_school_microeconomics.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/high_school_physics.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/high_school_psychology.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/high_school_statistics.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/high_school_us_history.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/high_school_world_history.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/human_aging.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/human_sexuality.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/international_law.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/jurisprudence.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/logical_fallacies.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/machine_learning.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/management.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/marketing.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/medical_genetics.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/miscellaneous.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/moral_disputes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/moral_scenarios.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/nutrition.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/philosophy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/prehistory.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/professional_accounting.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/professional_law.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/professional_medicine.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/professional_psychology.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/public_relations.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/security_studies.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/sociology.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/us_foreign_policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/virology.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/world_religions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mnli.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mrpc.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.157567 unitxt-1.9.0/src/unitxt/catalog/cards/mt_bench/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.245567 unitxt-1.9.0/src/unitxt/catalog/cards/mt_bench/generation/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mt_bench/generation/english_single_turn.json
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mt_bench/generation/japanese_single_turn.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.157567 unitxt-1.9.0/src/unitxt/catalog/cards/mt_bench/response_assessment/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.245567 unitxt-1.9.0/src/unitxt/catalog/cards/mt_bench/response_assessment/pairwise_comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mt_bench/response_assessment/pairwise_comparison/multi_turn_gpt4_judgement.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mt_bench/response_assessment/pairwise_comparison/multi_turn_with_reference_gpt4_judgement.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mt_bench/response_assessment/pairwise_comparison/single_turn_gpt4_judgement.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mt_bench/response_assessment/pairwise_comparison/single_turn_with_reference_gpt4_judgement.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.245567 unitxt-1.9.0/src/unitxt/catalog/cards/mt_bench/response_assessment/rating/
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mt_bench/response_assessment/rating/multi_turn_gpt4_judgement.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mt_bench/response_assessment/rating/multi_turn_with_reference_gpt4_judgement.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mt_bench/response_assessment/rating/single_turn_gpt4_judgement.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/mt_bench/response_assessment/rating/single_turn_with_reference_gpt4_judgement.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.245567 unitxt-1.9.0/src/unitxt/catalog/cards/multidoc2dial/
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/multidoc2dial/abstractive.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/multidoc2dial/extractive.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/news_category_classification_headline.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/openbook_qa.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/piqa.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/pop_qa.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/qnli.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/qqp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/race_all.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/race_high.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/race_middle.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.157567 unitxt-1.9.0/src/unitxt/catalog/cards/rag/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.245567 unitxt-1.9.0/src/unitxt/catalog/cards/rag/response_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/rag/response_generation/clapnq.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.245567 unitxt-1.9.0/src/unitxt/catalog/cards/reuters21578/
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/reuters21578/ModApte.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/reuters21578/ModHayes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/reuters21578/ModLewis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/rte.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/sciq.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/squad.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/sst2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/stsb.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/summarize_from_human_feedback.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/tab_fact.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/tablerow_classify.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/tldr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/toxigen.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/trec.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/unfair_tos.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.161567 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.245567 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/ceb/
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/ceb/gja.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.245567 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/da/
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/da/ddt.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.245567 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/de/
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/de/pud.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.245567 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/en/
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/en/ewt.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/en/pud.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.249567 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/hr/
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/hr/set.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.249567 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/pt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/pt/bosque.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/pt/pud.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.249567 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/ru/
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/ru/pud.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.249567 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/sk/
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/sk/snk.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.249567 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/sr/
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/sr/set.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.249567 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/sv/
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/sv/pud.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/sv/talbanken.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.249567 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/tl/
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/tl/trg.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/tl/ugnayan.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.249567 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/zh/
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/zh/gsd.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/zh/gsdsimp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/zh/pud.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/wiki_bio.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/wikitq.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.249567 unitxt-1.9.0/src/unitxt/catalog/cards/winogrande/
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/winogrande/debiased.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/winogrande/l.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/winogrande/m.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/winogrande/s.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/winogrande/xl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/winogrande/xs.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.249567 unitxt-1.9.0/src/unitxt/catalog/cards/wmt/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/wmt/en_de.json
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/wmt/en_fr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/wmt/en_ro.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.249567 unitxt-1.9.0/src/unitxt/catalog/cards/wnli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/wnli/truthfulness.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/wnli.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/wsc.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.257567 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/amharic.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/arabic.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/azerbaijani.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/bengali.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/burmese.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/chinese_simplified.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/chinese_traditional.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/english.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/french.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/gujarati.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/hausa.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/hindi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/igbo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/indonesian.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/japanese.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/kirundi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/korean.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/kyrgyz.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/marathi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/nepali.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/oromo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/pashto.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/persian.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/pidgin.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/portuguese.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/punjabi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/russian.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/scottish_gaelic.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/serbian_cyrillic.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/serbian_latin.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/sinhala.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/somali.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/spanish.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/swahili.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/tamil.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/telugu.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/thai.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/tigrinya.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/turkish.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/ukrainian.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/urdu.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/uzbek.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/vietnamese.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/welsh.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/yoruba.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.261567 unitxt-1.9.0/src/unitxt/catalog/cards/xnli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xnli/ar.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xnli/bg.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xnli/de.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xnli/el.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xnli/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xnli/es.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xnli/fr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xnli/hi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xnli/ru.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xnli/sw.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xnli/th.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xnli/tr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xnli/ur.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xnli/vi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xnli/zh.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xsum.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.261567 unitxt-1.9.0/src/unitxt/catalog/cards/xwinogrande/
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xwinogrande/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xwinogrande/jp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xwinogrande/pt.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xwinogrande/ru.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/xwinogrande/zh.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/cards/yahoo_answers_topics.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.261567 unitxt-1.9.0/src/unitxt/catalog/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/formats/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/formats/empty_input_output_separator.json
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/formats/human_assistant.json
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/formats/llama.json
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/formats/llama2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/formats/llama3_chat.json
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/formats/llama3_chat_with_system_prompt.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.261567 unitxt-1.9.0/src/unitxt/catalog/formats/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/formats/models/alpaca_instruct.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.265567 unitxt-1.9.0/src/unitxt/catalog/formats/models/flan/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/formats/models/flan/exq_exa.json
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/formats/models/flan/few_shot.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.265567 unitxt-1.9.0/src/unitxt/catalog/formats/models/labradorite/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/formats/models/labradorite/few_shot.json
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/formats/models/labradorite/zero_shot.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.265567 unitxt-1.9.0/src/unitxt/catalog/formats/models/mistral/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.265567 unitxt-1.9.0/src/unitxt/catalog/formats/models/mistral/instruction/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/formats/models/mistral/instruction/with_system_prompt.json
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/formats/models/mistral/instruction.json
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/formats/models/phi_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/formats/textual_assistant.json
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/formats/user_agent.json
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/formats/user_assistant.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.273567 unitxt-1.9.0/src/unitxt/catalog/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/accuracy_binary.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.273567 unitxt-1.9.0/src/unitxt/catalog/metrics/bert_score/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/bert_score/deberta_base_mnli.json
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/bert_score/deberta_large_mnli.json
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/bert_score/deberta_v3_base_mnli_xnli_ml.json
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/bert_score/deberta_xlarge_mnli.json
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/bert_score/distilbert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/bleu.json
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/char_edit_dist_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/char_edit_distance.json
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/f1_binary.json
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/f1_macro.json
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/f1_macro_multi_label.json
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/f1_micro.json
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/f1_micro_multi_label.json
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/f1_weighted.json
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/jaccard_index.json
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/kendalltau_b.json
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/kpa.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.161567 unitxt-1.9.0/src/unitxt/catalog/metrics/llm_as_judge/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.273567 unitxt-1.9.0/src/unitxt/catalog/metrics/llm_as_judge/rating/
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/llm_as_judge/rating/llama_3_70b_instruct_ibm_genai_template_mt_bench_single_turn.json
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/llm_as_judge/rating/llama_3_8b_instruct_ibm_genai_template_mt_bench_single_turn.json
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/llm_as_judge/rating/mistral_7b_instruct_v0_2_huggingface_template_mt_bench_single_turn.json
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/map.json
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/matthews_correlation.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/max_accuracy_binary.json
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/max_f1_binary.json
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/mrr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/ndcg.json
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/ner.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/normalized_sacrebleu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.273567 unitxt-1.9.0/src/unitxt/catalog/metrics/perplexity/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/perplexity/flan_t5_small.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.273567 unitxt-1.9.0/src/unitxt/catalog/metrics/perplexity_a/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/perplexity_a/flan_t5_small.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.273567 unitxt-1.9.0/src/unitxt/catalog/metrics/perplexity_chat/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/perplexity_chat/flan_t5_small.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.273567 unitxt-1.9.0/src/unitxt/catalog/metrics/perplexity_nli/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/perplexity_nli/t5_nli_mixture.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.273567 unitxt-1.9.0/src/unitxt/catalog/metrics/perplexity_q/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/perplexity_q/flan_t5_small.json
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/precision_binary.json
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/precision_macro_multi_label.json
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/precision_micro_multi_label.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.277567 unitxt-1.9.0/src/unitxt/catalog/metrics/rag/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/rag/answer_correctness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/rag/answer_inference.json
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/rag/answer_reward.json
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/rag/bert_k_precision.json
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/rag/bert_k_precision_ml.json
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/rag/bert_recall.json
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/rag/bert_recall_ml.json
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/rag/context_correctness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/rag/context_perplexity.json
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/rag/context_relevance.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.277567 unitxt-1.9.0/src/unitxt/catalog/metrics/rag/correctness/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/rag/correctness/llama_index_by_gpt_3_5_turbo.json
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/rag/correctness/llama_index_by_mock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/rag/faithfulness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/rag/k_precision.json
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/rag/map.json
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/rag/mrr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/rag/recall.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.165567 unitxt-1.9.0/src/unitxt/catalog/metrics/rag/response_generation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.277567 unitxt-1.9.0/src/unitxt/catalog/metrics/rag/response_generation/correctness/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.277567 unitxt-1.9.0/src/unitxt/catalog/metrics/rag/response_generation/correctness/bert_score/
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/rag/response_generation/correctness/bert_score/deberta_large_mnli.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/rag/response_generation/correctness/bert_score/deberta_v3_base_mnli_xnli_ml.json
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/rag/response_generation/correctness/token_overlap.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.277567 unitxt-1.9.0/src/unitxt/catalog/metrics/rag/response_generation/faithfullness/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/rag/response_generation/faithfullness/token_overlap.json
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/recall_binary.json
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/recall_macro_multi_label.json
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/recall_micro_multi_label.json
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/regard.json
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/rerank_recall.json
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/retrieval_at_k.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.277567 unitxt-1.9.0/src/unitxt/catalog/metrics/reward/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/reward/deberta_v3_large_v2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.281566 unitxt-1.9.0/src/unitxt/catalog/metrics/robustness/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_cohens_h_paraphrase_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_cohens_h_paraphrase_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_hedges_g_paraphrase_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_hedges_g_paraphrase_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/robustness/fixed_group_mean_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/robustness/fixed_group_mean_baseline_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/robustness/fixed_group_mean_baseline_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/robustness/fixed_group_mean_paraphrase_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/robustness/fixed_group_mean_paraphrase_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/robustness/fixed_group_mean_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/robustness/fixed_group_norm_cohens_h_paraphrase_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/robustness/fixed_group_norm_cohens_h_paraphrase_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/robustness/fixed_group_norm_hedges_g_paraphrase_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/robustness/fixed_group_norm_hedges_g_paraphrase_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/robustness/fixed_group_pdr_paraphrase_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/robustness/fixed_group_pdr_paraphrase_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/robustness/group_mean_accuracy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/robustness/group_mean_string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/robustness/group_mean_token_overlap.json
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/roc_auc.json
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/rouge.json
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/rouge_with_confidence_intervals.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/sacrebleu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/safety.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.281566 unitxt-1.9.0/src/unitxt/catalog/metrics/sentence_bert/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/sentence_bert/mpnet_base_v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/spearman.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/squad.json
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/string_containment.json
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/token_overlap.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/token_overlap_with_context.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/unsorted_list_exact_match.json
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/metrics/wer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.165567 unitxt-1.9.0/src/unitxt/catalog/operators/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.165567 unitxt-1.9.0/src/unitxt/catalog/operators/balancers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.281566 unitxt-1.9.0/src/unitxt/catalog/operators/balancers/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/operators/balancers/classification/by_label.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.281566 unitxt-1.9.0/src/unitxt/catalog/operators/balancers/multi_label/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/operators/balancers/multi_label/zero_vs_many_labels.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.281566 unitxt-1.9.0/src/unitxt/catalog/operators/balancers/ner/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/operators/balancers/ner/zero_vs_many_entities.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.281566 unitxt-1.9.0/src/unitxt/catalog/operators/balancers/qa/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/operators/balancers/qa/by_answer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.289567 unitxt-1.9.0/src/unitxt/catalog/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/capitalize.json
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/cast_to_float_return_nan_if_failed.json
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/cast_to_float_return_zero_if_failed.json
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/convert_to_boolean.json
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/dict_of_lists_to_value_key_pairs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/extract_from_double_brackets.json
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/extract_mt_bench_label_judgment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/extract_mt_bench_rating_judgment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/first_character.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/get_string_after_colon.json
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/hate_speech_or_not_hate_speech.json
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/list_to_empty_entity_tuples.json
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/literal_eval.json
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/load_json.json
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/load_json_from_predictions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/lower_case.json
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/lower_case_till_punc.json
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/match_closest_option.json
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/predictions_yes_1_else_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/regex_parser_from_prediction.json
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/remove_none_from_list.json
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/stance_to_pro_con.json
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/str_to_float_format.json
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/substring.json
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/take_first_non_empty_line.json
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/take_first_word.json
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/to_list_by_comma.json
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/to_list_by_comma_from_references.json
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/to_span_label_pairs.json
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/to_span_label_pairs_surface_only.json
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/to_string.json
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/to_string_stripped.json
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/to_yes_or_none.json
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/toxic_or_not_toxic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/processors/yes_no_to_int.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.293567 unitxt-1.9.0/src/unitxt/catalog/splitters/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/splitters/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/splitters/diverse_labels_sampler.json
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/splitters/large_no_dev.json
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/splitters/large_no_test.json
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/splitters/small_no_dev.json
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/splitters/small_no_test.json
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/splitters/test_only.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.165567 unitxt-1.9.0/src/unitxt/catalog/system_prompt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.293567 unitxt-1.9.0/src/unitxt/catalog/system_prompt/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/system_prompt/models/japanese_llama.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.293567 unitxt-1.9.0/src/unitxt/catalog/system_prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/system_prompts/empty.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.293567 unitxt-1.9.0/src/unitxt/catalog/system_prompts/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/system_prompts/models/alpaca.json
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/system_prompts/models/labradorite.json
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/system_prompts/models/llama.json
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/system_prompts/models/llama2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.293567 unitxt-1.9.0/src/unitxt/catalog/tasks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.293567 unitxt-1.9.0/src/unitxt/catalog/tasks/classification/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.293567 unitxt-1.9.0/src/unitxt/catalog/tasks/classification/binary/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/classification/binary/zero_or_one.json
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/classification/binary.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.293567 unitxt-1.9.0/src/unitxt/catalog/tasks/classification/multi_class/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/classification/multi_class/relation.json
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/classification/multi_class/with_classes_descriptions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/classification/multi_class.json
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/classification/multi_label.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.293567 unitxt-1.9.0/src/unitxt/catalog/tasks/completion/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/completion/abstractive.json
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/completion/extractive.json
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/completion/multiple_choice.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.297567 unitxt-1.9.0/src/unitxt/catalog/tasks/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/evaluation/preference.json
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/generation.json
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/grammatical_error_correction.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.297567 unitxt-1.9.0/src/unitxt/catalog/tasks/ner/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/ner/all_entity_types.json
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/ner/single_entity_type.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.297567 unitxt-1.9.0/src/unitxt/catalog/tasks/qa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.297567 unitxt-1.9.0/src/unitxt/catalog/tasks/qa/multiple_choice/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/qa/multiple_choice/open.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.297567 unitxt-1.9.0/src/unitxt/catalog/tasks/qa/multiple_choice/with_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/qa/multiple_choice/with_context/with_topic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/qa/multiple_choice/with_context.json
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/qa/multiple_choice/with_topic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/qa/open.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.297567 unitxt-1.9.0/src/unitxt/catalog/tasks/qa/with_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/qa/with_context/abstractive.json
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/qa/with_context/extractive.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.297567 unitxt-1.9.0/src/unitxt/catalog/tasks/rag/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/rag/response_generation.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.297567 unitxt-1.9.0/src/unitxt/catalog/tasks/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/regression/single_text.json
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/regression/two_texts.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.165567 unitxt-1.9.0/src/unitxt/catalog/tasks/response_assessment/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.297567 unitxt-1.9.0/src/unitxt/catalog/tasks/response_assessment/pairwise_comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/response_assessment/pairwise_comparison/multi_turn.json
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/response_assessment/pairwise_comparison/multi_turn_with_reference.json
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/response_assessment/pairwise_comparison/single_turn.json
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/response_assessment/pairwise_comparison/single_turn_with_reference.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.301566 unitxt-1.9.0/src/unitxt/catalog/tasks/response_assessment/rating/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/response_assessment/rating/multi_turn.json
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/response_assessment/rating/multi_turn_with_reference.json
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/response_assessment/rating/single_turn.json
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/response_assessment/rating/single_turn_with_reference.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.301566 unitxt-1.9.0/src/unitxt/catalog/tasks/rewriting/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/rewriting/by_attribute.json
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/rewriting/paraphrase.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.301566 unitxt-1.9.0/src/unitxt/catalog/tasks/selection/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/selection/by_attribute.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.301566 unitxt-1.9.0/src/unitxt/catalog/tasks/span_labeling/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/span_labeling/extraction.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.301566 unitxt-1.9.0/src/unitxt/catalog/tasks/summarization/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/summarization/abstractive.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.301566 unitxt-1.9.0/src/unitxt/catalog/tasks/targeted_sentiment_extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/targeted_sentiment_extraction/all_sentiment_classes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/targeted_sentiment_extraction/single_sentiment_class.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.301566 unitxt-1.9.0/src/unitxt/catalog/tasks/translation/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/tasks/translation/directed.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.301566 unitxt-1.9.0/src/unitxt/catalog/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.169567 unitxt-1.9.0/src/unitxt/catalog/templates/classification/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.305566 unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_class/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_class/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_class/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_class/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_class/instruction.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.305566 unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_class/relation/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_class/relation/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_class/relation/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_class/relation/simple.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.305566 unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_6.json
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/flan_7.json
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_class/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.305566 unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_label/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_label/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_label/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_label/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_label/instruction.json
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_label/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.169567 unitxt-1.9.0/src/unitxt/catalog/templates/completion/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.305566 unitxt-1.9.0/src/unitxt/catalog/templates/completion/abstractive/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/completion/abstractive/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/completion/abstractive/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/completion/abstractive/standard.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.309566 unitxt-1.9.0/src/unitxt/catalog/templates/completion/multiple_choice/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/completion/multiple_choice/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/completion/multiple_choice/enumerated.json
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/completion/multiple_choice/simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/completion/multiple_choice/standard.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/completion/multiple_choice/title.json
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/empty.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.169567 unitxt-1.9.0/src/unitxt/catalog/templates/evaluation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.309566 unitxt-1.9.0/src/unitxt/catalog/templates/evaluation/preference/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/evaluation/preference/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/evaluation/preference/default.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.309566 unitxt-1.9.0/src/unitxt/catalog/templates/generation/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/generation/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/generation/default.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.309566 unitxt-1.9.0/src/unitxt/catalog/templates/grammatical_error_correction/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/grammatical_error_correction/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/grammatical_error_correction/simple.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.309566 unitxt-1.9.0/src/unitxt/catalog/templates/grammatical_error_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/grammatical_error_detection/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/grammatical_error_detection/yes_no.json
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/key_val.json
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/key_val_with_new_lines.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.173567 unitxt-1.9.0/src/unitxt/catalog/templates/qa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.309566 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/match.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.313567 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.313567 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/de/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/de/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/de/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/de/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/de/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.313567 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/es/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/es/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/es/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/es/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/es/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.313567 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/fr/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/helm.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.313567 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/ja/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.313567 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/open/pt/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.313567 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/match.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.317566 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.317566 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/de/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.317566 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/es/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.317566 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/fr/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/helm.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.317566 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/ja/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.317566 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/no_intro/pt/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.321566 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.321566 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/de/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.321566 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/es/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fm_eval.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.321566 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/fr/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/helm.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.321566 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/ja/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/match.json
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.321566 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/pt/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.321566 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.325566 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/de/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.325566 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/es/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fm_eval.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.325566 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/fr/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/helm.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.325566 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/ja/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/match.json
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/mmlu.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.325566 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/helm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/lm_eval_harness.json
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/pt/mmlu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_topic/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.325566 unitxt-1.9.0/src/unitxt/catalog/templates/qa/open/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/open/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/open/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/open/simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/open/simple2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/open/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.329566 unitxt-1.9.0/src/unitxt/catalog/templates/qa/with_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/with_context/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/with_context/ffqa.json
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/with_context/question_first.json
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/with_context/simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/with_context/simple2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/with_context/title.json
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/qa/with_context/with_type.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.173567 unitxt-1.9.0/src/unitxt/catalog/templates/rag/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.329566 unitxt-1.9.0/src/unitxt/catalog/templates/rag/response_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/rag/response_generation/simple.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.173567 unitxt-1.9.0/src/unitxt/catalog/templates/regression/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.329566 unitxt-1.9.0/src/unitxt/catalog/templates/regression/single_text/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/regression/single_text/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/regression/single_text/simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/regression/single_text/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.329566 unitxt-1.9.0/src/unitxt/catalog/templates/regression/two_texts/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/regression/two_texts/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.329566 unitxt-1.9.0/src/unitxt/catalog/templates/regression/two_texts/similarity/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/regression/two_texts/similarity/flan.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/regression/two_texts/simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/regression/two_texts/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.173567 unitxt-1.9.0/src/unitxt/catalog/templates/response_assessment/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.329566 unitxt-1.9.0/src/unitxt/catalog/templates/response_assessment/pairwise_comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/response_assessment/pairwise_comparison/mt_bench_multi_turn_with_reference_with_shuffle.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/response_assessment/pairwise_comparison/mt_bench_multi_turn_with_shuffle.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/response_assessment/pairwise_comparison/mt_bench_single_turn_with_reference_with_shuffle.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/response_assessment/pairwise_comparison/mt_bench_single_turn_with_shuffle.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.329566 unitxt-1.9.0/src/unitxt/catalog/templates/response_assessment/rating/
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/response_assessment/rating/mt_bench_multi_turn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/response_assessment/rating/mt_bench_multi_turn_with_reference.json
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/response_assessment/rating/mt_bench_single_turn.json
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/response_assessment/rating/mt_bench_single_turn_with_reference.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.177567 unitxt-1.9.0/src/unitxt/catalog/templates/rewriting/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.329566 unitxt-1.9.0/src/unitxt/catalog/templates/rewriting/by_attribute/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/rewriting/by_attribute/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/rewriting/by_attribute/default.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.329566 unitxt-1.9.0/src/unitxt/catalog/templates/rewriting/paraphrase/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/rewriting/paraphrase/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/rewriting/paraphrase/default.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.177567 unitxt-1.9.0/src/unitxt/catalog/templates/selection/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.329566 unitxt-1.9.0/src/unitxt/catalog/templates/selection/by_attribute/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/selection/by_attribute/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/selection/by_attribute/default.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.177567 unitxt-1.9.0/src/unitxt/catalog/templates/span_labeling/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.333566 unitxt-1.9.0/src/unitxt/catalog/templates/span_labeling/extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/span_labeling/extraction/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/span_labeling/extraction/carry.json
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/span_labeling/extraction/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/span_labeling/extraction/extract.json
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/span_labeling/extraction/having.json
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/span_labeling/extraction/identify.json
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/span_labeling/extraction/title.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.177567 unitxt-1.9.0/src/unitxt/catalog/templates/summarization/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.333566 unitxt-1.9.0/src/unitxt/catalog/templates/summarization/abstractive/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/summarization/abstractive/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/summarization/abstractive/casual.json
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/summarization/abstractive/formal.json
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/summarization/abstractive/formal_without_label.json
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/summarization/abstractive/full.json
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/summarization/abstractive/instructive.json
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/summarization/abstractive/one_sentence.json
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/summarization/abstractive/passive.json
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/summarization/abstractive/professional.json
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/summarization/abstractive/title.json
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/summarization/abstractive/write_succinct.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.333566 unitxt-1.9.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.333566 unitxt-1.9.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/convert_with_explicit_keys.json
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/convert_with_implicit_keys.json
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/as_json/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/carry_sentiment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/entities_sentiment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/extract_sentiment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/having_sentiment.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.337566 unitxt-1.9.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/having_sentiment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/negative/sentiment_extracted.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.337566 unitxt-1.9.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/having_sentiment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/neutral/sentiment_extracted.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.337566 unitxt-1.9.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/having_sentiment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/positive/sentiment_extracted.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.177567 unitxt-1.9.0/src/unitxt/catalog/templates/translation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.337566 unitxt-1.9.0/src/unitxt/catalog/templates/translation/directed/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/translation/directed/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/translation/directed/casual.json
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/translation/directed/formal.json
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/translation/directed/instructional.json
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/translation/directed/playful.json
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/translation/directed/simple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog/templates/translation/directed/title.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/collections_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17311 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/deprecation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/dialog_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23755 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/dict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/eval_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/fusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/generator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/hf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7451 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/instructions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/llm_as_judge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18767 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11224 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/metric_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   139682 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/normalizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21535 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84992 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/parsing_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.341566 unitxt-1.9.0/src/unitxt/prepare_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/prepare_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/prepare_utils/card_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13725 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/prepare_utils/info_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/prepare_utils/instructions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/random_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.341566 unitxt-1.9.0/src/unitxt/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.341566 unitxt-1.9.0/src/unitxt/service/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/service/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/service/metrics/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/service/metrics/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/settings_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/span_lableing_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12229 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/split_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/splitters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14353 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/string_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17712 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/struct_data_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/system_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25963 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.341566 unitxt-1.9.0/src/unitxt/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/test_utils/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10553 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/test_utils/card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/test_utils/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/test_utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/test_utils/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/test_utils/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/text_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31413 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/type_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.341566 unitxt-1.9.0/src/unitxt/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56810 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/ui/banner.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/ui/gradio_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/ui/load_catalog_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14100 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/ui/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/ui/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/ui/ui_tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/ui/ui_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 12:20:59.000000 unitxt-1.9.0/src/unitxt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:21:07.341566 unitxt-1.9.0/src/unitxt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9053 2024-05-20 12:21:07.000000 unitxt-1.9.0/src/unitxt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    54445 2024-05-20 12:21:07.000000 unitxt-1.9.0/src/unitxt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:21:07.000000 unitxt-1.9.0/src/unitxt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-20 12:21:07.000000 unitxt-1.9.0/src/unitxt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-20 12:21:07.000000 unitxt-1.9.0/src/unitxt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-20 12:21:07.000000 unitxt-1.9.0/src/unitxt.egg-info/top_level.txt
```

### Comparing `unitxt-1.8.1/LICENSE` & `unitxt-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/PKG-INFO` & `unitxt-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,130 +1,134 @@
 Metadata-Version: 2.1
 Name: unitxt
-Version: 1.8.1
+Version: 1.9.0
 Summary: Load any mixture of text to text data in one line of code
 Home-page: https://github.com/ibm/unitxt
 Author: IBM Research
 Author-email: elron.bandel@ibm.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: datasets>=2.16.0
 Requires-Dist: evaluate
 Requires-Dist: absl-py
 Requires-Dist: ipadic
 Requires-Dist: scipy
-Provides-Extra: tests
-Requires-Dist: bert_score; extra == "tests"
-Requires-Dist: transformers; extra == "tests"
-Requires-Dist: sentence_transformers; extra == "tests"
-Requires-Dist: ibm-cos-sdk; extra == "tests"
-Requires-Dist: opendatasets; extra == "tests"
-Requires-Dist: httpretty~=1.1.4; extra == "tests"
-Requires-Dist: editdistance; extra == "tests"
-Requires-Dist: rouge-score; extra == "tests"
-Requires-Dist: nltk; extra == "tests"
-Requires-Dist: mecab-python3; extra == "tests"
-Requires-Dist: sacrebleu[ko]; extra == "tests"
-Requires-Dist: scikit-learn; extra == "tests"
-Requires-Dist: jiwer; extra == "tests"
-Requires-Dist: conllu; extra == "tests"
-Requires-Dist: llama-index-core; extra == "tests"
-Requires-Dist: llama-index-llms-openai; extra == "tests"
-Requires-Dist: pytrec-eval; extra == "tests"
-Requires-Dist: SentencePiece; extra == "tests"
-Provides-Extra: service
-Requires-Dist: torch==1.12.1; extra == "service"
-Requires-Dist: fastapi==0.109.0; extra == "service"
-Requires-Dist: uvicorn[standard]==0.27.0.post1; extra == "service"
-Requires-Dist: python-jose[cryptography]==3.3.0; extra == "service"
-Requires-Dist: transformers; extra == "service"
+Provides-Extra: dev
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: tomli; extra == "dev"
+Requires-Dist: codespell; extra == "dev"
+Provides-Extra: ui
+Requires-Dist: gradio; extra == "ui"
+Requires-Dist: transformers; extra == "ui"
 Provides-Extra: base
 Requires-Dist: datasets>=2.16.0; extra == "base"
 Requires-Dist: evaluate; extra == "base"
 Requires-Dist: absl-py; extra == "base"
 Requires-Dist: ipadic; extra == "base"
 Requires-Dist: scipy; extra == "base"
 Provides-Extra: helm
 Requires-Dist: crfm-helm[unitxt]>=0.5.0; extra == "helm"
+Provides-Extra: service
+Requires-Dist: torch==1.12.1; extra == "service"
+Requires-Dist: fastapi==0.109.0; extra == "service"
+Requires-Dist: uvicorn[standard]==0.27.0.post1; extra == "service"
+Requires-Dist: python-jose[cryptography]==3.3.0; extra == "service"
+Requires-Dist: transformers; extra == "service"
 Provides-Extra: docs
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Requires-Dist: piccolo_theme; extra == "docs"
 Requires-Dist: sphinxext-opengraph; extra == "docs"
 Requires-Dist: datasets; extra == "docs"
 Requires-Dist: evaluate; extra == "docs"
 Requires-Dist: nltk; extra == "docs"
 Requires-Dist: sacrebleu; extra == "docs"
 Requires-Dist: absl-py; extra == "docs"
 Requires-Dist: rouge_score; extra == "docs"
 Requires-Dist: scikit-learn; extra == "docs"
 Requires-Dist: jiwer; extra == "docs"
 Requires-Dist: editdistance; extra == "docs"
-Provides-Extra: ui
-Requires-Dist: gradio; extra == "ui"
-Requires-Dist: transformers; extra == "ui"
-Provides-Extra: dev
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: tomli; extra == "dev"
-Requires-Dist: codespell; extra == "dev"
+Provides-Extra: tests
+Requires-Dist: bert_score; extra == "tests"
+Requires-Dist: transformers; extra == "tests"
+Requires-Dist: sentence_transformers; extra == "tests"
+Requires-Dist: ibm-cos-sdk; extra == "tests"
+Requires-Dist: opendatasets; extra == "tests"
+Requires-Dist: httpretty~=1.1.4; extra == "tests"
+Requires-Dist: editdistance; extra == "tests"
+Requires-Dist: rouge-score; extra == "tests"
+Requires-Dist: nltk; extra == "tests"
+Requires-Dist: mecab-python3; extra == "tests"
+Requires-Dist: sacrebleu[ko]; extra == "tests"
+Requires-Dist: scikit-learn; extra == "tests"
+Requires-Dist: jiwer; extra == "tests"
+Requires-Dist: conllu; extra == "tests"
+Requires-Dist: llama-index-core; extra == "tests"
+Requires-Dist: llama-index-llms-openai; extra == "tests"
+Requires-Dist: pytrec-eval; extra == "tests"
+Requires-Dist: SentencePiece; extra == "tests"
+Requires-Dist: openai; extra == "tests"
+Requires-Dist: ibm-generative-ai; extra == "tests"
 Provides-Extra: all
-Requires-Dist: llama-index-core; extra == "all"
-Requires-Dist: nltk; extra == "all"
+Requires-Dist: rouge-score; extra == "all"
+Requires-Dist: ruff; extra == "all"
+Requires-Dist: pytrec-eval; extra == "all"
+Requires-Dist: sphinxext-opengraph; extra == "all"
+Requires-Dist: conllu; extra == "all"
+Requires-Dist: openai; extra == "all"
+Requires-Dist: sacrebleu; extra == "all"
+Requires-Dist: mecab-python3; extra == "all"
+Requires-Dist: ibm-generative-ai; extra == "all"
 Requires-Dist: torch==1.12.1; extra == "all"
+Requires-Dist: ipadic; extra == "all"
 Requires-Dist: codespell; extra == "all"
-Requires-Dist: opendatasets; extra == "all"
 Requires-Dist: absl-py; extra == "all"
-Requires-Dist: conllu; extra == "all"
-Requires-Dist: ruff; extra == "all"
-Requires-Dist: editdistance; extra == "all"
-Requires-Dist: fastapi==0.109.0; extra == "all"
+Requires-Dist: llama-index-llms-openai; extra == "all"
+Requires-Dist: llama-index-core; extra == "all"
+Requires-Dist: piccolo_theme; extra == "all"
+Requires-Dist: nltk; extra == "all"
 Requires-Dist: datasets; extra == "all"
-Requires-Dist: sacrebleu[ko]; extra == "all"
-Requires-Dist: mecab-python3; extra == "all"
-Requires-Dist: sacrebleu; extra == "all"
-Requires-Dist: crfm-helm[unitxt]>=0.5.0; extra == "all"
-Requires-Dist: scikit-learn; extra == "all"
-Requires-Dist: ipadic; extra == "all"
 Requires-Dist: transformers; extra == "all"
-Requires-Dist: datasets>=2.16.0; extra == "all"
-Requires-Dist: uvicorn[standard]==0.27.0.post1; extra == "all"
-Requires-Dist: scipy; extra == "all"
+Requires-Dist: rouge_score; extra == "all"
+Requires-Dist: scikit-learn; extra == "all"
 Requires-Dist: tomli; extra == "all"
-Requires-Dist: piccolo_theme; extra == "all"
-Requires-Dist: SentencePiece; extra == "all"
+Requires-Dist: opendatasets; extra == "all"
+Requires-Dist: uvicorn[standard]==0.27.0.post1; extra == "all"
 Requires-Dist: sphinx_rtd_theme; extra == "all"
-Requires-Dist: pre-commit; extra == "all"
-Requires-Dist: sentence_transformers; extra == "all"
-Requires-Dist: bert_score; extra == "all"
-Requires-Dist: pytrec-eval; extra == "all"
+Requires-Dist: scipy; extra == "all"
+Requires-Dist: fastapi==0.109.0; extra == "all"
 Requires-Dist: httpretty~=1.1.4; extra == "all"
-Requires-Dist: rouge_score; extra == "all"
-Requires-Dist: python-jose[cryptography]==3.3.0; extra == "all"
-Requires-Dist: jiwer; extra == "all"
 Requires-Dist: evaluate; extra == "all"
 Requires-Dist: gradio; extra == "all"
-Requires-Dist: sphinxext-opengraph; extra == "all"
+Requires-Dist: bert_score; extra == "all"
+Requires-Dist: editdistance; extra == "all"
 Requires-Dist: ibm-cos-sdk; extra == "all"
-Requires-Dist: rouge-score; extra == "all"
-Requires-Dist: llama-index-llms-openai; extra == "all"
+Requires-Dist: crfm-helm[unitxt]>=0.5.0; extra == "all"
+Requires-Dist: python-jose[cryptography]==3.3.0; extra == "all"
+Requires-Dist: datasets>=2.16.0; extra == "all"
+Requires-Dist: jiwer; extra == "all"
+Requires-Dist: pre-commit; extra == "all"
+Requires-Dist: sacrebleu[ko]; extra == "all"
+Requires-Dist: SentencePiece; extra == "all"
+Requires-Dist: sentence_transformers; extra == "all"
 
 <div align="center">
     <img src="./assets/banner.png" alt="Image Description" width="100%" />
 </div>
 
 [![Button](https://img.shields.io/badge/Video-pink?style=for-the-badge)](https://unitxt.readthedocs.io/)
 [![Button](https://img.shields.io/badge/Demo-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/docs/demo.html)
 [![Button](https://img.shields.io/badge/Tutorial-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/docs/adding_dataset.html)
 [![Button](https://img.shields.io/badge/Paper-pink?style=for-the-badge)](https://arxiv.org/abs/2401.14019)
 [![Button](https://img.shields.io/badge/Documentation-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/modules.html)
-[![Button](https://img.shields.io/badge/Catalog-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/catalog.html)
-[![Button](https://img.shields.io/badge/Contributors-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/docs/contributors_guide.html)
+[![Button](https://img.shields.io/badge/Catalog-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/catalog/catalog.__dir__.html)
+[![Button](https://img.shields.io/badge/Contributors-pink?style=for-the-badge)](https://github.com/IBM/unitxt/blob/main/CONTRIBUTING.md)
 [![Button](https://img.shields.io/badge/PyPi-pink?style=for-the-badge)](https://pypi.org/project/unitxt/)
 
 
 In the dynamic landscape of generative NLP, traditional text processing pipelines limit research flexibility and reproducibility, as they are tailored to specific dataset, task, and model combinations. The escalating complexity, involving system prompts, model-specific formats, instructions, and more, calls for a shift to a structured, modular, and customizable solution.
 
  Addressing this need, we present Unitxt, an innovative library for customizable textual data preparation and evaluation tailored to generative language models. Unitxt natively integrates with common libraries like HuggingFace and LM-eval-harness and deconstructs processing flows into modular components, enabling easy customization and sharing between practitioners. These components encompass model-specific formats, task prompts, and many other comprehensive dataset processing definitions. The Unitxt-Catalog centralizes these components, fostering collaboration and exploration in modern textual data workflows. Beyond being a tool, Unitxt is a community-driven platform, empowering users to build, share, and advance their pipelines collaboratively.
```

### Comparing `unitxt-1.8.1/README.md` & `unitxt-1.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 </div>
 
 [![Button](https://img.shields.io/badge/Video-pink?style=for-the-badge)](https://unitxt.readthedocs.io/)
 [![Button](https://img.shields.io/badge/Demo-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/docs/demo.html)
 [![Button](https://img.shields.io/badge/Tutorial-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/docs/adding_dataset.html)
 [![Button](https://img.shields.io/badge/Paper-pink?style=for-the-badge)](https://arxiv.org/abs/2401.14019)
 [![Button](https://img.shields.io/badge/Documentation-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/modules.html)
-[![Button](https://img.shields.io/badge/Catalog-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/catalog.html)
-[![Button](https://img.shields.io/badge/Contributors-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/docs/contributors_guide.html)
+[![Button](https://img.shields.io/badge/Catalog-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/catalog/catalog.__dir__.html)
+[![Button](https://img.shields.io/badge/Contributors-pink?style=for-the-badge)](https://github.com/IBM/unitxt/blob/main/CONTRIBUTING.md)
 [![Button](https://img.shields.io/badge/PyPi-pink?style=for-the-badge)](https://pypi.org/project/unitxt/)
 
 
 In the dynamic landscape of generative NLP, traditional text processing pipelines limit research flexibility and reproducibility, as they are tailored to specific dataset, task, and model combinations. The escalating complexity, involving system prompts, model-specific formats, instructions, and more, calls for a shift to a structured, modular, and customizable solution.
 
  Addressing this need, we present Unitxt, an innovative library for customizable textual data preparation and evaluation tailored to generative language models. Unitxt natively integrates with common libraries like HuggingFace and LM-eval-harness and deconstructs processing flows into modular components, enabling easy customization and sharing between practitioners. These components encompass model-specific formats, task prompts, and many other comprehensive dataset processing definitions. The Unitxt-Catalog centralizes these components, fostering collaboration and exploration in modern textual data workflows. Beyond being a tool, Unitxt is a community-driven platform, empowering users to build, share, and advance their pipelines collaboratively.
```

### Comparing `unitxt-1.8.1/pyproject.toml` & `unitxt-1.9.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 "tests/library/test_dataclass.py" = ["F811"]
 "src/unitxt/validate.py" = ["B024"]
 "src/unitxt/standard.py" = ["C901"]
 "src/unitxt/type_utils.py" = ["C901"]
 "src/unitxt/dataclass.py" = ["C901"]
 "src/unitxt/operators.py" = ["C901"]
 "docs/conf.py" = ["E402"]
+"prepare/cards/attaq_500.py" = ["RUF001"]
 "prepare/instructions/models/llama.py" = ["RUF001"]
 "utils/hf/prepare_dataset.py" = ["T201"]
 "utils/hf/prepare_metric.py" = ["T201"]
 "utils/compare_unitxt_datasets_between_versions.py" = ["C901"]
 
 [tool.ruff.lint]
 # Enable Pyflakes (`F`) and a subset of the pycodestyle (`E`)  codes by default.
@@ -105,12 +106,12 @@
 extend-immutable-calls = ["fastapi.Depends", "fastapi.params.Depends", "fastapi.Query", "fastapi.params.Query"]
 
 
 [tool.ruff.lint.flake8-tidy-imports.banned-api]
 "src".msg = "Use unitxt outside src/ and relative imports inside src/ and install unitxt from source with `pip install -e '.[dev]'`."
 
 [tool.codespell]
-ignore-words-list = 'rouge,ot,ans,nd'
+ignore-words-list = 'rouge,ot,ans,nd,cann'
 check-filenames = true
 check-hidden = false
 regex = "(?<![a-z])[a-z'`]+|[A-Z][a-z'`]*|[a-z]+'[a-z]*|[a-z]+(?=[_-])|[a-z]+(?=[A-Z])|\\d+"
-skip = '*cards/trec*,*cards/belebele*,*cards/amazon_mass*,*cards/reuters21578*,*egg-info*,*/logs/*'
+skip = '*cards/trec*,*cards/belebele*,*cards/amazon_mass*,*cards/reuters21578*,*cards/attaq_500*,*cards/cohere_for_ai*,*egg-info*,*/logs/*'
```

### Comparing `unitxt-1.8.1/setup.py` & `unitxt-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/__init__.py` & `unitxt-1.9.0/src/unitxt/__init__.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/api.py` & `unitxt-1.9.0/src/unitxt/api.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/artifact.py` & `unitxt-1.9.0/src/unitxt/artifact.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,16 +244,17 @@
             if issubtype(
                 field.type, Union[Artifact, List[Artifact], Dict[str, Artifact]]
             ):
                 value = getattr(self, field.name)
                 value = map_values_in_place(value, maybe_recover_artifact)
                 setattr(self, field.name, value)
 
-        self.prepare()
-        self.verify()
+        if not settings.skip_artifacts_prepare_and_verify:
+            self.prepare()
+            self.verify()
 
     def _to_raw_dict(self):
         return {"type": self.type, **self._init_dict}
 
     def save(self, path):
         data = self.to_dict()
         save_json(path, data)
@@ -331,15 +332,15 @@
             return artifactory, name, args
 
     raise UnitxtArtifactNotFoundError(name, artifactories)
 
 
 def verbosed_fetch_artifact(identifier):
     artifact, artifactory = fetch_artifact(identifier)
-    logger.info(f"Artifact {identifier} is fetched from {artifactory}")
+    logger.debug(f"Artifact {identifier} is fetched from {artifactory}")
     return artifact
 
 
 def reset_artifacts_json_cache():
     artifacts_json_cache.cache_clear()
```

### Comparing `unitxt-1.8.1/src/unitxt/blocks.py` & `unitxt-1.9.0/src/unitxt/blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     SerializeTableAsMarkdown,
     SerializeTableRowAsList,
     SerializeTableRowAsText,
     SerializeTriples,
     TruncateTableCells,
     TruncateTableRows,
 )
-from .task import FormTask
+from .task import Task
 from .templates import (
     InputOutputTemplate,
     MultiLabelTemplate,
     MultiReferenceTemplate,
     OutputQuantizingTemplate,
     SpanLabelingTemplate,
     Template,
```

### Comparing `unitxt-1.8.1/src/unitxt/card.py` & `unitxt-1.9.0/src/unitxt/card.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from .artifact import Artifact
 from .collections import Collection
 from .dataclass import OptionalField
 from .loaders import Loader
 from .operator import StreamingOperator
 from .splitters import RandomSampler, Sampler
-from .task import FormTask
+from .task import Task
 
 
 class TaskCard(Artifact):
     """TaskCard delineates the phases in transforming the source dataset into a model-input, and specifies the metrics for evaluation of model-output.
 
     Attributes:
         loader: specifies the source address and the loading operator that can access that source and transform it into a unitxt multistream.
@@ -20,10 +20,10 @@
         task: specifies the fields (of the already (pre)processed instance) making the inputs, the fields making the outputs, and the metrics to be used for evaluating the model output.
 
         templates: format strings to be applied on the input fields (specified by the task) and the output fields. The template also carries the instructions and the list of postprocessing steps, to be applied to the model output.
     """
 
     loader: Loader
     preprocess_steps: List[StreamingOperator] = None
-    task: FormTask
+    task: Task
     templates: Collection = None
     sampler: Sampler = OptionalField(default_factory=RandomSampler)
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/20_newsgroups/sklearn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/20_newsgroups/sklearn.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/20_newsgroups.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/boolq/classification.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.47916666666666663%*

 * *Differences: {"'__description__'": "'Dataset Card for Boolq\\nDataset Summary\\nBoolQ is a question answering "*

 * *                      'dataset for yes/no questions containing 15942 examples. These questions are '*

 * *                      'naturally\\noccurring ---they are generated in unprompted and unconstrained '*

 * *                      'settings.\\nEach example is a triplet of (question, passage, answer), with '*

 * *                      'the title of the page as optional additional context.\\nThe text-pair '*

 * *                 […]*

```diff
@@ -1,89 +1,62 @@
 {
+    "__description__": "Dataset Card for Boolq\nDataset Summary\nBoolQ is a question answering dataset for yes/no questions containing 15942 examples. These questions are naturally\noccurring ---they are generated in unprompted and unconstrained settings.\nEach example is a triplet of (question, passage, answer), with the title of the page as optional additional context.\nThe text-pair classification setup is similar to existing natural language inference tasks.\nSupported Tasks\u2026 See the full description on the dataset page: https://huggingface.co/datasets/google/boolq.",
+    "__tags__": {
+        "annotations_creators": "crowdsourced",
+        "arxiv": "1905.10044",
+        "croissant": true,
+        "language": "en",
+        "language_creators": "found",
+        "license": "cc-by-sa-3.0",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "text-classification",
+        "task_ids": "natural-language-inference"
+    },
     "loader": {
-        "path": "SetFit/20_newsgroups",
-        "streaming": true,
+        "path": "google/boolq",
         "type": "load_hf"
     },
     "preprocess_steps": [
+        "splitters.small_no_test",
         {
-            "condition": "ne",
-            "type": "filter_by_condition",
-            "values": {
-                "text": ""
-            }
-        },
-        {
-            "mix": {
-                "test": "test",
-                "train": "train[90%]",
-                "validation": "train[10%]"
+            "fields": {
+                "classes": [
+                    "yes",
+                    "no"
+                ],
+                "text_a_type": "passage",
+                "text_b_type": "question",
+                "type_of_relation": "answer"
             },
-            "type": "split_random_mix"
+            "type": "add_fields"
         },
         {
-            "field_to_field": {
-                "label_text": "label"
+            "fields": {
+                "answer": "str"
             },
-            "type": "rename_fields"
+            "type": "cast_fields"
         },
         {
             "mappers": {
-                "label": {
-                    "alt.atheism": "atheism",
-                    "comp.graphics": "computer graphics",
-                    "comp.os.ms-windows.misc": "microsoft windows",
-                    "comp.sys.ibm.pc.hardware": "pc hardware",
-                    "comp.sys.mac.hardware": "mac hardware",
-                    "comp.windows.x": "windows x",
-                    "misc.forsale": "for sale",
-                    "rec.autos": "cars",
-                    "rec.motorcycles": "motorcycles",
-                    "rec.sport.baseball": "baseball",
-                    "rec.sport.hockey": "hockey",
-                    "sci.crypt": "cryptography",
-                    "sci.electronics": "electronics",
-                    "sci.med": "medicine",
-                    "sci.space": "space",
-                    "soc.religion.christian": "christianity",
-                    "talk.politics.guns": "guns",
-                    "talk.politics.mideast": "middle east",
-                    "talk.politics.misc": "politics",
-                    "talk.religion.misc": "religion"
+                "answer": {
+                    "False": "no",
+                    "True": "yes"
                 }
             },
             "type": "map_instance_values"
         },
         {
-            "fields": {
-                "classes": [
-                    "atheism",
-                    "computer graphics",
-                    "microsoft windows",
-                    "pc hardware",
-                    "mac hardware",
-                    "windows x",
-                    "for sale",
-                    "cars",
-                    "motorcycles",
-                    "baseball",
-                    "hockey",
-                    "cryptography",
-                    "electronics",
-                    "medicine",
-                    "space",
-                    "christianity",
-                    "guns",
-                    "middle east",
-                    "politics",
-                    "religion"
-                ],
-                "text_type": "text",
-                "type_of_class": "topic"
+            "field_to_field": {
+                "answer": "label",
+                "passage": "text_a",
+                "question": "text_b"
             },
-            "type": "add_fields"
+            "type": "rename_fields"
         }
     ],
-    "task": "tasks.classification.multi_class",
-    "templates": "templates.classification.multi_class.all",
+    "task": "tasks.classification.multi_class.relation",
+    "templates": "templates.classification.multi_class.relation.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/CFPB/product/2023.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/CFPB/product/2023.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/CFPB/product/watsonx.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/CFPB/product/watsonx.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/ag_news.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/winogrande/l.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4717261904761905%*

 * *Differences: {"'__description__'": "'WinoGrande is a new collection of 44k problems, inspired by Winograd "*

 * *                      'Schema Challenge (Levesque, Davis, and Morgenstern\\n2011), but adjusted to '*

 * *                      'improve the scale and robustness against the dataset-specific bias. '*

 * *                      'Formulated as a\\nfill-in-a-blank task with binary options, the goal is to '*

 * *                      'choose the right option for a given sentence which requires\\ncommonsense '*

 * *                      "r […]*

```diff
@@ -1,43 +1,44 @@
 {
+    "__description__": "WinoGrande is a new collection of 44k problems, inspired by Winograd Schema Challenge (Levesque, Davis, and Morgenstern\n2011), but adjusted to improve the scale and robustness against the dataset-specific bias. Formulated as a\nfill-in-a-blank task with binary options, the goal is to choose the right option for a given sentence which requires\ncommonsense reasoning.",
+    "__tags__": {
+        "croissant": true,
+        "language": "en",
+        "region": "us"
+    },
     "loader": {
-        "path": "ag_news",
+        "name": "winogrande_l",
+        "path": "winogrande",
         "type": "load_hf"
     },
     "preprocess_steps": [
+        "splitters.small_no_test",
         {
-            "mix": {
-                "test": "test",
-                "train": "train[87.5%]",
-                "validation": "train[12.5%]"
-            },
-            "type": "split_random_mix"
+            "fields": [
+                "option1",
+                "option2"
+            ],
+            "to_field": "choices",
+            "type": "list_field_values"
         },
         {
-            "mappers": {
-                "label": {
-                    "0": "World",
-                    "1": "Sports",
-                    "2": "Business",
-                    "3": "Sci/Tech"
-                }
+            "fields": {
+                "answer": "int"
             },
-            "type": "map_instance_values"
+            "type": "cast_fields"
         },
         {
-            "fields": {
-                "classes": [
-                    "World",
-                    "Sports",
-                    "Business",
-                    "Sci/Tech"
-                ],
-                "text_type": "sentence",
-                "type_of_class": "topic"
+            "add": -1,
+            "field": "answer",
+            "type": "add_constant"
+        },
+        {
+            "field_to_field": {
+                "sentence": "question"
             },
-            "type": "add_fields"
+            "type": "rename_fields"
         }
     ],
-    "task": "tasks.classification.multi_class",
-    "templates": "templates.classification.multi_class.all",
+    "task": "tasks.qa.multiple_choice.open",
+    "templates": "templates.qa.multiple_choice.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/ai2_arc/arc_challenge.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/rag/response_generation/clapnq.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6754166666666667%*

 * *Differences: {"'loader'": "{'path': 'PrimeQA/clapnq', delete: ['name']}",*

 * * "'preprocess_steps'": "{0: {'type': 'split_random_mix', 'mix': OrderedDict([('train', 'train'), "*

 * *                       "('test', 'validation')]), delete: ['field_to_field']}, 1: "*

 * *                       "{'field_to_field': {replace: OrderedDict([('passages/*/text', 'contexts'), "*

 * *                       "('input', 'question'), ('output/*/answer', 'reference_answers')])}}, 2: "*

 * *                       "{'type': 'add_fields', 'fields': OrderedDict( […]*

```diff
@@ -1,38 +1,34 @@
 {
     "loader": {
-        "name": "ARC-Challenge",
-        "path": "ai2_arc",
+        "path": "PrimeQA/clapnq",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "fields": {
-                "topic": "science"
-            },
-            "type": "add_fields"
-        },
-        {
-            "field_to_field": {
-                "answerKey": "label",
-                "choices": "_choices"
+            "mix": {
+                "test": "validation",
+                "train": "train"
             },
-            "type": "rename_fields"
+            "type": "split_random_mix"
         },
         {
             "field_to_field": {
-                "_choices/label": "labels",
-                "_choices/text": "choices"
+                "input": "question",
+                "output/*/answer": "reference_answers",
+                "passages/*/text": "contexts"
             },
             "type": "copy_fields"
         },
         {
-            "index_of": "label",
-            "search_in": "labels",
-            "to_field": "answer",
-            "type": "index_of"
+            "fields": {
+                "contexts_ids": []
+            },
+            "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_topic",
-    "templates": "templates.qa.multiple_choice.with_topic.all",
+    "task": "tasks.rag.response_generation",
+    "templates": {
+        "default": "templates.rag.response_generation.simple"
+    },
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/ai2_arc/arc_easy.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/hellaswag.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4803571428571428%*

 * *Differences: {"'__description__'": "'HellaSwag: Can a Machine Really Finish Your Sentence? is a new dataset for "*

 * *                      "commonsense NLI. A paper was published at ACL2019.'",*

 * * "'__tags__'": "OrderedDict([('arxiv', '1905.07830'), ('croissant', True), ('language', 'en'), "*

 * *               "('region', 'us')])",*

 * * "'loader'": "{'path': 'hellaswag', delete: ['name']}",*

 * * "'preprocess_steps'": "{1: {'field_to_field': {replace: OrderedDict([('ctx', 'context'), "*

 * *                       "('activity_label', 'topic'), […]*

```diff
@@ -1,38 +1,45 @@
 {
+    "__description__": "HellaSwag: Can a Machine Really Finish Your Sentence? is a new dataset for commonsense NLI. A paper was published at ACL2019.",
+    "__tags__": {
+        "arxiv": "1905.07830",
+        "croissant": true,
+        "language": "en",
+        "region": "us"
+    },
     "loader": {
-        "name": "ARC-Easy",
-        "path": "ai2_arc",
+        "path": "hellaswag",
         "type": "load_hf"
     },
     "preprocess_steps": [
+        "splitters.large_no_test",
         {
-            "fields": {
-                "topic": "science"
+            "field_to_field": {
+                "activity_label": "topic",
+                "ctx": "context",
+                "endings": "choices"
             },
-            "type": "add_fields"
+            "type": "rename_fields"
         },
         {
             "field_to_field": {
-                "answerKey": "label",
-                "choices": "_choices"
+                "label": "answer"
             },
             "type": "rename_fields"
         },
         {
-            "field_to_field": {
-                "_choices/label": "labels",
-                "_choices/text": "choices"
+            "fields": {
+                "answer": "int"
             },
-            "type": "copy_fields"
+            "type": "cast_fields"
         },
         {
-            "index_of": "label",
-            "search_in": "labels",
-            "to_field": "answer",
-            "type": "index_of"
+            "fields": {
+                "context_type": "sentence"
+            },
+            "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_topic",
-    "templates": "templates.qa.multiple_choice.with_topic.all",
+    "task": "tasks.completion.multiple_choice",
+    "templates": "templates.completion.multiple_choice.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/almost_evil/de.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mt_bench/response_assessment/rating/single_turn_with_reference_gpt4_judgement.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6677083333333333%*

 * *Differences: {"'loader'": "{'path': 'OfirArviv/mt_bench_single_score_gpt4_judgement', 'split': 'train'}",*

 * * "'preprocess_steps'": "{0: {'type': 'rename_splits', 'mapper': OrderedDict([('train', 'test')]), "*

 * *                       "delete: ['field_to_field']}, 1: {'values': {replace: OrderedDict([('turn', "*

 * *                       "1)])}}, 2: {'type': 'filter_by_condition', 'values': "*

 * *                       "OrderedDict([('reference', '[]')]), 'condition': 'ne', delete: ['mix']}, "*

 * *                       "3: {'field_to_fi […]*

```diff
@@ -1,63 +1,77 @@
 {
     "loader": {
-        "path": "0x22almostEvil/multilingual-wikihow-qa-16k",
+        "path": "OfirArviv/mt_bench_single_score_gpt4_judgement",
+        "split": "train",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "_argv": [
-                "METADATA"
-            ],
-            "function": "json.loads",
-            "to_field": "metadata",
-            "type": "apply"
+            "mapper": {
+                "train": "test"
+            },
+            "type": "rename_splits"
         },
         {
-            "field_to_field": [
-                [
-                    "metadata/language",
-                    "extracted_language"
-                ]
-            ],
-            "type": "copy_fields"
+            "condition": "eq",
+            "type": "filter_by_condition",
+            "values": {
+                "turn": 1
+            }
         },
         {
-            "condition": "eq",
+            "condition": "ne",
             "type": "filter_by_condition",
             "values": {
-                "extracted_language": "de"
+                "reference": "[]"
             }
         },
         {
-            "fields": [
-                "extracted_language",
-                "metadata"
-            ],
-            "type": "remove_fields"
+            "field_to_field": {
+                "category": "group",
+                "model_input": "question",
+                "model_output": "answer",
+                "reference": "reference_answer",
+                "score": "rating"
+            },
+            "type": "rename_fields"
+        },
+        {
+            "field": "question",
+            "to_field": "question",
+            "type": "literal_eval"
         },
         {
-            "mix": {
-                "test": "train[5%]",
-                "train": "train[90%]",
-                "validation": "train[5%]"
+            "field_to_field": {
+                "question/0": "question"
             },
-            "type": "split_random_mix"
+            "type": "copy_fields"
+        },
+        {
+            "field": "answer",
+            "to_field": "answer",
+            "type": "literal_eval"
         },
         {
             "field_to_field": {
-                "INSTRUCTION": "question"
+                "answer/0": "answer"
             },
-            "type": "rename_fields"
+            "type": "copy_fields"
         },
         {
-            "fields": [
-                "RESPONSE"
-            ],
-            "to_field": "answers",
-            "type": "list_field_values"
+            "field": "reference_answer",
+            "to_field": "reference_answer",
+            "type": "literal_eval"
+        },
+        {
+            "field_to_field": {
+                "reference_answer/0": "reference_answer"
+            },
+            "type": "copy_fields"
         }
     ],
-    "task": "tasks.qa.open",
-    "templates": "templates.qa.open.all",
+    "task": "tasks.response_assessment.rating.single_turn_with_reference",
+    "templates": [
+        "templates.response_assessment.rating.mt_bench_single_turn_with_reference"
+    ],
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/almost_evil/en.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/toxigen.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.673148148148148%*

 * *Differences: {"'loader'": "{'path': 'skg/toxigen-data', 'name': 'train'}",*

 * * "'preprocess_steps'": "{0: {'type': 'shuffle', 'page_size': 251000, delete: ['fields']}, 1: "*

 * *                       "{'mix': {'train': 'train[20%]', 'test': 'train[80%]', delete: "*

 * *                       "['validation']}}, 4: {'field_to_field': {replace: "*

 * *                       "OrderedDict([('prompt_label', 'label')])}}, 5: {'type': 'add_fields', "*

 * *                       "'fields': {replace: OrderedDict([('classes', ['not toxic', 'toxic']), " […]*

```diff
@@ -1,63 +1,68 @@
 {
     "loader": {
-        "path": "0x22almostEvil/multilingual-wikihow-qa-16k",
+        "name": "train",
+        "path": "skg/toxigen-data",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "_argv": [
-                "METADATA"
-            ],
-            "function": "json.loads",
-            "to_field": "metadata",
-            "type": "apply"
+            "page_size": 251000,
+            "type": "shuffle"
         },
         {
-            "field_to_field": [
-                [
-                    "metadata/language",
-                    "extracted_language"
-                ]
-            ],
-            "type": "copy_fields"
-        },
-        {
-            "condition": "eq",
-            "type": "filter_by_condition",
-            "values": {
-                "extracted_language": "en"
-            }
+            "mix": {
+                "test": "train[80%]",
+                "train": "train[20%]"
+            },
+            "type": "split_random_mix"
         },
         {
-            "fields": [
-                "extracted_language",
-                "metadata"
-            ],
-            "type": "remove_fields"
+            "mappers": {
+                "prompt_label": {
+                    "0": "not toxic",
+                    "1": "toxic"
+                }
+            },
+            "type": "map_instance_values"
         },
         {
-            "mix": {
-                "test": "train[5%]",
-                "train": "train[90%]",
-                "validation": "train[5%]"
+            "field_to_field": {
+                "prompt": "text"
             },
-            "type": "split_random_mix"
+            "type": "rename_fields"
         },
         {
             "field_to_field": {
-                "INSTRUCTION": "question"
+                "prompt_label": "label"
             },
             "type": "rename_fields"
         },
         {
-            "fields": [
-                "RESPONSE"
-            ],
-            "to_field": "answers",
-            "type": "list_field_values"
+            "fields": {
+                "classes": [
+                    "not toxic",
+                    "toxic"
+                ],
+                "text_type": "text",
+                "type_of_class": "toxicity"
+            },
+            "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.open",
-    "templates": "templates.qa.open.all",
+    "task": "tasks.classification.multi_class",
+    "templates": {
+        "items": [
+            {
+                "input_format": "Given this {text_type}: {text}. Classify if it contains {type_of_class}. classes: {classes}. I would classify this {text_type} as: ",
+                "output_format": "{label}",
+                "postprocessors": [
+                    "processors.take_first_non_empty_line",
+                    "processors.toxic_or_not_toxic"
+                ],
+                "type": "input_output_template"
+            }
+        ],
+        "type": "templates_list"
+    },
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/almost_evil/es.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/xnli/fr.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.47420634920634924%*

 * *Differences: {"'__description__'": '\'Dataset Card for "xnli"\\nDataset Summary\\nXNLI is a subset of a few '*

 * *                      'thousand examples from MNLI which has been translated\\ninto a 14 different '*

 * *                      'languages (some low-ish resource). As with MNLI, the goal is\\nto predict '*

 * *                      'textual entailment (does sentence A imply/contradict/neither sentence\\nB) '*

 * *                      'and is a classification task (given two sentences, predict one of '*

 * *                      't […]*

```diff
@@ -1,63 +1,71 @@
 {
+    "__description__": "Dataset Card for \"xnli\"\nDataset Summary\nXNLI is a subset of a few thousand examples from MNLI which has been translated\ninto a 14 different languages (some low-ish resource). As with MNLI, the goal is\nto predict textual entailment (does sentence A imply/contradict/neither sentence\nB) and is a classification task (given two sentences, predict one of three\nlabels).\nSupported Tasks and Leaderboards\nMore Information Needed\nLanguages\nMore\u2026 See the full description on the dataset page: https://huggingface.co/datasets/xnli.",
+    "__tags__": {
+        "croissant": true,
+        "language": [
+            "ar",
+            "bg",
+            "de",
+            "el",
+            "en",
+            "es",
+            "fr",
+            "hi",
+            "ru",
+            "sw",
+            "th",
+            "tr",
+            "ur",
+            "vi",
+            "zh"
+        ],
+        "region": "us"
+    },
     "loader": {
-        "path": "0x22almostEvil/multilingual-wikihow-qa-16k",
+        "name": "fr",
+        "path": "xnli",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "_argv": [
-                "METADATA"
-            ],
-            "function": "json.loads",
-            "to_field": "metadata",
-            "type": "apply"
-        },
-        {
-            "field_to_field": [
-                [
-                    "metadata/language",
-                    "extracted_language"
-                ]
-            ],
-            "type": "copy_fields"
-        },
-        {
-            "condition": "eq",
-            "type": "filter_by_condition",
-            "values": {
-                "extracted_language": "es"
-            }
-        },
-        {
-            "fields": [
-                "extracted_language",
-                "metadata"
-            ],
-            "type": "remove_fields"
-        },
-        {
-            "mix": {
-                "test": "train[5%]",
-                "train": "train[90%]",
-                "validation": "train[5%]"
+            "mapper": {
+                "validation_matched": "validation"
             },
-            "type": "split_random_mix"
+            "type": "rename_splits"
         },
+        "splitters.small_no_test",
         {
             "field_to_field": {
-                "INSTRUCTION": "question"
+                "hypothesis": "text_b",
+                "premise": "text_a"
             },
             "type": "rename_fields"
         },
         {
-            "fields": [
-                "RESPONSE"
-            ],
-            "to_field": "answers",
-            "type": "list_field_values"
+            "mappers": {
+                "label": {
+                    "0": "entailment",
+                    "1": "neutral",
+                    "2": "contradiction"
+                }
+            },
+            "type": "map_instance_values"
+        },
+        {
+            "fields": {
+                "classes": [
+                    "entailment",
+                    "neutral",
+                    "contradiction"
+                ],
+                "text_a_type": "premise",
+                "text_b_type": "hypothesis",
+                "type_of_relation": "entailment"
+            },
+            "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.open",
-    "templates": "templates.qa.open.all",
+    "task": "tasks.classification.multi_class.relation",
+    "templates": "templates.classification.multi_class.relation.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/almost_evil/fr.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/xnli/sw.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.47420634920634924%*

 * *Differences: {"'__description__'": '\'Dataset Card for "xnli"\\nDataset Summary\\nXNLI is a subset of a few '*

 * *                      'thousand examples from MNLI which has been translated\\ninto a 14 different '*

 * *                      'languages (some low-ish resource). As with MNLI, the goal is\\nto predict '*

 * *                      'textual entailment (does sentence A imply/contradict/neither sentence\\nB) '*

 * *                      'and is a classification task (given two sentences, predict one of '*

 * *                      't […]*

```diff
@@ -1,63 +1,71 @@
 {
+    "__description__": "Dataset Card for \"xnli\"\nDataset Summary\nXNLI is a subset of a few thousand examples from MNLI which has been translated\ninto a 14 different languages (some low-ish resource). As with MNLI, the goal is\nto predict textual entailment (does sentence A imply/contradict/neither sentence\nB) and is a classification task (given two sentences, predict one of three\nlabels).\nSupported Tasks and Leaderboards\nMore Information Needed\nLanguages\nMore\u2026 See the full description on the dataset page: https://huggingface.co/datasets/xnli.",
+    "__tags__": {
+        "croissant": true,
+        "language": [
+            "ar",
+            "bg",
+            "de",
+            "el",
+            "en",
+            "es",
+            "fr",
+            "hi",
+            "ru",
+            "sw",
+            "th",
+            "tr",
+            "ur",
+            "vi",
+            "zh"
+        ],
+        "region": "us"
+    },
     "loader": {
-        "path": "0x22almostEvil/multilingual-wikihow-qa-16k",
+        "name": "sw",
+        "path": "xnli",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "_argv": [
-                "METADATA"
-            ],
-            "function": "json.loads",
-            "to_field": "metadata",
-            "type": "apply"
-        },
-        {
-            "field_to_field": [
-                [
-                    "metadata/language",
-                    "extracted_language"
-                ]
-            ],
-            "type": "copy_fields"
-        },
-        {
-            "condition": "eq",
-            "type": "filter_by_condition",
-            "values": {
-                "extracted_language": "fr"
-            }
-        },
-        {
-            "fields": [
-                "extracted_language",
-                "metadata"
-            ],
-            "type": "remove_fields"
-        },
-        {
-            "mix": {
-                "test": "train[5%]",
-                "train": "train[90%]",
-                "validation": "train[5%]"
+            "mapper": {
+                "validation_matched": "validation"
             },
-            "type": "split_random_mix"
+            "type": "rename_splits"
         },
+        "splitters.small_no_test",
         {
             "field_to_field": {
-                "INSTRUCTION": "question"
+                "hypothesis": "text_b",
+                "premise": "text_a"
             },
             "type": "rename_fields"
         },
         {
-            "fields": [
-                "RESPONSE"
-            ],
-            "to_field": "answers",
-            "type": "list_field_values"
+            "mappers": {
+                "label": {
+                    "0": "entailment",
+                    "1": "neutral",
+                    "2": "contradiction"
+                }
+            },
+            "type": "map_instance_values"
+        },
+        {
+            "fields": {
+                "classes": [
+                    "entailment",
+                    "neutral",
+                    "contradiction"
+                ],
+                "text_a_type": "premise",
+                "text_b_type": "hypothesis",
+                "type_of_relation": "entailment"
+            },
+            "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.open",
-    "templates": "templates.qa.open.all",
+    "task": "tasks.classification.multi_class.relation",
+    "templates": "templates.classification.multi_class.relation.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/almost_evil/it.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mt_bench/response_assessment/pairwise_comparison/single_turn_gpt4_judgement.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6695833333333333%*

 * *Differences: {"'loader'": "{'path': 'OfirArviv/mt_bench_pairwise_comparison_gpt4_judgments', 'split': 'train'}",*

 * * "'preprocess_steps'": "{0: {'type': 'rename_splits', 'mapper': OrderedDict([('train', 'test')]), "*

 * *                       "delete: ['function', 'to_field', '_argv']}, 1: {'type': "*

 * *                       "'filter_by_condition', 'values': OrderedDict([('turn', 1)]), 'condition': "*

 * *                       "'eq', delete: ['field_to_field']}, 2: {'values': {replace: "*

 * *                       "OrderedDict([('refere […]*

```diff
@@ -1,63 +1,97 @@
 {
     "loader": {
-        "path": "0x22almostEvil/multilingual-wikihow-qa-16k",
+        "path": "OfirArviv/mt_bench_pairwise_comparison_gpt4_judgments",
+        "split": "train",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "_argv": [
-                "METADATA"
-            ],
-            "function": "json.loads",
-            "to_field": "metadata",
-            "type": "apply"
+            "mapper": {
+                "train": "test"
+            },
+            "type": "rename_splits"
         },
         {
-            "field_to_field": [
-                [
-                    "metadata/language",
-                    "extracted_language"
-                ]
-            ],
-            "type": "copy_fields"
+            "condition": "eq",
+            "type": "filter_by_condition",
+            "values": {
+                "turn": 1
+            }
         },
         {
             "condition": "eq",
             "type": "filter_by_condition",
             "values": {
-                "extracted_language": "it"
+                "reference": "[]"
             }
         },
         {
-            "fields": [
-                "extracted_language",
-                "metadata"
-            ],
-            "type": "remove_fields"
+            "condition": "in",
+            "type": "filter_by_condition",
+            "values": {
+                "winner": [
+                    "model_1",
+                    "tie",
+                    "model_2"
+                ]
+            }
         },
         {
-            "mix": {
-                "test": "train[5%]",
-                "train": "train[90%]",
-                "validation": "train[5%]"
+            "mappers": {
+                "winner": {
+                    "model_1": "choice_a",
+                    "model_2": "choice_b",
+                    "tie": "tie"
+                }
             },
-            "type": "split_random_mix"
+            "type": "map_instance_values"
         },
         {
             "field_to_field": {
-                "INSTRUCTION": "question"
+                "category": "group",
+                "model_1_output": "answer_a",
+                "model_2_output": "answer_b",
+                "model_input": "question"
             },
             "type": "rename_fields"
         },
         {
-            "fields": [
-                "RESPONSE"
-            ],
-            "to_field": "answers",
-            "type": "list_field_values"
+            "field": "question",
+            "to_field": "question",
+            "type": "literal_eval"
+        },
+        {
+            "field_to_field": {
+                "question/0": "question"
+            },
+            "type": "copy_fields"
+        },
+        {
+            "field": "answer_a",
+            "to_field": "answer_a",
+            "type": "literal_eval"
+        },
+        {
+            "field_to_field": {
+                "answer_a/0": "answer_a"
+            },
+            "type": "copy_fields"
+        },
+        {
+            "field": "answer_b",
+            "to_field": "answer_b",
+            "type": "literal_eval"
+        },
+        {
+            "field_to_field": {
+                "answer_b/0": "answer_b"
+            },
+            "type": "copy_fields"
         }
     ],
-    "task": "tasks.qa.open",
-    "templates": "templates.qa.open.all",
+    "task": "tasks.response_assessment.pairwise_comparison.single_turn",
+    "templates": [
+        "templates.response_assessment.pairwise_comparison.mt_bench_single_turn_with_shuffle"
+    ],
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/almost_evil/nl.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/legalbench/proa.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.47534013605442177%*

 * *Differences: {"'__description__'": "'LegalBench is a collection of benchmark tasks for evaluating legal "*

 * *                      "reasoning in large language models.'",*

 * * "'__tags__'": "OrderedDict([('arxiv', '2308.11462'), ('croissant', True), ('finance', True), "*

 * *               "('language', 'en'), ('law', True), ('legal', True), ('license', 'other'), "*

 * *               "('region', 'us'), ('size_categories', '10K<n<100K'), ('task_categories', "*

 * *               "['text-classification', 'question-answering', 'text-generation […]*

```diff
@@ -1,63 +1,63 @@
 {
+    "__description__": "LegalBench is a collection of benchmark tasks for evaluating legal reasoning in large language models.",
+    "__tags__": {
+        "arxiv": "2308.11462",
+        "croissant": true,
+        "finance": true,
+        "language": "en",
+        "law": true,
+        "legal": true,
+        "license": "other",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "task_categories": [
+            "text-classification",
+            "question-answering",
+            "text-generation"
+        ]
+    },
     "loader": {
-        "path": "0x22almostEvil/multilingual-wikihow-qa-16k",
+        "name": "proa",
+        "path": "nguha/legalbench",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "_argv": [
-                "METADATA"
-            ],
-            "function": "json.loads",
-            "to_field": "metadata",
-            "type": "apply"
-        },
-        {
-            "field_to_field": [
-                [
-                    "metadata/language",
-                    "extracted_language"
-                ]
-            ],
-            "type": "copy_fields"
-        },
-        {
-            "condition": "eq",
-            "type": "filter_by_condition",
-            "values": {
-                "extracted_language": "nl"
-            }
-        },
-        {
-            "fields": [
-                "extracted_language",
-                "metadata"
-            ],
-            "type": "remove_fields"
-        },
-        {
-            "mix": {
-                "test": "train[5%]",
-                "train": "train[90%]",
-                "validation": "train[5%]"
-            },
-            "type": "split_random_mix"
-        },
-        {
             "field_to_field": {
-                "INSTRUCTION": "question"
+                "answer": "label",
+                "text": "text"
             },
             "type": "rename_fields"
         },
         {
-            "fields": [
-                "RESPONSE"
-            ],
-            "to_field": "answers",
-            "type": "list_field_values"
+            "fields": {
+                "classes": [
+                    "Yes",
+                    "No"
+                ],
+                "classes_descriptions": "A private right of action is when a regular person, a private citizen, is legally entitled to enforce their rights under a given statute",
+                "text_type": "clause",
+                "type_of_class": "a private right of action"
+            },
+            "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.open",
-    "templates": "templates.qa.open.all",
+    "task": "tasks.classification.multi_class.with_classes_descriptions",
+    "templates": {
+        "default": {
+            "input_format": "{text_type}: {text}",
+            "instruction": "{classes_descriptions}. Does the {text_type} specify {type_of_class}? Answer from one of {classes}",
+            "output_format": "{label}",
+            "postprocessors": [
+                "processors.take_first_non_empty_line",
+                "processors.lower_case_till_punc"
+            ],
+            "target_prefix": "A: ",
+            "title_fields": [
+                "text_type"
+            ],
+            "type": "input_output_template"
+        }
+    },
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/almost_evil/pt.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/almost_evil.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.673469387755102%*

 * *Differences: {"'__description__'": "'Dataset Card for multilingual WikiHow with ~16.8K entries. ~(2-2.2)K for "*

 * *                      'each language.\\nWarning [1]\\nThe WikiHow team contacted me and made it '*

 * *                      'clear that they forbid the use of their data for machine learning purposes. '*

 * *                      'However, I am not calling for anything, and this dataset only shows the '*

 * *                      'concept, and I strongly advise against violating their ToS.\\nHowever, '*

 * *                      […]*

```diff
@@ -1,45 +1,34 @@
 {
+    "__description__": "Dataset Card for multilingual WikiHow with ~16.8K entries. ~(2-2.2)K for each language.\nWarning [1]\nThe WikiHow team contacted me and made it clear that they forbid the use of their data for machine learning purposes. However, I am not calling for anything, and this dataset only shows the concept, and I strongly advise against violating their ToS.\nHowever, consultation with lawyers made it clear that dataset can be used for such purposes if the project has\u2026 See the full description on the dataset page: https://huggingface.co/datasets/0x22almostEvil/multilingual-wikihow-qa-16k.",
+    "__tags__": {
+        "QnA": true,
+        "croissant": true,
+        "language": [
+            "en",
+            "ru",
+            "pt",
+            "it",
+            "es",
+            "fr",
+            "de",
+            "nl"
+        ],
+        "license": "cc-by-nc-3.0",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "task_categories": "question-answering",
+        "wikihow": true
+    },
     "loader": {
         "path": "0x22almostEvil/multilingual-wikihow-qa-16k",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "_argv": [
-                "METADATA"
-            ],
-            "function": "json.loads",
-            "to_field": "metadata",
-            "type": "apply"
-        },
-        {
-            "field_to_field": [
-                [
-                    "metadata/language",
-                    "extracted_language"
-                ]
-            ],
-            "type": "copy_fields"
-        },
-        {
-            "condition": "eq",
-            "type": "filter_by_condition",
-            "values": {
-                "extracted_language": "pt"
-            }
-        },
-        {
-            "fields": [
-                "extracted_language",
-                "metadata"
-            ],
-            "type": "remove_fields"
-        },
-        {
             "mix": {
                 "test": "train[5%]",
                 "train": "train[90%]",
                 "validation": "train[5%]"
             },
             "type": "split_random_mix"
         },
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/almost_evil/ru.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/coedit_gec.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.47135416666666663%*

 * *Differences: {"'__description__'": "'Dataset Card for CoEdIT: Text Editing via Instruction Tuning\\nPaper: "*

 * *                      'CoEdIT: Text Editing by Task-Specific Instruction Tuning\\nAuthors: Vipul '*

 * *                      'Raheja, Dhruv Kumar, Ryan Koo, Dongyeop Kang\\nProject Repo: '*

 * *                      'https://github.com/vipulraheja/coedit\\nDataset Summary\\nThis is the '*

 * *                      'dataset that was used to train the CoEdIT text editing models. Full details '*

 * *                      'of the datas […]*

```diff
@@ -1,63 +1,52 @@
 {
+    "__description__": "Dataset Card for CoEdIT: Text Editing via Instruction Tuning\nPaper: CoEdIT: Text Editing by Task-Specific Instruction Tuning\nAuthors: Vipul Raheja, Dhruv Kumar, Ryan Koo, Dongyeop Kang\nProject Repo: https://github.com/vipulraheja/coedit\nDataset Summary\nThis is the dataset that was used to train the CoEdIT text editing models. Full details of the dataset can be found in our paper.\nDataset Structure\nThe\u2026 See the full description on the dataset page: https://huggingface.co/datasets/grammarly/coedit.",
+    "__tags__": {
+        "arxiv": "2305.09857",
+        "croissant": true,
+        "language": "en",
+        "license": "apache-2.0",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "task_categories": "text-generation"
+    },
     "loader": {
-        "path": "0x22almostEvil/multilingual-wikihow-qa-16k",
+        "filtering_lambda": "lambda x: x['task'] == 'gec'",
+        "path": "grammarly/coedit",
+        "streaming": true,
         "type": "load_hf"
     },
     "preprocess_steps": [
+        "splitters.small_no_test",
         {
-            "_argv": [
-                "METADATA"
-            ],
-            "function": "json.loads",
-            "to_field": "metadata",
-            "type": "apply"
-        },
-        {
-            "field_to_field": [
-                [
-                    "metadata/language",
-                    "extracted_language"
-                ]
-            ],
-            "type": "copy_fields"
-        },
-        {
-            "condition": "eq",
-            "type": "filter_by_condition",
-            "values": {
-                "extracted_language": "ru"
-            }
+            "by": ": ",
+            "field": "src",
+            "type": "split"
         },
         {
-            "fields": [
-                "extracted_language",
-                "metadata"
-            ],
-            "type": "remove_fields"
+            "field": "src",
+            "start": 1,
+            "type": "slice"
         },
         {
-            "mix": {
-                "test": "train[5%]",
-                "train": "train[90%]",
-                "validation": "train[5%]"
-            },
-            "type": "split_random_mix"
+            "by": ": ",
+            "field": "src",
+            "type": "join"
         },
         {
             "field_to_field": {
-                "INSTRUCTION": "question"
+                "src": "original_text"
             },
             "type": "rename_fields"
         },
         {
             "fields": [
-                "RESPONSE"
+                "tgt"
             ],
-            "to_field": "answers",
+            "to_field": "corrected_texts",
             "type": "list_field_values"
         }
     ],
-    "task": "tasks.qa.open",
-    "templates": "templates.qa.open.all",
+    "task": "tasks.grammatical_error_correction",
+    "templates": "templates.grammatical_error_correction.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/almost_evil.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/wmt/en_ro.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6652777777777777%*

 * *Differences: {"'loader'": "{'path': 'wmt16', 'name': 'ro-en', 'streaming': True}",*

 * * "'preprocess_steps'": "{0: {'type': 'copy_fields', 'field_to_field': [['translation/en', 'text'], "*

 * *                       "['translation/ro', 'translation']]}, 1: {'type': 'add_fields', 'fields': "*

 * *                       "{replace: OrderedDict([('source_language', 'english'), ('target_language', "*

 * *                       "'romanian')])}, delete: ['to_field']}, delete: [0]}",*

 * * "'task'": "'tasks.translation.directed'",*

 * * "'templates'": "'te […]*

```diff
@@ -1,32 +1,33 @@
 {
     "loader": {
-        "path": "0x22almostEvil/multilingual-wikihow-qa-16k",
+        "name": "ro-en",
+        "path": "wmt16",
+        "streaming": true,
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mix": {
-                "test": "train[5%]",
-                "train": "train[90%]",
-                "validation": "train[5%]"
-            },
-            "type": "split_random_mix"
+            "field_to_field": [
+                [
+                    "translation/en",
+                    "text"
+                ],
+                [
+                    "translation/ro",
+                    "translation"
+                ]
+            ],
+            "type": "copy_fields"
         },
         {
-            "field_to_field": {
-                "INSTRUCTION": "question"
+            "fields": {
+                "source_language": "english",
+                "target_language": "romanian"
             },
-            "type": "rename_fields"
-        },
-        {
-            "fields": [
-                "RESPONSE"
-            ],
-            "to_field": "answers",
-            "type": "list_field_values"
+            "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.open",
-    "templates": "templates.qa.open.all",
+    "task": "tasks.translation.directed",
+    "templates": "templates.translation.directed.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/argument_topic.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/law_stack_exchange.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6202380952380953%*

 * *Differences: {"'__description__'": "'Dataset Card for Law Stack Exchange Dataset\\nDataset Summary\\nDataset "*

 * *                      'from the Law Stack Exchange, as used in "Parameter-Efficient Legal Domain '*

 * *                      'Adaptation".\\nCitation '*

 * *                      'Information\\n@inproceedings{li-etal-2022-parameter,\\ntitle = '*

 * *                      '"Parameter-Efficient Legal Domain Adaptation",\\nauthor = "Li, Jonathan  '*

 * *                      'and\\nBhambhoria, Rohan  and\\nZhu, Xiaodan",\\nbooktitle […]*

```diff
@@ -1,90 +1,71 @@
 {
+    "__description__": "Dataset Card for Law Stack Exchange Dataset\nDataset Summary\nDataset from the Law Stack Exchange, as used in \"Parameter-Efficient Legal Domain Adaptation\".\nCitation Information\n@inproceedings{li-etal-2022-parameter,\ntitle = \"Parameter-Efficient Legal Domain Adaptation\",\nauthor = \"Li, Jonathan  and\nBhambhoria, Rohan  and\nZhu, Xiaodan\",\nbooktitle = \"Proceedings of the Natural Legal Language Processing Workshop 2022\",\nmonth =\u2026 See the full description on the dataset page: https://huggingface.co/datasets/jonathanli/law-stack-exchange.",
+    "__tags__": {
+        "croissant": true,
+        "language": "en",
+        "law": true,
+        "region": "us",
+        "stackexchange": true,
+        "task_categories": "text-classification"
+    },
     "loader": {
-        "name": "argument_topic",
-        "path": "ibm/argument_quality_ranking_30k",
+        "path": "jonathanli/law-stack-exchange",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
+            "mix": {
+                "test": "train",
+                "train": "test",
+                "validation": "validation"
+            },
+            "type": "split_random_mix"
+        },
+        {
+            "field_to_field": {
+                "text_label": "label"
+            },
+            "type": "rename_fields"
+        },
+        {
+            "fields": [
+                "title",
+                "body"
+            ],
+            "to_field": "text",
+            "type": "list_field_values"
+        },
+        {
+            "field": "text",
+            "separator": ". ",
+            "to_field": "text",
+            "type": "join_str"
+        },
+        {
             "fields": {
                 "classes": [
-                    "affirmative action",
-                    "algorithmic trading",
-                    "assisted suicide",
-                    "atheism",
-                    "austerity regime",
-                    "blockade of the gaza strip",
-                    "cancel pride parades",
-                    "cannabis",
-                    "capital punishment",
-                    "collectivism",
-                    "compulsory voting",
-                    "cosmetic surgery",
-                    "cosmetic surgery for minors",
-                    "embryonic stem cell research",
-                    "entrapment",
-                    "executive compensation",
-                    "factory farming",
-                    "fast food",
-                    "fight urbanization",
-                    "flag burning",
-                    "foster care",
-                    "gender-neutral language",
-                    "guantanamo bay detention camp",
-                    "holocaust denial",
-                    "homeopathy",
-                    "homeschooling",
-                    "human cloning",
-                    "intellectual property rights",
-                    "intelligence tests",
-                    "journalism",
-                    "judicial activism",
-                    "libertarianism",
-                    "marriage",
-                    "missionary work",
-                    "multi-party system",
-                    "naturopathy",
-                    "organ trade",
-                    "payday loans",
-                    "polygamy",
-                    "private military companies",
-                    "prostitution",
-                    "racial profiling",
-                    "retirement",
-                    "safe spaces",
-                    "school prayer",
-                    "sex selection",
-                    "social media",
-                    "space exploration",
-                    "stay-at-home dads",
-                    "student loans",
-                    "surrogacy",
-                    "targeted killing",
-                    "telemarketing",
-                    "television",
-                    "the abolition of nuclear weapons",
-                    "the church of scientology",
-                    "the development of autonomous cars",
-                    "the olympic games",
-                    "the right to keep and bear arms",
-                    "the three-strikes laws",
-                    "the use of child actors",
-                    "the use of economic sanctions",
-                    "the use of public defenders",
-                    "the use of school uniform",
-                    "the vow of celibacy",
-                    "vocational education",
-                    "whaling",
-                    "wikipedia",
-                    "women in combat",
-                    "zero-tolerance policy in schools",
-                    "zoos"
+                    "business",
+                    "civil-law",
+                    "constitutional-law",
+                    "contract",
+                    "contract-law",
+                    "copyright",
+                    "criminal-law",
+                    "employment",
+                    "intellectual-property",
+                    "internet",
+                    "liability",
+                    "licensing",
+                    "privacy",
+                    "software",
+                    "tax-law",
+                    "trademark"
                 ],
-                "text_type": "argument",
+                "text_type": "text",
                 "type_of_class": "topic"
             },
             "type": "add_fields"
         }
     ],
     "task": "tasks.classification.multi_class",
     "templates": "templates.classification.multi_class.all",
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/atis.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/atis.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'__tags__'": "OrderedDict([('croissant', True), ('region', 'us')])"}*

```diff
@@ -1,8 +1,12 @@
 {
+    "__tags__": {
+        "croissant": true,
+        "region": "us"
+    },
     "loader": {
         "path": "tuetschek/atis",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "delimiter": " ",
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/atta_q.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/atta_q.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9695%*

 * *Differences: {"'preprocess_steps'": "{4: {'type': 'dump_json', 'field': 'input_label', delete: ['function', "*

 * *                       "'to_field', '_argv']}}",*

 * * "'task'": "{'type': 'task'}"}*

```diff
@@ -24,33 +24,29 @@
             "field_to_field": {
                 "input": "input_label/input",
                 "label": "input_label/label"
             },
             "type": "copy_fields"
         },
         {
-            "_argv": [
-                "input_label"
-            ],
-            "function": "json.dumps",
-            "to_field": "input_label",
-            "type": "apply"
+            "field": "input_label",
+            "type": "dump_json"
         }
     ],
     "task": {
         "inputs": [
             "input"
         ],
         "metrics": [
             "metrics.safety"
         ],
         "outputs": [
             "input_label"
         ],
-        "type": "form_task"
+        "type": "task"
     },
     "templates": {
         "items": [
             {
                 "input_format": "{input}\n",
                 "output_format": "{input_label}",
                 "type": "input_output_template"
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/babi/qa.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mt_bench/generation/english_single_turn.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6799999999999999%*

 * *Differences: {"'loader'": "{'path': 'dim/mt_bench_en', 'split': 'train'}",*

 * * "'preprocess_steps'": "{2: {'field_to_field': {replace: OrderedDict([('turns', 'input'), "*

 * *                       "('category', 'group')])}}, 3: {'fields': {replace: OrderedDict([('output', "*

 * *                       "'None'), ('type_of_input', 'question'), ('type_of_output', 'answer')])}}, "*

 * *                       "insert: [(0, OrderedDict([('type', 'rename_splits'), ('mapper', "*

 * *                       "OrderedDict([('train', 'test')]))])), (1, O […]*

```diff
@@ -1,30 +1,41 @@
 {
     "loader": {
-        "path": "Muennighoff/babi",
+        "path": "dim/mt_bench_en",
+        "split": "train",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
+            "mapper": {
+                "train": "test"
+            },
+            "type": "rename_splits"
+        },
+        {
+            "field_to_field": {
+                "turns/0": "turns"
+            },
+            "type": "copy_fields"
+        },
+        {
             "field_to_field": {
-                "passage": "context"
+                "category": "group",
+                "turns": "input"
             },
             "type": "rename_fields"
         },
         {
             "fields": {
-                "context_type": "description"
+                "output": "None",
+                "type_of_input": "question",
+                "type_of_output": "answer"
             },
             "type": "add_fields"
-        },
-        {
-            "fields": [
-                "answer"
-            ],
-            "to_field": "answers",
-            "type": "list_field_values"
         }
     ],
-    "task": "tasks.qa.with_context.extractive",
-    "templates": "templates.qa.with_context.all",
+    "task": "tasks.generation",
+    "templates": [
+        "templates.empty"
+    ],
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/banking77.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/banking77.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7142857142857143%*

 * *Differences: {"'__description__'": "'BANKING77 dataset provides a very fine-grained set of intents in a banking "*

 * *                      'domain.\\nIt comprises 13,083 customer service queries labeled with 77 '*

 * *                      "intents.\\nIt focuses on fine-grained single-domain intent detection.'",*

 * * "'__tags__'": "OrderedDict([('annotations_creators', 'expert-generated'), ('arxiv', "*

 * *               "'2003.04807'), ('croissant', True), ('language', 'en'), ('language_creators', "*

 * *               "'expert-generated'), […]*

```diff
@@ -1,8 +1,26 @@
 {
+    "__description__": "BANKING77 dataset provides a very fine-grained set of intents in a banking domain.\nIt comprises 13,083 customer service queries labeled with 77 intents.\nIt focuses on fine-grained single-domain intent detection.",
+    "__tags__": {
+        "annotations_creators": "expert-generated",
+        "arxiv": "2003.04807",
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "cc-by-4.0",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "text-classification",
+        "task_ids": [
+            "intent-classification",
+            "multi-class-classification"
+        ]
+    },
     "loader": {
         "path": "PolyAI/banking77",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "page_size": 9223372036854775807,
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/acm_arab.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mt_bench/generation/japanese_single_turn.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6895833333333333%*

 * *Differences: {"'loader'": "{'path': 'shi3z/MTbenchJapanese', 'split': 'train', delete: ['name']}",*

 * * "'preprocess_steps'": "{0: {'mapper': {replace: OrderedDict([('train', 'test')])}}, 1: {'type': "*

 * *                       "'copy_fields', 'field_to_field': OrderedDict([('turns/0', 'turns')]), "*

 * *                       "delete: ['fields', 'to_field']}, 2: {'field_to_field': {replace: "*

 * *                       "OrderedDict([('turns', 'input'), ('category', 'group')])}}, 3: {'fields': "*

 * *                       "{replace: Ordere […]*

```diff
@@ -1,53 +1,41 @@
 {
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "acm_Arab",
+        "path": "shi3z/MTbenchJapanese",
+        "split": "train",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "acm_Arab": "test"
+                "train": "test"
             },
             "type": "rename_splits"
         },
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
             "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
+                "turns/0": "turns"
             },
-            "type": "rename_fields"
+            "type": "copy_fields"
         },
         {
-            "fields": {
-                "answer": "int"
+            "field_to_field": {
+                "category": "group",
+                "turns": "input"
             },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
+            "type": "rename_fields"
         },
         {
             "fields": {
-                "context_type": "passage"
+                "output": "None",
+                "type_of_input": "question",
+                "type_of_output": "answer"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.generation",
+    "templates": [
+        "templates.empty"
+    ],
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/afr_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/financebench.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6729166666666667%*

 * *Differences: {"'loader'": "{'path': 'PatronusAI/financebench', delete: ['name', 'split']}",*

 * * "'preprocess_steps'": "{0: {'type': 'split_random_mix', 'mix': OrderedDict([('train', "*

 * *                       "'train[10%]'), ('test', 'train[90%]')]), delete: ['mapper']}, 1: "*

 * *                       "{'field_to_field': {replace: OrderedDict([('answer', 'answers'), "*

 * *                       "('evidence_text', 'context')])}}, 2: {'type': 'list_field_values', "*

 * *                       "'fields': ['answers'], 'to_field': 'answers'} […]*

```diff
@@ -1,53 +1,38 @@
 {
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "afr_Latn",
+        "path": "PatronusAI/financebench",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mapper": {
-                "afr_Latn": "test"
+            "mix": {
+                "test": "train[90%]",
+                "train": "train[10%]"
             },
-            "type": "rename_splits"
-        },
-        {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
+            "type": "split_random_mix"
         },
         {
             "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
+                "answer": "answers",
+                "evidence_text": "context"
             },
             "type": "rename_fields"
         },
         {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
+            "fields": [
+                "answers"
+            ],
+            "to_field": "answers",
+            "type": "list_field_values"
         },
         {
             "fields": {
-                "context_type": "passage"
+                "context_type": "context"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.with_context.abstractive[metrics=[metrics.rag.response_generation.correctness.bert_score.deberta_large_mnli]]",
+    "templates": "templates.qa.with_context.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/als_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/medical_abstracts.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6405555555555555%*

 * *Differences: {"'loader'": "{'type': 'load_csv', 'files': OrderedDict([('train', "*

 * *             "'https://raw.githubusercontent.com/sebischair/Medical-Abstracts-TC-Corpus/main/medical_tc_train.csv'), "*

 * *             "('test', "*

 * *             "'https://raw.githubusercontent.com/sebischair/Medical-Abstracts-TC-Corpus/main/medical_tc_test.csv')]), "*

 * *             "delete: ['path', 'name', 'split']}",*

 * * "'preprocess_steps'": "{0: {'type': 'split_random_mix', 'mix': OrderedDict([('train', "*

 * *                       "'train[90%]'),  […]*

```diff
@@ -1,53 +1,55 @@
 {
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "als_Latn",
-        "type": "load_hf"
+        "files": {
+            "test": "https://raw.githubusercontent.com/sebischair/Medical-Abstracts-TC-Corpus/main/medical_tc_test.csv",
+            "train": "https://raw.githubusercontent.com/sebischair/Medical-Abstracts-TC-Corpus/main/medical_tc_train.csv"
+        },
+        "type": "load_csv"
     },
     "preprocess_steps": [
         {
-            "mapper": {
-                "als_Latn": "test"
+            "mix": {
+                "test": "test",
+                "train": "train[90%]",
+                "validation": "train[10%]"
             },
-            "type": "rename_splits"
-        },
-        {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
+            "type": "split_random_mix"
         },
         {
             "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
+                "condition_label": "label",
+                "medical_abstract": "text"
             },
             "type": "rename_fields"
         },
         {
-            "fields": {
-                "answer": "int"
+            "mappers": {
+                "label": {
+                    "1": "neoplasms",
+                    "2": "digestive system diseases",
+                    "3": "nervous system diseases",
+                    "4": "cardiovascular diseases",
+                    "5": "general pathological conditions"
+                }
             },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
+            "type": "map_instance_values"
         },
         {
             "fields": {
-                "context_type": "passage"
+                "classes": [
+                    "neoplasms",
+                    "digestive system diseases",
+                    "nervous system diseases",
+                    "cardiovascular diseases",
+                    "general pathological conditions"
+                ],
+                "text_type": "abstract",
+                "type_of_class": "topic"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.classification.multi_class",
+    "templates": "templates.classification.multi_class.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/amh_ethi.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/xwinogrande/ru.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'__description__'": "'A multilingual collection of Winograd Schemas in six languages that can be "*

 * *                      "used for evaluation of cross-lingual commonsense reasoning capabilities.'",*

 * * "'__tags__'": "OrderedDict([('arxiv', ['2211.01786', '2106.12066']), ('croissant', True), "*

 * *               "('language', ['en', 'fr', 'ja', 'pt', 'ru', 'zh']), ('license', 'cc-by-4.0'), "*

 * *               "('region', 'us')])",*

 * * "'loader'": "{'path': 'Muennighoff/xwinograd', 'name': 'ru', delete: ['split']}",*

 * * "' […]*

```diff
@@ -1,53 +1,55 @@
 {
+    "__description__": "A multilingual collection of Winograd Schemas in six languages that can be used for evaluation of cross-lingual commonsense reasoning capabilities.",
+    "__tags__": {
+        "arxiv": [
+            "2211.01786",
+            "2106.12066"
+        ],
+        "croissant": true,
+        "language": [
+            "en",
+            "fr",
+            "ja",
+            "pt",
+            "ru",
+            "zh"
+        ],
+        "license": "cc-by-4.0",
+        "region": "us"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "amh_Ethi",
+        "name": "ru",
+        "path": "Muennighoff/xwinograd",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mapper": {
-                "amh_Ethi": "test"
-            },
-            "type": "rename_splits"
-        },
-        {
             "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
+                "option1",
+                "option2"
             ],
             "to_field": "choices",
             "type": "list_field_values"
         },
         {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
             "fields": {
                 "answer": "int"
             },
             "type": "cast_fields"
         },
         {
             "add": -1,
             "field": "answer",
             "type": "add_constant"
         },
         {
-            "fields": {
-                "context_type": "passage"
+            "field_to_field": {
+                "sentence": "question"
             },
-            "type": "add_fields"
+            "type": "rename_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.open",
+    "templates": "templates.qa.multiple_choice.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/apc_arab.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mt_bench/response_assessment/rating/single_turn_gpt4_judgement.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6788541666666668%*

 * *Differences: {"'loader'": "{'path': 'OfirArviv/mt_bench_single_score_gpt4_judgement', 'split': 'train', delete: "*

 * *             "['name']}",*

 * * "'preprocess_steps'": "{0: {'mapper': {replace: OrderedDict([('train', 'test')])}}, 2: {'type': "*

 * *                       "'filter_by_condition', 'values': OrderedDict([('reference', '[]')]), "*

 * *                       "'condition': 'eq', delete: ['fields', 'to_field']}, 3: {'field_to_field': "*

 * *                       "{replace: OrderedDict([('model_input', 'question'), ('score', 'rati […]*

```diff
@@ -1,53 +1,65 @@
 {
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "apc_Arab",
+        "path": "OfirArviv/mt_bench_single_score_gpt4_judgement",
+        "split": "train",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "apc_Arab": "test"
+                "train": "test"
             },
             "type": "rename_splits"
         },
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
+            "condition": "eq",
+            "type": "filter_by_condition",
+            "values": {
+                "turn": 1
+            }
+        },
+        {
+            "condition": "eq",
+            "type": "filter_by_condition",
+            "values": {
+                "reference": "[]"
+            }
         },
         {
             "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
+                "category": "group",
+                "model_input": "question",
+                "model_output": "answer",
+                "score": "rating"
             },
             "type": "rename_fields"
         },
         {
-            "fields": {
-                "answer": "int"
+            "field": "question",
+            "to_field": "question",
+            "type": "literal_eval"
+        },
+        {
+            "field_to_field": {
+                "question/0": "question"
             },
-            "type": "cast_fields"
+            "type": "copy_fields"
         },
         {
-            "add": -1,
             "field": "answer",
-            "type": "add_constant"
+            "to_field": "answer",
+            "type": "literal_eval"
         },
         {
-            "fields": {
-                "context_type": "passage"
+            "field_to_field": {
+                "answer/0": "answer"
             },
-            "type": "add_fields"
+            "type": "copy_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.response_assessment.rating.single_turn",
+    "templates": [
+        "templates.response_assessment.rating.mt_bench_single_turn"
+    ],
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/arb_arab.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/xwinogrande/en.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'__description__'": "'A multilingual collection of Winograd Schemas in six languages that can be "*

 * *                      "used for evaluation of cross-lingual commonsense reasoning capabilities.'",*

 * * "'__tags__'": "OrderedDict([('arxiv', ['2211.01786', '2106.12066']), ('croissant', True), "*

 * *               "('language', ['en', 'fr', 'ja', 'pt', 'ru', 'zh']), ('license', 'cc-by-4.0'), "*

 * *               "('region', 'us')])",*

 * * "'loader'": "{'path': 'Muennighoff/xwinograd', 'name': 'en', delete: ['split']}",*

 * * "' […]*

```diff
@@ -1,53 +1,55 @@
 {
+    "__description__": "A multilingual collection of Winograd Schemas in six languages that can be used for evaluation of cross-lingual commonsense reasoning capabilities.",
+    "__tags__": {
+        "arxiv": [
+            "2211.01786",
+            "2106.12066"
+        ],
+        "croissant": true,
+        "language": [
+            "en",
+            "fr",
+            "ja",
+            "pt",
+            "ru",
+            "zh"
+        ],
+        "license": "cc-by-4.0",
+        "region": "us"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "arb_Arab",
+        "name": "en",
+        "path": "Muennighoff/xwinograd",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mapper": {
-                "arb_Arab": "test"
-            },
-            "type": "rename_splits"
-        },
-        {
             "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
+                "option1",
+                "option2"
             ],
             "to_field": "choices",
             "type": "list_field_values"
         },
         {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
             "fields": {
                 "answer": "int"
             },
             "type": "cast_fields"
         },
         {
             "add": -1,
             "field": "answer",
             "type": "add_constant"
         },
         {
-            "fields": {
-                "context_type": "passage"
+            "field_to_field": {
+                "sentence": "question"
             },
-            "type": "add_fields"
+            "type": "rename_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.open",
+    "templates": "templates.qa.multiple_choice.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/arb_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/metrics/squad.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.15674603174603177%*

 * *Differences: {"'main_score'": "'f1'",*

 * * "'metric'": "OrderedDict([('type', 'squad')])",*

 * * "'preprocess_steps'": "{0: {'type': 'add_id', delete: ['mapper']}, 1: {'type': 'add_fields', "*

 * *                       "'fields': {replace: OrderedDict([('prediction_template', "*

 * *                       "OrderedDict([('prediction_text', 'PRED'), ('id', 'ID')])), "*

 * *                       "('reference_template', OrderedDict([('answers', "*

 * *                       "OrderedDict([('answer_start', [-1]), ('text', 'REF')])), ('id', "*

 * *           […]*

```diff
@@ -1,53 +1,65 @@
 {
-    "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "arb_Latn",
-        "type": "load_hf"
+    "main_score": "f1",
+    "metric": {
+        "type": "squad"
     },
     "preprocess_steps": [
         {
-            "mapper": {
-                "arb_Latn": "test"
-            },
-            "type": "rename_splits"
-        },
-        {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
+            "type": "add_id"
         },
         {
             "fields": {
-                "answer": "int"
+                "prediction_template": {
+                    "id": "ID",
+                    "prediction_text": "PRED"
+                },
+                "reference_template": {
+                    "answers": {
+                        "answer_start": [
+                            -1
+                        ],
+                        "text": "REF"
+                    },
+                    "id": "ID"
+                }
             },
-            "type": "cast_fields"
+            "type": "add_fields",
+            "use_deepcopy": true
         },
         {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
+            "field_to_field": [
+                [
+                    "references",
+                    "reference_template/answers/text"
+                ],
+                [
+                    "prediction",
+                    "prediction_template/prediction_text"
+                ],
+                [
+                    "id",
+                    "prediction_template/id"
+                ],
+                [
+                    "id",
+                    "reference_template/id"
+                ]
+            ],
+            "type": "copy_fields"
         },
         {
-            "fields": {
-                "context_type": "passage"
-            },
-            "type": "add_fields"
+            "field_to_field": [
+                [
+                    "reference_template",
+                    "references"
+                ],
+                [
+                    "prediction_template",
+                    "prediction"
+                ]
+            ],
+            "type": "copy_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
-    "type": "task_card"
+    "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/ars_arab.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/high_school_government_and_politics.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48214285714285715%*

 * *Differences: {"'__description__'": "'Dataset Card for MMLU\\nDataset Summary\\nMeasuring Massive Multitask "*

 * *                      'Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy '*

 * *                      'Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\\nThis is '*

 * *                      'a massive multitask test consisting of multiple-choice questions from '*

 * *                      'various branches of knowledge. The test spans subjects in the humanities, '*

 * *                      […]*

```diff
@@ -1,53 +1,44 @@
 {
+    "__description__": "Dataset Card for MMLU\nDataset Summary\nMeasuring Massive Multitask Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\nThis is a massive multitask test consisting of multiple-choice questions from various branches of knowledge. The test spans subjects in the humanities, social sciences, hard sciences, and other areas that are important for some people to learn. This covers 57\u2026 See the full description on the dataset page: https://huggingface.co/datasets/cais/mmlu.",
+    "__tags__": {
+        "annotations_creators": "no-annotation",
+        "arxiv": [
+            "2009.03300",
+            "2005.00700",
+            "2005.14165",
+            "2008.02275"
+        ],
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "mit",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": "multiple-choice-qa"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "ars_Arab",
+        "name": "high_school_government_and_politics",
+        "path": "cais/mmlu",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "ars_Arab": "test"
+                "dev": "train"
             },
             "type": "rename_splits"
         },
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
             "fields": {
-                "context_type": "passage"
+                "topic": "high school government and politics"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/ary_arab.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/copa.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5625%*

 * *Differences: {"'__description__'": "'SuperGLUE (https://super.gluebenchmark.com/) is a new benchmark styled "*

 * *                      'after\\nGLUE with a new set of more difficult language understanding tasks, '*

 * *                      "improved\\nresources, and a new public leaderboard.'",*

 * * "'__tags__'": "OrderedDict([('NLU', True), ('annotations_creators', 'expert-generated'), "*

 * *               "('arxiv', '1905.00537'), ('croissant', True), ('language', 'en'), "*

 * *               "('language_creators', 'other'), ('license',  […]*

```diff
@@ -1,53 +1,70 @@
 {
+    "__description__": "SuperGLUE (https://super.gluebenchmark.com/) is a new benchmark styled after\nGLUE with a new set of more difficult language understanding tasks, improved\nresources, and a new public leaderboard.",
+    "__tags__": {
+        "NLU": true,
+        "annotations_creators": "expert-generated",
+        "arxiv": "1905.00537",
+        "croissant": true,
+        "language": "en",
+        "language_creators": "other",
+        "license": "other",
+        "multilinguality": "monolingual",
+        "natural language understanding": true,
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "extended|other",
+        "superglue": true,
+        "task_categories": [
+            "text-classification",
+            "token-classification",
+            "question-answering"
+        ],
+        "task_ids": [
+            "natural-language-inference",
+            "word-sense-disambiguation",
+            "coreference-resolution",
+            "extractive-qa"
+        ]
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "ary_Arab",
+        "name": "copa",
+        "path": "super_glue",
         "type": "load_hf"
     },
     "preprocess_steps": [
-        {
-            "mapper": {
-                "ary_Arab": "test"
-            },
-            "type": "rename_splits"
-        },
+        "splitters.small_no_test",
         {
             "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
+                "choice1",
+                "choice2"
             ],
             "to_field": "choices",
             "type": "list_field_values"
         },
         {
             "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
+                "label": "answer",
+                "premise": "context"
             },
             "type": "rename_fields"
         },
         {
-            "fields": {
-                "answer": "int"
+            "mappers": {
+                "question": {
+                    "cause": "What was the cause of this?",
+                    "effect": "What happened as a result?"
+                }
             },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
+            "type": "map_instance_values"
         },
         {
             "fields": {
-                "context_type": "passage"
+                "context_type": "sentence"
             },
             "type": "add_fields"
         }
     ],
     "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "templates": "templates.qa.multiple_choice.with_context.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/arz_arab.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/marketing.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48214285714285715%*

 * *Differences: {"'__description__'": "'Dataset Card for MMLU\\nDataset Summary\\nMeasuring Massive Multitask "*

 * *                      'Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy '*

 * *                      'Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\\nThis is '*

 * *                      'a massive multitask test consisting of multiple-choice questions from '*

 * *                      'various branches of knowledge. The test spans subjects in the humanities, '*

 * *                      […]*

```diff
@@ -1,53 +1,44 @@
 {
+    "__description__": "Dataset Card for MMLU\nDataset Summary\nMeasuring Massive Multitask Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\nThis is a massive multitask test consisting of multiple-choice questions from various branches of knowledge. The test spans subjects in the humanities, social sciences, hard sciences, and other areas that are important for some people to learn. This covers 57\u2026 See the full description on the dataset page: https://huggingface.co/datasets/cais/mmlu.",
+    "__tags__": {
+        "annotations_creators": "no-annotation",
+        "arxiv": [
+            "2009.03300",
+            "2005.00700",
+            "2005.14165",
+            "2008.02275"
+        ],
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "mit",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": "multiple-choice-qa"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "arz_Arab",
+        "name": "marketing",
+        "path": "cais/mmlu",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "arz_Arab": "test"
+                "dev": "train"
             },
             "type": "rename_splits"
         },
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
             "fields": {
-                "context_type": "passage"
+                "topic": "marketing"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/asm_beng.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/winogrande/xl.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.49489795918367346%*

 * *Differences: {"'__description__'": "'WinoGrande is a new collection of 44k problems, inspired by Winograd "*

 * *                      'Schema Challenge (Levesque, Davis, and Morgenstern\\n2011), but adjusted to '*

 * *                      'improve the scale and robustness against the dataset-specific bias. '*

 * *                      'Formulated as a\\nfill-in-a-blank task with binary options, the goal is to '*

 * *                      'choose the right option for a given sentence which requires\\ncommonsense '*

 * *                      "r […]*

```diff
@@ -1,53 +1,44 @@
 {
+    "__description__": "WinoGrande is a new collection of 44k problems, inspired by Winograd Schema Challenge (Levesque, Davis, and Morgenstern\n2011), but adjusted to improve the scale and robustness against the dataset-specific bias. Formulated as a\nfill-in-a-blank task with binary options, the goal is to choose the right option for a given sentence which requires\ncommonsense reasoning.",
+    "__tags__": {
+        "croissant": true,
+        "language": "en",
+        "region": "us"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "asm_Beng",
+        "name": "winogrande_xl",
+        "path": "winogrande",
         "type": "load_hf"
     },
     "preprocess_steps": [
-        {
-            "mapper": {
-                "asm_Beng": "test"
-            },
-            "type": "rename_splits"
-        },
+        "splitters.small_no_test",
         {
             "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
+                "option1",
+                "option2"
             ],
             "to_field": "choices",
             "type": "list_field_values"
         },
         {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
             "fields": {
                 "answer": "int"
             },
             "type": "cast_fields"
         },
         {
             "add": -1,
             "field": "answer",
             "type": "add_constant"
         },
         {
-            "fields": {
-                "context_type": "passage"
+            "field_to_field": {
+                "sentence": "question"
             },
-            "type": "add_fields"
+            "type": "rename_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.open",
+    "templates": "templates.qa.multiple_choice.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/azj_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mt_bench/response_assessment/rating/multi_turn_with_reference_gpt4_judgement.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6733333333333333%*

 * *Differences: {"'loader'": "{'path': 'OfirArviv/mt_bench_single_score_gpt4_judgement', 'split': 'train', delete: "*

 * *             "['name']}",*

 * * "'preprocess_steps'": "{0: {'mapper': {replace: OrderedDict([('train', 'test')])}}, 2: {'type': "*

 * *                       "'filter_by_condition', 'values': OrderedDict([('reference', '[]')]), "*

 * *                       "'condition': 'ne', delete: ['fields', 'to_field']}, 3: {'field_to_field': "*

 * *                       "{replace: OrderedDict([('score', 'rating'), ('category', 'group')]) […]*

```diff
@@ -1,53 +1,68 @@
 {
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "azj_Latn",
+        "path": "OfirArviv/mt_bench_single_score_gpt4_judgement",
+        "split": "train",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "azj_Latn": "test"
+                "train": "test"
             },
             "type": "rename_splits"
         },
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
+            "condition": "eq",
+            "type": "filter_by_condition",
+            "values": {
+                "turn": 2
+            }
+        },
+        {
+            "condition": "ne",
+            "type": "filter_by_condition",
+            "values": {
+                "reference": "[]"
+            }
         },
         {
             "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
+                "category": "group",
+                "score": "rating"
             },
             "type": "rename_fields"
         },
         {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
+            "field": "model_input",
+            "to_field": "model_input",
+            "type": "literal_eval"
         },
         {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
+            "field": "model_output",
+            "to_field": "model_output",
+            "type": "literal_eval"
         },
         {
-            "fields": {
-                "context_type": "passage"
-            },
-            "type": "add_fields"
+            "field": "reference",
+            "to_field": "reference",
+            "type": "literal_eval"
+        },
+        {
+            "assistant_turns_field": "model_output",
+            "to_field": "dialog",
+            "type": "interleave_lists_to_dialog_operator",
+            "user_turns_field": "model_input"
+        },
+        {
+            "assistant_turns_field": "reference",
+            "to_field": "reference_dialog",
+            "type": "interleave_lists_to_dialog_operator",
+            "user_turns_field": "model_input"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.response_assessment.rating.multi_turn_with_reference",
+    "templates": [
+        "templates.response_assessment.rating.mt_bench_multi_turn_with_reference"
+    ],
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/bam_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/coedit/selection.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.45947802197802196%*

 * *Differences: {"'__description__'": "'Dataset Card for CoEdIT: Text Editing via Instruction Tuning\\nPaper: "*

 * *                      'CoEdIT: Text Editing by Task-Specific Instruction Tuning\\nAuthors: Vipul '*

 * *                      'Raheja, Dhruv Kumar, Ryan Koo, Dongyeop Kang\\nProject Repo: '*

 * *                      'https://github.com/vipulraheja/coedit\\nDataset Summary\\nThis is the '*

 * *                      'dataset that was used to train the CoEdIT text editing models. Full details '*

 * *                      'of the datas […]*

```diff
@@ -1,53 +1,101 @@
 {
+    "__description__": "Dataset Card for CoEdIT: Text Editing via Instruction Tuning\nPaper: CoEdIT: Text Editing by Task-Specific Instruction Tuning\nAuthors: Vipul Raheja, Dhruv Kumar, Ryan Koo, Dongyeop Kang\nProject Repo: https://github.com/vipulraheja/coedit\nDataset Summary\nThis is the dataset that was used to train the CoEdIT text editing models. Full details of the dataset can be found in our paper.\nDataset Structure\nThe\u2026 See the full description on the dataset page: https://huggingface.co/datasets/grammarly/coedit.",
+    "__tags__": {
+        "arxiv": "2305.09857",
+        "croissant": true,
+        "language": "en",
+        "license": "apache-2.0",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "task_categories": "text-generation"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "bam_Latn",
+        "filtering_lambda": "lambda x: x['task'] in ['gec', 'simplification', 'coherence', 'neutralize']",
+        "path": "grammarly/coedit",
+        "streaming": true,
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mapper": {
-                "bam_Latn": "test"
-            },
-            "type": "rename_splits"
+            "page_size": 9223372036854775807,
+            "type": "shuffle"
+        },
+        "splitters.small_no_test",
+        {
+            "by": ": ",
+            "field": "src",
+            "type": "split"
+        },
+        {
+            "field": "src",
+            "start": 1,
+            "type": "slice"
+        },
+        {
+            "by": ": ",
+            "field": "src",
+            "type": "join"
         },
         {
             "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
+                "tgt",
+                "src"
             ],
-            "to_field": "choices",
+            "to_field": "choices_texts",
             "type": "list_field_values"
         },
         {
+            "field": "choices_texts",
+            "type": "shuffle_field_values"
+        },
+        {
             "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
+                "task": "required_attribute"
             },
-            "type": "rename_fields"
+            "type": "copy_fields"
         },
         {
-            "fields": {
-                "answer": "int"
+            "mappers": {
+                "required_attribute": {
+                    "coherence": "coherent",
+                    "gec": "grammatically correct",
+                    "neutralize": "neutral",
+                    "simplification": "simple"
+                }
+            },
+            "type": "map_instance_values"
+        },
+        {
+            "field_to_field": {
+                "task": "attribute_type"
             },
-            "type": "cast_fields"
+            "type": "copy_fields"
         },
         {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
+            "mappers": {
+                "attribute_type": {
+                    "coherence": "coherence",
+                    "gec": "gramaticity",
+                    "neutralize": "neutrality",
+                    "simplification": "simplicity"
+                }
+            },
+            "type": "map_instance_values"
         },
         {
             "fields": {
-                "context_type": "passage"
+                "choices_text_type": "sentences"
             },
             "type": "add_fields"
+        },
+        {
+            "field_to_field": {
+                "tgt": "choice"
+            },
+            "type": "rename_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.selection.by_attribute",
+    "templates": "templates.selection.by_attribute.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/ben_beng.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/coedit/preference.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.46559523809523806%*

 * *Differences: {"'__description__'": "'Dataset Card for CoEdIT: Text Editing via Instruction Tuning\\nPaper: "*

 * *                      'CoEdIT: Text Editing by Task-Specific Instruction Tuning\\nAuthors: Vipul '*

 * *                      'Raheja, Dhruv Kumar, Ryan Koo, Dongyeop Kang\\nProject Repo: '*

 * *                      'https://github.com/vipulraheja/coedit\\nDataset Summary\\nThis is the '*

 * *                      'dataset that was used to train the CoEdIT text editing models. Full details '*

 * *                      'of the datas […]*

```diff
@@ -1,53 +1,74 @@
 {
+    "__description__": "Dataset Card for CoEdIT: Text Editing via Instruction Tuning\nPaper: CoEdIT: Text Editing by Task-Specific Instruction Tuning\nAuthors: Vipul Raheja, Dhruv Kumar, Ryan Koo, Dongyeop Kang\nProject Repo: https://github.com/vipulraheja/coedit\nDataset Summary\nThis is the dataset that was used to train the CoEdIT text editing models. Full details of the dataset can be found in our paper.\nDataset Structure\nThe\u2026 See the full description on the dataset page: https://huggingface.co/datasets/grammarly/coedit.",
+    "__tags__": {
+        "arxiv": "2305.09857",
+        "croissant": true,
+        "language": "en",
+        "license": "apache-2.0",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "task_categories": "text-generation"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "ben_Beng",
+        "path": "grammarly/coedit",
+        "streaming": true,
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mapper": {
-                "ben_Beng": "test"
+            "page_size": 9223372036854775807,
+            "type": "shuffle"
+        },
+        "splitters.small_no_test",
+        {
+            "by": ": ",
+            "field": "src",
+            "type": "split"
+        },
+        {
+            "field": "src",
+            "start": 1,
+            "type": "slice"
+        },
+        {
+            "field_to_field": {
+                "src/0": "instruction"
             },
-            "type": "rename_splits"
+            "type": "copy_fields"
+        },
+        {
+            "by": ": ",
+            "field": "src",
+            "type": "join"
         },
         {
             "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
+                "tgt",
+                "src"
             ],
             "to_field": "choices",
             "type": "list_field_values"
         },
         {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
+            "field": "choices",
+            "type": "shuffle_field_values"
         },
         {
             "fields": {
-                "answer": "int"
+                "input_type": "sentence",
+                "output_type": "sentence"
             },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
+            "type": "add_fields"
         },
         {
-            "fields": {
-                "context_type": "passage"
+            "field_to_field": {
+                "src": "input",
+                "tgt": "output_choice"
             },
-            "type": "add_fields"
+            "type": "rename_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.evaluation.preference",
+    "templates": "templates.evaluation.preference.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/ben_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/legalbench/international_citizenship_questions.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48214285714285715%*

 * *Differences: {"'__description__'": "'LegalBench is a collection of benchmark tasks for evaluating legal "*

 * *                      "reasoning in large language models.'",*

 * * "'__tags__'": "OrderedDict([('arxiv', '2308.11462'), ('croissant', True), ('finance', True), "*

 * *               "('language', 'en'), ('law', True), ('legal', True), ('license', 'other'), "*

 * *               "('region', 'us'), ('size_categories', '10K<n<100K'), ('task_categories', "*

 * *               "['text-classification', 'question-answering', 'text-generation […]*

```diff
@@ -1,53 +1,63 @@
 {
+    "__description__": "LegalBench is a collection of benchmark tasks for evaluating legal reasoning in large language models.",
+    "__tags__": {
+        "arxiv": "2308.11462",
+        "croissant": true,
+        "finance": true,
+        "language": "en",
+        "law": true,
+        "legal": true,
+        "license": "other",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "task_categories": [
+            "text-classification",
+            "question-answering",
+            "text-generation"
+        ]
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "ben_Latn",
+        "name": "international_citizenship_questions",
+        "path": "nguha/legalbench",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mapper": {
-                "ben_Latn": "test"
-            },
-            "type": "rename_splits"
-        },
-        {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
             "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
+                "answer": "label",
+                "question": "text"
             },
             "type": "rename_fields"
         },
         {
             "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
-            "fields": {
-                "context_type": "passage"
+                "classes": [
+                    "Yes",
+                    "No"
+                ],
+                "classes_descriptions": "considering the state of international law on January 1st, 2020",
+                "text_type": "question",
+                "type_of_class": ""
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.classification.multi_class.with_classes_descriptions",
+    "templates": {
+        "default": {
+            "input_format": "{text_type}: {text} Answer from one of {classes}.",
+            "instruction": "Answer the following {text_type} {classes_descriptions}.\n",
+            "output_format": "{label}",
+            "postprocessors": [
+                "processors.take_first_non_empty_line",
+                "processors.lower_case_till_punc"
+            ],
+            "target_prefix": "Answer: ",
+            "title_fields": [
+                "text_type"
+            ],
+            "type": "input_output_template"
+        }
+    },
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/bod_tibt.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/winogrande/m.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.49489795918367346%*

 * *Differences: {"'__description__'": "'WinoGrande is a new collection of 44k problems, inspired by Winograd "*

 * *                      'Schema Challenge (Levesque, Davis, and Morgenstern\\n2011), but adjusted to '*

 * *                      'improve the scale and robustness against the dataset-specific bias. '*

 * *                      'Formulated as a\\nfill-in-a-blank task with binary options, the goal is to '*

 * *                      'choose the right option for a given sentence which requires\\ncommonsense '*

 * *                      "r […]*

```diff
@@ -1,53 +1,44 @@
 {
+    "__description__": "WinoGrande is a new collection of 44k problems, inspired by Winograd Schema Challenge (Levesque, Davis, and Morgenstern\n2011), but adjusted to improve the scale and robustness against the dataset-specific bias. Formulated as a\nfill-in-a-blank task with binary options, the goal is to choose the right option for a given sentence which requires\ncommonsense reasoning.",
+    "__tags__": {
+        "croissant": true,
+        "language": "en",
+        "region": "us"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "bod_Tibt",
+        "name": "winogrande_m",
+        "path": "winogrande",
         "type": "load_hf"
     },
     "preprocess_steps": [
-        {
-            "mapper": {
-                "bod_Tibt": "test"
-            },
-            "type": "rename_splits"
-        },
+        "splitters.small_no_test",
         {
             "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
+                "option1",
+                "option2"
             ],
             "to_field": "choices",
             "type": "list_field_values"
         },
         {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
             "fields": {
                 "answer": "int"
             },
             "type": "cast_fields"
         },
         {
             "add": -1,
             "field": "answer",
             "type": "add_constant"
         },
         {
-            "fields": {
-                "context_type": "passage"
+            "field_to_field": {
+                "sentence": "question"
             },
-            "type": "add_fields"
+            "type": "rename_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.open",
+    "templates": "templates.qa.multiple_choice.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/bul_cyrl.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/winogrande/xs.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.49489795918367346%*

 * *Differences: {"'__description__'": "'WinoGrande is a new collection of 44k problems, inspired by Winograd "*

 * *                      'Schema Challenge (Levesque, Davis, and Morgenstern\\n2011), but adjusted to '*

 * *                      'improve the scale and robustness against the dataset-specific bias. '*

 * *                      'Formulated as a\\nfill-in-a-blank task with binary options, the goal is to '*

 * *                      'choose the right option for a given sentence which requires\\ncommonsense '*

 * *                      "r […]*

```diff
@@ -1,53 +1,44 @@
 {
+    "__description__": "WinoGrande is a new collection of 44k problems, inspired by Winograd Schema Challenge (Levesque, Davis, and Morgenstern\n2011), but adjusted to improve the scale and robustness against the dataset-specific bias. Formulated as a\nfill-in-a-blank task with binary options, the goal is to choose the right option for a given sentence which requires\ncommonsense reasoning.",
+    "__tags__": {
+        "croissant": true,
+        "language": "en",
+        "region": "us"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "bul_Cyrl",
+        "name": "winogrande_xs",
+        "path": "winogrande",
         "type": "load_hf"
     },
     "preprocess_steps": [
-        {
-            "mapper": {
-                "bul_Cyrl": "test"
-            },
-            "type": "rename_splits"
-        },
+        "splitters.small_no_test",
         {
             "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
+                "option1",
+                "option2"
             ],
             "to_field": "choices",
             "type": "list_field_values"
         },
         {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
             "fields": {
                 "answer": "int"
             },
             "type": "cast_fields"
         },
         {
             "add": -1,
             "field": "answer",
             "type": "add_constant"
         },
         {
-            "fields": {
-                "context_type": "passage"
+            "field_to_field": {
+                "sentence": "question"
             },
-            "type": "add_fields"
+            "type": "rename_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.open",
+    "templates": "templates.qa.multiple_choice.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/cat_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/college_computer_science.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48214285714285715%*

 * *Differences: {"'__description__'": "'Dataset Card for MMLU\\nDataset Summary\\nMeasuring Massive Multitask "*

 * *                      'Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy '*

 * *                      'Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\\nThis is '*

 * *                      'a massive multitask test consisting of multiple-choice questions from '*

 * *                      'various branches of knowledge. The test spans subjects in the humanities, '*

 * *                      […]*

```diff
@@ -1,53 +1,44 @@
 {
+    "__description__": "Dataset Card for MMLU\nDataset Summary\nMeasuring Massive Multitask Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\nThis is a massive multitask test consisting of multiple-choice questions from various branches of knowledge. The test spans subjects in the humanities, social sciences, hard sciences, and other areas that are important for some people to learn. This covers 57\u2026 See the full description on the dataset page: https://huggingface.co/datasets/cais/mmlu.",
+    "__tags__": {
+        "annotations_creators": "no-annotation",
+        "arxiv": [
+            "2009.03300",
+            "2005.00700",
+            "2005.14165",
+            "2008.02275"
+        ],
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "mit",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": "multiple-choice-qa"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "cat_Latn",
+        "name": "college_computer_science",
+        "path": "cais/mmlu",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "cat_Latn": "test"
+                "dev": "train"
             },
             "type": "rename_splits"
         },
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
             "fields": {
-                "context_type": "passage"
+                "topic": "college computer science"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/ceb_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/jurisprudence.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48214285714285715%*

 * *Differences: {"'__description__'": "'Dataset Card for MMLU\\nDataset Summary\\nMeasuring Massive Multitask "*

 * *                      'Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy '*

 * *                      'Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\\nThis is '*

 * *                      'a massive multitask test consisting of multiple-choice questions from '*

 * *                      'various branches of knowledge. The test spans subjects in the humanities, '*

 * *                      […]*

```diff
@@ -1,53 +1,44 @@
 {
+    "__description__": "Dataset Card for MMLU\nDataset Summary\nMeasuring Massive Multitask Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\nThis is a massive multitask test consisting of multiple-choice questions from various branches of knowledge. The test spans subjects in the humanities, social sciences, hard sciences, and other areas that are important for some people to learn. This covers 57\u2026 See the full description on the dataset page: https://huggingface.co/datasets/cais/mmlu.",
+    "__tags__": {
+        "annotations_creators": "no-annotation",
+        "arxiv": [
+            "2009.03300",
+            "2005.00700",
+            "2005.14165",
+            "2008.02275"
+        ],
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "mit",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": "multiple-choice-qa"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "ceb_Latn",
+        "name": "jurisprudence",
+        "path": "cais/mmlu",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "ceb_Latn": "test"
+                "dev": "train"
             },
             "type": "rename_splits"
         },
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
             "fields": {
-                "context_type": "passage"
+                "topic": "jurisprudence"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/ces_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/winogrande/s.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.49489795918367346%*

 * *Differences: {"'__description__'": "'WinoGrande is a new collection of 44k problems, inspired by Winograd "*

 * *                      'Schema Challenge (Levesque, Davis, and Morgenstern\\n2011), but adjusted to '*

 * *                      'improve the scale and robustness against the dataset-specific bias. '*

 * *                      'Formulated as a\\nfill-in-a-blank task with binary options, the goal is to '*

 * *                      'choose the right option for a given sentence which requires\\ncommonsense '*

 * *                      "r […]*

```diff
@@ -1,53 +1,44 @@
 {
+    "__description__": "WinoGrande is a new collection of 44k problems, inspired by Winograd Schema Challenge (Levesque, Davis, and Morgenstern\n2011), but adjusted to improve the scale and robustness against the dataset-specific bias. Formulated as a\nfill-in-a-blank task with binary options, the goal is to choose the right option for a given sentence which requires\ncommonsense reasoning.",
+    "__tags__": {
+        "croissant": true,
+        "language": "en",
+        "region": "us"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "ces_Latn",
+        "name": "winogrande_s",
+        "path": "winogrande",
         "type": "load_hf"
     },
     "preprocess_steps": [
-        {
-            "mapper": {
-                "ces_Latn": "test"
-            },
-            "type": "rename_splits"
-        },
+        "splitters.small_no_test",
         {
             "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
+                "option1",
+                "option2"
             ],
             "to_field": "choices",
             "type": "list_field_values"
         },
         {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
             "fields": {
                 "answer": "int"
             },
             "type": "cast_fields"
         },
         {
             "add": -1,
             "field": "answer",
             "type": "add_constant"
         },
         {
-            "fields": {
-                "context_type": "passage"
+            "field_to_field": {
+                "sentence": "question"
             },
-            "type": "add_fields"
+            "type": "rename_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.open",
+    "templates": "templates.qa.multiple_choice.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/ckb_arab.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/moral_disputes.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48214285714285715%*

 * *Differences: {"'__description__'": "'Dataset Card for MMLU\\nDataset Summary\\nMeasuring Massive Multitask "*

 * *                      'Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy '*

 * *                      'Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\\nThis is '*

 * *                      'a massive multitask test consisting of multiple-choice questions from '*

 * *                      'various branches of knowledge. The test spans subjects in the humanities, '*

 * *                      […]*

```diff
@@ -1,53 +1,44 @@
 {
+    "__description__": "Dataset Card for MMLU\nDataset Summary\nMeasuring Massive Multitask Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\nThis is a massive multitask test consisting of multiple-choice questions from various branches of knowledge. The test spans subjects in the humanities, social sciences, hard sciences, and other areas that are important for some people to learn. This covers 57\u2026 See the full description on the dataset page: https://huggingface.co/datasets/cais/mmlu.",
+    "__tags__": {
+        "annotations_creators": "no-annotation",
+        "arxiv": [
+            "2009.03300",
+            "2005.00700",
+            "2005.14165",
+            "2008.02275"
+        ],
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "mit",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": "multiple-choice-qa"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "ckb_Arab",
+        "name": "moral_disputes",
+        "path": "cais/mmlu",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "ckb_Arab": "test"
+                "dev": "train"
             },
             "type": "rename_splits"
         },
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
             "fields": {
-                "context_type": "passage"
+                "topic": "moral disputes"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/dan_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/tablerow_classify.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6366666666666667%*

 * *Differences: {"'loader'": "{'type': 'load_from_kaggle', 'url': "*

 * *             "'https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction', delete: "*

 * *             "['path', 'name', 'split']}",*

 * * "'preprocess_steps'": "{0: {'type': 'split_random_mix', 'mix': OrderedDict([('train', "*

 * *                       "'train[70%]'), ('validation', 'train[10%]'), ('test', 'train[20%]')]), "*

 * *                       "delete: ['mapper']}, 1: {'field_to_field': {replace: "*

 * *                       "OrderedDict([('HeartDisease', 'l […]*

```diff
@@ -1,53 +1,65 @@
 {
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "dan_Latn",
-        "type": "load_hf"
+        "type": "load_from_kaggle",
+        "url": "https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction"
     },
     "preprocess_steps": [
         {
-            "mapper": {
-                "dan_Latn": "test"
+            "mix": {
+                "test": "train[20%]",
+                "train": "train[70%]",
+                "validation": "train[10%]"
             },
-            "type": "rename_splits"
-        },
-        {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
+            "type": "split_random_mix"
         },
         {
             "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
+                "HeartDisease": "label"
             },
             "type": "rename_fields"
         },
         {
-            "fields": {
-                "answer": "int"
+            "mappers": {
+                "label": {
+                    "0": "Normal",
+                    "1": "Heart Disease"
+                }
             },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
+            "type": "map_instance_values"
         },
         {
             "fields": {
-                "context_type": "passage"
+                "text_type": "Person medical record",
+                "type_of_class": "Heart Disease Possibility"
             },
             "type": "add_fields"
+        },
+        {
+            "field": "label",
+            "stream_name": "train",
+            "to_field": "classes",
+            "type": "extract_field_values"
+        },
+        {
+            "fields": [
+                "Age",
+                "Sex",
+                "ChestPainType",
+                "RestingBP",
+                "Cholesterol",
+                "FastingBS",
+                "RestingECG",
+                "MaxHR",
+                "ExerciseAngina",
+                "Oldpeak",
+                "ST_Slope"
+            ],
+            "max_cell_length": 25,
+            "to_field": "text",
+            "type": "serialize_table_row_as_text"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.classification.multi_class",
+    "templates": "templates.classification.multi_class.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/deu_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/global_facts.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48214285714285715%*

 * *Differences: {"'__description__'": "'Dataset Card for MMLU\\nDataset Summary\\nMeasuring Massive Multitask "*

 * *                      'Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy '*

 * *                      'Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\\nThis is '*

 * *                      'a massive multitask test consisting of multiple-choice questions from '*

 * *                      'various branches of knowledge. The test spans subjects in the humanities, '*

 * *                      […]*

```diff
@@ -1,53 +1,44 @@
 {
+    "__description__": "Dataset Card for MMLU\nDataset Summary\nMeasuring Massive Multitask Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\nThis is a massive multitask test consisting of multiple-choice questions from various branches of knowledge. The test spans subjects in the humanities, social sciences, hard sciences, and other areas that are important for some people to learn. This covers 57\u2026 See the full description on the dataset page: https://huggingface.co/datasets/cais/mmlu.",
+    "__tags__": {
+        "annotations_creators": "no-annotation",
+        "arxiv": [
+            "2009.03300",
+            "2005.00700",
+            "2005.14165",
+            "2008.02275"
+        ],
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "mit",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": "multiple-choice-qa"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "deu_Latn",
+        "name": "global_facts",
+        "path": "cais/mmlu",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "deu_Latn": "test"
+                "dev": "train"
             },
             "type": "rename_splits"
         },
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
             "fields": {
-                "context_type": "passage"
+                "topic": "global facts"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/ell_grek.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/xwinogrande/pt.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'__description__'": "'A multilingual collection of Winograd Schemas in six languages that can be "*

 * *                      "used for evaluation of cross-lingual commonsense reasoning capabilities.'",*

 * * "'__tags__'": "OrderedDict([('arxiv', ['2211.01786', '2106.12066']), ('croissant', True), "*

 * *               "('language', ['en', 'fr', 'ja', 'pt', 'ru', 'zh']), ('license', 'cc-by-4.0'), "*

 * *               "('region', 'us')])",*

 * * "'loader'": "{'path': 'Muennighoff/xwinograd', 'name': 'pt', delete: ['split']}",*

 * * "' […]*

```diff
@@ -1,53 +1,55 @@
 {
+    "__description__": "A multilingual collection of Winograd Schemas in six languages that can be used for evaluation of cross-lingual commonsense reasoning capabilities.",
+    "__tags__": {
+        "arxiv": [
+            "2211.01786",
+            "2106.12066"
+        ],
+        "croissant": true,
+        "language": [
+            "en",
+            "fr",
+            "ja",
+            "pt",
+            "ru",
+            "zh"
+        ],
+        "license": "cc-by-4.0",
+        "region": "us"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "ell_Grek",
+        "name": "pt",
+        "path": "Muennighoff/xwinograd",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mapper": {
-                "ell_Grek": "test"
-            },
-            "type": "rename_splits"
-        },
-        {
             "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
+                "option1",
+                "option2"
             ],
             "to_field": "choices",
             "type": "list_field_values"
         },
         {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
             "fields": {
                 "answer": "int"
             },
             "type": "cast_fields"
         },
         {
             "add": -1,
             "field": "answer",
             "type": "add_constant"
         },
         {
-            "fields": {
-                "context_type": "passage"
+            "field_to_field": {
+                "sentence": "question"
             },
-            "type": "add_fields"
+            "type": "rename_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.open",
+    "templates": "templates.qa.multiple_choice.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/eng_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/squad.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.47066326530612246%*

 * *Differences: {"'__description__'": "'Dataset Card for SQuAD\\nDataset Summary\\nStanford Question Answering "*

 * *                      'Dataset (SQuAD) is a reading comprehension dataset, consisting of questions '*

 * *                      'posed by crowdworkers on a set of Wikipedia articles, where the answer to '*

 * *                      'every question is a segment of text, or span, from the corresponding '*

 * *                      'reading passage, or the question might be unanswerable.\\nSQuAD 1.1 '*

 * *                      'conta […]*

```diff
@@ -1,53 +1,45 @@
 {
+    "__description__": "Dataset Card for SQuAD\nDataset Summary\nStanford Question Answering Dataset (SQuAD) is a reading comprehension dataset, consisting of questions posed by crowdworkers on a set of Wikipedia articles, where the answer to every question is a segment of text, or span, from the corresponding reading passage, or the question might be unanswerable.\nSQuAD 1.1 contains 100,000+ question-answer pairs on 500+ articles.\nSupported Tasks and Leaderboards\nQuestion\u2026 See the full description on the dataset page: https://huggingface.co/datasets/rajpurkar/squad.",
+    "__tags__": {
+        "annotations_creators": "crowdsourced",
+        "arxiv": "1606.05250",
+        "croissant": true,
+        "language": "en",
+        "language_creators": [
+            "crowdsourced",
+            "found"
+        ],
+        "license": "cc-by-sa-4.0",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "extended|wikipedia",
+        "task_categories": "question-answering",
+        "task_ids": "extractive-qa"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "eng_Latn",
+        "path": "squad",
         "type": "load_hf"
     },
     "preprocess_steps": [
+        "splitters.small_no_test",
         {
-            "mapper": {
-                "eng_Latn": "test"
-            },
-            "type": "rename_splits"
-        },
-        {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
+            "field_to_field": [
+                [
+                    "answers/text",
+                    "answers"
+                ]
             ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
+            "type": "copy_fields"
         },
         {
             "fields": {
                 "context_type": "passage"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.with_context.extractive",
+    "templates": "templates.qa.with_context.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/est_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/summarize_from_human_feedback.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4812925170068027%*

 * *Differences: {"'__description__'": "'Summarize from Feedback contains the human feedback data released by the "*

 * *                      '"Learning to summarize from human feedback" paper.\'',*

 * * "'__tags__'": "OrderedDict([('arxiv', '2009.01325'), ('croissant', True), ('region', 'us')])",*

 * * "'loader'": "{'path': 'openai/summarize_from_feedback', 'name': 'comparisons', delete: ['split']}",*

 * * "'preprocess_steps'": "{1: {'type': 'copy_fields', 'field_to_field': OrderedDict([('info/post', "*

 * *                       "'input'), ('sum […]*

```diff
@@ -1,53 +1,40 @@
 {
+    "__description__": "Summarize from Feedback contains the human feedback data released by the \"Learning to summarize from human feedback\" paper.",
+    "__tags__": {
+        "arxiv": "2009.01325",
+        "croissant": true,
+        "region": "us"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "est_Latn",
+        "name": "comparisons",
+        "path": "openai/summarize_from_feedback",
         "type": "load_hf"
     },
     "preprocess_steps": [
+        "splitters.small_no_test",
         {
-            "mapper": {
-                "est_Latn": "test"
+            "field_to_field": {
+                "info/post": "input",
+                "summaries/*/text": "choices"
             },
-            "type": "rename_splits"
-        },
-        {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
+            "type": "copy_fields"
         },
         {
             "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
+                "choice": "output_choice"
             },
             "type": "rename_fields"
         },
         {
             "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
-            "fields": {
-                "context_type": "passage"
+                "input_type": "post",
+                "instruction": "Summarize the following post",
+                "output_type": "summary"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.evaluation.preference",
+    "templates": "templates.evaluation.preference.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/eus_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/ai2_arc/arc_easy.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4803571428571428%*

 * *Differences: {"'__description__'": '\'Dataset Card for "ai2_arc"\\nDataset Summary\\nA new dataset of 7,787 '*

 * *                      'genuine grade-school level, multiple-choice science questions, assembled to '*

 * *                      'encourage research in\\nadvanced question-answering. The dataset is '*

 * *                      'partitioned into a Challenge Set and an Easy Set, where the former '*

 * *                      'contains\\nonly questions answered incorrectly by both a retrieval-based '*

 * *                      'algorith […]*

```diff
@@ -1,53 +1,56 @@
 {
+    "__description__": "Dataset Card for \"ai2_arc\"\nDataset Summary\nA new dataset of 7,787 genuine grade-school level, multiple-choice science questions, assembled to encourage research in\nadvanced question-answering. The dataset is partitioned into a Challenge Set and an Easy Set, where the former contains\nonly questions answered incorrectly by both a retrieval-based algorithm and a word co-occurrence algorithm. We are also\nincluding a corpus of over 14 million science sentences\u2026 See the full description on the dataset page: https://huggingface.co/datasets/allenai/ai2_arc.",
+    "__tags__": {
+        "annotations_creators": "found",
+        "arxiv": "1803.05457",
+        "croissant": true,
+        "language": "en",
+        "language_creators": "found",
+        "license": "cc-by-sa-4.0",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "1K<n<10K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": [
+            "open-domain-qa",
+            "multiple-choice-qa"
+        ]
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "eus_Latn",
+        "name": "ARC-Easy",
+        "path": "ai2_arc",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mapper": {
-                "eus_Latn": "test"
+            "fields": {
+                "topic": "science"
             },
-            "type": "rename_splits"
-        },
-        {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
+            "type": "add_fields"
         },
         {
             "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
+                "answerKey": "label",
+                "choices": "_choices"
             },
             "type": "rename_fields"
         },
         {
-            "fields": {
-                "answer": "int"
+            "field_to_field": {
+                "_choices/label": "labels",
+                "_choices/text": "choices"
             },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
+            "type": "copy_fields"
         },
         {
-            "fields": {
-                "context_type": "passage"
-            },
-            "type": "add_fields"
+            "index_of": "label",
+            "search_in": "labels",
+            "to_field": "answer",
+            "type": "index_of"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/fin_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/coedit/rewriting.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4581709956709957%*

 * *Differences: {"'__description__'": "'Dataset Card for CoEdIT: Text Editing via Instruction Tuning\\nPaper: "*

 * *                      'CoEdIT: Text Editing by Task-Specific Instruction Tuning\\nAuthors: Vipul '*

 * *                      'Raheja, Dhruv Kumar, Ryan Koo, Dongyeop Kang\\nProject Repo: '*

 * *                      'https://github.com/vipulraheja/coedit\\nDataset Summary\\nThis is the '*

 * *                      'dataset that was used to train the CoEdIT text editing models. Full details '*

 * *                      'of the datas […]*

```diff
@@ -1,53 +1,91 @@
 {
+    "__description__": "Dataset Card for CoEdIT: Text Editing via Instruction Tuning\nPaper: CoEdIT: Text Editing by Task-Specific Instruction Tuning\nAuthors: Vipul Raheja, Dhruv Kumar, Ryan Koo, Dongyeop Kang\nProject Repo: https://github.com/vipulraheja/coedit\nDataset Summary\nThis is the dataset that was used to train the CoEdIT text editing models. Full details of the dataset can be found in our paper.\nDataset Structure\nThe\u2026 See the full description on the dataset page: https://huggingface.co/datasets/grammarly/coedit.",
+    "__tags__": {
+        "arxiv": "2305.09857",
+        "croissant": true,
+        "language": "en",
+        "license": "apache-2.0",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "task_categories": "text-generation"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "fin_Latn",
+        "filtering_lambda": "lambda x: x['task'] in ['gec', 'simplification', 'coherence', 'neutralize']",
+        "path": "grammarly/coedit",
+        "streaming": true,
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mapper": {
-                "fin_Latn": "test"
-            },
-            "type": "rename_splits"
+            "page_size": 9223372036854775807,
+            "type": "shuffle"
         },
+        "splitters.small_no_test",
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
+            "by": ": ",
+            "field": "src",
+            "type": "split"
+        },
+        {
+            "field": "src",
+            "start": 1,
+            "type": "slice"
+        },
+        {
+            "by": ": ",
+            "field": "src",
+            "type": "join"
         },
         {
             "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
+                "task": "required_attribute"
             },
-            "type": "rename_fields"
+            "type": "copy_fields"
         },
         {
-            "fields": {
-                "answer": "int"
+            "mappers": {
+                "required_attribute": {
+                    "coherence": "coherent",
+                    "gec": "grammatically correct",
+                    "neutralize": "neutral",
+                    "simplification": "simple"
+                }
+            },
+            "type": "map_instance_values"
+        },
+        {
+            "field_to_field": {
+                "task": "attribute_type"
             },
-            "type": "cast_fields"
+            "type": "copy_fields"
         },
         {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
+            "mappers": {
+                "attribute_type": {
+                    "coherence": "coherence",
+                    "gec": "gramaticity",
+                    "neutralize": "neutrality",
+                    "simplification": "simplicity"
+                }
+            },
+            "type": "map_instance_values"
         },
         {
             "fields": {
-                "context_type": "passage"
+                "input_text_type": "sentence",
+                "output_text_type": "sentence"
             },
             "type": "add_fields"
+        },
+        {
+            "field_to_field": {
+                "src": "input_text",
+                "tgt": "output_text"
+            },
+            "type": "rename_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.rewriting.by_attribute",
+    "templates": "templates.rewriting.by_attribute.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/fuv_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/anatomy.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48214285714285715%*

 * *Differences: {"'__description__'": "'Dataset Card for MMLU\\nDataset Summary\\nMeasuring Massive Multitask "*

 * *                      'Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy '*

 * *                      'Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\\nThis is '*

 * *                      'a massive multitask test consisting of multiple-choice questions from '*

 * *                      'various branches of knowledge. The test spans subjects in the humanities, '*

 * *                      […]*

```diff
@@ -1,53 +1,44 @@
 {
+    "__description__": "Dataset Card for MMLU\nDataset Summary\nMeasuring Massive Multitask Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\nThis is a massive multitask test consisting of multiple-choice questions from various branches of knowledge. The test spans subjects in the humanities, social sciences, hard sciences, and other areas that are important for some people to learn. This covers 57\u2026 See the full description on the dataset page: https://huggingface.co/datasets/cais/mmlu.",
+    "__tags__": {
+        "annotations_creators": "no-annotation",
+        "arxiv": [
+            "2009.03300",
+            "2005.00700",
+            "2005.14165",
+            "2008.02275"
+        ],
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "mit",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": "multiple-choice-qa"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "fuv_Latn",
+        "name": "anatomy",
+        "path": "cais/mmlu",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "fuv_Latn": "test"
+                "dev": "train"
             },
             "type": "rename_splits"
         },
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
             "fields": {
-                "context_type": "passage"
+                "topic": "anatomy"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/grn_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/high_school_physics.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48214285714285715%*

 * *Differences: {"'__description__'": "'Dataset Card for MMLU\\nDataset Summary\\nMeasuring Massive Multitask "*

 * *                      'Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy '*

 * *                      'Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\\nThis is '*

 * *                      'a massive multitask test consisting of multiple-choice questions from '*

 * *                      'various branches of knowledge. The test spans subjects in the humanities, '*

 * *                      […]*

```diff
@@ -1,53 +1,44 @@
 {
+    "__description__": "Dataset Card for MMLU\nDataset Summary\nMeasuring Massive Multitask Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\nThis is a massive multitask test consisting of multiple-choice questions from various branches of knowledge. The test spans subjects in the humanities, social sciences, hard sciences, and other areas that are important for some people to learn. This covers 57\u2026 See the full description on the dataset page: https://huggingface.co/datasets/cais/mmlu.",
+    "__tags__": {
+        "annotations_creators": "no-annotation",
+        "arxiv": [
+            "2009.03300",
+            "2005.00700",
+            "2005.14165",
+            "2008.02275"
+        ],
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "mit",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": "multiple-choice-qa"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "grn_Latn",
+        "name": "high_school_physics",
+        "path": "cais/mmlu",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "grn_Latn": "test"
+                "dev": "train"
             },
             "type": "rename_splits"
         },
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
             "fields": {
-                "context_type": "passage"
+                "topic": "high school physics"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/hat_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/xsum.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4642857142857143%*

 * *Differences: {"'__description__'": "'Extreme Summarization (XSum) Dataset.\\nThere are three features:\\n- "*

 * *                      'document: Input news article.\\n- summary: One sentence summary of the '*

 * *                      "article.\\n- id: BBC ID of the article.'",*

 * * "'__tags__'": "OrderedDict([('annotations_creators', 'found'), ('arxiv', '1808.08745'), "*

 * *               "('croissant', True), ('language', 'en'), ('language_creators', 'found'), "*

 * *               "('license', 'unknown'), ('multilinguality', 'monolingual […]*

```diff
@@ -1,53 +1,32 @@
 {
+    "__description__": "Extreme Summarization (XSum) Dataset.\nThere are three features:\n- document: Input news article.\n- summary: One sentence summary of the article.\n- id: BBC ID of the article.",
+    "__tags__": {
+        "annotations_creators": "found",
+        "arxiv": "1808.08745",
+        "croissant": true,
+        "language": "en",
+        "language_creators": "found",
+        "license": "unknown",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "100K<n<1M",
+        "source_datasets": "original",
+        "task_categories": "summarization",
+        "task_ids": "news-articles-summarization"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "hat_Latn",
+        "path": "EdinburghNLP/xsum",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mapper": {
-                "hat_Latn": "test"
-            },
-            "type": "rename_splits"
-        },
-        {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
             "fields": {
-                "context_type": "passage"
+                "document_type": "document"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.summarization.abstractive",
+    "templates": "templates.summarization.abstractive.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/hau_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/xwinogrande/jp.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'__description__'": "'A multilingual collection of Winograd Schemas in six languages that can be "*

 * *                      "used for evaluation of cross-lingual commonsense reasoning capabilities.'",*

 * * "'__tags__'": "OrderedDict([('arxiv', ['2211.01786', '2106.12066']), ('croissant', True), "*

 * *               "('language', ['en', 'fr', 'ja', 'pt', 'ru', 'zh']), ('license', 'cc-by-4.0'), "*

 * *               "('region', 'us')])",*

 * * "'loader'": "{'path': 'Muennighoff/xwinograd', 'name': 'jp', delete: ['split']}",*

 * * "' […]*

```diff
@@ -1,53 +1,55 @@
 {
+    "__description__": "A multilingual collection of Winograd Schemas in six languages that can be used for evaluation of cross-lingual commonsense reasoning capabilities.",
+    "__tags__": {
+        "arxiv": [
+            "2211.01786",
+            "2106.12066"
+        ],
+        "croissant": true,
+        "language": [
+            "en",
+            "fr",
+            "ja",
+            "pt",
+            "ru",
+            "zh"
+        ],
+        "license": "cc-by-4.0",
+        "region": "us"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "hau_Latn",
+        "name": "jp",
+        "path": "Muennighoff/xwinograd",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mapper": {
-                "hau_Latn": "test"
-            },
-            "type": "rename_splits"
-        },
-        {
             "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
+                "option1",
+                "option2"
             ],
             "to_field": "choices",
             "type": "list_field_values"
         },
         {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
             "fields": {
                 "answer": "int"
             },
             "type": "cast_fields"
         },
         {
             "add": -1,
             "field": "answer",
             "type": "add_constant"
         },
         {
-            "fields": {
-                "context_type": "passage"
+            "field_to_field": {
+                "sentence": "question"
             },
-            "type": "add_fields"
+            "type": "rename_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.open",
+    "templates": "templates.qa.multiple_choice.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/heb_hebr.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/xwinogrande/zh.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'__description__'": "'A multilingual collection of Winograd Schemas in six languages that can be "*

 * *                      "used for evaluation of cross-lingual commonsense reasoning capabilities.'",*

 * * "'__tags__'": "OrderedDict([('arxiv', ['2211.01786', '2106.12066']), ('croissant', True), "*

 * *               "('language', ['en', 'fr', 'ja', 'pt', 'ru', 'zh']), ('license', 'cc-by-4.0'), "*

 * *               "('region', 'us')])",*

 * * "'loader'": "{'path': 'Muennighoff/xwinograd', 'name': 'zh', delete: ['split']}",*

 * * "' […]*

```diff
@@ -1,53 +1,55 @@
 {
+    "__description__": "A multilingual collection of Winograd Schemas in six languages that can be used for evaluation of cross-lingual commonsense reasoning capabilities.",
+    "__tags__": {
+        "arxiv": [
+            "2211.01786",
+            "2106.12066"
+        ],
+        "croissant": true,
+        "language": [
+            "en",
+            "fr",
+            "ja",
+            "pt",
+            "ru",
+            "zh"
+        ],
+        "license": "cc-by-4.0",
+        "region": "us"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "heb_Hebr",
+        "name": "zh",
+        "path": "Muennighoff/xwinograd",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mapper": {
-                "heb_Hebr": "test"
-            },
-            "type": "rename_splits"
-        },
-        {
             "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
+                "option1",
+                "option2"
             ],
             "to_field": "choices",
             "type": "list_field_values"
         },
         {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
             "fields": {
                 "answer": "int"
             },
             "type": "cast_fields"
         },
         {
             "add": -1,
             "field": "answer",
             "type": "add_constant"
         },
         {
-            "fields": {
-                "context_type": "passage"
+            "field_to_field": {
+                "sentence": "question"
             },
-            "type": "add_fields"
+            "type": "rename_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.open",
+    "templates": "templates.qa.multiple_choice.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/hin_deva.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/high_school_macroeconomics.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48214285714285715%*

 * *Differences: {"'__description__'": "'Dataset Card for MMLU\\nDataset Summary\\nMeasuring Massive Multitask "*

 * *                      'Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy '*

 * *                      'Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\\nThis is '*

 * *                      'a massive multitask test consisting of multiple-choice questions from '*

 * *                      'various branches of knowledge. The test spans subjects in the humanities, '*

 * *                      […]*

```diff
@@ -1,53 +1,44 @@
 {
+    "__description__": "Dataset Card for MMLU\nDataset Summary\nMeasuring Massive Multitask Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\nThis is a massive multitask test consisting of multiple-choice questions from various branches of knowledge. The test spans subjects in the humanities, social sciences, hard sciences, and other areas that are important for some people to learn. This covers 57\u2026 See the full description on the dataset page: https://huggingface.co/datasets/cais/mmlu.",
+    "__tags__": {
+        "annotations_creators": "no-annotation",
+        "arxiv": [
+            "2009.03300",
+            "2005.00700",
+            "2005.14165",
+            "2008.02275"
+        ],
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "mit",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": "multiple-choice-qa"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "hin_Deva",
+        "name": "high_school_macroeconomics",
+        "path": "cais/mmlu",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "hin_Deva": "test"
+                "dev": "train"
             },
             "type": "rename_splits"
         },
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
             "fields": {
-                "context_type": "passage"
+                "topic": "high school macroeconomics"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/hin_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/management.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48214285714285715%*

 * *Differences: {"'__description__'": "'Dataset Card for MMLU\\nDataset Summary\\nMeasuring Massive Multitask "*

 * *                      'Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy '*

 * *                      'Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\\nThis is '*

 * *                      'a massive multitask test consisting of multiple-choice questions from '*

 * *                      'various branches of knowledge. The test spans subjects in the humanities, '*

 * *                      […]*

```diff
@@ -1,53 +1,44 @@
 {
+    "__description__": "Dataset Card for MMLU\nDataset Summary\nMeasuring Massive Multitask Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\nThis is a massive multitask test consisting of multiple-choice questions from various branches of knowledge. The test spans subjects in the humanities, social sciences, hard sciences, and other areas that are important for some people to learn. This covers 57\u2026 See the full description on the dataset page: https://huggingface.co/datasets/cais/mmlu.",
+    "__tags__": {
+        "annotations_creators": "no-annotation",
+        "arxiv": [
+            "2009.03300",
+            "2005.00700",
+            "2005.14165",
+            "2008.02275"
+        ],
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "mit",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": "multiple-choice-qa"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "hin_Latn",
+        "name": "management",
+        "path": "cais/mmlu",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "hin_Latn": "test"
+                "dev": "train"
             },
             "type": "rename_splits"
         },
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
             "fields": {
-                "context_type": "passage"
+                "topic": "management"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/hun_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/high_school_computer_science.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48214285714285715%*

 * *Differences: {"'__description__'": "'Dataset Card for MMLU\\nDataset Summary\\nMeasuring Massive Multitask "*

 * *                      'Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy '*

 * *                      'Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\\nThis is '*

 * *                      'a massive multitask test consisting of multiple-choice questions from '*

 * *                      'various branches of knowledge. The test spans subjects in the humanities, '*

 * *                      […]*

```diff
@@ -1,53 +1,44 @@
 {
+    "__description__": "Dataset Card for MMLU\nDataset Summary\nMeasuring Massive Multitask Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\nThis is a massive multitask test consisting of multiple-choice questions from various branches of knowledge. The test spans subjects in the humanities, social sciences, hard sciences, and other areas that are important for some people to learn. This covers 57\u2026 See the full description on the dataset page: https://huggingface.co/datasets/cais/mmlu.",
+    "__tags__": {
+        "annotations_creators": "no-annotation",
+        "arxiv": [
+            "2009.03300",
+            "2005.00700",
+            "2005.14165",
+            "2008.02275"
+        ],
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "mit",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": "multiple-choice-qa"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "hun_Latn",
+        "name": "high_school_computer_science",
+        "path": "cais/mmlu",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "hun_Latn": "test"
+                "dev": "train"
             },
             "type": "rename_splits"
         },
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
             "fields": {
-                "context_type": "passage"
+                "topic": "high school computer science"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/isl_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/astronomy.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48214285714285715%*

 * *Differences: {"'__description__'": "'Dataset Card for MMLU\\nDataset Summary\\nMeasuring Massive Multitask "*

 * *                      'Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy '*

 * *                      'Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\\nThis is '*

 * *                      'a massive multitask test consisting of multiple-choice questions from '*

 * *                      'various branches of knowledge. The test spans subjects in the humanities, '*

 * *                      […]*

```diff
@@ -1,53 +1,44 @@
 {
+    "__description__": "Dataset Card for MMLU\nDataset Summary\nMeasuring Massive Multitask Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\nThis is a massive multitask test consisting of multiple-choice questions from various branches of knowledge. The test spans subjects in the humanities, social sciences, hard sciences, and other areas that are important for some people to learn. This covers 57\u2026 See the full description on the dataset page: https://huggingface.co/datasets/cais/mmlu.",
+    "__tags__": {
+        "annotations_creators": "no-annotation",
+        "arxiv": [
+            "2009.03300",
+            "2005.00700",
+            "2005.14165",
+            "2008.02275"
+        ],
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "mit",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": "multiple-choice-qa"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "isl_Latn",
+        "name": "astronomy",
+        "path": "cais/mmlu",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "isl_Latn": "test"
+                "dev": "train"
             },
             "type": "rename_splits"
         },
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
             "fields": {
-                "context_type": "passage"
+                "topic": "astronomy"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/kac_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/econometrics.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48214285714285715%*

 * *Differences: {"'__description__'": "'Dataset Card for MMLU\\nDataset Summary\\nMeasuring Massive Multitask "*

 * *                      'Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy '*

 * *                      'Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\\nThis is '*

 * *                      'a massive multitask test consisting of multiple-choice questions from '*

 * *                      'various branches of knowledge. The test spans subjects in the humanities, '*

 * *                      […]*

```diff
@@ -1,53 +1,44 @@
 {
+    "__description__": "Dataset Card for MMLU\nDataset Summary\nMeasuring Massive Multitask Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\nThis is a massive multitask test consisting of multiple-choice questions from various branches of knowledge. The test spans subjects in the humanities, social sciences, hard sciences, and other areas that are important for some people to learn. This covers 57\u2026 See the full description on the dataset page: https://huggingface.co/datasets/cais/mmlu.",
+    "__tags__": {
+        "annotations_creators": "no-annotation",
+        "arxiv": [
+            "2009.03300",
+            "2005.00700",
+            "2005.14165",
+            "2008.02275"
+        ],
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "mit",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": "multiple-choice-qa"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "kac_Latn",
+        "name": "econometrics",
+        "path": "cais/mmlu",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "kac_Latn": "test"
+                "dev": "train"
             },
             "type": "rename_splits"
         },
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
             "fields": {
-                "context_type": "passage"
+                "topic": "econometrics"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/kor_hang.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/high_school_microeconomics.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48214285714285715%*

 * *Differences: {"'__description__'": "'Dataset Card for MMLU\\nDataset Summary\\nMeasuring Massive Multitask "*

 * *                      'Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy '*

 * *                      'Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\\nThis is '*

 * *                      'a massive multitask test consisting of multiple-choice questions from '*

 * *                      'various branches of knowledge. The test spans subjects in the humanities, '*

 * *                      […]*

```diff
@@ -1,53 +1,44 @@
 {
+    "__description__": "Dataset Card for MMLU\nDataset Summary\nMeasuring Massive Multitask Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\nThis is a massive multitask test consisting of multiple-choice questions from various branches of knowledge. The test spans subjects in the humanities, social sciences, hard sciences, and other areas that are important for some people to learn. This covers 57\u2026 See the full description on the dataset page: https://huggingface.co/datasets/cais/mmlu.",
+    "__tags__": {
+        "annotations_creators": "no-annotation",
+        "arxiv": [
+            "2009.03300",
+            "2005.00700",
+            "2005.14165",
+            "2008.02275"
+        ],
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "mit",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": "multiple-choice-qa"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "kor_Hang",
+        "name": "high_school_microeconomics",
+        "path": "cais/mmlu",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "kor_Hang": "test"
+                "dev": "train"
             },
             "type": "rename_splits"
         },
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
             "fields": {
-                "context_type": "passage"
+                "topic": "high school microeconomics"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/lug_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/business_ethics.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48214285714285715%*

 * *Differences: {"'__description__'": "'Dataset Card for MMLU\\nDataset Summary\\nMeasuring Massive Multitask "*

 * *                      'Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy '*

 * *                      'Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\\nThis is '*

 * *                      'a massive multitask test consisting of multiple-choice questions from '*

 * *                      'various branches of knowledge. The test spans subjects in the humanities, '*

 * *                      […]*

```diff
@@ -1,53 +1,44 @@
 {
+    "__description__": "Dataset Card for MMLU\nDataset Summary\nMeasuring Massive Multitask Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\nThis is a massive multitask test consisting of multiple-choice questions from various branches of knowledge. The test spans subjects in the humanities, social sciences, hard sciences, and other areas that are important for some people to learn. This covers 57\u2026 See the full description on the dataset page: https://huggingface.co/datasets/cais/mmlu.",
+    "__tags__": {
+        "annotations_creators": "no-annotation",
+        "arxiv": [
+            "2009.03300",
+            "2005.00700",
+            "2005.14165",
+            "2008.02275"
+        ],
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "mit",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": "multiple-choice-qa"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "lug_Latn",
+        "name": "business_ethics",
+        "path": "cais/mmlu",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "lug_Latn": "test"
+                "dev": "train"
             },
             "type": "rename_splits"
         },
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
             "fields": {
-                "context_type": "passage"
+                "topic": "business ethics"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/luo_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/high_school_mathematics.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48214285714285715%*

 * *Differences: {"'__description__'": "'Dataset Card for MMLU\\nDataset Summary\\nMeasuring Massive Multitask "*

 * *                      'Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy '*

 * *                      'Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\\nThis is '*

 * *                      'a massive multitask test consisting of multiple-choice questions from '*

 * *                      'various branches of knowledge. The test spans subjects in the humanities, '*

 * *                      […]*

```diff
@@ -1,53 +1,44 @@
 {
+    "__description__": "Dataset Card for MMLU\nDataset Summary\nMeasuring Massive Multitask Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\nThis is a massive multitask test consisting of multiple-choice questions from various branches of knowledge. The test spans subjects in the humanities, social sciences, hard sciences, and other areas that are important for some people to learn. This covers 57\u2026 See the full description on the dataset page: https://huggingface.co/datasets/cais/mmlu.",
+    "__tags__": {
+        "annotations_creators": "no-annotation",
+        "arxiv": [
+            "2009.03300",
+            "2005.00700",
+            "2005.14165",
+            "2008.02275"
+        ],
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "mit",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": "multiple-choice-qa"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "luo_Latn",
+        "name": "high_school_mathematics",
+        "path": "cais/mmlu",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "luo_Latn": "test"
+                "dev": "train"
             },
             "type": "rename_splits"
         },
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
             "fields": {
-                "context_type": "passage"
+                "topic": "high school mathematics"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/mkd_cyrl.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/formal_logic.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48214285714285715%*

 * *Differences: {"'__description__'": "'Dataset Card for MMLU\\nDataset Summary\\nMeasuring Massive Multitask "*

 * *                      'Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy '*

 * *                      'Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\\nThis is '*

 * *                      'a massive multitask test consisting of multiple-choice questions from '*

 * *                      'various branches of knowledge. The test spans subjects in the humanities, '*

 * *                      […]*

```diff
@@ -1,53 +1,44 @@
 {
+    "__description__": "Dataset Card for MMLU\nDataset Summary\nMeasuring Massive Multitask Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\nThis is a massive multitask test consisting of multiple-choice questions from various branches of knowledge. The test spans subjects in the humanities, social sciences, hard sciences, and other areas that are important for some people to learn. This covers 57\u2026 See the full description on the dataset page: https://huggingface.co/datasets/cais/mmlu.",
+    "__tags__": {
+        "annotations_creators": "no-annotation",
+        "arxiv": [
+            "2009.03300",
+            "2005.00700",
+            "2005.14165",
+            "2008.02275"
+        ],
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "mit",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": "multiple-choice-qa"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "mkd_Cyrl",
+        "name": "formal_logic",
+        "path": "cais/mmlu",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "mkd_Cyrl": "test"
+                "dev": "train"
             },
             "type": "rename_splits"
         },
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
             "fields": {
-                "context_type": "passage"
+                "topic": "formal logic"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/mri_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/philosophy.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48214285714285715%*

 * *Differences: {"'__description__'": "'Dataset Card for MMLU\\nDataset Summary\\nMeasuring Massive Multitask "*

 * *                      'Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy '*

 * *                      'Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\\nThis is '*

 * *                      'a massive multitask test consisting of multiple-choice questions from '*

 * *                      'various branches of knowledge. The test spans subjects in the humanities, '*

 * *                      […]*

```diff
@@ -1,53 +1,44 @@
 {
+    "__description__": "Dataset Card for MMLU\nDataset Summary\nMeasuring Massive Multitask Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\nThis is a massive multitask test consisting of multiple-choice questions from various branches of knowledge. The test spans subjects in the humanities, social sciences, hard sciences, and other areas that are important for some people to learn. This covers 57\u2026 See the full description on the dataset page: https://huggingface.co/datasets/cais/mmlu.",
+    "__tags__": {
+        "annotations_creators": "no-annotation",
+        "arxiv": [
+            "2009.03300",
+            "2005.00700",
+            "2005.14165",
+            "2008.02275"
+        ],
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "mit",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": "multiple-choice-qa"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "mri_Latn",
+        "name": "philosophy",
+        "path": "cais/mmlu",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "mri_Latn": "test"
+                "dev": "train"
             },
             "type": "rename_splits"
         },
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
             "fields": {
-                "context_type": "passage"
+                "topic": "philosophy"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/nso_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/public_relations.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48214285714285715%*

 * *Differences: {"'__description__'": "'Dataset Card for MMLU\\nDataset Summary\\nMeasuring Massive Multitask "*

 * *                      'Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy '*

 * *                      'Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\\nThis is '*

 * *                      'a massive multitask test consisting of multiple-choice questions from '*

 * *                      'various branches of knowledge. The test spans subjects in the humanities, '*

 * *                      […]*

```diff
@@ -1,53 +1,44 @@
 {
+    "__description__": "Dataset Card for MMLU\nDataset Summary\nMeasuring Massive Multitask Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\nThis is a massive multitask test consisting of multiple-choice questions from various branches of knowledge. The test spans subjects in the humanities, social sciences, hard sciences, and other areas that are important for some people to learn. This covers 57\u2026 See the full description on the dataset page: https://huggingface.co/datasets/cais/mmlu.",
+    "__tags__": {
+        "annotations_creators": "no-annotation",
+        "arxiv": [
+            "2009.03300",
+            "2005.00700",
+            "2005.14165",
+            "2008.02275"
+        ],
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "mit",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": "multiple-choice-qa"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "nso_Latn",
+        "name": "public_relations",
+        "path": "cais/mmlu",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "nso_Latn": "test"
+                "dev": "train"
             },
             "type": "rename_splits"
         },
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
             "fields": {
-                "context_type": "passage"
+                "topic": "public relations"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/nya_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/tl/trg.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.47232142857142856%*

 * *Differences: {"'__description__'": "'Universal Named Entity Recognition (UNER) aims to fill a gap in "*

 * *                      'multilingual NLP: high quality NER datasets in many languages with a shared '*

 * *                      'tagset.\\nUNER is modeled after the Universal Dependencies project, in that '*

 * *                      'it is intended to be a large community annotation effort with '*

 * *                      'language-universal guidelines. Further, we use the same text corpora as '*

 * *                      "Universal Dep […]*

```diff
@@ -1,53 +1,97 @@
 {
+    "__description__": "Universal Named Entity Recognition (UNER) aims to fill a gap in multilingual NLP: high quality NER datasets in many languages with a shared tagset.\nUNER is modeled after the Universal Dependencies project, in that it is intended to be a large community annotation effort with language-universal guidelines. Further, we use the same text corpora as Universal Dependencies.",
+    "__tags__": {
+        "arxiv": "2311.09122",
+        "language": [
+            "ceb",
+            "da",
+            "de",
+            "en",
+            "hr",
+            "pt",
+            "ru",
+            "sk",
+            "sr",
+            "sv",
+            "tl",
+            "zh"
+        ],
+        "license": "cc-by-sa-4.0",
+        "region": "us",
+        "task_categories": "token-classification"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "nya_Latn",
+        "name": "tl_trg",
+        "path": "universalner/universal_ner",
+        "requirements_list": [
+            "conllu"
+        ],
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mapper": {
-                "nya_Latn": "test"
+            "field_to_field": {
+                "ner_tags": "labels"
             },
-            "type": "rename_splits"
+            "type": "rename_fields"
         },
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
+            "field": "labels",
+            "items_list": [
+                "O",
+                "B-PER",
+                "I-PER",
+                "B-ORG",
+                "I-ORG",
+                "B-LOC",
+                "I-LOC"
             ],
-            "to_field": "choices",
-            "type": "list_field_values"
+            "process_every_value": true,
+            "type": "get_item_by_index"
         },
         {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
+            "begin_labels": [
+                "B-PER",
+                "B-ORG",
+                "B-LOC"
+            ],
+            "inside_labels": [
+                "I-PER",
+                "I-ORG",
+                "I-LOC"
+            ],
+            "labels": [
+                "Person",
+                "Organization",
+                "Location"
+            ],
+            "outside_label": "O",
+            "type": "iob_extractor"
         },
         {
-            "fields": {
-                "answer": "int"
+            "field_to_field": {
+                "spans/*/end": "spans_ends",
+                "spans/*/label": "labels",
+                "spans/*/start": "spans_starts"
             },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
+            "get_default": [],
+            "not_exist_ok": true,
+            "type": "copy_fields"
         },
         {
             "fields": {
-                "context_type": "passage"
+                "class_type": "entity type",
+                "classes": [
+                    "Person",
+                    "Organization",
+                    "Location"
+                ],
+                "text_type": "text"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.span_labeling.extraction",
+    "templates": "templates.span_labeling.extraction.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/plt_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/college_medicine.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48214285714285715%*

 * *Differences: {"'__description__'": "'Dataset Card for MMLU\\nDataset Summary\\nMeasuring Massive Multitask "*

 * *                      'Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy '*

 * *                      'Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\\nThis is '*

 * *                      'a massive multitask test consisting of multiple-choice questions from '*

 * *                      'various branches of knowledge. The test spans subjects in the humanities, '*

 * *                      […]*

```diff
@@ -1,53 +1,44 @@
 {
+    "__description__": "Dataset Card for MMLU\nDataset Summary\nMeasuring Massive Multitask Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\nThis is a massive multitask test consisting of multiple-choice questions from various branches of knowledge. The test spans subjects in the humanities, social sciences, hard sciences, and other areas that are important for some people to learn. This covers 57\u2026 See the full description on the dataset page: https://huggingface.co/datasets/cais/mmlu.",
+    "__tags__": {
+        "annotations_creators": "no-annotation",
+        "arxiv": [
+            "2009.03300",
+            "2005.00700",
+            "2005.14165",
+            "2008.02275"
+        ],
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "mit",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": "multiple-choice-qa"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "plt_Latn",
+        "name": "college_medicine",
+        "path": "cais/mmlu",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "plt_Latn": "test"
+                "dev": "train"
             },
             "type": "rename_splits"
         },
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
             "fields": {
-                "context_type": "passage"
+                "topic": "college medicine"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/tir_ethi.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/tldr.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.46984126984126984%*

 * *Differences: {"'__description__'": "'This corpus contains preprocessed posts from the Reddit dataset.\\nThe "*

 * *                      'dataset consists of 3,848,330 posts with an average length of 270 words for '*

 * *                      'content,\\nand 28 words for the summary.\\nFeatures includes strings: '*

 * *                      'author, body, normalizedBody, content, summary, subreddit, '*

 * *                      'subreddit_id.\\nContent is used as document and summary is used as '*

 * *                      "summary.'",*

 * * "'__tag […]*

```diff
@@ -1,53 +1,45 @@
 {
+    "__description__": "This corpus contains preprocessed posts from the Reddit dataset.\nThe dataset consists of 3,848,330 posts with an average length of 270 words for content,\nand 28 words for the summary.\nFeatures includes strings: author, body, normalizedBody, content, summary, subreddit, subreddit_id.\nContent is used as document and summary is used as summary.",
+    "__tags__": {
+        "annotations_creators": "no-annotation",
+        "croissant": true,
+        "language": "en",
+        "language_creators": "crowdsourced",
+        "license": "cc-by-4.0",
+        "multilinguality": "monolingual",
+        "reddit-posts-summarization": true,
+        "region": "us",
+        "size_categories": "1M<n<10M",
+        "source_datasets": "original",
+        "task_categories": "summarization"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "tir_Ethi",
+        "path": "webis/tldr-17",
+        "streaming": true,
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mapper": {
-                "tir_Ethi": "test"
+            "mix": {
+                "test": "train[50%]",
+                "train": "train[50%]"
             },
-            "type": "rename_splits"
-        },
-        {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
+            "type": "split_random_mix"
         },
         {
             "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
+                "content": "document"
             },
             "type": "rename_fields"
         },
         {
             "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
-            "fields": {
-                "context_type": "passage"
+                "document_type": "document"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.summarization.abstractive",
+    "templates": "templates.summarization.abstractive.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/tsn_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/us_foreign_policy.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48214285714285715%*

 * *Differences: {"'__description__'": "'Dataset Card for MMLU\\nDataset Summary\\nMeasuring Massive Multitask "*

 * *                      'Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy '*

 * *                      'Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\\nThis is '*

 * *                      'a massive multitask test consisting of multiple-choice questions from '*

 * *                      'various branches of knowledge. The test spans subjects in the humanities, '*

 * *                      […]*

```diff
@@ -1,53 +1,44 @@
 {
+    "__description__": "Dataset Card for MMLU\nDataset Summary\nMeasuring Massive Multitask Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\nThis is a massive multitask test consisting of multiple-choice questions from various branches of knowledge. The test spans subjects in the humanities, social sciences, hard sciences, and other areas that are important for some people to learn. This covers 57\u2026 See the full description on the dataset page: https://huggingface.co/datasets/cais/mmlu.",
+    "__tags__": {
+        "annotations_creators": "no-annotation",
+        "arxiv": [
+            "2009.03300",
+            "2005.00700",
+            "2005.14165",
+            "2008.02275"
+        ],
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "mit",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": "multiple-choice-qa"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "tsn_Latn",
+        "name": "us_foreign_policy",
+        "path": "cais/mmlu",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "tsn_Latn": "test"
+                "dev": "train"
             },
             "type": "rename_splits"
         },
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
             "fields": {
-                "context_type": "passage"
+                "topic": "us foreign policy"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/tso_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/en/ewt.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.47232142857142856%*

 * *Differences: {"'__description__'": "'Universal Named Entity Recognition (UNER) aims to fill a gap in "*

 * *                      'multilingual NLP: high quality NER datasets in many languages with a shared '*

 * *                      'tagset.\\nUNER is modeled after the Universal Dependencies project, in that '*

 * *                      'it is intended to be a large community annotation effort with '*

 * *                      'language-universal guidelines. Further, we use the same text corpora as '*

 * *                      "Universal Dep […]*

```diff
@@ -1,53 +1,97 @@
 {
+    "__description__": "Universal Named Entity Recognition (UNER) aims to fill a gap in multilingual NLP: high quality NER datasets in many languages with a shared tagset.\nUNER is modeled after the Universal Dependencies project, in that it is intended to be a large community annotation effort with language-universal guidelines. Further, we use the same text corpora as Universal Dependencies.",
+    "__tags__": {
+        "arxiv": "2311.09122",
+        "language": [
+            "ceb",
+            "da",
+            "de",
+            "en",
+            "hr",
+            "pt",
+            "ru",
+            "sk",
+            "sr",
+            "sv",
+            "tl",
+            "zh"
+        ],
+        "license": "cc-by-sa-4.0",
+        "region": "us",
+        "task_categories": "token-classification"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "tso_Latn",
+        "name": "en_ewt",
+        "path": "universalner/universal_ner",
+        "requirements_list": [
+            "conllu"
+        ],
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mapper": {
-                "tso_Latn": "test"
+            "field_to_field": {
+                "ner_tags": "labels"
             },
-            "type": "rename_splits"
+            "type": "rename_fields"
         },
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
+            "field": "labels",
+            "items_list": [
+                "O",
+                "B-PER",
+                "I-PER",
+                "B-ORG",
+                "I-ORG",
+                "B-LOC",
+                "I-LOC"
             ],
-            "to_field": "choices",
-            "type": "list_field_values"
+            "process_every_value": true,
+            "type": "get_item_by_index"
         },
         {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
+            "begin_labels": [
+                "B-PER",
+                "B-ORG",
+                "B-LOC"
+            ],
+            "inside_labels": [
+                "I-PER",
+                "I-ORG",
+                "I-LOC"
+            ],
+            "labels": [
+                "Person",
+                "Organization",
+                "Location"
+            ],
+            "outside_label": "O",
+            "type": "iob_extractor"
         },
         {
-            "fields": {
-                "answer": "int"
+            "field_to_field": {
+                "spans/*/end": "spans_ends",
+                "spans/*/label": "labels",
+                "spans/*/start": "spans_starts"
             },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
+            "get_default": [],
+            "not_exist_ok": true,
+            "type": "copy_fields"
         },
         {
             "fields": {
-                "context_type": "passage"
+                "class_type": "entity type",
+                "classes": [
+                    "Person",
+                    "Organization",
+                    "Location"
+                ],
+                "text_type": "text"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.span_labeling.extraction",
+    "templates": "templates.span_labeling.extraction.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/zho_hans.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/wikitq.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.46354166666666663%*

 * *Differences: {"'__description__'": "'This WikiTableQuestions dataset is a large-scale dataset for the task of "*

 * *                      "question answering on semi-structured tables.'",*

 * * "'__tags__'": "OrderedDict([('annotations_creators', 'crowdsourced'), ('arxiv', '1508.00305'), "*

 * *               "('croissant', True), ('language', 'en'), ('language_creators', 'found'), "*

 * *               "('license', 'cc-by-4.0'), ('multilinguality', 'monolingual'), ('region', 'us'), "*

 * *               "('size_categories', '10K<n<100K'), ('s […]*

```diff
@@ -1,53 +1,53 @@
 {
+    "__description__": "This WikiTableQuestions dataset is a large-scale dataset for the task of question answering on semi-structured tables.",
+    "__tags__": {
+        "annotations_creators": "crowdsourced",
+        "arxiv": "1508.00305",
+        "croissant": true,
+        "language": "en",
+        "language_creators": "found",
+        "license": "cc-by-4.0",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "table-question-answering": true,
+        "task_categories": "question-answering"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "zho_Hans",
+        "path": "wikitablequestions",
         "type": "load_hf"
     },
     "preprocess_steps": [
+        "splitters.small_no_test",
         {
-            "mapper": {
-                "zho_Hans": "test"
-            },
-            "type": "rename_splits"
-        },
-        {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
+            "fields": {
+                "context_type": "table"
             },
-            "type": "rename_fields"
+            "type": "add_fields"
         },
         {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
+            "max_length": 15,
+            "table": "table",
+            "text_output": "answers",
+            "type": "truncate_table_cells"
         },
         {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
+            "field": "table",
+            "rows_to_keep": 50,
+            "type": "truncate_table_rows"
         },
         {
-            "fields": {
-                "context_type": "passage"
-            },
-            "type": "add_fields"
+            "field_to_field": [
+                [
+                    "table",
+                    "context"
+                ]
+            ],
+            "type": "serialize_table_as_indexed_row_major"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.qa.with_context.extractive",
+    "templates": "templates.qa.with_context.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/belebele/zul_latn.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/en/pud.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.47232142857142856%*

 * *Differences: {"'__description__'": "'Universal Named Entity Recognition (UNER) aims to fill a gap in "*

 * *                      'multilingual NLP: high quality NER datasets in many languages with a shared '*

 * *                      'tagset.\\nUNER is modeled after the Universal Dependencies project, in that '*

 * *                      'it is intended to be a large community annotation effort with '*

 * *                      'language-universal guidelines. Further, we use the same text corpora as '*

 * *                      "Universal Dep […]*

```diff
@@ -1,53 +1,97 @@
 {
+    "__description__": "Universal Named Entity Recognition (UNER) aims to fill a gap in multilingual NLP: high quality NER datasets in many languages with a shared tagset.\nUNER is modeled after the Universal Dependencies project, in that it is intended to be a large community annotation effort with language-universal guidelines. Further, we use the same text corpora as Universal Dependencies.",
+    "__tags__": {
+        "arxiv": "2311.09122",
+        "language": [
+            "ceb",
+            "da",
+            "de",
+            "en",
+            "hr",
+            "pt",
+            "ru",
+            "sk",
+            "sr",
+            "sv",
+            "tl",
+            "zh"
+        ],
+        "license": "cc-by-sa-4.0",
+        "region": "us",
+        "task_categories": "token-classification"
+    },
     "loader": {
-        "name": "default",
-        "path": "facebook/belebele",
-        "split": "zul_Latn",
+        "name": "en_pud",
+        "path": "universalner/universal_ner",
+        "requirements_list": [
+            "conllu"
+        ],
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mapper": {
-                "zul_Latn": "test"
+            "field_to_field": {
+                "ner_tags": "labels"
             },
-            "type": "rename_splits"
+            "type": "rename_fields"
         },
         {
-            "fields": [
-                "mc_answer1",
-                "mc_answer2",
-                "mc_answer3",
-                "mc_answer4"
+            "field": "labels",
+            "items_list": [
+                "O",
+                "B-PER",
+                "I-PER",
+                "B-ORG",
+                "I-ORG",
+                "B-LOC",
+                "I-LOC"
             ],
-            "to_field": "choices",
-            "type": "list_field_values"
+            "process_every_value": true,
+            "type": "get_item_by_index"
         },
         {
-            "field_to_field": {
-                "correct_answer_num": "answer",
-                "flores_passage": "context"
-            },
-            "type": "rename_fields"
+            "begin_labels": [
+                "B-PER",
+                "B-ORG",
+                "B-LOC"
+            ],
+            "inside_labels": [
+                "I-PER",
+                "I-ORG",
+                "I-LOC"
+            ],
+            "labels": [
+                "Person",
+                "Organization",
+                "Location"
+            ],
+            "outside_label": "O",
+            "type": "iob_extractor"
         },
         {
-            "fields": {
-                "answer": "int"
+            "field_to_field": {
+                "spans/*/end": "spans_ends",
+                "spans/*/label": "labels",
+                "spans/*/start": "spans_starts"
             },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
+            "get_default": [],
+            "not_exist_ok": true,
+            "type": "copy_fields"
         },
         {
             "fields": {
-                "context_type": "passage"
+                "class_type": "entity type",
+                "classes": [
+                    "Person",
+                    "Organization",
+                    "Location"
+                ],
+                "text_type": "text"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.no_intro.all",
+    "task": "tasks.span_labeling.extraction",
+    "templates": "templates.span_labeling.extraction.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/bold.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/vietnamese.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4724702380952381%*

 * *Differences: {"'__description__'": "'We present XLSum, a comprehensive and diverse dataset comprising 1.35 "*

 * *                      'million professionally\\nannotated article-summary pairs from BBC, '*

 * *                      'extracted using a set of carefully designed heuristics.\\nThe dataset '*

 * *                      'covers 45 languages ranging from low to high-resource, for many of which '*

 * *                      'no\\npublic dataset is currently available. XL-Sum is highly abstractive, '*

 * *                      'concise,\ […]*

```diff
@@ -1,91 +1,39 @@
 {
+    "__description__": "We present XLSum, a comprehensive and diverse dataset comprising 1.35 million professionally\nannotated article-summary pairs from BBC, extracted using a set of carefully designed heuristics.\nThe dataset covers 45 languages ranging from low to high-resource, for many of which no\npublic dataset is currently available. XL-Sum is highly abstractive, concise,\nand of high quality, as indicated by human and intrinsic evaluation.",
+    "__tags__": {
+        "annotations_creators": "none",
+        "arxiv": "1607.01759",
+        "croissant": true,
+        "language": "und",
+        "language_creators": "unknown",
+        "license": "cc-by-nc-sa-4.0",
+        "multilinguality": "unknown",
+        "region": "us",
+        "size_categories": "unknown",
+        "source_datasets": "original",
+        "task_categories": "summarization"
+    },
     "loader": {
-        "path": "AlexaAI/bold",
+        "name": "vietnamese",
+        "path": "GEM/xlsum",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mapper": {
-                "train": "test"
+            "field_to_field": {
+                "target": "summary",
+                "text": "document"
             },
-            "type": "rename_splits"
+            "type": "rename_fields"
         },
         {
             "fields": {
-                "input_label": {}
+                "document_type": "document"
             },
             "type": "add_fields"
-        },
-        {
-            "field_to_field": [
-                [
-                    "prompts/0",
-                    "first_prompt"
-                ]
-            ],
-            "type": "copy_fields"
-        },
-        {
-            "field_to_field": [
-                [
-                    "wikipedia/0",
-                    "first_wiki"
-                ]
-            ],
-            "type": "copy_fields"
-        },
-        {
-            "condition": "in",
-            "type": "filter_by_condition",
-            "values": {
-                "domain": [
-                    "race",
-                    "gender"
-                ]
-            }
-        },
-        {
-            "page_size": 10000,
-            "type": "shuffle"
-        },
-        {
-            "field_to_field": {
-                "category": "input_label/category",
-                "first_prompt": "input_label/input",
-                "first_wiki": "input_label/wiki"
-            },
-            "type": "copy_fields"
-        },
-        {
-            "_argv": [
-                "input_label"
-            ],
-            "function": "json.dumps",
-            "to_field": "input_label",
-            "type": "apply"
         }
     ],
-    "task": {
-        "inputs": [
-            "first_prompt"
-        ],
-        "metrics": [
-            "metrics.regard"
-        ],
-        "outputs": [
-            "input_label"
-        ],
-        "type": "form_task"
-    },
-    "templates": {
-        "items": [
-            {
-                "input_format": "{first_prompt}\n",
-                "output_format": "{input_label}",
-                "type": "input_output_template"
-            }
-        ],
-        "type": "templates_list"
-    },
+    "task": "tasks.summarization.abstractive",
+    "templates": "templates.summarization.abstractive.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/boolq/classification.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/japanese.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4732142857142857%*

 * *Differences: {"'__description__'": "'We present XLSum, a comprehensive and diverse dataset comprising 1.35 "*

 * *                      'million professionally\\nannotated article-summary pairs from BBC, '*

 * *                      'extracted using a set of carefully designed heuristics.\\nThe dataset '*

 * *                      'covers 45 languages ranging from low to high-resource, for many of which '*

 * *                      'no\\npublic dataset is currently available. XL-Sum is highly abstractive, '*

 * *                      'concise,\ […]*

```diff
@@ -1,47 +1,39 @@
 {
+    "__description__": "We present XLSum, a comprehensive and diverse dataset comprising 1.35 million professionally\nannotated article-summary pairs from BBC, extracted using a set of carefully designed heuristics.\nThe dataset covers 45 languages ranging from low to high-resource, for many of which no\npublic dataset is currently available. XL-Sum is highly abstractive, concise,\nand of high quality, as indicated by human and intrinsic evaluation.",
+    "__tags__": {
+        "annotations_creators": "none",
+        "arxiv": "1607.01759",
+        "croissant": true,
+        "language": "und",
+        "language_creators": "unknown",
+        "license": "cc-by-nc-sa-4.0",
+        "multilinguality": "unknown",
+        "region": "us",
+        "size_categories": "unknown",
+        "source_datasets": "original",
+        "task_categories": "summarization"
+    },
     "loader": {
-        "path": "google/boolq",
+        "name": "japanese",
+        "path": "GEM/xlsum",
         "type": "load_hf"
     },
     "preprocess_steps": [
-        "splitters.small_no_test",
         {
-            "fields": {
-                "classes": [
-                    "yes",
-                    "no"
-                ],
-                "text_a_type": "passage",
-                "text_b_type": "question",
-                "type_of_relation": "answer"
+            "field_to_field": {
+                "target": "summary",
+                "text": "document"
             },
-            "type": "add_fields"
+            "type": "rename_fields"
         },
         {
             "fields": {
-                "answer": "str"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "mappers": {
-                "answer": {
-                    "False": "no",
-                    "True": "yes"
-                }
+                "document_type": "document"
             },
-            "type": "map_instance_values"
-        },
-        {
-            "field_to_field": {
-                "answer": "label",
-                "passage": "text_a",
-                "question": "text_b"
-            },
-            "type": "rename_fields"
+            "type": "add_fields"
         }
     ],
-    "task": "tasks.classification.multi_class.relation",
-    "templates": "templates.classification.multi_class.relation.all",
+    "task": "tasks.summarization.abstractive",
+    "templates": "templates.summarization.abstractive.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/claim_stance_topic.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/qqp.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.494047619047619%*

 * *Differences: {"'__description__'": "'Dataset Card for GLUE\\nDataset Summary\\nGLUE, the General Language "*

 * *                      'Understanding Evaluation benchmark (https://gluebenchmark.com/) is a '*

 * *                      'collection of resources for training, evaluating, and analyzing natural '*

 * *                      'language understanding systems.\\nSupported Tasks and Leaderboards\\nThe '*

 * *                      'leaderboard for the GLUE benchmark can be found at this address. It '*

 * *                      'comprises th […]*

```diff
@@ -1,76 +1,77 @@
 {
+    "__description__": "Dataset Card for GLUE\nDataset Summary\nGLUE, the General Language Understanding Evaluation benchmark (https://gluebenchmark.com/) is a collection of resources for training, evaluating, and analyzing natural language understanding systems.\nSupported Tasks and Leaderboards\nThe leaderboard for the GLUE benchmark can be found at this address. It comprises the following tasks:\nax\nA manually-curated evaluation dataset for fine-grained\u2026 See the full description on the dataset page: https://huggingface.co/datasets/nyu-mll/glue.",
+    "__tags__": {
+        "annotations_creators": "other",
+        "arxiv": "1804.07461",
+        "coreference-nli": true,
+        "croissant": true,
+        "language": "en",
+        "language_creators": "other",
+        "license": "other",
+        "multilinguality": "monolingual",
+        "paraphrase-identification": true,
+        "qa-nli": true,
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "text-classification",
+        "task_ids": [
+            "acceptability-classification",
+            "natural-language-inference",
+            "semantic-similarity-scoring",
+            "sentiment-classification",
+            "text-scoring"
+        ]
+    },
     "loader": {
-        "name": "claim_stance_topic",
-        "path": "ibm/claim_stance",
+        "name": "qqp",
+        "path": "glue",
         "type": "load_hf"
     },
     "preprocess_steps": [
+        "splitters.large_no_test",
+        {
+            "mappers": {
+                "label": {
+                    "0": "not duplicated",
+                    "1": "duplicated"
+                }
+            },
+            "type": "map_instance_values"
+        },
         {
             "fields": {
-                "classes": [
-                    "advertising",
-                    "all nations a right to nuclear weapons",
-                    "a mandatory retirement age",
-                    "american jobs act",
-                    "asean",
-                    "atheism",
-                    "austerity measures",
-                    "barrier methods of contraception",
-                    "blasphemy",
-                    "boxing",
-                    "bribery",
-                    "burning the stars and stripes",
-                    "children",
-                    "collective bargaining rights claimed by trades unions",
-                    "congressional earmarks",
-                    "democratic governments should require voters to present photo identification at the polling station",
-                    "democratization",
-                    "endangered species",
-                    "enforce term limits on the legislative branch of government",
-                    "freedom of speech",
-                    "fund education using a voucher scheme",
-                    "gambling",
-                    "governments should choose open source software",
-                    "high rises for housing",
-                    "holocaust denial",
-                    "housewives should be paid for their work",
-                    "hydroelectric dams",
-                    "implement playoffs in collegiate level american football",
-                    "intellectual property rights",
-                    "israel's 2008-2009 military operations against gaza",
-                    "leaking of military documents",
-                    "multiculturalism",
-                    "national service",
-                    "only teach abstinence for sex education in schools",
-                    "open primaries",
-                    "partial birth abortions",
-                    "physical education",
-                    "poor communities",
-                    "raising the school leaving age to 18",
-                    "re-engage with myanmar",
-                    "the blockade of gaza",
-                    "the creation of private universities in the uk",
-                    "the free market",
-                    "the growing of tobacco",
-                    "the keystone xl pipeline",
-                    "the monarchy",
-                    "the one-child policy of the republic of china",
-                    "the right to asylum",
-                    "the right to bear arms",
-                    "the sale of violent video games to minors",
-                    "the use of affirmative action",
-                    "the use of performance enhancing drugs in professional sports",
-                    "the use of truth and reconciliation commissions",
-                    "wind power",
-                    "year round schooling"
-                ],
-                "text_type": "argument",
-                "type_of_class": "topic"
+                "choices": [
+                    "not duplicated",
+                    "duplicated"
+                ]
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.classification.multi_class",
-    "templates": "templates.classification.multi_class.all",
+    "task": {
+        "inputs": [
+            "choices",
+            "question1",
+            "question2"
+        ],
+        "metrics": [
+            "metrics.accuracy"
+        ],
+        "outputs": [
+            "label"
+        ],
+        "type": "task"
+    },
+    "templates": {
+        "items": [
+            {
+                "input_format": "Given this question: {question1}, classify if this question: {question2} is {choices}.",
+                "output_format": "{label}",
+                "type": "input_output_template"
+            }
+        ],
+        "type": "templates_list"
+    },
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/clinc_oos/imbalanced.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/clinc_oos/plus.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7023809523809524%*

 * *Differences: {"'__description__'": '"Dataset Card for CLINC150\\nDataset Summary\\nTask-oriented dialog systems '*

 * *                      'need to know when a query falls outside their range of supported intents, '*

 * *                      'but current text classification corpora only define label sets that cover '*

 * *                      'every example. We introduce a new dataset that includes queries that are '*

 * *                      "out-of-scope (OOS), i.e., queries that do not fall into any of the system's "*

 * *               […]*

```diff
@@ -1,10 +1,24 @@
 {
+    "__description__": "Dataset Card for CLINC150\nDataset Summary\nTask-oriented dialog systems need to know when a query falls outside their range of supported intents, but current text classification corpora only define label sets that cover every example. We introduce a new dataset that includes queries that are out-of-scope (OOS), i.e., queries that do not fall into any of the system's supported intents. This poses a new challenge because models cannot assume that every query at\u2026 See the full description on the dataset page: https://huggingface.co/datasets/clinc_oos.",
+    "__tags__": {
+        "annotations_creators": "expert-generated",
+        "croissant": true,
+        "language": "en",
+        "language_creators": "crowdsourced",
+        "license": "cc-by-3.0",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "text-classification",
+        "task_ids": "intent-classification"
+    },
     "loader": {
-        "name": "imbalanced",
+        "name": "plus",
         "path": "clinc_oos",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "page_size": 9223372036854775807,
             "type": "shuffle"
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/clinc_oos/plus.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/clinc_oos/small.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7023809523809524%*

 * *Differences: {"'__description__'": '"Dataset Card for CLINC150\\nDataset Summary\\nTask-oriented dialog systems '*

 * *                      'need to know when a query falls outside their range of supported intents, '*

 * *                      'but current text classification corpora only define label sets that cover '*

 * *                      'every example. We introduce a new dataset that includes queries that are '*

 * *                      "out-of-scope (OOS), i.e., queries that do not fall into any of the system's "*

 * *               […]*

```diff
@@ -1,10 +1,24 @@
 {
+    "__description__": "Dataset Card for CLINC150\nDataset Summary\nTask-oriented dialog systems need to know when a query falls outside their range of supported intents, but current text classification corpora only define label sets that cover every example. We introduce a new dataset that includes queries that are out-of-scope (OOS), i.e., queries that do not fall into any of the system's supported intents. This poses a new challenge because models cannot assume that every query at\u2026 See the full description on the dataset page: https://huggingface.co/datasets/clinc_oos.",
+    "__tags__": {
+        "annotations_creators": "expert-generated",
+        "croissant": true,
+        "language": "en",
+        "language_creators": "crowdsourced",
+        "license": "cc-by-3.0",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "text-classification",
+        "task_ids": "intent-classification"
+    },
     "loader": {
-        "name": "plus",
+        "name": "small",
         "path": "clinc_oos",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "page_size": 9223372036854775807,
             "type": "shuffle"
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/clinc_oos/small.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/clinc_oos/imbalanced.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7023809523809524%*

 * *Differences: {"'__description__'": '"Dataset Card for CLINC150\\nDataset Summary\\nTask-oriented dialog systems '*

 * *                      'need to know when a query falls outside their range of supported intents, '*

 * *                      'but current text classification corpora only define label sets that cover '*

 * *                      'every example. We introduce a new dataset that includes queries that are '*

 * *                      "out-of-scope (OOS), i.e., queries that do not fall into any of the system's "*

 * *               […]*

```diff
@@ -1,10 +1,24 @@
 {
+    "__description__": "Dataset Card for CLINC150\nDataset Summary\nTask-oriented dialog systems need to know when a query falls outside their range of supported intents, but current text classification corpora only define label sets that cover every example. We introduce a new dataset that includes queries that are out-of-scope (OOS), i.e., queries that do not fall into any of the system's supported intents. This poses a new challenge because models cannot assume that every query at\u2026 See the full description on the dataset page: https://huggingface.co/datasets/clinc_oos.",
+    "__tags__": {
+        "annotations_creators": "expert-generated",
+        "croissant": true,
+        "language": "en",
+        "language_creators": "crowdsourced",
+        "license": "cc-by-3.0",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "text-classification",
+        "task_ids": "intent-classification"
+    },
     "loader": {
-        "name": "small",
+        "name": "imbalanced",
         "path": "clinc_oos",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "page_size": 9223372036854775807,
             "type": "shuffle"
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/cnn_dailymail.json` & `unitxt-1.9.0/src/unitxt/catalog/metrics/rag/answer_inference.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.16666666666666666%*

 * *Differences: {"'main_score'": "'perplexity'",*

 * * "'metric'": "'metrics.perplexity_nli.t5_nli_mixture'",*

 * * "'preprocess_steps'": "{0: {'type': 'copy_fields', 'field_to_field': [['contexts', "*

 * *                       "'references']]}, 1: {'type': 'copy_fields', 'field_to_field': [['answer', "*

 * *                       "'prediction']], delete: ['fields']}}",*

 * * "'type'": "'metric_pipeline'",*

 * * 'delete': "['loader', 'task', 'templates']"}*

```diff
@@ -1,25 +1,25 @@
 {
-    "loader": {
-        "name": "3.0.0",
-        "path": "cnn_dailymail",
-        "type": "load_hf"
-    },
+    "main_score": "perplexity",
+    "metric": "metrics.perplexity_nli.t5_nli_mixture",
     "preprocess_steps": [
         {
-            "field_to_field": {
-                "article": "document",
-                "highlights": "summary"
-            },
-            "type": "rename_fields"
+            "field_to_field": [
+                [
+                    "contexts",
+                    "references"
+                ]
+            ],
+            "type": "copy_fields"
         },
         {
-            "fields": {
-                "document_type": "article"
-            },
-            "type": "add_fields"
+            "field_to_field": [
+                [
+                    "answer",
+                    "prediction"
+                ]
+            ],
+            "type": "copy_fields"
         }
     ],
-    "task": "tasks.summarization.abstractive",
-    "templates": "templates.summarization.abstractive.all",
-    "type": "task_card"
+    "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/coedit/paraphrase.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/winogrande/debiased.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4739795918367347%*

 * *Differences: {"'__description__'": "'WinoGrande is a new collection of 44k problems, inspired by Winograd "*

 * *                      'Schema Challenge (Levesque, Davis, and Morgenstern\\n2011), but adjusted to '*

 * *                      'improve the scale and robustness against the dataset-specific bias. '*

 * *                      'Formulated as a\\nfill-in-a-blank task with binary options, the goal is to '*

 * *                      'choose the right option for a given sentence which requires\\ncommonsense '*

 * *                      "r […]*

```diff
@@ -1,42 +1,44 @@
 {
+    "__description__": "WinoGrande is a new collection of 44k problems, inspired by Winograd Schema Challenge (Levesque, Davis, and Morgenstern\n2011), but adjusted to improve the scale and robustness against the dataset-specific bias. Formulated as a\nfill-in-a-blank task with binary options, the goal is to choose the right option for a given sentence which requires\ncommonsense reasoning.",
+    "__tags__": {
+        "croissant": true,
+        "language": "en",
+        "region": "us"
+    },
     "loader": {
-        "filtering_lambda": "lambda x: x['task'] == 'paraphrase'",
-        "path": "grammarly/coedit",
-        "streaming": true,
+        "name": "winogrande_debiased",
+        "path": "winogrande",
         "type": "load_hf"
     },
     "preprocess_steps": [
         "splitters.small_no_test",
         {
-            "by": ": ",
-            "field": "src",
-            "type": "split"
-        },
-        {
-            "field": "src",
-            "start": 1,
-            "type": "slice"
-        },
-        {
-            "by": ": ",
-            "field": "src",
-            "type": "join"
+            "fields": [
+                "option1",
+                "option2"
+            ],
+            "to_field": "choices",
+            "type": "list_field_values"
         },
         {
             "fields": {
-                "text_type": "sentence"
+                "answer": "int"
             },
-            "type": "add_fields"
+            "type": "cast_fields"
+        },
+        {
+            "add": -1,
+            "field": "answer",
+            "type": "add_constant"
         },
         {
             "field_to_field": {
-                "src": "input_text",
-                "tgt": "output_text"
+                "sentence": "question"
             },
             "type": "rename_fields"
         }
     ],
-    "task": "tasks.rewriting.paraphrase",
-    "templates": "templates.rewriting.paraphrase.all",
+    "task": "tasks.qa.multiple_choice.open",
+    "templates": "templates.qa.multiple_choice.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/coedit/preference.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/ffqa_filtered/4k.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.47891865079365076%*

 * *Differences: {"'__description__'": '\'Dataset Card for "WikiQA-Free_Form_QA"\\nThe WikiQA task is the task of '*

 * *                      'answering a question based on the information given in a Wikipedia '*

 * *                      'document. We have built upon the short answer format data in Google Natural '*

 * *                      'Questions to construct our QA task. It is formatted as a document and a '*

 * *                      'question. We ensure the answer to the question is a short answer which is '*

 * *                      'e […]*

```diff
@@ -1,64 +1,68 @@
 {
+    "__description__": "Dataset Card for \"WikiQA-Free_Form_QA\"\nThe WikiQA task is the task of answering a question based on the information given in a Wikipedia document. We have built upon the short answer format data in Google Natural Questions to construct our QA task. It is formatted as a document and a question. We ensure the answer to the question is a short answer which is either a single word or a small sentence directly cut pasted from the document. Having the task structured as such, we can\u2026 See the full description on the dataset page: https://huggingface.co/datasets/abacusai/WikiQA-Free_Form_QA.",
+    "__tags__": {
+        "croissant": true,
+        "region": "us"
+    },
     "loader": {
-        "path": "grammarly/coedit",
-        "streaming": true,
+        "path": "abacusai/WikiQA-Free_Form_QA",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "page_size": 9223372036854775807,
-            "type": "shuffle"
-        },
-        "splitters.small_no_test",
-        {
-            "by": ": ",
-            "field": "src",
-            "type": "split"
-        },
-        {
-            "field": "src",
-            "start": 1,
-            "type": "slice"
-        },
-        {
             "field_to_field": {
-                "src/0": "instruction"
+                "conversations/0/tok_len": "inputs_len",
+                "conversations/0/value": "inputs",
+                "conversations/1/value": "answer"
             },
             "type": "copy_fields"
         },
         {
-            "by": ": ",
-            "field": "src",
-            "type": "join"
-        },
-        {
             "fields": [
-                "tgt",
-                "src"
+                "answer"
             ],
-            "to_field": "choices",
+            "to_field": "answers",
             "type": "list_field_values"
         },
         {
-            "field": "choices",
-            "type": "shuffle_field_values"
+            "condition": "lt",
+            "type": "filter_by_condition",
+            "values": {
+                "inputs_len": 4096
+            }
+        },
+        {
+            "expression": "re.search(r\"Document:\\s(.*)(\\n\\n|$)\", inputs).group(1)",
+            "imports_list": [
+                "re"
+            ],
+            "to_field": "context",
+            "type": "execute_expression"
+        },
+        {
+            "expression": "re.search(r\"Question:\\s(.*)(\\n\\n|$)\", inputs).group(1)",
+            "imports_list": [
+                "re"
+            ],
+            "to_field": "question",
+            "type": "execute_expression"
         },
         {
             "fields": {
-                "input_type": "sentence",
-                "output_type": "sentence"
+                "context_type": "document"
             },
             "type": "add_fields"
         },
         {
-            "field_to_field": {
-                "src": "input",
-                "tgt": "output_choice"
+            "mix": {
+                "test": "4k[10%]",
+                "train": "4k[80%]",
+                "validation": "4k[10%]"
             },
-            "type": "rename_fields"
+            "type": "split_random_mix"
         }
     ],
-    "task": "tasks.evaluation.preference",
-    "templates": "templates.evaluation.preference.all",
+    "task": "tasks.qa.with_context.extractive",
+    "templates": "templates.qa.with_context.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/coedit/rewriting.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/wsc.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4662337662337662%*

 * *Differences: {"'__description__'": "'SuperGLUE (https://super.gluebenchmark.com/) is a new benchmark styled "*

 * *                      'after\\nGLUE with a new set of more difficult language understanding tasks, '*

 * *                      "improved\\nresources, and a new public leaderboard.'",*

 * * "'__tags__'": "OrderedDict([('NLU', True), ('annotations_creators', 'expert-generated'), "*

 * *               "('arxiv', '1905.00537'), ('croissant', True), ('language', 'en'), "*

 * *               "('language_creators', 'other'), ('license',  […]*

```diff
@@ -1,81 +1,81 @@
 {
+    "__description__": "SuperGLUE (https://super.gluebenchmark.com/) is a new benchmark styled after\nGLUE with a new set of more difficult language understanding tasks, improved\nresources, and a new public leaderboard.",
+    "__tags__": {
+        "NLU": true,
+        "annotations_creators": "expert-generated",
+        "arxiv": "1905.00537",
+        "croissant": true,
+        "language": "en",
+        "language_creators": "other",
+        "license": "other",
+        "multilinguality": "monolingual",
+        "natural language understanding": true,
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "extended|other",
+        "superglue": true,
+        "task_categories": [
+            "text-classification",
+            "token-classification",
+            "question-answering"
+        ],
+        "task_ids": [
+            "natural-language-inference",
+            "word-sense-disambiguation",
+            "coreference-resolution",
+            "extractive-qa"
+        ]
+    },
     "loader": {
-        "filtering_lambda": "lambda x: x['task'] in ['gec', 'simplification', 'coherence', 'neutralize']",
-        "path": "grammarly/coedit",
-        "streaming": true,
+        "name": "wsc",
+        "path": "super_glue",
         "type": "load_hf"
     },
     "preprocess_steps": [
-        {
-            "page_size": 9223372036854775807,
-            "type": "shuffle"
-        },
         "splitters.small_no_test",
         {
-            "by": ": ",
-            "field": "src",
-            "type": "split"
-        },
-        {
-            "field": "src",
-            "start": 1,
-            "type": "slice"
-        },
-        {
-            "by": ": ",
-            "field": "src",
-            "type": "join"
-        },
-        {
-            "field_to_field": {
-                "task": "required_attribute"
-            },
-            "type": "copy_fields"
-        },
-        {
-            "mappers": {
-                "required_attribute": {
-                    "coherence": "coherent",
-                    "gec": "grammatically correct",
-                    "neutralize": "neutral",
-                    "simplification": "simple"
-                }
-            },
-            "type": "map_instance_values"
-        },
-        {
-            "field_to_field": {
-                "task": "attribute_type"
-            },
-            "type": "copy_fields"
-        },
-        {
             "mappers": {
-                "attribute_type": {
-                    "coherence": "coherence",
-                    "gec": "gramaticity",
-                    "neutralize": "neutrality",
-                    "simplification": "simplicity"
+                "label": {
+                    "0": "False",
+                    "1": "True"
                 }
             },
             "type": "map_instance_values"
         },
         {
             "fields": {
-                "input_text_type": "sentence",
-                "output_text_type": "sentence"
+                "choices": [
+                    "False",
+                    "True"
+                ]
             },
             "type": "add_fields"
-        },
-        {
-            "field_to_field": {
-                "src": "input_text",
-                "tgt": "output_text"
-            },
-            "type": "rename_fields"
         }
     ],
-    "task": "tasks.rewriting.by_attribute",
-    "templates": "templates.rewriting.by_attribute.all",
+    "task": {
+        "inputs": [
+            "choices",
+            "text",
+            "span1_text",
+            "span2_text"
+        ],
+        "metrics": [
+            "metrics.accuracy"
+        ],
+        "outputs": [
+            "label"
+        ],
+        "type": "task"
+    },
+    "templates": {
+        "items": [
+            {
+                "input_format": "Given this sentence: {text} classify if \"{span2_text}\" refers to \"{span1_text}\".",
+                "output_format": "{label}",
+                "type": "input_output_template"
+            }
+        ],
+        "type": "templates_list"
+    },
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/coedit/selection.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/boolq/multiple_choice.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.47184065934065933%*

 * *Differences: {"'__description__'": "'Dataset Card for Boolq\\nDataset Summary\\nBoolQ is a question answering "*

 * *                      'dataset for yes/no questions containing 15942 examples. These questions are '*

 * *                      'naturally\\noccurring ---they are generated in unprompted and unconstrained '*

 * *                      'settings.\\nEach example is a triplet of (question, passage, answer), with '*

 * *                      'the title of the page as optional additional context.\\nThe text-pair '*

 * *                 […]*

```diff
@@ -1,91 +1,58 @@
 {
+    "__description__": "Dataset Card for Boolq\nDataset Summary\nBoolQ is a question answering dataset for yes/no questions containing 15942 examples. These questions are naturally\noccurring ---they are generated in unprompted and unconstrained settings.\nEach example is a triplet of (question, passage, answer), with the title of the page as optional additional context.\nThe text-pair classification setup is similar to existing natural language inference tasks.\nSupported Tasks\u2026 See the full description on the dataset page: https://huggingface.co/datasets/google/boolq.",
+    "__tags__": {
+        "annotations_creators": "crowdsourced",
+        "arxiv": "1905.10044",
+        "croissant": true,
+        "language": "en",
+        "language_creators": "found",
+        "license": "cc-by-sa-3.0",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "text-classification",
+        "task_ids": "natural-language-inference"
+    },
     "loader": {
-        "filtering_lambda": "lambda x: x['task'] in ['gec', 'simplification', 'coherence', 'neutralize']",
-        "path": "grammarly/coedit",
-        "streaming": true,
+        "path": "google/boolq",
         "type": "load_hf"
     },
     "preprocess_steps": [
-        {
-            "page_size": 9223372036854775807,
-            "type": "shuffle"
-        },
         "splitters.small_no_test",
         {
-            "by": ": ",
-            "field": "src",
-            "type": "split"
-        },
-        {
-            "field": "src",
-            "start": 1,
-            "type": "slice"
-        },
-        {
-            "by": ": ",
-            "field": "src",
-            "type": "join"
-        },
-        {
-            "fields": [
-                "tgt",
-                "src"
-            ],
-            "to_field": "choices_texts",
-            "type": "list_field_values"
-        },
-        {
-            "field": "choices_texts",
-            "type": "shuffle_field_values"
-        },
-        {
-            "field_to_field": {
-                "task": "required_attribute"
-            },
-            "type": "copy_fields"
-        },
-        {
-            "mappers": {
-                "required_attribute": {
-                    "coherence": "coherent",
-                    "gec": "grammatically correct",
-                    "neutralize": "neutral",
-                    "simplification": "simple"
-                }
+            "fields": {
+                "choices": [
+                    "yes",
+                    "no"
+                ],
+                "context_type": "passage"
             },
-            "type": "map_instance_values"
+            "type": "add_fields"
         },
         {
-            "field_to_field": {
-                "task": "attribute_type"
+            "fields": {
+                "answer": "str"
             },
-            "type": "copy_fields"
+            "type": "cast_fields"
         },
         {
             "mappers": {
-                "attribute_type": {
-                    "coherence": "coherence",
-                    "gec": "gramaticity",
-                    "neutralize": "neutrality",
-                    "simplification": "simplicity"
+                "answer": {
+                    "False": "no",
+                    "True": "yes"
                 }
             },
             "type": "map_instance_values"
         },
         {
-            "fields": {
-                "choices_text_type": "sentences"
-            },
-            "type": "add_fields"
-        },
-        {
             "field_to_field": {
-                "tgt": "choice"
+                "passage": "context"
             },
             "type": "rename_fields"
         }
     ],
-    "task": "tasks.selection.by_attribute",
-    "templates": "templates.selection.by_attribute.all",
+    "task": "tasks.qa.multiple_choice.with_context",
+    "templates": "templates.qa.multiple_choice.with_context.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/coedit_error_detection.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/coedit_error_detection.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7142857142857143%*

 * *Differences: {"'__description__'": "'Dataset Card for CoEdIT: Text Editing via Instruction Tuning\\nPaper: "*

 * *                      'CoEdIT: Text Editing by Task-Specific Instruction Tuning\\nAuthors: Vipul '*

 * *                      'Raheja, Dhruv Kumar, Ryan Koo, Dongyeop Kang\\nProject Repo: '*

 * *                      'https://github.com/vipulraheja/coedit\\nDataset Summary\\nThis is the '*

 * *                      'dataset that was used to train the CoEdIT text editing models. Full details '*

 * *                      'of the datas […]*

```diff
@@ -1,8 +1,18 @@
 {
+    "__description__": "Dataset Card for CoEdIT: Text Editing via Instruction Tuning\nPaper: CoEdIT: Text Editing by Task-Specific Instruction Tuning\nAuthors: Vipul Raheja, Dhruv Kumar, Ryan Koo, Dongyeop Kang\nProject Repo: https://github.com/vipulraheja/coedit\nDataset Summary\nThis is the dataset that was used to train the CoEdIT text editing models. Full details of the dataset can be found in our paper.\nDataset Structure\nThe\u2026 See the full description on the dataset page: https://huggingface.co/datasets/grammarly/coedit.",
+    "__tags__": {
+        "arxiv": "2305.09857",
+        "croissant": true,
+        "language": "en",
+        "license": "apache-2.0",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "task_categories": "text-generation"
+    },
     "loader": {
         "filtering_lambda": "lambda x: x['task'] == 'gec'",
         "path": "grammarly/coedit",
         "streaming": true,
         "type": "load_hf"
     },
     "preprocess_steps": [
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/coedit_gec.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/wmt/en_de.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.663888888888889%*

 * *Differences: {"'loader'": "{'path': 'wmt16', 'name': 'de-en', delete: ['filtering_lambda']}",*

 * * "'preprocess_steps'": "{0: {'type': 'copy_fields', 'field_to_field': [['translation/en', 'text'], "*

 * *                       "['translation/de', 'translation']]}, 1: {'type': 'add_fields', 'fields': "*

 * *                       "{replace: OrderedDict([('source_language', 'english'), ('target_language', "*

 * *                       "'deutch')])}, delete: ['to_field']}, delete: [3, 2, 1, 0]}",*

 * * "'task'": "'tasks.translation.directed'",*

 * * " […]*

```diff
@@ -1,42 +1,33 @@
 {
     "loader": {
-        "filtering_lambda": "lambda x: x['task'] == 'gec'",
-        "path": "grammarly/coedit",
+        "name": "de-en",
+        "path": "wmt16",
         "streaming": true,
         "type": "load_hf"
     },
     "preprocess_steps": [
-        "splitters.small_no_test",
         {
-            "by": ": ",
-            "field": "src",
-            "type": "split"
-        },
-        {
-            "field": "src",
-            "start": 1,
-            "type": "slice"
-        },
-        {
-            "by": ": ",
-            "field": "src",
-            "type": "join"
+            "field_to_field": [
+                [
+                    "translation/en",
+                    "text"
+                ],
+                [
+                    "translation/de",
+                    "translation"
+                ]
+            ],
+            "type": "copy_fields"
         },
         {
-            "field_to_field": {
-                "src": "original_text"
+            "fields": {
+                "source_language": "english",
+                "target_language": "deutch"
             },
-            "type": "rename_fields"
-        },
-        {
-            "fields": [
-                "tgt"
-            ],
-            "to_field": "corrected_texts",
-            "type": "list_field_values"
+            "type": "add_fields"
         }
     ],
-    "task": "tasks.grammatical_error_correction",
-    "templates": "templates.grammatical_error_correction.all",
+    "task": "tasks.translation.directed",
+    "templates": "templates.translation.directed.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/cohere_for_ai/aya_human_annotated/arb.json` & `unitxt-1.9.0/src/unitxt/catalog/metrics/normalized_sacrebleu.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.15119047619047618%*

 * *Differences: {"'main_score'": "'sacrebleu'",*

 * * "'metric'": "OrderedDict([('type', 'normalized_sacrebleu')])",*

 * * "'preprocess_steps'": "{0: {'type': 'copy_fields', 'field_to_field': "*

 * *                       "[['task_data/target_language', 'task_data/tokenize']], 'not_exist_ok': "*

 * *                       "True, 'get_default': 'en'}, 1: {'type': 'map_instance_values', 'mappers': "*

 * *                       "OrderedDict([('task_data/tokenize', OrderedDict([('deutch', None), "*

 * *                       "('french', None), ('romanian', […]*

```diff
@@ -1,36 +1,48 @@
 {
-    "loader": {
-        "filtering_lambda": "lambda instance: instance[\"language\"]==\"arb\"",
-        "name": "aya_human_annotated",
-        "path": "CohereForAI/aya_evaluation_suite",
-        "streaming": true,
-        "type": "load_hf"
+    "main_score": "sacrebleu",
+    "metric": {
+        "type": "normalized_sacrebleu"
     },
     "preprocess_steps": [
         {
-            "mix": {
-                "test": "test[5%]",
-                "train": "test[90%]",
-                "validation": "test[5%]"
-            },
-            "type": "split_random_mix"
+            "field_to_field": [
+                [
+                    "task_data/target_language",
+                    "task_data/tokenize"
+                ]
+            ],
+            "get_default": "en",
+            "not_exist_ok": true,
+            "type": "copy_fields"
         },
         {
-            "field_to_field": {
-                "inputs": "question",
-                "targets": "answers"
+            "mappers": {
+                "task_data/tokenize": {
+                    "Arabic": "intl",
+                    "French": null,
+                    "German": null,
+                    "Japanese": "ja-mecab",
+                    "Korean": "ko-mecab",
+                    "Portuguese": null,
+                    "Spanish": null,
+                    "ar": "intl",
+                    "de": null,
+                    "deutch": null,
+                    "en": null,
+                    "english": null,
+                    "es": null,
+                    "fr": null,
+                    "french": null,
+                    "ja": "ja-mecab",
+                    "japanese": "ja-mecab",
+                    "ko": "ko-mecab",
+                    "pt": null,
+                    "romanian": null
+                }
             },
-            "type": "rename_fields"
-        },
-        {
-            "fields": [
-                "answers"
-            ],
-            "to_field": "answers",
-            "type": "list_field_values"
+            "strict": true,
+            "type": "map_instance_values"
         }
     ],
-    "task": "tasks.qa.open[metrics=[metrics.rag.correctness.llama_index_by_gpt_3_5_turbo]]",
-    "templates": "templates.qa.open.all",
-    "type": "task_card"
+    "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/fra.json` & `unitxt-1.9.0/src/unitxt/catalog/metrics/token_overlap_with_context.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.14930555555555555%*

 * *Differences: {"'main_score'": "'score'",*

 * * "'metric'": "OrderedDict([('type', 'token_overlap')])",*

 * * "'postpreprocess_steps'": "[OrderedDict([('type', 'copy_fields'), ('field_to_field', "*

 * *                           "[['score/global/f1', 'score/global/f1_overlap_with_context'], "*

 * *                           "['score/global/recall', 'score/global/recall_overlap_with_context'], "*

 * *                           "['score/global/precision', "*

 * *                           "'score/global/precision_overlap_with_context']])])]",*

 * * "'prepro […]*

```diff
@@ -1,36 +1,44 @@
 {
-    "loader": {
-        "filtering_lambda": "lambda instance: instance[\"language\"]==\"fra\"",
-        "name": "dolly_human_edited",
-        "path": "CohereForAI/aya_evaluation_suite",
-        "streaming": true,
-        "type": "load_hf"
+    "main_score": "score",
+    "metric": {
+        "type": "token_overlap"
     },
-    "preprocess_steps": [
+    "postpreprocess_steps": [
         {
-            "mix": {
-                "test": "test[5%]",
-                "train": "test[90%]",
-                "validation": "test[5%]"
-            },
-            "type": "split_random_mix"
-        },
+            "field_to_field": [
+                [
+                    "score/global/f1",
+                    "score/global/f1_overlap_with_context"
+                ],
+                [
+                    "score/global/recall",
+                    "score/global/recall_overlap_with_context"
+                ],
+                [
+                    "score/global/precision",
+                    "score/global/precision_overlap_with_context"
+                ]
+            ],
+            "type": "copy_fields"
+        }
+    ],
+    "preprocess_steps": [
         {
-            "field_to_field": {
-                "inputs": "question",
-                "targets": "answers"
-            },
-            "type": "rename_fields"
+            "field_to_field": [
+                [
+                    "task_data/context",
+                    "references"
+                ]
+            ],
+            "type": "copy_fields"
         },
         {
             "fields": [
-                "answers"
+                "references"
             ],
-            "to_field": "answers",
+            "to_field": "references",
             "type": "list_field_values"
         }
     ],
-    "task": "tasks.qa.open[metrics=[metrics.rag.correctness.llama_index_by_gpt_3_5_turbo]]",
-    "templates": "templates.qa.open.all",
-    "type": "task_card"
+    "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/cohere_for_ai/dolly_human_edited/spa.json` & `unitxt-1.9.0/src/unitxt/catalog/metrics/sacrebleu.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.15119047619047618%*

 * *Differences: {"'main_score'": "'sacrebleu'",*

 * * "'metric'": "OrderedDict([('type', 'huggingface_metric'), ('hf_metric_name', 'sacrebleu'), "*

 * *             "('hf_main_score', 'score'), ('prediction_type', 'str'), ('main_score', 'sacrebleu'), "*

 * *             "('scale', 1.0), ('scaled_fields', ['sacrebleu', 'precisions']), "*

 * *             "('hf_additional_input_fields_pass_one_value', ['tokenize'])])",*

 * * "'preprocess_steps'": "{0: {'type': 'copy_fields', 'field_to_field': "*

 * *                       "[['task_data/target_language',  […]*

```diff
@@ -1,36 +1,42 @@
 {
-    "loader": {
-        "filtering_lambda": "lambda instance: instance[\"language\"]==\"spa\"",
-        "name": "dolly_human_edited",
-        "path": "CohereForAI/aya_evaluation_suite",
-        "streaming": true,
-        "type": "load_hf"
+    "main_score": "sacrebleu",
+    "metric": {
+        "hf_additional_input_fields_pass_one_value": [
+            "tokenize"
+        ],
+        "hf_main_score": "score",
+        "hf_metric_name": "sacrebleu",
+        "main_score": "sacrebleu",
+        "prediction_type": "str",
+        "scale": 1.0,
+        "scaled_fields": [
+            "sacrebleu",
+            "precisions"
+        ],
+        "type": "huggingface_metric"
     },
     "preprocess_steps": [
         {
-            "mix": {
-                "test": "test[5%]",
-                "train": "test[90%]",
-                "validation": "test[5%]"
-            },
-            "type": "split_random_mix"
+            "field_to_field": [
+                [
+                    "task_data/target_language",
+                    "task_data/tokenize"
+                ]
+            ],
+            "get_default": "en",
+            "not_exist_ok": true,
+            "type": "copy_fields"
         },
         {
-            "field_to_field": {
-                "inputs": "question",
-                "targets": "answers"
+            "mappers": {
+                "task_data/tokenize": {
+                    "en": "",
+                    "ja": "ja-mecab"
+                }
             },
-            "type": "rename_fields"
-        },
-        {
-            "fields": [
-                "answers"
-            ],
-            "to_field": "answers",
-            "type": "list_field_values"
+            "strict": true,
+            "type": "map_instance_values"
         }
     ],
-    "task": "tasks.qa.open[metrics=[metrics.rag.correctness.llama_index_by_gpt_3_5_turbo]]",
-    "templates": "templates.qa.open.all",
-    "type": "task_card"
+    "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/deu.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mt_bench/response_assessment/rating/multi_turn_gpt4_judgement.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6416666666666667%*

 * *Differences: {"'loader'": "{'path': 'OfirArviv/mt_bench_single_score_gpt4_judgement', 'split': 'train', delete: "*

 * *             "['name', 'streaming', 'filtering_lambda']}",*

 * * "'preprocess_steps'": "{0: {'type': 'rename_splits', 'mapper': OrderedDict([('train', 'test')]), "*

 * *                       "delete: ['mix']}, 3: {'field_to_field': {replace: OrderedDict([('score', "*

 * *                       "'rating'), ('category', 'group')])}}, 5: {'type': 'literal_eval', "*

 * *                       "'to_field': 'model_output', 'field':  […]*

```diff
@@ -1,36 +1,57 @@
 {
     "loader": {
-        "filtering_lambda": "lambda instance: instance[\"language\"]==\"deu\"",
-        "name": "dolly_machine_translated",
-        "path": "CohereForAI/aya_evaluation_suite",
-        "streaming": true,
+        "path": "OfirArviv/mt_bench_single_score_gpt4_judgement",
+        "split": "train",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mix": {
-                "test": "test[5%]",
-                "train": "test[90%]",
-                "validation": "test[5%]"
+            "mapper": {
+                "train": "test"
             },
-            "type": "split_random_mix"
+            "type": "rename_splits"
+        },
+        {
+            "condition": "eq",
+            "type": "filter_by_condition",
+            "values": {
+                "turn": 2
+            }
+        },
+        {
+            "condition": "eq",
+            "type": "filter_by_condition",
+            "values": {
+                "reference": "[]"
+            }
         },
         {
             "field_to_field": {
-                "inputs": "question",
-                "targets": "answers"
+                "category": "group",
+                "score": "rating"
             },
             "type": "rename_fields"
         },
         {
-            "fields": [
-                "answers"
-            ],
-            "to_field": "answers",
-            "type": "list_field_values"
+            "field": "model_input",
+            "to_field": "model_input",
+            "type": "literal_eval"
+        },
+        {
+            "field": "model_output",
+            "to_field": "model_output",
+            "type": "literal_eval"
+        },
+        {
+            "assistant_turns_field": "model_output",
+            "to_field": "dialog",
+            "type": "interleave_lists_to_dialog_operator",
+            "user_turns_field": "model_input"
         }
     ],
-    "task": "tasks.qa.open[metrics=[metrics.rag.correctness.llama_index_by_gpt_3_5_turbo]]",
-    "templates": "templates.qa.open.all",
+    "task": "tasks.response_assessment.rating.multi_turn",
+    "templates": [
+        "templates.response_assessment.rating.mt_bench_multi_turn"
+    ],
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/cola.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/babi/qa.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4857142857142857%*

 * *Differences: {"'__description__'": "'Creation (Copied & adapted from "*

 * *                      'https://github.com/stanford-crfm/helm/blob/0eaaa62a2263ddb94e9850ee629423b010f57e4a/src/helm/benchmark/scenarios/babi_qa_scenario.py):\\n!wget '*

 * *                      'http://www.thespermwhale.com/jaseweston/babi/tasks_1-20_v1-2.tar.gz\\n!tar '*

 * *                      '-xf tasks_1-20_v1-2.tar.gz\\nimport json\\nfrom typing import List\\ntasks '*

 * *                      '= list(range(1, 20))\\nsplits = ["train", "valid", "test"]\\nde […]*

```diff
@@ -1,39 +1,35 @@
 {
+    "__description__": "Creation (Copied & adapted from https://github.com/stanford-crfm/helm/blob/0eaaa62a2263ddb94e9850ee629423b010f57e4a/src/helm/benchmark/scenarios/babi_qa_scenario.py):\n!wget http://www.thespermwhale.com/jaseweston/babi/tasks_1-20_v1-2.tar.gz\n!tar -xf tasks_1-20_v1-2.tar.gz\nimport json\nfrom typing import List\ntasks = list(range(1, 20))\nsplits = [\"train\", \"valid\", \"test\"]\ndef process_path(path: str) -> str:\n\"\"\"Turn a path string (task 19) from the original format 's,w' to a verbal\u2026 See the full description on the dataset page: https://huggingface.co/datasets/Muennighoff/babi.",
+    "__tags__": {
+        "croissant": true,
+        "region": "us"
+    },
     "loader": {
-        "name": "cola",
-        "path": "glue",
+        "path": "Muennighoff/babi",
         "type": "load_hf"
     },
     "preprocess_steps": [
-        "splitters.small_no_test",
-        {
-            "mappers": {
-                "label": {
-                    "0": "unacceptable",
-                    "1": "acceptable"
-                }
-            },
-            "type": "map_instance_values"
-        },
         {
             "field_to_field": {
-                "sentence": "text"
+                "passage": "context"
             },
             "type": "rename_fields"
         },
         {
             "fields": {
-                "classes": [
-                    "unacceptable",
-                    "acceptable"
-                ],
-                "text_type": "text",
-                "type_of_class": "grammatical acceptability"
+                "context_type": "description"
             },
             "type": "add_fields"
+        },
+        {
+            "fields": [
+                "answer"
+            ],
+            "to_field": "answers",
+            "type": "list_field_values"
         }
     ],
-    "task": "tasks.classification.multi_class[metrics=[metrics.matthews_correlation]]",
-    "templates": "templates.classification.multi_class.all",
+    "task": "tasks.qa.with_context.extractive",
+    "templates": "templates.qa.with_context.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/copa.json` & `unitxt-1.9.0/src/unitxt/catalog/metrics/rag/context_perplexity.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.13333333333333333%*

 * *Differences: {"'main_score'": "'score'",*

 * * "'metric'": "'metrics.perplexity_q.flan_t5_small'",*

 * * "'postpreprocess_steps'": "[OrderedDict([('type', 'copy_fields'), ('field_to_field', "*

 * *                           "[['score/instance/reference_scores', 'score/instance/score']])])]",*

 * * "'preprocess_steps'": "{0: {'type': 'copy_fields', 'field_to_field': [['contexts', "*

 * *                       "'references']]}, 1: {'type': 'copy_fields', 'field_to_field': "*

 * *                       "[['question', 'prediction']], delete: ['fields']} […]*

```diff
@@ -1,43 +1,36 @@
 {
-    "loader": {
-        "name": "copa",
-        "path": "super_glue",
-        "type": "load_hf"
-    },
-    "preprocess_steps": [
-        "splitters.small_no_test",
+    "main_score": "score",
+    "metric": "metrics.perplexity_q.flan_t5_small",
+    "postpreprocess_steps": [
         {
-            "fields": [
-                "choice1",
-                "choice2"
+            "field_to_field": [
+                [
+                    "score/instance/reference_scores",
+                    "score/instance/score"
+                ]
             ],
-            "to_field": "choices",
-            "type": "list_field_values"
-        },
-        {
-            "field_to_field": {
-                "label": "answer",
-                "premise": "context"
-            },
-            "type": "rename_fields"
-        },
+            "type": "copy_fields"
+        }
+    ],
+    "preprocess_steps": [
         {
-            "mappers": {
-                "question": {
-                    "cause": "What was the cause of this?",
-                    "effect": "What happened as a result?"
-                }
-            },
-            "type": "map_instance_values"
+            "field_to_field": [
+                [
+                    "contexts",
+                    "references"
+                ]
+            ],
+            "type": "copy_fields"
         },
         {
-            "fields": {
-                "context_type": "sentence"
-            },
-            "type": "add_fields"
+            "field_to_field": [
+                [
+                    "question",
+                    "prediction"
+                ]
+            ],
+            "type": "copy_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.all",
-    "type": "task_card"
+    "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/coqa/completion.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mt_bench/response_assessment/pairwise_comparison/single_turn_with_reference_gpt4_judgement.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6583333333333333%*

 * *Differences: {"'loader'": "{'path': 'OfirArviv/mt_bench_pairwise_comparison_gpt4_judgments', 'split': 'train'}",*

 * * "'preprocess_steps'": "{5: {'type': 'rename_fields', 'field_to_field': "*

 * *                       "OrderedDict([('model_input', 'question'), ('model_1_output', 'answer_a'), "*

 * *                       "('model_2_output', 'answer_b'), ('reference', 'reference_answer'), "*

 * *                       "('category', 'group')]), delete: ['fields']}, 6: {'type': 'literal_eval', "*

 * *                       "'to_field': 'question […]*

```diff
@@ -1,47 +1,109 @@
 {
     "loader": {
-        "path": "stanfordnlp/coqa",
+        "path": "OfirArviv/mt_bench_pairwise_comparison_gpt4_judgments",
+        "split": "train",
         "type": "load_hf"
     },
     "preprocess_steps": [
-        "splitters.small_no_test",
         {
-            "fields": {
-                "completion_type": "response",
-                "context_type": "dialog"
+            "mapper": {
+                "train": "test"
             },
-            "type": "add_fields"
+            "type": "rename_splits"
         },
         {
-            "fields": [
-                "questions",
-                "answers/input_text"
-            ],
-            "to_field": "dialog",
-            "type": "zip_field_values"
+            "condition": "eq",
+            "type": "filter_by_condition",
+            "values": {
+                "turn": 1
+            }
         },
         {
-            "field": "dialog",
-            "process_every_value": true,
-            "type": "dictify",
-            "with_keys": [
-                "user",
-                "system"
-            ]
+            "condition": "ne",
+            "type": "filter_by_condition",
+            "values": {
+                "reference": "[]"
+            }
         },
         {
-            "field": "dialog",
-            "type": "duplicate_by_sub_lists"
+            "condition": "in",
+            "type": "filter_by_condition",
+            "values": {
+                "winner": [
+                    "model_1",
+                    "tie",
+                    "model_2"
+                ]
+            }
         },
         {
-            "context_field": "story",
-            "field": "dialog",
-            "last_response_to_field": "completion",
-            "to_field": "context",
-            "type": "serialize_dialog"
+            "mappers": {
+                "winner": {
+                    "model_1": "choice_a",
+                    "model_2": "choice_b",
+                    "tie": "tie"
+                }
+            },
+            "type": "map_instance_values"
+        },
+        {
+            "field_to_field": {
+                "category": "group",
+                "model_1_output": "answer_a",
+                "model_2_output": "answer_b",
+                "model_input": "question",
+                "reference": "reference_answer"
+            },
+            "type": "rename_fields"
+        },
+        {
+            "field": "question",
+            "to_field": "question",
+            "type": "literal_eval"
+        },
+        {
+            "field_to_field": {
+                "question/0": "question"
+            },
+            "type": "copy_fields"
+        },
+        {
+            "field": "answer_a",
+            "to_field": "answer_a",
+            "type": "literal_eval"
+        },
+        {
+            "field_to_field": {
+                "answer_a/0": "answer_a"
+            },
+            "type": "copy_fields"
+        },
+        {
+            "field": "answer_b",
+            "to_field": "answer_b",
+            "type": "literal_eval"
+        },
+        {
+            "field_to_field": {
+                "answer_b/0": "answer_b"
+            },
+            "type": "copy_fields"
+        },
+        {
+            "field": "reference_answer",
+            "to_field": "reference_answer",
+            "type": "literal_eval"
+        },
+        {
+            "field_to_field": {
+                "reference_answer/0": "reference_answer"
+            },
+            "type": "copy_fields"
         }
     ],
-    "task": "tasks.completion.abstractive",
-    "templates": "templates.completion.abstractive.all",
+    "task": "tasks.response_assessment.pairwise_comparison.single_turn_with_reference",
+    "templates": [
+        "templates.response_assessment.pairwise_comparison.mt_bench_single_turn_with_reference_with_shuffle"
+    ],
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/coqa/qa.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/multidoc2dial/abstractive.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5617724867724868%*

 * *Differences: {"'__description__'": "'MultiDoc2Dial is a new task and dataset on modeling goal-oriented "*

 * *                      'dialogues grounded in multiple documents. Most previous works treat '*

 * *                      'document-grounded dialogue modeling as a machine reading comprehension task '*

 * *                      'based on a single given document or passage. We aim to address more '*

 * *                      'realistic scenarios where a goal-oriented information-seeking conversation '*

 * *                      "involves m […]*

```diff
@@ -1,64 +1,57 @@
 {
+    "__description__": "MultiDoc2Dial is a new task and dataset on modeling goal-oriented dialogues grounded in multiple documents. Most previous works treat document-grounded dialogue modeling as a machine reading comprehension task based on a single given document or passage. We aim to address more realistic scenarios where a goal-oriented information-seeking conversation involves multiple topics, and hence is grounded on different documents.",
+    "__tags__": {
+        "annotations_creators": "crowdsourced",
+        "arxiv": "2109.12595",
+        "croissant": true,
+        "language": "en",
+        "language_creators": [
+            "crowdsourced",
+            "expert-generated"
+        ],
+        "license": "apache-2.0",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": [
+            "10K<n<100K",
+            "1K<n<10K",
+            "n<1K"
+        ],
+        "source_datasets": "extended|doc2dial",
+        "task_categories": "question-answering",
+        "task_ids": "open-domain-qa"
+    },
     "loader": {
-        "path": "stanfordnlp/coqa",
+        "path": "multidoc2dial",
         "type": "load_hf"
     },
     "preprocess_steps": [
-        "splitters.small_no_test",
         {
-            "fields": {
-                "context_type": "story"
+            "field_to_field": {
+                "answers/text/0": "relevant_context"
             },
-            "type": "add_fields"
+            "type": "rename_fields"
         },
         {
             "fields": [
-                "questions",
-                "answers/input_text"
+                "utterance"
             ],
-            "to_field": "dialog",
-            "type": "zip_field_values"
-        },
-        {
-            "field": "dialog",
-            "process_every_value": true,
-            "type": "dictify",
-            "with_keys": [
-                "user",
-                "system"
-            ]
-        },
-        {
-            "field": "dialog",
-            "type": "duplicate_by_sub_lists"
+            "to_field": "answers",
+            "type": "list_field_values"
         },
         {
-            "field": "dialog",
-            "item": -1,
-            "to_field": "last_turn",
-            "type": "get"
+            "expression": "question.split('[SEP]')[0]",
+            "to_field": "question",
+            "type": "execute_expression"
         },
         {
-            "field_to_field": {
-                "last_turn/system": "answer",
-                "last_turn/user": "question"
+            "fields": {
+                "context_type": "document"
             },
-            "type": "copy_fields"
-        },
-        {
-            "field": "answer",
-            "inside": "list",
-            "to_field": "answers",
-            "type": "wrap"
-        },
-        {
-            "context_field": "story",
-            "field": "dialog",
-            "to_field": "context",
-            "type": "serialize_dialog"
+            "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.with_context.extractive",
+    "task": "tasks.qa.with_context.abstractive",
     "templates": "templates.qa.with_context.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/dbpedia_14.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mt_bench/response_assessment/pairwise_comparison/multi_turn_gpt4_judgement.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6674242424242424%*

 * *Differences: {"'loader'": "{'path': 'OfirArviv/mt_bench_pairwise_comparison_gpt4_judgments', 'split': 'train'}",*

 * * "'preprocess_steps'": "{0: {'type': 'rename_splits', 'mapper': OrderedDict([('train', 'test')]), "*

 * *                       "delete: ['page_size']}, 3: {'type': 'filter_by_condition', 'values': "*

 * *                       "OrderedDict([('winner', ['model_1', 'tie', 'model_2'])]), 'condition': "*

 * *                       "'in', delete: ['mix']}, 4: {'mappers': {replace: OrderedDict([('winner', "*

 * *                      […]*

```diff
@@ -1,73 +1,88 @@
 {
     "loader": {
-        "path": "dbpedia_14",
+        "path": "OfirArviv/mt_bench_pairwise_comparison_gpt4_judgments",
+        "split": "train",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "page_size": 9223372036854775807,
-            "type": "shuffle"
+            "mapper": {
+                "train": "test"
+            },
+            "type": "rename_splits"
         },
         {
-            "mix": {
-                "test": "test",
-                "train": "train[87.5%]",
-                "validation": "train[12.5%]"
-            },
-            "type": "split_random_mix"
+            "condition": "eq",
+            "type": "filter_by_condition",
+            "values": {
+                "turn": 2
+            }
+        },
+        {
+            "condition": "eq",
+            "type": "filter_by_condition",
+            "values": {
+                "reference": "[]"
+            }
+        },
+        {
+            "condition": "in",
+            "type": "filter_by_condition",
+            "values": {
+                "winner": [
+                    "model_1",
+                    "tie",
+                    "model_2"
+                ]
+            }
         },
         {
             "mappers": {
-                "label": {
-                    "0": "Company",
-                    "1": "Educational Institution",
-                    "10": "Plant",
-                    "11": "Album",
-                    "12": "Film",
-                    "13": "Written Work",
-                    "2": "Artist",
-                    "3": "Athlete",
-                    "4": "Office Holder",
-                    "5": "Mean Of Transportation",
-                    "6": "Building",
-                    "7": "Natural Place",
-                    "8": "Village",
-                    "9": "Animal"
+                "winner": {
+                    "model_1": "choice_a",
+                    "model_2": "choice_b",
+                    "tie": "tie"
                 }
             },
             "type": "map_instance_values"
         },
         {
             "field_to_field": {
-                "content": "text"
+                "category": "group"
             },
             "type": "rename_fields"
         },
         {
-            "fields": {
-                "classes": [
-                    "Company",
-                    "Educational Institution",
-                    "Artist",
-                    "Athlete",
-                    "Office Holder",
-                    "Mean Of Transportation",
-                    "Building",
-                    "Natural Place",
-                    "Village",
-                    "Animal",
-                    "Plant",
-                    "Album",
-                    "Film",
-                    "Written Work"
-                ],
-                "text_type": "paragraph",
-                "type_of_class": "topic"
-            },
-            "type": "add_fields"
+            "field": "model_input",
+            "to_field": "model_input",
+            "type": "literal_eval"
+        },
+        {
+            "field": "model_1_output",
+            "to_field": "model_1_output",
+            "type": "literal_eval"
+        },
+        {
+            "field": "model_2_output",
+            "to_field": "model_2_output",
+            "type": "literal_eval"
+        },
+        {
+            "assistant_turns_field": "model_1_output",
+            "to_field": "dialog_a",
+            "type": "interleave_lists_to_dialog_operator",
+            "user_turns_field": "model_input"
+        },
+        {
+            "assistant_turns_field": "model_2_output",
+            "to_field": "dialog_b",
+            "type": "interleave_lists_to_dialog_operator",
+            "user_turns_field": "model_input"
         }
     ],
-    "task": "tasks.classification.multi_class",
-    "templates": "templates.classification.multi_class.all",
+    "task": "tasks.response_assessment.pairwise_comparison.multi_turn",
+    "templates": [
+        "templates.response_assessment.pairwise_comparison.mt_bench_multi_turn_with_shuffle"
+    ],
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/ethos_binary.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/bold.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5286871693121693%*

 * *Differences: {"'__description__'": "'Dataset Card for Bias in Open-ended Language Generation Dataset "*

 * *                      '(BOLD)\\nDataset Description\\nBias in Open-ended Language Generation '*

 * *                      'Dataset (BOLD) is a dataset to evaluate fairness in open-ended language '*

 * *                      'generation in English language. It consists of 23,679 different text '*

 * *                      'generation prompts that allow fairness measurement across five domains: '*

 * *                      'profession, gend […]*

```diff
@@ -1,81 +1,99 @@
 {
+    "__description__": "Dataset Card for Bias in Open-ended Language Generation Dataset (BOLD)\nDataset Description\nBias in Open-ended Language Generation Dataset (BOLD) is a dataset to evaluate fairness in open-ended language generation in English language. It consists of 23,679 different text generation prompts that allow fairness measurement across five domains: profession, gender, race, religious ideologies, and political ideologies.\nSome examples of prompts in BOLD are as follows:\u2026 See the full description on the dataset page: https://huggingface.co/datasets/AlexaAI/bold.",
+    "__tags__": {
+        "arxiv": "2101.11718",
+        "croissant": true,
+        "language": "en",
+        "license": "cc-by-4.0",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "text-generation"
+    },
     "loader": {
-        "name": "binary",
-        "path": "ethos",
+        "path": "AlexaAI/bold",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "page_size": 1000000,
-            "type": "shuffle"
+            "mapper": {
+                "train": "test"
+            },
+            "type": "rename_splits"
         },
         {
-            "mix": {
-                "test": "train[80%]",
-                "train": "train[20%]"
+            "fields": {
+                "input_label": {}
             },
-            "type": "split_random_mix"
+            "type": "add_fields"
         },
         {
-            "mappers": {
-                "label": {
-                    "0": "not hate speech",
-                    "1": "hate speech"
-                }
-            },
-            "type": "map_instance_values"
+            "field_to_field": [
+                [
+                    "prompts/0",
+                    "first_prompt"
+                ]
+            ],
+            "type": "copy_fields"
         },
         {
-            "fields": {
-                "classes": [
-                    "not hate speech",
-                    "hate speech"
-                ],
-                "text_type": "sentence",
-                "type_of_class": "hate speech"
+            "field_to_field": [
+                [
+                    "wikipedia/0",
+                    "first_wiki"
+                ]
+            ],
+            "type": "copy_fields"
+        },
+        {
+            "condition": "in",
+            "type": "filter_by_condition",
+            "values": {
+                "domain": [
+                    "race",
+                    "gender"
+                ]
+            }
+        },
+        {
+            "page_size": 10000,
+            "type": "shuffle"
+        },
+        {
+            "field_to_field": {
+                "category": "input_label/category",
+                "first_prompt": "input_label/input",
+                "first_wiki": "input_label/wiki"
             },
-            "type": "add_fields"
+            "type": "copy_fields"
+        },
+        {
+            "field": "input_label",
+            "type": "dump_json"
         }
     ],
-    "task": "tasks.classification.multi_class",
+    "task": {
+        "inputs": [
+            "first_prompt"
+        ],
+        "metrics": [
+            "metrics.regard"
+        ],
+        "outputs": [
+            "input_label"
+        ],
+        "type": "task"
+    },
     "templates": {
         "items": [
             {
-                "input_format": "Given this {text_type}: {text}. Classify if it contains {type_of_class}. classes: {classes}.",
-                "output_format": "{label}",
-                "postprocessors": [
-                    "processors.take_first_non_empty_line"
-                ],
-                "type": "input_output_template"
-            },
-            {
-                "input_format": "Does the following {text_type} contains {type_of_class}? Answer only by choosing one of the options {classes}. {text_type}: {text}.",
-                "output_format": "{label}",
-                "postprocessors": [
-                    "processors.take_first_non_empty_line"
-                ],
-                "type": "input_output_template"
-            },
-            {
-                "input_format": "Given this {text_type}: {text}. Classify if it contains {type_of_class}. classes: {classes}. I would classify this {text_type} as: ",
-                "output_format": "{label}",
-                "postprocessors": [
-                    "processors.take_first_non_empty_line",
-                    "processors.lower_case_till_punc"
-                ],
-                "type": "input_output_template"
-            },
-            {
-                "input_format": "Given this {text_type}: {text}. Classify if it contains {type_of_class}. classes: {classes}. I would classify this {text_type} as: ",
-                "output_format": "{label}",
-                "postprocessors": [
-                    "processors.take_first_non_empty_line",
-                    "processors.hate_speech_or_not_hate_speech"
-                ],
+                "input_format": "{first_prompt}\n",
+                "output_format": "{input_label}",
                 "type": "input_output_template"
             }
         ],
         "type": "templates_list"
     },
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/ffqa_filtered/16k.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/coedit/paraphrase.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.46644345238095236%*

 * *Differences: {"'__description__'": "'Dataset Card for CoEdIT: Text Editing via Instruction Tuning\\nPaper: "*

 * *                      'CoEdIT: Text Editing by Task-Specific Instruction Tuning\\nAuthors: Vipul '*

 * *                      'Raheja, Dhruv Kumar, Ryan Koo, Dongyeop Kang\\nProject Repo: '*

 * *                      'https://github.com/vipulraheja/coedit\\nDataset Summary\\nThis is the '*

 * *                      'dataset that was used to train the CoEdIT text editing models. Full details '*

 * *                      'of the datas […]*

```diff
@@ -1,63 +1,52 @@
 {
+    "__description__": "Dataset Card for CoEdIT: Text Editing via Instruction Tuning\nPaper: CoEdIT: Text Editing by Task-Specific Instruction Tuning\nAuthors: Vipul Raheja, Dhruv Kumar, Ryan Koo, Dongyeop Kang\nProject Repo: https://github.com/vipulraheja/coedit\nDataset Summary\nThis is the dataset that was used to train the CoEdIT text editing models. Full details of the dataset can be found in our paper.\nDataset Structure\nThe\u2026 See the full description on the dataset page: https://huggingface.co/datasets/grammarly/coedit.",
+    "__tags__": {
+        "arxiv": "2305.09857",
+        "croissant": true,
+        "language": "en",
+        "license": "apache-2.0",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "task_categories": "text-generation"
+    },
     "loader": {
-        "path": "abacusai/WikiQA-Free_Form_QA",
+        "filtering_lambda": "lambda x: x['task'] == 'paraphrase'",
+        "path": "grammarly/coedit",
+        "streaming": true,
         "type": "load_hf"
     },
     "preprocess_steps": [
+        "splitters.small_no_test",
         {
-            "field_to_field": {
-                "conversations/0/tok_len": "inputs_len",
-                "conversations/0/value": "inputs",
-                "conversations/1/value": "answer"
-            },
-            "type": "copy_fields"
-        },
-        {
-            "fields": [
-                "answer"
-            ],
-            "to_field": "answers",
-            "type": "list_field_values"
-        },
-        {
-            "condition": "lt",
-            "type": "filter_by_condition",
-            "values": {
-                "inputs_len": 16384
-            }
+            "by": ": ",
+            "field": "src",
+            "type": "split"
         },
         {
-            "expression": "re.search(r\"Document:\\s(.*)(\\n\\n|$)\", inputs).group(1)",
-            "imports_list": [
-                "re"
-            ],
-            "to_field": "context",
-            "type": "execute_expression"
+            "field": "src",
+            "start": 1,
+            "type": "slice"
         },
         {
-            "expression": "re.search(r\"Question:\\s(.*)(\\n\\n|$)\", inputs).group(1)",
-            "imports_list": [
-                "re"
-            ],
-            "to_field": "question",
-            "type": "execute_expression"
+            "by": ": ",
+            "field": "src",
+            "type": "join"
         },
         {
             "fields": {
-                "context_type": "document"
+                "text_type": "sentence"
             },
             "type": "add_fields"
         },
         {
-            "mix": {
-                "test": "16k[10%]",
-                "train": "16k[80%]",
-                "validation": "16k[10%]"
+            "field_to_field": {
+                "src": "input_text",
+                "tgt": "output_text"
             },
-            "type": "split_random_mix"
+            "type": "rename_fields"
         }
     ],
-    "task": "tasks.qa.with_context.extractive",
-    "templates": "templates.qa.with_context.all",
+    "task": "tasks.rewriting.paraphrase",
+    "templates": "templates.rewriting.paraphrase.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/financial_tweets.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/dbpedia_14.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6780059523809524%*

 * *Differences: {"'__description__'": "'Dataset Card for DBpedia14\\nDataset Summary\\nThe DBpedia ontology "*

 * *                      'classification dataset is constructed by picking 14 non-overlapping '*

 * *                      'classes\\nfrom DBpedia 2014. They are listed in classes.txt. From each of '*

 * *                      'these 14 ontology classes, we\\nrandomly choose 40,000 training samples and '*

 * *                      '5,000 testing samples. Therefore, the total size\\nof the training dataset '*

 * *                      'is […]*

```diff
@@ -1,77 +1,86 @@
 {
+    "__description__": "Dataset Card for DBpedia14\nDataset Summary\nThe DBpedia ontology classification dataset is constructed by picking 14 non-overlapping classes\nfrom DBpedia 2014. They are listed in classes.txt. From each of these 14 ontology classes, we\nrandomly choose 40,000 training samples and 5,000 testing samples. Therefore, the total size\nof the training dataset is 560,000 and testing dataset 70,000.\nThere are 3 columns in the dataset (same for train and test splits)\u2026 See the full description on the dataset page: https://huggingface.co/datasets/fancyzhx/dbpedia_14.",
+    "__tags__": {
+        "annotations_creators": "machine-generated",
+        "arxiv": "1509.01626",
+        "croissant": true,
+        "language": "en",
+        "language_creators": "crowdsourced",
+        "license": "cc-by-sa-3.0",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "100K<n<1M",
+        "source_datasets": "original",
+        "task_categories": "text-classification",
+        "task_ids": "topic-classification"
+    },
     "loader": {
-        "path": "zeroshot/twitter-financial-news-topic",
+        "path": "dbpedia_14",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "page_size": 9223372036854775807,
             "type": "shuffle"
         },
         {
             "mix": {
-                "test": "validation",
-                "train": "train[85%]",
-                "validation": "train[15%]"
+                "test": "test",
+                "train": "train[87.5%]",
+                "validation": "train[12.5%]"
             },
             "type": "split_random_mix"
         },
         {
             "mappers": {
                 "label": {
-                    "0": "analyst update",
-                    "1": "fed and central banks",
-                    "10": "gold, metals and materials",
-                    "11": "initial public offering",
-                    "12": "legal and regulation",
-                    "13": "mergers, acquisitions and investments",
-                    "14": "macro",
-                    "15": "markets",
-                    "16": "politics",
-                    "17": "personnel change",
-                    "18": "stock commentary",
-                    "19": "stock movement",
-                    "2": "company and product news",
-                    "3": "treasuries and corporate debt",
-                    "4": "dividend",
-                    "5": "earnings",
-                    "6": "energy and oil",
-                    "7": "financials",
-                    "8": "currencies",
-                    "9": "general News and opinion"
+                    "0": "Company",
+                    "1": "Educational Institution",
+                    "10": "Plant",
+                    "11": "Album",
+                    "12": "Film",
+                    "13": "Written Work",
+                    "2": "Artist",
+                    "3": "Athlete",
+                    "4": "Office Holder",
+                    "5": "Mean Of Transportation",
+                    "6": "Building",
+                    "7": "Natural Place",
+                    "8": "Village",
+                    "9": "Animal"
                 }
             },
             "type": "map_instance_values"
         },
         {
+            "field_to_field": {
+                "content": "text"
+            },
+            "type": "rename_fields"
+        },
+        {
             "fields": {
                 "classes": [
-                    "analyst update",
-                    "fed and central banks",
-                    "company and product news",
-                    "treasuries and corporate debt",
-                    "dividend",
-                    "earnings",
-                    "energy and oil",
-                    "financials",
-                    "currencies",
-                    "general News and opinion",
-                    "gold, metals and materials",
-                    "initial public offering",
-                    "legal and regulation",
-                    "mergers, acquisitions and investments",
-                    "macro",
-                    "markets",
-                    "politics",
-                    "personnel change",
-                    "stock commentary",
-                    "stock movement"
+                    "Company",
+                    "Educational Institution",
+                    "Artist",
+                    "Athlete",
+                    "Office Holder",
+                    "Mean Of Transportation",
+                    "Building",
+                    "Natural Place",
+                    "Village",
+                    "Animal",
+                    "Plant",
+                    "Album",
+                    "Film",
+                    "Written Work"
                 ],
-                "text_type": "tweet",
+                "text_type": "paragraph",
                 "type_of_class": "topic"
             },
             "type": "add_fields"
         }
     ],
     "task": "tasks.classification.multi_class",
     "templates": "templates.classification.multi_class.all",
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/head_qa/es.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/wmt/en_fr.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7125%*

 * *Differences: {"'loader'": "{'path': 'wmt14', 'name': 'fr-en', 'streaming': True}",*

 * * "'preprocess_steps'": "{0: {'type': 'copy_fields', 'field_to_field': [['translation/en', 'text'], "*

 * *                       "['translation/fr', 'translation']]}, 1: {'fields': {replace: "*

 * *                       "OrderedDict([('source_language', 'english'), ('target_language', "*

 * *                       "'french')])}}}",*

 * * "'task'": "'tasks.translation.directed'",*

 * * "'templates'": "'templates.translation.directed.all'"}*

```diff
@@ -1,34 +1,33 @@
 {
     "loader": {
-        "name": "es",
-        "path": "head_qa",
+        "name": "fr-en",
+        "path": "wmt14",
+        "streaming": true,
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "field_to_field": {
-                "category": "label",
-                "qtext": "text"
-            },
-            "type": "rename_fields"
+            "field_to_field": [
+                [
+                    "translation/en",
+                    "text"
+                ],
+                [
+                    "translation/fr",
+                    "translation"
+                ]
+            ],
+            "type": "copy_fields"
         },
         {
             "fields": {
-                "classes": [
-                    "biology",
-                    "chemistry",
-                    "medicine",
-                    "nursery",
-                    "pharmacology",
-                    "psychology"
-                ],
-                "text_type": "question",
-                "type_of_class": "topic"
+                "source_language": "english",
+                "target_language": "french"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.classification.multi_class",
-    "templates": "templates.classification.multi_class.all",
+    "task": "tasks.translation.directed",
+    "templates": "templates.translation.directed.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/hh_rlhf.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/sst2.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.47087585034013607%*

 * *Differences: {"'__description__'": "'Dataset Card for GLUE\\nDataset Summary\\nGLUE, the General Language "*

 * *                      'Understanding Evaluation benchmark (https://gluebenchmark.com/) is a '*

 * *                      'collection of resources for training, evaluating, and analyzing natural '*

 * *                      'language understanding systems.\\nSupported Tasks and Leaderboards\\nThe '*

 * *                      'leaderboard for the GLUE benchmark can be found at this address. It '*

 * *                      'comprises th […]*

```diff
@@ -1,75 +1,64 @@
 {
+    "__description__": "Dataset Card for GLUE\nDataset Summary\nGLUE, the General Language Understanding Evaluation benchmark (https://gluebenchmark.com/) is a collection of resources for training, evaluating, and analyzing natural language understanding systems.\nSupported Tasks and Leaderboards\nThe leaderboard for the GLUE benchmark can be found at this address. It comprises the following tasks:\nax\nA manually-curated evaluation dataset for fine-grained\u2026 See the full description on the dataset page: https://huggingface.co/datasets/nyu-mll/glue.",
+    "__tags__": {
+        "annotations_creators": "other",
+        "arxiv": "1804.07461",
+        "coreference-nli": true,
+        "croissant": true,
+        "language": "en",
+        "language_creators": "other",
+        "license": "other",
+        "multilinguality": "monolingual",
+        "paraphrase-identification": true,
+        "qa-nli": true,
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "text-classification",
+        "task_ids": [
+            "acceptability-classification",
+            "natural-language-inference",
+            "semantic-similarity-scoring",
+            "sentiment-classification",
+            "text-scoring"
+        ]
+    },
     "loader": {
-        "path": "Anthropic/hh-rlhf",
+        "name": "sst2",
+        "path": "glue",
         "type": "load_hf"
     },
     "preprocess_steps": [
-        "splitters.small_no_dev",
-        {
-            "field": "chosen",
-            "type": "strip"
-        },
-        {
-            "field": "chosen",
-            "new": "\n",
-            "old": "\n\n",
-            "type": "replace"
-        },
-        {
-            "by": "\nAssistant:",
-            "field": "chosen",
-            "type": "split"
-        },
-        {
-            "field": "chosen",
-            "item": -1,
-            "to_field": "output_choice",
-            "type": "get"
-        },
-        {
-            "field": "chosen",
-            "stop": -1,
-            "type": "slice"
-        },
-        {
-            "by": "\nAssistant:",
-            "field": "chosen",
-            "to_field": "input",
-            "type": "join"
-        },
-        {
-            "by": "\nAssistant:",
-            "field": "rejected",
-            "type": "split"
-        },
+        "splitters.small_no_test",
         {
-            "field": "rejected",
-            "item": -1,
-            "to_field": "output_rejected",
-            "type": "get"
-        },
-        {
-            "fields": [
-                "output_choice",
-                "output_rejected"
-            ],
-            "to_field": "choices",
-            "type": "list_field_values"
+            "mappers": {
+                "label": {
+                    "0": "negative",
+                    "1": "positive"
+                }
+            },
+            "type": "map_instance_values"
         },
         {
-            "field": "choices",
-            "type": "shuffle_field_values"
+            "field": "sentence",
+            "to_field": "text",
+            "type": "rename_fields"
         },
         {
             "fields": {
-                "input_type": "dialog",
-                "instruction": "Respond the following dialog in an helpful and harmfull way.",
-                "output_type": "response"
+                "text_type": "sentence",
+                "type_of_class": "sentiment"
             },
             "type": "add_fields"
+        },
+        {
+            "field": "label",
+            "stream_name": "train",
+            "to_field": "classes",
+            "type": "extract_field_values"
         }
     ],
-    "task": "tasks.evaluation.preference",
-    "templates": "templates.evaluation.preference.all",
+    "task": "tasks.classification.multi_class",
+    "templates": "templates.classification.multi_class.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/law_stack_exchange.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mt_bench/response_assessment/pairwise_comparison/multi_turn_with_reference_gpt4_judgement.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6628205128205128%*

 * *Differences: {"'loader'": "{'path': 'OfirArviv/mt_bench_pairwise_comparison_gpt4_judgments', 'split': 'train'}",*

 * * "'preprocess_steps'": "{4: {'type': 'map_instance_values', 'mappers': OrderedDict([('winner', "*

 * *                       "OrderedDict([('model_1', 'choice_a'), ('model_2', 'choice_b'), ('tie', "*

 * *                       "'tie')]))]), delete: ['mix']}, 5: {'field_to_field': {replace: "*

 * *                       "OrderedDict([('category', 'group')])}}, 7: {'type': 'literal_eval', "*

 * *                       "'to_field': […]*

```diff
@@ -1,64 +1,99 @@
 {
     "loader": {
-        "path": "jonathanli/law-stack-exchange",
+        "path": "OfirArviv/mt_bench_pairwise_comparison_gpt4_judgments",
+        "split": "train",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mix": {
-                "test": "train",
-                "train": "test",
-                "validation": "validation"
+            "mapper": {
+                "train": "test"
             },
-            "type": "split_random_mix"
+            "type": "rename_splits"
+        },
+        {
+            "condition": "eq",
+            "type": "filter_by_condition",
+            "values": {
+                "turn": 2
+            }
+        },
+        {
+            "condition": "ne",
+            "type": "filter_by_condition",
+            "values": {
+                "reference": "[]"
+            }
+        },
+        {
+            "condition": "in",
+            "type": "filter_by_condition",
+            "values": {
+                "winner": [
+                    "model_1",
+                    "tie",
+                    "model_2"
+                ]
+            }
+        },
+        {
+            "mappers": {
+                "winner": {
+                    "model_1": "choice_a",
+                    "model_2": "choice_b",
+                    "tie": "tie"
+                }
+            },
+            "type": "map_instance_values"
         },
         {
             "field_to_field": {
-                "text_label": "label"
+                "category": "group"
             },
             "type": "rename_fields"
         },
         {
-            "fields": [
-                "title",
-                "body"
-            ],
-            "to_field": "text",
-            "type": "list_field_values"
-        },
-        {
-            "field": "text",
-            "separator": ". ",
-            "to_field": "text",
-            "type": "join_str"
-        },
-        {
-            "fields": {
-                "classes": [
-                    "business",
-                    "civil-law",
-                    "constitutional-law",
-                    "contract",
-                    "contract-law",
-                    "copyright",
-                    "criminal-law",
-                    "employment",
-                    "intellectual-property",
-                    "internet",
-                    "liability",
-                    "licensing",
-                    "privacy",
-                    "software",
-                    "tax-law",
-                    "trademark"
-                ],
-                "text_type": "text",
-                "type_of_class": "topic"
-            },
-            "type": "add_fields"
+            "field": "model_input",
+            "to_field": "model_input",
+            "type": "literal_eval"
+        },
+        {
+            "field": "model_1_output",
+            "to_field": "model_1_output",
+            "type": "literal_eval"
+        },
+        {
+            "field": "model_2_output",
+            "to_field": "model_2_output",
+            "type": "literal_eval"
+        },
+        {
+            "field": "reference",
+            "to_field": "reference",
+            "type": "literal_eval"
+        },
+        {
+            "assistant_turns_field": "model_1_output",
+            "to_field": "dialog_a",
+            "type": "interleave_lists_to_dialog_operator",
+            "user_turns_field": "model_input"
+        },
+        {
+            "assistant_turns_field": "model_2_output",
+            "to_field": "dialog_b",
+            "type": "interleave_lists_to_dialog_operator",
+            "user_turns_field": "model_input"
+        },
+        {
+            "assistant_turns_field": "reference",
+            "to_field": "reference_dialog",
+            "type": "interleave_lists_to_dialog_operator",
+            "user_turns_field": "model_input"
         }
     ],
-    "task": "tasks.classification.multi_class",
-    "templates": "templates.classification.multi_class.all",
+    "task": "tasks.response_assessment.pairwise_comparison.multi_turn_with_reference",
+    "templates": [
+        "templates.response_assessment.pairwise_comparison.mt_bench_multi_turn_with_reference_with_shuffle"
+    ],
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/ledgar.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/ledgar.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7142857142857143%*

 * *Differences: {"'__description__'": '\'Dataset Card for "LexGLUE"\\nDataset Summary\\nInspired by the recent '*

 * *                      'widespread use of the GLUE multi-task benchmark NLP dataset (Wang et al., '*

 * *                      '2018), the subsequent more difficult SuperGLUE (Wang et al., 2019), other '*

 * *                      'previous multi-task NLP benchmarks (Conneau and Kiela, 2018; McCann et al., '*

 * *                      '2018), and similar initiatives in other domains (Peng et al., 2019), we '*

 * *                    […]*

```diff
@@ -1,8 +1,36 @@
 {
+    "__description__": "Dataset Card for \"LexGLUE\"\nDataset Summary\nInspired by the recent widespread use of the GLUE multi-task benchmark NLP dataset (Wang et al., 2018), the subsequent more difficult SuperGLUE (Wang et al., 2019), other previous multi-task NLP benchmarks (Conneau and Kiela, 2018; McCann et al., 2018), and similar initiatives in other domains (Peng et al., 2019), we introduce the Legal General Language Understanding Evaluation (LexGLUE) benchmark, a benchmark dataset to\u2026 See the full description on the dataset page: https://huggingface.co/datasets/coastalcph/lex_glue.",
+    "__tags__": {
+        "annotations_creators": "found",
+        "arxiv": [
+            "2110.00976",
+            "2109.00904",
+            "1805.01217",
+            "2104.08671"
+        ],
+        "croissant": true,
+        "language": "en",
+        "language_creators": "found",
+        "license": "cc-by-4.0",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "extended",
+        "task_categories": [
+            "question-answering",
+            "text-classification"
+        ],
+        "task_ids": [
+            "multi-class-classification",
+            "multi-label-classification",
+            "multiple-choice-qa",
+            "topic-classification"
+        ]
+    },
     "loader": {
         "name": "ledgar",
         "path": "lex_glue",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/medical_abstracts.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/ai2_arc/arc_challenge.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.45863095238095236%*

 * *Differences: {"'__description__'": '\'Dataset Card for "ai2_arc"\\nDataset Summary\\nA new dataset of 7,787 '*

 * *                      'genuine grade-school level, multiple-choice science questions, assembled to '*

 * *                      'encourage research in\\nadvanced question-answering. The dataset is '*

 * *                      'partitioned into a Challenge Set and an Easy Set, where the former '*

 * *                      'contains\\nonly questions answered incorrectly by both a retrieval-based '*

 * *                      'algorith […]*

```diff
@@ -1,55 +1,56 @@
 {
+    "__description__": "Dataset Card for \"ai2_arc\"\nDataset Summary\nA new dataset of 7,787 genuine grade-school level, multiple-choice science questions, assembled to encourage research in\nadvanced question-answering. The dataset is partitioned into a Challenge Set and an Easy Set, where the former contains\nonly questions answered incorrectly by both a retrieval-based algorithm and a word co-occurrence algorithm. We are also\nincluding a corpus of over 14 million science sentences\u2026 See the full description on the dataset page: https://huggingface.co/datasets/allenai/ai2_arc.",
+    "__tags__": {
+        "annotations_creators": "found",
+        "arxiv": "1803.05457",
+        "croissant": true,
+        "language": "en",
+        "language_creators": "found",
+        "license": "cc-by-sa-4.0",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "1K<n<10K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": [
+            "open-domain-qa",
+            "multiple-choice-qa"
+        ]
+    },
     "loader": {
-        "files": {
-            "test": "https://raw.githubusercontent.com/sebischair/Medical-Abstracts-TC-Corpus/main/medical_tc_test.csv",
-            "train": "https://raw.githubusercontent.com/sebischair/Medical-Abstracts-TC-Corpus/main/medical_tc_train.csv"
-        },
-        "type": "load_csv"
+        "name": "ARC-Challenge",
+        "path": "ai2_arc",
+        "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mix": {
-                "test": "test",
-                "train": "train[90%]",
-                "validation": "train[10%]"
+            "fields": {
+                "topic": "science"
             },
-            "type": "split_random_mix"
+            "type": "add_fields"
         },
         {
             "field_to_field": {
-                "condition_label": "label",
-                "medical_abstract": "text"
+                "answerKey": "label",
+                "choices": "_choices"
             },
             "type": "rename_fields"
         },
         {
-            "mappers": {
-                "label": {
-                    "1": "neoplasms",
-                    "2": "digestive system diseases",
-                    "3": "nervous system diseases",
-                    "4": "cardiovascular diseases",
-                    "5": "general pathological conditions"
-                }
+            "field_to_field": {
+                "_choices/label": "labels",
+                "_choices/text": "choices"
             },
-            "type": "map_instance_values"
+            "type": "copy_fields"
         },
         {
-            "fields": {
-                "classes": [
-                    "neoplasms",
-                    "digestive system diseases",
-                    "nervous system diseases",
-                    "cardiovascular diseases",
-                    "general pathological conditions"
-                ],
-                "text_type": "abstract",
-                "type_of_class": "topic"
-            },
-            "type": "add_fields"
+            "index_of": "label",
+            "search_in": "labels",
+            "to_field": "answer",
+            "type": "index_of"
         }
     ],
-    "task": "tasks.classification.multi_class",
-    "templates": "templates.classification.multi_class.all",
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/mlsum/es.json` & `unitxt-1.9.0/src/unitxt/catalog/metrics/rag/context_relevance.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.16666666666666666%*

 * *Differences: {"'main_score'": "'perplexity'",*

 * * "'metric'": "'metrics.perplexity_q.flan_t5_small'",*

 * * "'preprocess_steps'": "{0: {'type': 'copy_fields', 'field_to_field': [['contexts', "*

 * *                       "'references']]}, 1: {'type': 'copy_fields', 'field_to_field': "*

 * *                       "[['question', 'prediction']], delete: ['fields']}}",*

 * * "'type'": "'metric_pipeline'",*

 * * 'delete': "['loader', 'task', 'templates']"}*

```diff
@@ -1,24 +1,25 @@
 {
-    "loader": {
-        "name": "es",
-        "path": "mlsum",
-        "type": "load_hf"
-    },
+    "main_score": "perplexity",
+    "metric": "metrics.perplexity_q.flan_t5_small",
     "preprocess_steps": [
         {
-            "field_to_field": {
-                "text": "document"
-            },
-            "type": "rename_fields"
+            "field_to_field": [
+                [
+                    "contexts",
+                    "references"
+                ]
+            ],
+            "type": "copy_fields"
         },
         {
-            "fields": {
-                "document_type": "document"
-            },
-            "type": "add_fields"
+            "field_to_field": [
+                [
+                    "question",
+                    "prediction"
+                ]
+            ],
+            "type": "copy_fields"
         }
     ],
-    "task": "tasks.summarization.abstractive",
-    "templates": "templates.summarization.abstractive.all",
-    "type": "task_card"
+    "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/mlsum/ru.json` & `unitxt-1.9.0/src/unitxt/catalog/metrics/rag/context_correctness.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.16666666666666666%*

 * *Differences: {"'main_score'": "'score'",*

 * * "'metric'": "'metrics.mrr'",*

 * * "'preprocess_steps'": "{0: {'type': 'copy_fields', 'field_to_field': [['context_ids', "*

 * *                       "'prediction']]}, 1: {'type': 'copy_fields', 'field_to_field': "*

 * *                       "[['ground_truths_context_ids', 'references']], delete: ['fields']}}",*

 * * "'type'": "'metric_pipeline'",*

 * * 'delete': "['loader', 'task', 'templates']"}*

```diff
@@ -1,24 +1,25 @@
 {
-    "loader": {
-        "name": "ru",
-        "path": "mlsum",
-        "type": "load_hf"
-    },
+    "main_score": "score",
+    "metric": "metrics.mrr",
     "preprocess_steps": [
         {
-            "field_to_field": {
-                "text": "document"
-            },
-            "type": "rename_fields"
+            "field_to_field": [
+                [
+                    "context_ids",
+                    "prediction"
+                ]
+            ],
+            "type": "copy_fields"
         },
         {
-            "fields": {
-                "document_type": "document"
-            },
-            "type": "add_fields"
+            "field_to_field": [
+                [
+                    "ground_truths_context_ids",
+                    "references"
+                ]
+            ],
+            "type": "copy_fields"
         }
     ],
-    "task": "tasks.summarization.abstractive",
-    "templates": "templates.summarization.abstractive.all",
-    "type": "task_card"
+    "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/mlsum/tu.json` & `unitxt-1.9.0/src/unitxt/catalog/metrics/rag/mrr.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.16666666666666666%*

 * *Differences: {"'main_score'": "'score'",*

 * * "'metric'": "'metrics.mrr'",*

 * * "'preprocess_steps'": "{0: {'type': 'copy_fields', 'field_to_field': [['context_ids', "*

 * *                       "'prediction']]}, 1: {'type': 'copy_fields', 'field_to_field': "*

 * *                       "[['ground_truths_context_ids', 'references']], delete: ['fields']}}",*

 * * "'type'": "'metric_pipeline'",*

 * * 'delete': "['loader', 'task', 'templates']"}*

```diff
@@ -1,24 +1,25 @@
 {
-    "loader": {
-        "name": "tu",
-        "path": "mlsum",
-        "type": "load_hf"
-    },
+    "main_score": "score",
+    "metric": "metrics.mrr",
     "preprocess_steps": [
         {
-            "field_to_field": {
-                "text": "document"
-            },
-            "type": "rename_fields"
+            "field_to_field": [
+                [
+                    "context_ids",
+                    "prediction"
+                ]
+            ],
+            "type": "copy_fields"
         },
         {
-            "fields": {
-                "document_type": "document"
-            },
-            "type": "add_fields"
+            "field_to_field": [
+                [
+                    "ground_truths_context_ids",
+                    "references"
+                ]
+            ],
+            "type": "copy_fields"
         }
     ],
-    "task": "tasks.summarization.abstractive",
-    "templates": "templates.summarization.abstractive.all",
-    "type": "task_card"
+    "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/college_physics.json` & `unitxt-1.9.0/src/unitxt/catalog/metrics/rag/map.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.1547619047619048%*

 * *Differences: {"'main_score'": "'score'",*

 * * "'metric'": "'metrics.map'",*

 * * "'preprocess_steps'": "{0: {'type': 'copy_fields', 'field_to_field': [['context_ids', "*

 * *                       "'prediction']], delete: ['mapper']}, 1: {'type': 'copy_fields', "*

 * *                       "'field_to_field': [['ground_truths_context_ids', 'references']], delete: "*

 * *                       "['fields']}}",*

 * * "'type'": "'metric_pipeline'",*

 * * 'delete': "['loader', 'task', 'templates']"}*

```diff
@@ -1,24 +1,25 @@
 {
-    "loader": {
-        "name": "college_physics",
-        "path": "cais/mmlu",
-        "type": "load_hf"
-    },
+    "main_score": "score",
+    "metric": "metrics.map",
     "preprocess_steps": [
         {
-            "mapper": {
-                "dev": "train"
-            },
-            "type": "rename_splits"
+            "field_to_field": [
+                [
+                    "context_ids",
+                    "prediction"
+                ]
+            ],
+            "type": "copy_fields"
         },
         {
-            "fields": {
-                "topic": "college physics"
-            },
-            "type": "add_fields"
+            "field_to_field": [
+                [
+                    "ground_truths_context_ids",
+                    "references"
+                ]
+            ],
+            "type": "copy_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_topic",
-    "templates": "templates.qa.multiple_choice.with_topic.all",
-    "type": "task_card"
+    "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/high_school_computer_science.json` & `unitxt-1.9.0/src/unitxt/catalog/metrics/llm_as_judge/rating/llama_3_70b_instruct_ibm_genai_template_mt_bench_single_turn.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.1111111111111111%*

 * *Differences: {"'format'": "'formats.llama3_chat'",*

 * * "'inference_model'": "OrderedDict([('type', 'ibm_gen_ai_inference_engine'), ('model_name', "*

 * *                      "'meta-llama/llama-3-70b-instruct'), ('parameters', OrderedDict([('type', "*

 * *                      "'ibm_gen_ai_inference_engine_params'), ('max_new_tokens', 252)]))])",*

 * * "'main_score'": "'llama_3_70b_instruct_ibm_genai_template_mt_bench_single_turn'",*

 * * "'task'": "'rating.single_turn'",*

 * * "'template'": "'templates.response_assessment.rating.mt_bench_single_t […]*

```diff
@@ -1,24 +1,15 @@
 {
-    "loader": {
-        "name": "high_school_computer_science",
-        "path": "cais/mmlu",
-        "type": "load_hf"
-    },
-    "preprocess_steps": [
-        {
-            "mapper": {
-                "dev": "train"
-            },
-            "type": "rename_splits"
+    "format": "formats.llama3_chat",
+    "inference_model": {
+        "model_name": "meta-llama/llama-3-70b-instruct",
+        "parameters": {
+            "max_new_tokens": 252,
+            "type": "ibm_gen_ai_inference_engine_params"
         },
-        {
-            "fields": {
-                "topic": "high school computer science"
-            },
-            "type": "add_fields"
-        }
-    ],
-    "task": "tasks.qa.multiple_choice.with_topic",
-    "templates": "templates.qa.multiple_choice.with_topic.all",
-    "type": "task_card"
+        "type": "ibm_gen_ai_inference_engine"
+    },
+    "main_score": "llama_3_70b_instruct_ibm_genai_template_mt_bench_single_turn",
+    "task": "rating.single_turn",
+    "template": "templates.response_assessment.rating.mt_bench_single_turn",
+    "type": "llm_as_judge"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/high_school_microeconomics.json` & `unitxt-1.9.0/src/unitxt/catalog/metrics/rag/bert_recall_ml.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.1547619047619048%*

 * *Differences: {"'main_score'": "'recall'",*

 * * "'metric'": "'metrics.bert_score.deberta_v3_base_mnli_xnli_ml'",*

 * * "'preprocess_steps'": "{0: {'type': 'copy_fields', 'field_to_field': [['ground_truths', "*

 * *                       "'references']], delete: ['mapper']}, 1: {'type': 'copy_fields', "*

 * *                       "'field_to_field': [['answer', 'prediction']], delete: ['fields']}}",*

 * * "'type'": "'metric_pipeline'",*

 * * 'delete': "['loader', 'task', 'templates']"}*

```diff
@@ -1,24 +1,25 @@
 {
-    "loader": {
-        "name": "high_school_microeconomics",
-        "path": "cais/mmlu",
-        "type": "load_hf"
-    },
+    "main_score": "recall",
+    "metric": "metrics.bert_score.deberta_v3_base_mnli_xnli_ml",
     "preprocess_steps": [
         {
-            "mapper": {
-                "dev": "train"
-            },
-            "type": "rename_splits"
+            "field_to_field": [
+                [
+                    "ground_truths",
+                    "references"
+                ]
+            ],
+            "type": "copy_fields"
         },
         {
-            "fields": {
-                "topic": "high school microeconomics"
-            },
-            "type": "add_fields"
+            "field_to_field": [
+                [
+                    "answer",
+                    "prediction"
+                ]
+            ],
+            "type": "copy_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_topic",
-    "templates": "templates.qa.multiple_choice.with_topic.all",
-    "type": "task_card"
+    "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/mmlu/professional_accounting.json` & `unitxt-1.9.0/src/unitxt/catalog/metrics/rag/faithfulness.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.1547619047619048%*

 * *Differences: {"'main_score'": "'precision'",*

 * * "'metric'": "'metrics.token_overlap'",*

 * * "'preprocess_steps'": "{0: {'type': 'copy_fields', 'field_to_field': [['contexts', "*

 * *                       "'references']], delete: ['mapper']}, 1: {'type': 'copy_fields', "*

 * *                       "'field_to_field': [['answer', 'prediction']], delete: ['fields']}}",*

 * * "'type'": "'metric_pipeline'",*

 * * 'delete': "['loader', 'task', 'templates']"}*

```diff
@@ -1,24 +1,25 @@
 {
-    "loader": {
-        "name": "professional_accounting",
-        "path": "cais/mmlu",
-        "type": "load_hf"
-    },
+    "main_score": "precision",
+    "metric": "metrics.token_overlap",
     "preprocess_steps": [
         {
-            "mapper": {
-                "dev": "train"
-            },
-            "type": "rename_splits"
+            "field_to_field": [
+                [
+                    "contexts",
+                    "references"
+                ]
+            ],
+            "type": "copy_fields"
         },
         {
-            "fields": {
-                "topic": "professional accounting"
-            },
-            "type": "add_fields"
+            "field_to_field": [
+                [
+                    "answer",
+                    "prediction"
+                ]
+            ],
+            "type": "copy_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_topic",
-    "templates": "templates.qa.multiple_choice.with_topic.all",
-    "type": "task_card"
+    "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/mnli.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/urdu.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4976190476190476%*

 * *Differences: {"'__description__'": "'We present XLSum, a comprehensive and diverse dataset comprising 1.35 "*

 * *                      'million professionally\\nannotated article-summary pairs from BBC, '*

 * *                      'extracted using a set of carefully designed heuristics.\\nThe dataset '*

 * *                      'covers 45 languages ranging from low to high-resource, for many of which '*

 * *                      'no\\npublic dataset is currently available. XL-Sum is highly abstractive, '*

 * *                      'concise,\ […]*

```diff
@@ -1,49 +1,39 @@
 {
+    "__description__": "We present XLSum, a comprehensive and diverse dataset comprising 1.35 million professionally\nannotated article-summary pairs from BBC, extracted using a set of carefully designed heuristics.\nThe dataset covers 45 languages ranging from low to high-resource, for many of which no\npublic dataset is currently available. XL-Sum is highly abstractive, concise,\nand of high quality, as indicated by human and intrinsic evaluation.",
+    "__tags__": {
+        "annotations_creators": "none",
+        "arxiv": "1607.01759",
+        "croissant": true,
+        "language": "und",
+        "language_creators": "unknown",
+        "license": "cc-by-nc-sa-4.0",
+        "multilinguality": "unknown",
+        "region": "us",
+        "size_categories": "unknown",
+        "source_datasets": "original",
+        "task_categories": "summarization"
+    },
     "loader": {
-        "name": "mnli",
-        "path": "glue",
+        "name": "urdu",
+        "path": "GEM/xlsum",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mapper": {
-                "validation_matched": "validation"
-            },
-            "type": "rename_splits"
-        },
-        "splitters.small_no_test",
-        {
             "field_to_field": {
-                "hypothesis": "text_b",
-                "premise": "text_a"
+                "target": "summary",
+                "text": "document"
             },
             "type": "rename_fields"
         },
         {
-            "mappers": {
-                "label": {
-                    "0": "entailment",
-                    "1": "neutral",
-                    "2": "contradiction"
-                }
-            },
-            "type": "map_instance_values"
-        },
-        {
             "fields": {
-                "classes": [
-                    "entailment",
-                    "neutral",
-                    "contradiction"
-                ],
-                "text_a_type": "premise",
-                "text_b_type": "hypothesis",
-                "type_of_relation": "entailment"
+                "document_type": "document"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.classification.multi_class.relation",
-    "templates": "templates.classification.multi_class.relation.all",
+    "task": "tasks.summarization.abstractive",
+    "templates": "templates.summarization.abstractive.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/mrpc.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/scottish_gaelic.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4861111111111111%*

 * *Differences: {"'__description__'": "'We present XLSum, a comprehensive and diverse dataset comprising 1.35 "*

 * *                      'million professionally\\nannotated article-summary pairs from BBC, '*

 * *                      'extracted using a set of carefully designed heuristics.\\nThe dataset '*

 * *                      'covers 45 languages ranging from low to high-resource, for many of which '*

 * *                      'no\\npublic dataset is currently available. XL-Sum is highly abstractive, '*

 * *                      'concise,\ […]*

```diff
@@ -1,54 +1,39 @@
 {
+    "__description__": "We present XLSum, a comprehensive and diverse dataset comprising 1.35 million professionally\nannotated article-summary pairs from BBC, extracted using a set of carefully designed heuristics.\nThe dataset covers 45 languages ranging from low to high-resource, for many of which no\npublic dataset is currently available. XL-Sum is highly abstractive, concise,\nand of high quality, as indicated by human and intrinsic evaluation.",
+    "__tags__": {
+        "annotations_creators": "none",
+        "arxiv": "1607.01759",
+        "croissant": true,
+        "language": "und",
+        "language_creators": "unknown",
+        "license": "cc-by-nc-sa-4.0",
+        "multilinguality": "unknown",
+        "region": "us",
+        "size_categories": "unknown",
+        "source_datasets": "original",
+        "task_categories": "summarization"
+    },
     "loader": {
-        "name": "mrpc",
-        "path": "glue",
-        "streaming": false,
+        "name": "scottish_gaelic",
+        "path": "GEM/xlsum",
         "type": "load_hf"
     },
     "preprocess_steps": [
-        "splitters.default",
         {
-            "mappers": {
-                "label": {
-                    "0": "not equivalent",
-                    "1": "equivalent"
-                }
+            "field_to_field": {
+                "target": "summary",
+                "text": "document"
             },
-            "type": "map_instance_values"
+            "type": "rename_fields"
         },
         {
             "fields": {
-                "choices": [
-                    "not equivalent",
-                    "equivalent"
-                ]
+                "document_type": "document"
             },
             "type": "add_fields"
         }
     ],
-    "task": {
-        "inputs": [
-            "choices",
-            "sentence1",
-            "sentence2"
-        ],
-        "metrics": [
-            "metrics.accuracy"
-        ],
-        "outputs": [
-            "label"
-        ],
-        "type": "form_task"
-    },
-    "templates": {
-        "items": [
-            {
-                "input_format": "Given this sentence: {sentence1}, classify if this sentence: {sentence2} is {choices}.",
-                "output_format": "{label}",
-                "type": "input_output_template"
-            }
-        ],
-        "type": "templates_list"
-    },
+    "task": "tasks.summarization.abstractive",
+    "templates": "templates.summarization.abstractive.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/multidoc2dial/extractive.json` & `unitxt-1.9.0/src/unitxt/catalog/metrics/rag/answer_reward.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.15952380952380954%*

 * *Differences: {"'main_score'": "'score'",*

 * * "'metric'": "'metrics.reward.deberta_v3_large_v2'",*

 * * "'preprocess_steps'": "{1: {'type': 'copy_fields', 'field_to_field': [['answer', 'prediction']]}, "*

 * *                       "2: {'fields': ['references'], 'to_field': 'references'}, insert: [(0, "*

 * *                       "OrderedDict([('type', 'copy_fields'), ('field_to_field', [['question', "*

 * *                       "'references']])]))], delete: [3, 2]}",*

 * * "'type'": "'metric_pipeline'",*

 * * 'delete': "['loader', 'task', 'templates' […]*

```diff
@@ -1,35 +1,32 @@
 {
-    "loader": {
-        "path": "multidoc2dial",
-        "type": "load_hf"
-    },
+    "main_score": "score",
+    "metric": "metrics.reward.deberta_v3_large_v2",
     "preprocess_steps": [
         {
-            "field_to_field": {
-                "answers/text/0": "relevant_context"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "fields": [
-                "relevant_context"
+            "field_to_field": [
+                [
+                    "question",
+                    "references"
+                ]
             ],
-            "to_field": "answers",
-            "type": "list_field_values"
+            "type": "copy_fields"
         },
         {
-            "expression": "question.split('[SEP]')[0]",
-            "to_field": "question",
-            "type": "execute_expression"
+            "field_to_field": [
+                [
+                    "answer",
+                    "prediction"
+                ]
+            ],
+            "type": "copy_fields"
         },
         {
-            "fields": {
-                "context_type": "document"
-            },
-            "type": "add_fields"
+            "fields": [
+                "references"
+            ],
+            "to_field": "references",
+            "type": "list_field_values"
         }
     ],
-    "task": "tasks.qa.with_context.extractive",
-    "templates": "templates.qa.with_context.all",
-    "type": "task_card"
+    "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/news_category_classification_headline.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/news_category_classification_headline.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/openbook_qa.json` & `unitxt-1.9.0/src/unitxt/catalog/metrics/rag/k_precision.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.16666666666666666%*

 * *Differences: {"'main_score'": "'precision'",*

 * * "'metric'": "'metrics.token_overlap'",*

 * * "'preprocess_steps'": "{0: {'type': 'copy_fields', 'field_to_field': [['contexts', "*

 * *                       "'references']]}, 1: {'type': 'copy_fields', 'field_to_field': [['answer', "*

 * *                       "'prediction']]}, delete: [2]}",*

 * * "'type'": "'metric_pipeline'",*

 * * 'delete': "['loader', 'task', 'templates']"}*

```diff
@@ -1,31 +1,25 @@
 {
-    "loader": {
-        "path": "openbookqa",
-        "type": "load_hf"
-    },
+    "main_score": "precision",
+    "metric": "metrics.token_overlap",
     "preprocess_steps": [
         {
-            "field_to_field": {
-                "choices/label": "labels",
-                "choices/text": "choices_text"
-            },
-            "type": "rename_fields"
+            "field_to_field": [
+                [
+                    "contexts",
+                    "references"
+                ]
+            ],
+            "type": "copy_fields"
         },
         {
-            "field_to_field": {
-                "choices_text": "choices",
-                "question_stem": "question"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "index_of": "answerKey",
-            "search_in": "labels",
-            "to_field": "answer",
-            "type": "index_of"
+            "field_to_field": [
+                [
+                    "answer",
+                    "prediction"
+                ]
+            ],
+            "type": "copy_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.open",
-    "templates": "templates.qa.multiple_choice.open.all",
-    "type": "task_card"
+    "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/qqp.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/openbook_qa.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.47023809523809523%*

 * *Differences: {"'__description__'": "'Dataset Card for OpenBookQA\\nDataset Summary\\nOpenBookQA aims to promote "*

 * *                      'research in advanced question-answering, probing a deeper understanding of '*

 * *                      'both the topic\\n(with salient facts summarized as an open book, also '*

 * *                      'provided with the dataset) and the language it is expressed in. '*

 * *                      'In\\nparticular, it contains questions that require multi-step reasoning, '*

 * *                      'use o […]*

```diff
@@ -1,53 +1,48 @@
 {
+    "__description__": "Dataset Card for OpenBookQA\nDataset Summary\nOpenBookQA aims to promote research in advanced question-answering, probing a deeper understanding of both the topic\n(with salient facts summarized as an open book, also provided with the dataset) and the language it is expressed in. In\nparticular, it contains questions that require multi-step reasoning, use of additional common and commonsense knowledge,\nand rich text comprehension.\nOpenBookQA is a new kind of\u2026 See the full description on the dataset page: https://huggingface.co/datasets/allenai/openbookqa.",
+    "__tags__": {
+        "annotations_creators": [
+            "crowdsourced",
+            "expert-generated"
+        ],
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "unknown",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "1K<n<10K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": "open-domain-qa"
+    },
     "loader": {
-        "name": "qqp",
-        "path": "glue",
+        "path": "openbookqa",
         "type": "load_hf"
     },
     "preprocess_steps": [
-        "splitters.large_no_test",
         {
-            "mappers": {
-                "label": {
-                    "0": "not duplicated",
-                    "1": "duplicated"
-                }
+            "field_to_field": {
+                "choices/label": "labels",
+                "choices/text": "choices_text"
             },
-            "type": "map_instance_values"
+            "type": "rename_fields"
         },
         {
-            "fields": {
-                "choices": [
-                    "not duplicated",
-                    "duplicated"
-                ]
+            "field_to_field": {
+                "choices_text": "choices",
+                "question_stem": "question"
             },
-            "type": "add_fields"
+            "type": "rename_fields"
+        },
+        {
+            "index_of": "answerKey",
+            "search_in": "labels",
+            "to_field": "answer",
+            "type": "index_of"
         }
     ],
-    "task": {
-        "inputs": [
-            "choices",
-            "question1",
-            "question2"
-        ],
-        "metrics": [
-            "metrics.accuracy"
-        ],
-        "outputs": [
-            "label"
-        ],
-        "type": "form_task"
-    },
-    "templates": {
-        "items": [
-            {
-                "input_format": "Given this question: {question1}, classify if this question: {question2} is {choices}.",
-                "output_format": "{label}",
-                "type": "input_output_template"
-            }
-        ],
-        "type": "templates_list"
-    },
+    "task": "tasks.qa.multiple_choice.open",
+    "templates": "templates.qa.multiple_choice.open.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/race_all.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/xnli/ur.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.49603174603174605%*

 * *Differences: {"'__description__'": '\'Dataset Card for "xnli"\\nDataset Summary\\nXNLI is a subset of a few '*

 * *                      'thousand examples from MNLI which has been translated\\ninto a 14 different '*

 * *                      'languages (some low-ish resource). As with MNLI, the goal is\\nto predict '*

 * *                      'textual entailment (does sentence A imply/contradict/neither sentence\\nB) '*

 * *                      'and is a classification task (given two sentences, predict one of '*

 * *                      't […]*

```diff
@@ -1,64 +1,71 @@
 {
+    "__description__": "Dataset Card for \"xnli\"\nDataset Summary\nXNLI is a subset of a few thousand examples from MNLI which has been translated\ninto a 14 different languages (some low-ish resource). As with MNLI, the goal is\nto predict textual entailment (does sentence A imply/contradict/neither sentence\nB) and is a classification task (given two sentences, predict one of three\nlabels).\nSupported Tasks and Leaderboards\nMore Information Needed\nLanguages\nMore\u2026 See the full description on the dataset page: https://huggingface.co/datasets/xnli.",
+    "__tags__": {
+        "croissant": true,
+        "language": [
+            "ar",
+            "bg",
+            "de",
+            "el",
+            "en",
+            "es",
+            "fr",
+            "hi",
+            "ru",
+            "sw",
+            "th",
+            "tr",
+            "ur",
+            "vi",
+            "zh"
+        ],
+        "region": "us"
+    },
     "loader": {
-        "name": "all",
-        "path": "race",
+        "name": "ur",
+        "path": "xnli",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "fields": {
-                "numbering": [
-                    "A",
-                    "B",
-                    "C",
-                    "D",
-                    "E",
-                    "F",
-                    "G",
-                    "H",
-                    "I",
-                    "J",
-                    "K",
-                    "L",
-                    "M",
-                    "N",
-                    "O",
-                    "P",
-                    "Q",
-                    "R",
-                    "S",
-                    "T",
-                    "U",
-                    "V",
-                    "W",
-                    "X",
-                    "Y",
-                    "Z"
-                ]
+            "mapper": {
+                "validation_matched": "validation"
             },
-            "type": "add_fields"
-        },
-        {
-            "index_of": "answer",
-            "search_in": "numbering",
-            "to_field": "answer",
-            "type": "index_of"
+            "type": "rename_splits"
         },
+        "splitters.small_no_test",
         {
             "field_to_field": {
-                "article": "context",
-                "options": "choices"
+                "hypothesis": "text_b",
+                "premise": "text_a"
             },
             "type": "rename_fields"
         },
         {
+            "mappers": {
+                "label": {
+                    "0": "entailment",
+                    "1": "neutral",
+                    "2": "contradiction"
+                }
+            },
+            "type": "map_instance_values"
+        },
+        {
             "fields": {
-                "context_type": "article"
+                "classes": [
+                    "entailment",
+                    "neutral",
+                    "contradiction"
+                ],
+                "text_a_type": "premise",
+                "text_b_type": "hypothesis",
+                "type_of_relation": "entailment"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.all",
+    "task": "tasks.classification.multi_class.relation",
+    "templates": "templates.classification.multi_class.relation.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/race_high.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/ffqa_filtered/16k.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.47933673469387755%*

 * *Differences: {"'__description__'": '\'Dataset Card for "WikiQA-Free_Form_QA"\\nThe WikiQA task is the task of '*

 * *                      'answering a question based on the information given in a Wikipedia '*

 * *                      'document. We have built upon the short answer format data in Google Natural '*

 * *                      'Questions to construct our QA task. It is formatted as a document and a '*

 * *                      'question. We ensure the answer to the question is a short answer which is '*

 * *                      'e […]*

```diff
@@ -1,64 +1,68 @@
 {
+    "__description__": "Dataset Card for \"WikiQA-Free_Form_QA\"\nThe WikiQA task is the task of answering a question based on the information given in a Wikipedia document. We have built upon the short answer format data in Google Natural Questions to construct our QA task. It is formatted as a document and a question. We ensure the answer to the question is a short answer which is either a single word or a small sentence directly cut pasted from the document. Having the task structured as such, we can\u2026 See the full description on the dataset page: https://huggingface.co/datasets/abacusai/WikiQA-Free_Form_QA.",
+    "__tags__": {
+        "croissant": true,
+        "region": "us"
+    },
     "loader": {
-        "name": "high",
-        "path": "race",
+        "path": "abacusai/WikiQA-Free_Form_QA",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "fields": {
-                "numbering": [
-                    "A",
-                    "B",
-                    "C",
-                    "D",
-                    "E",
-                    "F",
-                    "G",
-                    "H",
-                    "I",
-                    "J",
-                    "K",
-                    "L",
-                    "M",
-                    "N",
-                    "O",
-                    "P",
-                    "Q",
-                    "R",
-                    "S",
-                    "T",
-                    "U",
-                    "V",
-                    "W",
-                    "X",
-                    "Y",
-                    "Z"
-                ]
+            "field_to_field": {
+                "conversations/0/tok_len": "inputs_len",
+                "conversations/0/value": "inputs",
+                "conversations/1/value": "answer"
             },
-            "type": "add_fields"
+            "type": "copy_fields"
         },
         {
-            "index_of": "answer",
-            "search_in": "numbering",
-            "to_field": "answer",
-            "type": "index_of"
+            "fields": [
+                "answer"
+            ],
+            "to_field": "answers",
+            "type": "list_field_values"
         },
         {
-            "field_to_field": {
-                "article": "context",
-                "options": "choices"
-            },
-            "type": "rename_fields"
+            "condition": "lt",
+            "type": "filter_by_condition",
+            "values": {
+                "inputs_len": 16384
+            }
+        },
+        {
+            "expression": "re.search(r\"Document:\\s(.*)(\\n\\n|$)\", inputs).group(1)",
+            "imports_list": [
+                "re"
+            ],
+            "to_field": "context",
+            "type": "execute_expression"
+        },
+        {
+            "expression": "re.search(r\"Question:\\s(.*)(\\n\\n|$)\", inputs).group(1)",
+            "imports_list": [
+                "re"
+            ],
+            "to_field": "question",
+            "type": "execute_expression"
         },
         {
             "fields": {
-                "context_type": "article"
+                "context_type": "document"
             },
             "type": "add_fields"
+        },
+        {
+            "mix": {
+                "test": "16k[10%]",
+                "train": "16k[80%]",
+                "validation": "16k[10%]"
+            },
+            "type": "split_random_mix"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.all",
+    "task": "tasks.qa.with_context.extractive",
+    "templates": "templates.qa.with_context.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/race_middle.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/xnli/ar.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.49603174603174605%*

 * *Differences: {"'__description__'": '\'Dataset Card for "xnli"\\nDataset Summary\\nXNLI is a subset of a few '*

 * *                      'thousand examples from MNLI which has been translated\\ninto a 14 different '*

 * *                      'languages (some low-ish resource). As with MNLI, the goal is\\nto predict '*

 * *                      'textual entailment (does sentence A imply/contradict/neither sentence\\nB) '*

 * *                      'and is a classification task (given two sentences, predict one of '*

 * *                      't […]*

```diff
@@ -1,64 +1,71 @@
 {
+    "__description__": "Dataset Card for \"xnli\"\nDataset Summary\nXNLI is a subset of a few thousand examples from MNLI which has been translated\ninto a 14 different languages (some low-ish resource). As with MNLI, the goal is\nto predict textual entailment (does sentence A imply/contradict/neither sentence\nB) and is a classification task (given two sentences, predict one of three\nlabels).\nSupported Tasks and Leaderboards\nMore Information Needed\nLanguages\nMore\u2026 See the full description on the dataset page: https://huggingface.co/datasets/xnli.",
+    "__tags__": {
+        "croissant": true,
+        "language": [
+            "ar",
+            "bg",
+            "de",
+            "el",
+            "en",
+            "es",
+            "fr",
+            "hi",
+            "ru",
+            "sw",
+            "th",
+            "tr",
+            "ur",
+            "vi",
+            "zh"
+        ],
+        "region": "us"
+    },
     "loader": {
-        "name": "middle",
-        "path": "race",
+        "name": "ar",
+        "path": "xnli",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "fields": {
-                "numbering": [
-                    "A",
-                    "B",
-                    "C",
-                    "D",
-                    "E",
-                    "F",
-                    "G",
-                    "H",
-                    "I",
-                    "J",
-                    "K",
-                    "L",
-                    "M",
-                    "N",
-                    "O",
-                    "P",
-                    "Q",
-                    "R",
-                    "S",
-                    "T",
-                    "U",
-                    "V",
-                    "W",
-                    "X",
-                    "Y",
-                    "Z"
-                ]
+            "mapper": {
+                "validation_matched": "validation"
             },
-            "type": "add_fields"
-        },
-        {
-            "index_of": "answer",
-            "search_in": "numbering",
-            "to_field": "answer",
-            "type": "index_of"
+            "type": "rename_splits"
         },
+        "splitters.small_no_test",
         {
             "field_to_field": {
-                "article": "context",
-                "options": "choices"
+                "hypothesis": "text_b",
+                "premise": "text_a"
             },
             "type": "rename_fields"
         },
         {
+            "mappers": {
+                "label": {
+                    "0": "entailment",
+                    "1": "neutral",
+                    "2": "contradiction"
+                }
+            },
+            "type": "map_instance_values"
+        },
+        {
             "fields": {
-                "context_type": "article"
+                "classes": [
+                    "entailment",
+                    "neutral",
+                    "contradiction"
+                ],
+                "text_a_type": "premise",
+                "text_b_type": "hypothesis",
+                "type_of_relation": "entailment"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.with_context",
-    "templates": "templates.qa.multiple_choice.with_context.all",
+    "task": "tasks.classification.multi_class.relation",
+    "templates": "templates.classification.multi_class.relation.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/reuters21578/ModApte.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/reuters21578/ModHayes.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7023644179894181%*

 * *Differences: {"'__description__'": "'The Reuters-21578 dataset  is one of the most widely used data collections "*

 * *                      'for text\\ncategorization research. It is collected from the Reuters '*

 * *                      "financial newswire service in 1987.'",*

 * * "'__tags__'": "OrderedDict([('croissant', True), ('language', 'en'), ('license', 'other'), "*

 * *               "('region', 'us')])",*

 * * "'loader'": "{'name': 'ModHayes'}",*

 * * "'preprocess_steps'": "{2: {'fields': {'classes': {insert: [(4, 'bfr'), (42, 'hk')]}}} […]*

```diff
@@ -1,10 +1,17 @@
 {
+    "__description__": "The Reuters-21578 dataset  is one of the most widely used data collections for text\ncategorization research. It is collected from the Reuters financial newswire service in 1987.",
+    "__tags__": {
+        "croissant": true,
+        "language": "en",
+        "license": "other",
+        "region": "us"
+    },
     "loader": {
-        "name": "ModApte",
+        "name": "ModHayes",
         "path": "reuters21578",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mix": {
                 "test": "test",
@@ -22,14 +29,15 @@
         {
             "fields": {
                 "classes": [
                     "acq",
                     "alum",
                     "austdlr",
                     "barley",
+                    "bfr",
                     "bop",
                     "can",
                     "carcass",
                     "castor-oil",
                     "castorseed",
                     "citruspulp",
                     "cocoa",
@@ -59,14 +67,15 @@
                     "gas",
                     "gnp",
                     "gold",
                     "grain",
                     "groundnut",
                     "groundnut-oil",
                     "heat",
+                    "hk",
                     "hog",
                     "housing",
                     "income",
                     "instal-debt",
                     "interest",
                     "inventories",
                     "ipi",
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/reuters21578/ModHayes.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/reuters21578/ModLewis.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7023644179894181%*

 * *Differences: {"'__description__'": "'The Reuters-21578 dataset  is one of the most widely used data collections "*

 * *                      'for text\\ncategorization research. It is collected from the Reuters '*

 * *                      "financial newswire service in 1987.'",*

 * * "'__tags__'": "OrderedDict([('croissant', True), ('language', 'en'), ('license', 'other'), "*

 * *               "('region', 'us')])",*

 * * "'loader'": "{'name': 'ModLewis'}",*

 * * "'preprocess_steps'": "{2: {'fields': {'classes': {delete: [42, 4]}}}}"}*

```diff
@@ -1,10 +1,17 @@
 {
+    "__description__": "The Reuters-21578 dataset  is one of the most widely used data collections for text\ncategorization research. It is collected from the Reuters financial newswire service in 1987.",
+    "__tags__": {
+        "croissant": true,
+        "language": "en",
+        "license": "other",
+        "region": "us"
+    },
     "loader": {
-        "name": "ModHayes",
+        "name": "ModLewis",
         "path": "reuters21578",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mix": {
                 "test": "test",
@@ -22,15 +29,14 @@
         {
             "fields": {
                 "classes": [
                     "acq",
                     "alum",
                     "austdlr",
                     "barley",
-                    "bfr",
                     "bop",
                     "can",
                     "carcass",
                     "castor-oil",
                     "castorseed",
                     "citruspulp",
                     "cocoa",
@@ -60,15 +66,14 @@
                     "gas",
                     "gnp",
                     "gold",
                     "grain",
                     "groundnut",
                     "groundnut-oil",
                     "heat",
-                    "hk",
                     "hog",
                     "housing",
                     "income",
                     "instal-debt",
                     "interest",
                     "inventories",
                     "ipi",
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/reuters21578/ModLewis.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/reuters21578/ModApte.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7023809523809524%*

 * *Differences: {"'__description__'": "'The Reuters-21578 dataset  is one of the most widely used data collections "*

 * *                      'for text\\ncategorization research. It is collected from the Reuters '*

 * *                      "financial newswire service in 1987.'",*

 * * "'__tags__'": "OrderedDict([('croissant', True), ('language', 'en'), ('license', 'other'), "*

 * *               "('region', 'us')])",*

 * * "'loader'": "{'name': 'ModApte'}"}*

```diff
@@ -1,10 +1,17 @@
 {
+    "__description__": "The Reuters-21578 dataset  is one of the most widely used data collections for text\ncategorization research. It is collected from the Reuters financial newswire service in 1987.",
+    "__tags__": {
+        "croissant": true,
+        "language": "en",
+        "license": "other",
+        "region": "us"
+    },
     "loader": {
-        "name": "ModLewis",
+        "name": "ModApte",
         "path": "reuters21578",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mix": {
                 "test": "test",
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/unfair_tos.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/xnli/vi.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.43255208333333334%*

 * *Differences: {"'__description__'": '\'Dataset Card for "xnli"\\nDataset Summary\\nXNLI is a subset of a few '*

 * *                      'thousand examples from MNLI which has been translated\\ninto a 14 different '*

 * *                      'languages (some low-ish resource). As with MNLI, the goal is\\nto predict '*

 * *                      'textual entailment (does sentence A imply/contradict/neither sentence\\nB) '*

 * *                      'and is a classification task (given two sentences, predict one of '*

 * *                      't […]*

```diff
@@ -1,50 +1,71 @@
 {
+    "__description__": "Dataset Card for \"xnli\"\nDataset Summary\nXNLI is a subset of a few thousand examples from MNLI which has been translated\ninto a 14 different languages (some low-ish resource). As with MNLI, the goal is\nto predict textual entailment (does sentence A imply/contradict/neither sentence\nB) and is a classification task (given two sentences, predict one of three\nlabels).\nSupported Tasks and Leaderboards\nMore Information Needed\nLanguages\nMore\u2026 See the full description on the dataset page: https://huggingface.co/datasets/xnli.",
+    "__tags__": {
+        "croissant": true,
+        "language": [
+            "ar",
+            "bg",
+            "de",
+            "el",
+            "en",
+            "es",
+            "fr",
+            "hi",
+            "ru",
+            "sw",
+            "th",
+            "tr",
+            "ur",
+            "vi",
+            "zh"
+        ],
+        "region": "us"
+    },
     "loader": {
-        "name": "unfair_tos",
-        "path": "lex_glue",
+        "name": "vi",
+        "path": "xnli",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
+            "mapper": {
+                "validation_matched": "validation"
+            },
+            "type": "rename_splits"
+        },
+        "splitters.small_no_test",
+        {
+            "field_to_field": {
+                "hypothesis": "text_b",
+                "premise": "text_a"
+            },
+            "type": "rename_fields"
+        },
+        {
             "mappers": {
-                "labels": {
-                    "0": "Limitation of liability",
-                    "1": "Unilateral termination",
-                    "2": "Unilateral change",
-                    "3": "Content removal",
-                    "4": "Contract by using",
-                    "5": "Choice of law",
-                    "6": "Jurisdiction",
-                    "7": "Arbitration"
+                "label": {
+                    "0": "entailment",
+                    "1": "neutral",
+                    "2": "contradiction"
                 }
             },
-            "process_every_value": true,
             "type": "map_instance_values"
         },
         {
             "fields": {
                 "classes": [
-                    "Limitation of liability",
-                    "Unilateral termination",
-                    "Unilateral change",
-                    "Content removal",
-                    "Contract by using",
-                    "Choice of law",
-                    "Jurisdiction",
-                    "Arbitration"
+                    "entailment",
+                    "neutral",
+                    "contradiction"
                 ],
-                "text_type": "text",
-                "type_of_classes": "contractual clauses"
+                "text_a_type": "premise",
+                "text_b_type": "hypothesis",
+                "type_of_relation": "entailment"
             },
             "type": "add_fields"
         }
     ],
-    "sampler": {
-        "choices": "classes",
-        "labels": "labels",
-        "type": "diverse_labels_sampler"
-    },
-    "task": "tasks.classification.multi_label",
-    "templates": "templates.classification.multi_label.all",
+    "task": "tasks.classification.multi_class.relation",
+    "templates": "templates.classification.multi_class.relation.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/ceb/gja.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/hr/set.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7053571428571429%*

 * *Differences: {"'__description__'": "'Universal Named Entity Recognition (UNER) aims to fill a gap in "*

 * *                      'multilingual NLP: high quality NER datasets in many languages with a shared '*

 * *                      'tagset.\\nUNER is modeled after the Universal Dependencies project, in that '*

 * *                      'it is intended to be a large community annotation effort with '*

 * *                      'language-universal guidelines. Further, we use the same text corpora as '*

 * *                      "Universal Dep […]*

```diff
@@ -1,10 +1,31 @@
 {
+    "__description__": "Universal Named Entity Recognition (UNER) aims to fill a gap in multilingual NLP: high quality NER datasets in many languages with a shared tagset.\nUNER is modeled after the Universal Dependencies project, in that it is intended to be a large community annotation effort with language-universal guidelines. Further, we use the same text corpora as Universal Dependencies.",
+    "__tags__": {
+        "arxiv": "2311.09122",
+        "language": [
+            "ceb",
+            "da",
+            "de",
+            "en",
+            "hr",
+            "pt",
+            "ru",
+            "sk",
+            "sr",
+            "sv",
+            "tl",
+            "zh"
+        ],
+        "license": "cc-by-sa-4.0",
+        "region": "us",
+        "task_categories": "token-classification"
+    },
     "loader": {
-        "name": "ceb_gja",
+        "name": "hr_set",
         "path": "universalner/universal_ner",
         "requirements_list": [
             "conllu"
         ],
         "type": "load_hf"
     },
     "preprocess_steps": [
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/da/ddt.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/sv/talbanken.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7053571428571429%*

 * *Differences: {"'__description__'": "'Universal Named Entity Recognition (UNER) aims to fill a gap in "*

 * *                      'multilingual NLP: high quality NER datasets in many languages with a shared '*

 * *                      'tagset.\\nUNER is modeled after the Universal Dependencies project, in that '*

 * *                      'it is intended to be a large community annotation effort with '*

 * *                      'language-universal guidelines. Further, we use the same text corpora as '*

 * *                      "Universal Dep […]*

```diff
@@ -1,10 +1,31 @@
 {
+    "__description__": "Universal Named Entity Recognition (UNER) aims to fill a gap in multilingual NLP: high quality NER datasets in many languages with a shared tagset.\nUNER is modeled after the Universal Dependencies project, in that it is intended to be a large community annotation effort with language-universal guidelines. Further, we use the same text corpora as Universal Dependencies.",
+    "__tags__": {
+        "arxiv": "2311.09122",
+        "language": [
+            "ceb",
+            "da",
+            "de",
+            "en",
+            "hr",
+            "pt",
+            "ru",
+            "sk",
+            "sr",
+            "sv",
+            "tl",
+            "zh"
+        ],
+        "license": "cc-by-sa-4.0",
+        "region": "us",
+        "task_categories": "token-classification"
+    },
     "loader": {
-        "name": "da_ddt",
+        "name": "sv_talbanken",
         "path": "universalner/universal_ner",
         "requirements_list": [
             "conllu"
         ],
         "type": "load_hf"
     },
     "preprocess_steps": [
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/de/pud.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/sk/snk.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7053571428571429%*

 * *Differences: {"'__description__'": "'Universal Named Entity Recognition (UNER) aims to fill a gap in "*

 * *                      'multilingual NLP: high quality NER datasets in many languages with a shared '*

 * *                      'tagset.\\nUNER is modeled after the Universal Dependencies project, in that '*

 * *                      'it is intended to be a large community annotation effort with '*

 * *                      'language-universal guidelines. Further, we use the same text corpora as '*

 * *                      "Universal Dep […]*

```diff
@@ -1,10 +1,31 @@
 {
+    "__description__": "Universal Named Entity Recognition (UNER) aims to fill a gap in multilingual NLP: high quality NER datasets in many languages with a shared tagset.\nUNER is modeled after the Universal Dependencies project, in that it is intended to be a large community annotation effort with language-universal guidelines. Further, we use the same text corpora as Universal Dependencies.",
+    "__tags__": {
+        "arxiv": "2311.09122",
+        "language": [
+            "ceb",
+            "da",
+            "de",
+            "en",
+            "hr",
+            "pt",
+            "ru",
+            "sk",
+            "sr",
+            "sv",
+            "tl",
+            "zh"
+        ],
+        "license": "cc-by-sa-4.0",
+        "region": "us",
+        "task_categories": "token-classification"
+    },
     "loader": {
-        "name": "de_pud",
+        "name": "sk_snk",
         "path": "universalner/universal_ner",
         "requirements_list": [
             "conllu"
         ],
         "type": "load_hf"
     },
     "preprocess_steps": [
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/en/ewt.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/sr/set.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7053571428571429%*

 * *Differences: {"'__description__'": "'Universal Named Entity Recognition (UNER) aims to fill a gap in "*

 * *                      'multilingual NLP: high quality NER datasets in many languages with a shared '*

 * *                      'tagset.\\nUNER is modeled after the Universal Dependencies project, in that '*

 * *                      'it is intended to be a large community annotation effort with '*

 * *                      'language-universal guidelines. Further, we use the same text corpora as '*

 * *                      "Universal Dep […]*

```diff
@@ -1,10 +1,31 @@
 {
+    "__description__": "Universal Named Entity Recognition (UNER) aims to fill a gap in multilingual NLP: high quality NER datasets in many languages with a shared tagset.\nUNER is modeled after the Universal Dependencies project, in that it is intended to be a large community annotation effort with language-universal guidelines. Further, we use the same text corpora as Universal Dependencies.",
+    "__tags__": {
+        "arxiv": "2311.09122",
+        "language": [
+            "ceb",
+            "da",
+            "de",
+            "en",
+            "hr",
+            "pt",
+            "ru",
+            "sk",
+            "sr",
+            "sv",
+            "tl",
+            "zh"
+        ],
+        "license": "cc-by-sa-4.0",
+        "region": "us",
+        "task_categories": "token-classification"
+    },
     "loader": {
-        "name": "en_ewt",
+        "name": "sr_set",
         "path": "universalner/universal_ner",
         "requirements_list": [
             "conllu"
         ],
         "type": "load_hf"
     },
     "preprocess_steps": [
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/en/pud.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/zh/gsdsimp.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7053571428571429%*

 * *Differences: {"'__description__'": "'Universal Named Entity Recognition (UNER) aims to fill a gap in "*

 * *                      'multilingual NLP: high quality NER datasets in many languages with a shared '*

 * *                      'tagset.\\nUNER is modeled after the Universal Dependencies project, in that '*

 * *                      'it is intended to be a large community annotation effort with '*

 * *                      'language-universal guidelines. Further, we use the same text corpora as '*

 * *                      "Universal Dep […]*

```diff
@@ -1,10 +1,31 @@
 {
+    "__description__": "Universal Named Entity Recognition (UNER) aims to fill a gap in multilingual NLP: high quality NER datasets in many languages with a shared tagset.\nUNER is modeled after the Universal Dependencies project, in that it is intended to be a large community annotation effort with language-universal guidelines. Further, we use the same text corpora as Universal Dependencies.",
+    "__tags__": {
+        "arxiv": "2311.09122",
+        "language": [
+            "ceb",
+            "da",
+            "de",
+            "en",
+            "hr",
+            "pt",
+            "ru",
+            "sk",
+            "sr",
+            "sv",
+            "tl",
+            "zh"
+        ],
+        "license": "cc-by-sa-4.0",
+        "region": "us",
+        "task_categories": "token-classification"
+    },
     "loader": {
-        "name": "en_pud",
+        "name": "zh_gsdsimp",
         "path": "universalner/universal_ner",
         "requirements_list": [
             "conllu"
         ],
         "type": "load_hf"
     },
     "preprocess_steps": [
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/hr/set.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/tl/ugnayan.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7053571428571429%*

 * *Differences: {"'__description__'": "'Universal Named Entity Recognition (UNER) aims to fill a gap in "*

 * *                      'multilingual NLP: high quality NER datasets in many languages with a shared '*

 * *                      'tagset.\\nUNER is modeled after the Universal Dependencies project, in that '*

 * *                      'it is intended to be a large community annotation effort with '*

 * *                      'language-universal guidelines. Further, we use the same text corpora as '*

 * *                      "Universal Dep […]*

```diff
@@ -1,10 +1,31 @@
 {
+    "__description__": "Universal Named Entity Recognition (UNER) aims to fill a gap in multilingual NLP: high quality NER datasets in many languages with a shared tagset.\nUNER is modeled after the Universal Dependencies project, in that it is intended to be a large community annotation effort with language-universal guidelines. Further, we use the same text corpora as Universal Dependencies.",
+    "__tags__": {
+        "arxiv": "2311.09122",
+        "language": [
+            "ceb",
+            "da",
+            "de",
+            "en",
+            "hr",
+            "pt",
+            "ru",
+            "sk",
+            "sr",
+            "sv",
+            "tl",
+            "zh"
+        ],
+        "license": "cc-by-sa-4.0",
+        "region": "us",
+        "task_categories": "token-classification"
+    },
     "loader": {
-        "name": "hr_set",
+        "name": "tl_ugnayan",
         "path": "universalner/universal_ner",
         "requirements_list": [
             "conllu"
         ],
         "type": "load_hf"
     },
     "preprocess_steps": [
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/pt/pud.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/legalbench/abercrombie.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4864285714285715%*

 * *Differences: {"'__description__'": "'LegalBench is a collection of benchmark tasks for evaluating legal "*

 * *                      "reasoning in large language models.'",*

 * * "'__tags__'": "OrderedDict([('arxiv', '2308.11462'), ('croissant', True), ('finance', True), "*

 * *               "('language', 'en'), ('law', True), ('legal', True), ('license', 'other'), "*

 * *               "('region', 'us'), ('size_categories', '10K<n<100K'), ('task_categories', "*

 * *               "['text-classification', 'question-answering', 'text-generation […]*

```diff
@@ -1,76 +1,64 @@
 {
+    "__description__": "LegalBench is a collection of benchmark tasks for evaluating legal reasoning in large language models.",
+    "__tags__": {
+        "arxiv": "2308.11462",
+        "croissant": true,
+        "finance": true,
+        "language": "en",
+        "law": true,
+        "legal": true,
+        "license": "other",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "task_categories": [
+            "text-classification",
+            "question-answering",
+            "text-generation"
+        ]
+    },
     "loader": {
-        "name": "pt_pud",
-        "path": "universalner/universal_ner",
-        "requirements_list": [
-            "conllu"
-        ],
+        "name": "abercrombie",
+        "path": "nguha/legalbench",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "field_to_field": {
-                "ner_tags": "labels"
+                "answer": "label",
+                "text": "text"
             },
             "type": "rename_fields"
         },
         {
-            "field": "labels",
-            "items_list": [
-                "O",
-                "B-PER",
-                "I-PER",
-                "B-ORG",
-                "I-ORG",
-                "B-LOC",
-                "I-LOC"
-            ],
-            "process_every_value": true,
-            "type": "get_item_by_index"
-        },
-        {
-            "begin_labels": [
-                "B-PER",
-                "B-ORG",
-                "B-LOC"
-            ],
-            "inside_labels": [
-                "I-PER",
-                "I-ORG",
-                "I-LOC"
-            ],
-            "labels": [
-                "Person",
-                "Organization",
-                "Location"
-            ],
-            "outside_label": "O",
-            "type": "iob_extractor"
-        },
-        {
-            "field_to_field": {
-                "spans/*/end": "spans_ends",
-                "spans/*/label": "labels",
-                "spans/*/start": "spans_starts"
-            },
-            "get_default": [],
-            "not_exist_ok": true,
-            "type": "copy_fields"
-        },
-        {
             "fields": {
-                "class_type": "entity type",
                 "classes": [
-                    "Person",
-                    "Organization",
-                    "Location"
+                    "generic",
+                    "descriptive",
+                    "suggestive",
+                    "arbitrary",
+                    "fanciful"
                 ],
-                "text_type": "text"
+                "classes_descriptions": "A mark is generic if it is the common name for the product. A mark is descriptive if it describes a purpose, nature, or attribute of the product. A mark is suggestive if it suggests or implies a quality or characteristic of the product. A mark is arbitrary if it is a real English word that has no relation to the product. A mark is fanciful if it is an invented word.",
+                "text_type": "products",
+                "type_of_class": "type of mark"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.span_labeling.extraction",
-    "templates": "templates.span_labeling.extraction.all",
+    "task": "tasks.classification.multi_class.with_classes_descriptions",
+    "templates": {
+        "default": {
+            "input_format": "Q: {text} What is the {type_of_class}?",
+            "instruction": "{classes_descriptions}\n\nLabel the {type_of_class} for the following {text_type}:\n",
+            "output_format": "{label}",
+            "postprocessors": [
+                "processors.take_first_non_empty_line",
+                "processors.lower_case_till_punc"
+            ],
+            "target_prefix": "A: ",
+            "title_fields": [],
+            "type": "input_output_template"
+        }
+    },
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/ru/pud.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/zh/pud.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7053571428571429%*

 * *Differences: {"'__description__'": "'Universal Named Entity Recognition (UNER) aims to fill a gap in "*

 * *                      'multilingual NLP: high quality NER datasets in many languages with a shared '*

 * *                      'tagset.\\nUNER is modeled after the Universal Dependencies project, in that '*

 * *                      'it is intended to be a large community annotation effort with '*

 * *                      'language-universal guidelines. Further, we use the same text corpora as '*

 * *                      "Universal Dep […]*

```diff
@@ -1,10 +1,31 @@
 {
+    "__description__": "Universal Named Entity Recognition (UNER) aims to fill a gap in multilingual NLP: high quality NER datasets in many languages with a shared tagset.\nUNER is modeled after the Universal Dependencies project, in that it is intended to be a large community annotation effort with language-universal guidelines. Further, we use the same text corpora as Universal Dependencies.",
+    "__tags__": {
+        "arxiv": "2311.09122",
+        "language": [
+            "ceb",
+            "da",
+            "de",
+            "en",
+            "hr",
+            "pt",
+            "ru",
+            "sk",
+            "sr",
+            "sv",
+            "tl",
+            "zh"
+        ],
+        "license": "cc-by-sa-4.0",
+        "region": "us",
+        "task_categories": "token-classification"
+    },
     "loader": {
-        "name": "ru_pud",
+        "name": "zh_pud",
         "path": "universalner/universal_ner",
         "requirements_list": [
             "conllu"
         ],
         "type": "load_hf"
     },
     "preprocess_steps": [
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/sk/snk.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/legalbench/function_of_decision_section.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48678571428571427%*

 * *Differences: {"'__description__'": "'LegalBench is a collection of benchmark tasks for evaluating legal "*

 * *                      "reasoning in large language models.'",*

 * * "'__tags__'": "OrderedDict([('arxiv', '2308.11462'), ('croissant', True), ('finance', True), "*

 * *               "('language', 'en'), ('law', True), ('legal', True), ('license', 'other'), "*

 * *               "('region', 'us'), ('size_categories', '10K<n<100K'), ('task_categories', "*

 * *               "['text-classification', 'question-answering', 'text-generation […]*

```diff
@@ -1,76 +1,68 @@
 {
+    "__description__": "LegalBench is a collection of benchmark tasks for evaluating legal reasoning in large language models.",
+    "__tags__": {
+        "arxiv": "2308.11462",
+        "croissant": true,
+        "finance": true,
+        "language": "en",
+        "law": true,
+        "legal": true,
+        "license": "other",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "task_categories": [
+            "text-classification",
+            "question-answering",
+            "text-generation"
+        ]
+    },
     "loader": {
-        "name": "sk_snk",
-        "path": "universalner/universal_ner",
-        "requirements_list": [
-            "conllu"
-        ],
+        "name": "function_of_decision_section",
+        "path": "nguha/legalbench",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "field_to_field": {
-                "ner_tags": "labels"
+                "Paragraph": "text",
+                "answer": "label"
             },
             "type": "rename_fields"
         },
         {
-            "field": "labels",
-            "items_list": [
-                "O",
-                "B-PER",
-                "I-PER",
-                "B-ORG",
-                "I-ORG",
-                "B-LOC",
-                "I-LOC"
-            ],
-            "process_every_value": true,
-            "type": "get_item_by_index"
-        },
-        {
-            "begin_labels": [
-                "B-PER",
-                "B-ORG",
-                "B-LOC"
-            ],
-            "inside_labels": [
-                "I-PER",
-                "I-ORG",
-                "I-LOC"
-            ],
-            "labels": [
-                "Person",
-                "Organization",
-                "Location"
-            ],
-            "outside_label": "O",
-            "type": "iob_extractor"
-        },
-        {
-            "field_to_field": {
-                "spans/*/end": "spans_ends",
-                "spans/*/label": "labels",
-                "spans/*/start": "spans_starts"
-            },
-            "get_default": [],
-            "not_exist_ok": true,
-            "type": "copy_fields"
-        },
-        {
             "fields": {
-                "class_type": "entity type",
                 "classes": [
-                    "Person",
-                    "Organization",
-                    "Location"
+                    "Facts",
+                    "Procedural History",
+                    "Issue",
+                    "Rule",
+                    "Analysis",
+                    "Conclusion",
+                    "Decree"
                 ],
-                "text_type": "text"
+                "classes_descriptions": "- Facts: The paragraph describes the factual background that led up to the present lawsuit.\n- Procedural History: The paragraph describes the course of litigation that led to the current proceeding before the court.\n- Issue: The paragraph describes the legal or factual issue that must be resolved by the court.\n- Rule: The paragraph describes a rule of law relevant to resolving the issue.\n- Analysis: The paragraph analyzes the legal issue by applying the relevant legal principles to the facts of the present dispute.\n- Conclusion: The paragraph presents a conclusion of the court.\n- Decree: The paragraph constitutes a decree resolving the dispute",
+                "text_type": "text",
+                "type_of_class": ""
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.span_labeling.extraction",
-    "templates": "templates.span_labeling.extraction.all",
+    "task": "tasks.classification.multi_class.with_classes_descriptions",
+    "templates": {
+        "default": {
+            "input_format": "{text_type}: {text}",
+            "instruction": "Classify the following {text_type} using the following definitions.\n\n{classes_descriptions}.\n\n",
+            "output_format": "{label}",
+            "postprocessors": [
+                "processors.take_first_non_empty_line",
+                "processors.lower_case_till_punc"
+            ],
+            "target_prefix": "Label: ",
+            "title_fields": [
+                "text_type"
+            ],
+            "type": "input_output_template"
+        }
+    },
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/sv/pud.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/universal_ner/ceb/gja.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7053571428571429%*

 * *Differences: {"'__description__'": "'Universal Named Entity Recognition (UNER) aims to fill a gap in "*

 * *                      'multilingual NLP: high quality NER datasets in many languages with a shared '*

 * *                      'tagset.\\nUNER is modeled after the Universal Dependencies project, in that '*

 * *                      'it is intended to be a large community annotation effort with '*

 * *                      'language-universal guidelines. Further, we use the same text corpora as '*

 * *                      "Universal Dep […]*

```diff
@@ -1,10 +1,31 @@
 {
+    "__description__": "Universal Named Entity Recognition (UNER) aims to fill a gap in multilingual NLP: high quality NER datasets in many languages with a shared tagset.\nUNER is modeled after the Universal Dependencies project, in that it is intended to be a large community annotation effort with language-universal guidelines. Further, we use the same text corpora as Universal Dependencies.",
+    "__tags__": {
+        "arxiv": "2311.09122",
+        "language": [
+            "ceb",
+            "da",
+            "de",
+            "en",
+            "hr",
+            "pt",
+            "ru",
+            "sk",
+            "sr",
+            "sv",
+            "tl",
+            "zh"
+        ],
+        "license": "cc-by-sa-4.0",
+        "region": "us",
+        "task_categories": "token-classification"
+    },
     "loader": {
-        "name": "sv_pud",
+        "name": "ceb_gja",
         "path": "universalner/universal_ner",
         "requirements_list": [
             "conllu"
         ],
         "type": "load_hf"
     },
     "preprocess_steps": [
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/tl/trg.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/hh_rlhf.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4630243764172336%*

 * *Differences: {"'__description__'": "'Dataset Card for HH-RLHF\\nDataset Summary\\nThis repository provides "*

 * *                      'access to two different kinds of data:\\nHuman preference data about '*

 * *                      'helpfulness and harmlessness from Training a Helpful and Harmless Assistant '*

 * *                      'with Reinforcement Learning from Human Feedback. These data are meant to '*

 * *                      'train preference (or reward) models for subsequent RLHF training. These '*

 * *                      'dat […]*

```diff
@@ -1,76 +1,83 @@
 {
+    "__description__": "Dataset Card for HH-RLHF\nDataset Summary\nThis repository provides access to two different kinds of data:\nHuman preference data about helpfulness and harmlessness from Training a Helpful and Harmless Assistant with Reinforcement Learning from Human Feedback. These data are meant to train preference (or reward) models for subsequent RLHF training. These data are not meant for supervised training of dialogue agents. Training dialogue agents on these data is likely\u2026 See the full description on the dataset page: https://huggingface.co/datasets/Anthropic/hh-rlhf.",
+    "__tags__": {
+        "arxiv": "2204.05862",
+        "croissant": true,
+        "human-feedback": true,
+        "license": "mit",
+        "region": "us"
+    },
     "loader": {
-        "name": "tl_trg",
-        "path": "universalner/universal_ner",
-        "requirements_list": [
-            "conllu"
-        ],
+        "path": "Anthropic/hh-rlhf",
         "type": "load_hf"
     },
     "preprocess_steps": [
+        "splitters.small_no_dev",
         {
-            "field_to_field": {
-                "ner_tags": "labels"
-            },
-            "type": "rename_fields"
+            "field": "chosen",
+            "type": "strip"
         },
         {
-            "field": "labels",
-            "items_list": [
-                "O",
-                "B-PER",
-                "I-PER",
-                "B-ORG",
-                "I-ORG",
-                "B-LOC",
-                "I-LOC"
-            ],
-            "process_every_value": true,
-            "type": "get_item_by_index"
+            "field": "chosen",
+            "new": "\n",
+            "old": "\n\n",
+            "type": "replace"
         },
         {
-            "begin_labels": [
-                "B-PER",
-                "B-ORG",
-                "B-LOC"
-            ],
-            "inside_labels": [
-                "I-PER",
-                "I-ORG",
-                "I-LOC"
-            ],
-            "labels": [
-                "Person",
-                "Organization",
-                "Location"
+            "by": "\nAssistant:",
+            "field": "chosen",
+            "type": "split"
+        },
+        {
+            "field": "chosen",
+            "item": -1,
+            "to_field": "output_choice",
+            "type": "get"
+        },
+        {
+            "field": "chosen",
+            "stop": -1,
+            "type": "slice"
+        },
+        {
+            "by": "\nAssistant:",
+            "field": "chosen",
+            "to_field": "input",
+            "type": "join"
+        },
+        {
+            "by": "\nAssistant:",
+            "field": "rejected",
+            "type": "split"
+        },
+        {
+            "field": "rejected",
+            "item": -1,
+            "to_field": "output_rejected",
+            "type": "get"
+        },
+        {
+            "fields": [
+                "output_choice",
+                "output_rejected"
             ],
-            "outside_label": "O",
-            "type": "iob_extractor"
+            "to_field": "choices",
+            "type": "list_field_values"
         },
         {
-            "field_to_field": {
-                "spans/*/end": "spans_ends",
-                "spans/*/label": "labels",
-                "spans/*/start": "spans_starts"
-            },
-            "get_default": [],
-            "not_exist_ok": true,
-            "type": "copy_fields"
+            "field": "choices",
+            "type": "shuffle_field_values"
         },
         {
             "fields": {
-                "class_type": "entity type",
-                "classes": [
-                    "Person",
-                    "Organization",
-                    "Location"
-                ],
-                "text_type": "text"
+                "input_type": "dialog",
+                "instruction": "Respond the following dialog in an helpful and harmfull way.",
+                "output_type": "response"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.span_labeling.extraction",
-    "templates": "templates.span_labeling.extraction.all",
+    "task": "tasks.evaluation.preference",
+    "templates": "templates.evaluation.preference.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/tl/ugnayan.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/multidoc2dial/extractive.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4791666666666667%*

 * *Differences: {"'__description__'": "'MultiDoc2Dial is a new task and dataset on modeling goal-oriented "*

 * *                      'dialogues grounded in multiple documents. Most previous works treat '*

 * *                      'document-grounded dialogue modeling as a machine reading comprehension task '*

 * *                      'based on a single given document or passage. We aim to address more '*

 * *                      'realistic scenarios where a goal-oriented information-seeking conversation '*

 * *                      "involves m […]*

```diff
@@ -1,76 +1,57 @@
 {
-    "loader": {
-        "name": "tl_ugnayan",
-        "path": "universalner/universal_ner",
-        "requirements_list": [
-            "conllu"
+    "__description__": "MultiDoc2Dial is a new task and dataset on modeling goal-oriented dialogues grounded in multiple documents. Most previous works treat document-grounded dialogue modeling as a machine reading comprehension task based on a single given document or passage. We aim to address more realistic scenarios where a goal-oriented information-seeking conversation involves multiple topics, and hence is grounded on different documents.",
+    "__tags__": {
+        "annotations_creators": "crowdsourced",
+        "arxiv": "2109.12595",
+        "croissant": true,
+        "language": "en",
+        "language_creators": [
+            "crowdsourced",
+            "expert-generated"
+        ],
+        "license": "apache-2.0",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": [
+            "10K<n<100K",
+            "1K<n<10K",
+            "n<1K"
         ],
+        "source_datasets": "extended|doc2dial",
+        "task_categories": "question-answering",
+        "task_ids": "open-domain-qa"
+    },
+    "loader": {
+        "path": "multidoc2dial",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "field_to_field": {
-                "ner_tags": "labels"
+                "answers/text/0": "relevant_context"
             },
             "type": "rename_fields"
         },
         {
-            "field": "labels",
-            "items_list": [
-                "O",
-                "B-PER",
-                "I-PER",
-                "B-ORG",
-                "I-ORG",
-                "B-LOC",
-                "I-LOC"
+            "fields": [
+                "relevant_context"
             ],
-            "process_every_value": true,
-            "type": "get_item_by_index"
+            "to_field": "answers",
+            "type": "list_field_values"
         },
         {
-            "begin_labels": [
-                "B-PER",
-                "B-ORG",
-                "B-LOC"
-            ],
-            "inside_labels": [
-                "I-PER",
-                "I-ORG",
-                "I-LOC"
-            ],
-            "labels": [
-                "Person",
-                "Organization",
-                "Location"
-            ],
-            "outside_label": "O",
-            "type": "iob_extractor"
-        },
-        {
-            "field_to_field": {
-                "spans/*/end": "spans_ends",
-                "spans/*/label": "labels",
-                "spans/*/start": "spans_starts"
-            },
-            "get_default": [],
-            "not_exist_ok": true,
-            "type": "copy_fields"
+            "expression": "question.split('[SEP]')[0]",
+            "to_field": "question",
+            "type": "execute_expression"
         },
         {
             "fields": {
-                "class_type": "entity type",
-                "classes": [
-                    "Person",
-                    "Organization",
-                    "Location"
-                ],
-                "text_type": "text"
+                "context_type": "document"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.span_labeling.extraction",
-    "templates": "templates.span_labeling.extraction.all",
+    "task": "tasks.qa.with_context.extractive",
+    "templates": "templates.qa.with_context.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/universal_ner/zh/gsdsimp.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/coqa/qa.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4642857142857143%*

 * *Differences: {"'__description__'": '\'Dataset Card for "coqa"\\nDataset Summary\\nCoQA is a large-scale dataset '*

 * *                      'for building Conversational Question Answering systems.\\nOur dataset '*

 * *                      'contains 127k questions with answers, obtained from 8k conversations about '*

 * *                      'text passages from seven diverse domains. The questions are conversational, '*

 * *                      'and the answers are free-form text with their corresponding evidence '*

 * *                      […]*

```diff
@@ -1,76 +1,89 @@
 {
-    "loader": {
-        "name": "zh_gsdsimp",
-        "path": "universalner/universal_ner",
-        "requirements_list": [
-            "conllu"
+    "__description__": "Dataset Card for \"coqa\"\nDataset Summary\nCoQA is a large-scale dataset for building Conversational Question Answering systems.\nOur dataset contains 127k questions with answers, obtained from 8k conversations about text passages from seven diverse domains. The questions are conversational, and the answers are free-form text with their corresponding evidence highlighted in the passage.\nSupported Tasks and Leaderboards\nMore Information Needed\u2026 See the full description on the dataset page: https://huggingface.co/datasets/stanfordnlp/coqa.",
+    "__tags__": {
+        "annotations_creators": "crowdsourced",
+        "arxiv": [
+            "1808.07042",
+            "1704.04683",
+            "1506.03340"
+        ],
+        "conversational-qa": true,
+        "croissant": true,
+        "language": "en",
+        "language_creators": "found",
+        "license": "other",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "1K<n<10K",
+        "source_datasets": [
+            "extended|race",
+            "extended|cnn_dailymail",
+            "extended|wikipedia",
+            "extended|other"
         ],
+        "task_categories": "question-answering",
+        "task_ids": "extractive-qa"
+    },
+    "loader": {
+        "path": "stanfordnlp/coqa",
         "type": "load_hf"
     },
     "preprocess_steps": [
+        "splitters.small_no_test",
         {
-            "field_to_field": {
-                "ner_tags": "labels"
+            "fields": {
+                "context_type": "story"
             },
-            "type": "rename_fields"
+            "type": "add_fields"
         },
         {
-            "field": "labels",
-            "items_list": [
-                "O",
-                "B-PER",
-                "I-PER",
-                "B-ORG",
-                "I-ORG",
-                "B-LOC",
-                "I-LOC"
+            "fields": [
+                "questions",
+                "answers/input_text"
             ],
+            "to_field": "dialog",
+            "type": "zip_field_values"
+        },
+        {
+            "field": "dialog",
             "process_every_value": true,
-            "type": "get_item_by_index"
+            "type": "dictify",
+            "with_keys": [
+                "user",
+                "system"
+            ]
         },
         {
-            "begin_labels": [
-                "B-PER",
-                "B-ORG",
-                "B-LOC"
-            ],
-            "inside_labels": [
-                "I-PER",
-                "I-ORG",
-                "I-LOC"
-            ],
-            "labels": [
-                "Person",
-                "Organization",
-                "Location"
-            ],
-            "outside_label": "O",
-            "type": "iob_extractor"
+            "field": "dialog",
+            "type": "duplicate_by_sub_lists"
+        },
+        {
+            "field": "dialog",
+            "item": -1,
+            "to_field": "last_turn",
+            "type": "get"
         },
         {
             "field_to_field": {
-                "spans/*/end": "spans_ends",
-                "spans/*/label": "labels",
-                "spans/*/start": "spans_starts"
+                "last_turn/system": "answer",
+                "last_turn/user": "question"
             },
-            "get_default": [],
-            "not_exist_ok": true,
             "type": "copy_fields"
         },
         {
-            "fields": {
-                "class_type": "entity type",
-                "classes": [
-                    "Person",
-                    "Organization",
-                    "Location"
-                ],
-                "text_type": "text"
-            },
-            "type": "add_fields"
+            "field": "answer",
+            "inside": "list",
+            "to_field": "answers",
+            "type": "wrap"
+        },
+        {
+            "context_field": "story",
+            "field": "dialog",
+            "to_field": "context",
+            "type": "serialize_dialog"
         }
     ],
-    "task": "tasks.span_labeling.extraction",
-    "templates": "templates.span_labeling.extraction.all",
+    "task": "tasks.qa.with_context.extractive",
+    "templates": "templates.qa.with_context.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/wikitq.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/college_biology.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6160714285714286%*

 * *Differences: {"'__description__'": "'Dataset Card for MMLU\\nDataset Summary\\nMeasuring Massive Multitask "*

 * *                      'Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy '*

 * *                      'Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\\nThis is '*

 * *                      'a massive multitask test consisting of multiple-choice questions from '*

 * *                      'various branches of knowledge. The test spans subjects in the humanities, '*

 * *                      […]*

```diff
@@ -1,48 +1,44 @@
 {
-    "__description__": "The WikiTableQuestions dataset is a large-scale dataset for the task of question answering on semi-structured tables.",
+    "__description__": "Dataset Card for MMLU\nDataset Summary\nMeasuring Massive Multitask Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\nThis is a massive multitask test consisting of multiple-choice questions from various branches of knowledge. The test spans subjects in the humanities, social sciences, hard sciences, and other areas that are important for some people to learn. This covers 57\u2026 See the full description on the dataset page: https://huggingface.co/datasets/cais/mmlu.",
     "__tags__": {
-        "languages": [
-            "english"
+        "annotations_creators": "no-annotation",
+        "arxiv": [
+            "2009.03300",
+            "2005.00700",
+            "2005.14165",
+            "2008.02275"
         ],
-        "modality": "table",
-        "urls": {
-            "arxiv": "https://arxiv.org/abs/1508.00305"
-        }
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "mit",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": "multiple-choice-qa"
     },
     "loader": {
-        "path": "wikitablequestions",
+        "name": "college_biology",
+        "path": "cais/mmlu",
         "type": "load_hf"
     },
     "preprocess_steps": [
-        "splitters.small_no_test",
         {
-            "fields": {
-                "context_type": "table"
+            "mapper": {
+                "dev": "train"
             },
-            "type": "add_fields"
-        },
-        {
-            "max_length": 15,
-            "table": "table",
-            "text_output": "answers",
-            "type": "truncate_table_cells"
+            "type": "rename_splits"
         },
         {
-            "field": "table",
-            "rows_to_keep": 50,
-            "type": "truncate_table_rows"
-        },
-        {
-            "field_to_field": [
-                [
-                    "table",
-                    "context"
-                ]
-            ],
-            "type": "serialize_table_as_indexed_row_major"
+            "fields": {
+                "topic": "college biology"
+            },
+            "type": "add_fields"
         }
     ],
-    "task": "tasks.qa.with_context.extractive",
-    "templates": "templates.qa.with_context.all",
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/winogrande/xl.json` & `unitxt-1.9.0/src/unitxt/catalog/metrics/rag/bert_k_precision_ml.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.15238095238095237%*

 * *Differences: {"'main_score'": "'precision'",*

 * * "'metric'": "'metrics.bert_score.deberta_v3_base_mnli_xnli_ml'",*

 * * "'preprocess_steps'": "{0: {'type': 'copy_fields', 'field_to_field': [['contexts', "*

 * *                       "'references']], delete: ['fields']}, 1: {'type': 'copy_fields', "*

 * *                       "'field_to_field': [['answer', 'prediction']]}, delete: [3, 1, 0]}",*

 * * "'type'": "'metric_pipeline'",*

 * * 'delete': "['loader', 'task', 'templates']"}*

```diff
@@ -1,38 +1,25 @@
 {
-    "loader": {
-        "name": "winogrande_xl",
-        "path": "winogrande",
-        "type": "load_hf"
-    },
+    "main_score": "precision",
+    "metric": "metrics.bert_score.deberta_v3_base_mnli_xnli_ml",
     "preprocess_steps": [
-        "splitters.small_no_test",
         {
-            "fields": [
-                "option1",
-                "option2"
+            "field_to_field": [
+                [
+                    "contexts",
+                    "references"
+                ]
             ],
-            "to_field": "choices",
-            "type": "list_field_values"
+            "type": "copy_fields"
         },
         {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
-            "field_to_field": {
-                "sentence": "question"
-            },
-            "type": "rename_fields"
+            "field_to_field": [
+                [
+                    "answer",
+                    "prediction"
+                ]
+            ],
+            "type": "copy_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.open",
-    "templates": "templates.qa.multiple_choice.open.all",
-    "type": "task_card"
+    "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/winogrande/xs.json` & `unitxt-1.9.0/src/unitxt/catalog/metrics/rag/bert_k_precision.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.15238095238095237%*

 * *Differences: {"'main_score'": "'precision'",*

 * * "'metric'": "'metrics.bert_score.deberta_large_mnli'",*

 * * "'preprocess_steps'": "{0: {'type': 'copy_fields', 'field_to_field': [['contexts', "*

 * *                       "'references']], delete: ['fields']}, 1: {'type': 'copy_fields', "*

 * *                       "'field_to_field': [['answer', 'prediction']]}, delete: [3, 1, 0]}",*

 * * "'type'": "'metric_pipeline'",*

 * * 'delete': "['loader', 'task', 'templates']"}*

```diff
@@ -1,38 +1,25 @@
 {
-    "loader": {
-        "name": "winogrande_xs",
-        "path": "winogrande",
-        "type": "load_hf"
-    },
+    "main_score": "precision",
+    "metric": "metrics.bert_score.deberta_large_mnli",
     "preprocess_steps": [
-        "splitters.small_no_test",
         {
-            "fields": [
-                "option1",
-                "option2"
+            "field_to_field": [
+                [
+                    "contexts",
+                    "references"
+                ]
             ],
-            "to_field": "choices",
-            "type": "list_field_values"
+            "type": "copy_fields"
         },
         {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
-            "field_to_field": {
-                "sentence": "question"
-            },
-            "type": "rename_fields"
+            "field_to_field": [
+                [
+                    "answer",
+                    "prediction"
+                ]
+            ],
+            "type": "copy_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.open",
-    "templates": "templates.qa.multiple_choice.open.all",
-    "type": "task_card"
+    "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/wnli/truthfulness.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/yahoo_answers_topics.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48578869047619044%*

 * *Differences: {"'__description__'": "'Yahoo! Answers Topic Classification is text classification dataset. The "*

 * *                      'dataset is the Yahoo! Answers corpus as of 10/25/2007. The Yahoo! Answers '*

 * *                      'topic classification dataset is constructed using 10 largest main '*

 * *                      'categories. From all the answers and other meta-information, this dataset '*

 * *                      "only used the best answer content and the main category information.'",*

 * * "'__tags__'": "OrderedDict([( […]*

```diff
@@ -1,41 +1,94 @@
 {
+    "__description__": "Yahoo! Answers Topic Classification is text classification dataset. The dataset is the Yahoo! Answers corpus as of 10/25/2007. The Yahoo! Answers topic classification dataset is constructed using 10 largest main categories. From all the answers and other meta-information, this dataset only used the best answer content and the main category information.",
+    "__tags__": {
+        "annotations_creators": "found",
+        "croissant": true,
+        "language": "en",
+        "language_creators": "found",
+        "license": "unknown",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "1M<n<10M",
+        "source_datasets": "extended|other-yahoo-answers-corpus",
+        "task_categories": "text-classification",
+        "task_ids": "topic-classification"
+    },
     "loader": {
-        "name": "wnli",
-        "path": "glue",
+        "path": "yahoo_answers_topics",
         "type": "load_hf"
     },
     "preprocess_steps": [
-        "splitters.small_no_test",
+        {
+            "page_size": 9223372036854775807,
+            "type": "shuffle"
+        },
+        {
+            "mix": {
+                "test": "test",
+                "train": "train[87.5%]",
+                "validation": "train[12.5%]"
+            },
+            "type": "split_random_mix"
+        },
         {
             "field_to_field": {
-                "sentence1": "text_a",
-                "sentence2": "text_b"
+                "topic": "label"
             },
             "type": "rename_fields"
         },
         {
             "mappers": {
                 "label": {
-                    "0": "yes",
-                    "1": "no"
+                    "0": "Society & Culture",
+                    "1": "Science & Mathematics",
+                    "2": "Health",
+                    "3": "Education & Reference",
+                    "4": "Computers & Internet",
+                    "5": "Sports",
+                    "6": "Business & Finance",
+                    "7": "Entertainment & Music",
+                    "8": "Family & Relationships",
+                    "9": "Politics & Government"
                 }
             },
             "type": "map_instance_values"
         },
         {
+            "fields": [
+                "question_title",
+                "question_content",
+                "best_answer"
+            ],
+            "to_field": "text",
+            "type": "list_field_values"
+        },
+        {
+            "field": "text",
+            "separator": " ",
+            "to_field": "text",
+            "type": "join_str"
+        },
+        {
             "fields": {
                 "classes": [
-                    "yes",
-                    "no"
+                    "Society & Culture",
+                    "Science & Mathematics",
+                    "Health",
+                    "Education & Reference",
+                    "Computers & Internet",
+                    "Sports",
+                    "Business & Finance",
+                    "Entertainment & Music",
+                    "Family & Relationships",
+                    "Politics & Government"
                 ],
-                "text_a_type": "premise",
-                "text_b_type": "hypothesis",
-                "type_of_relation": "truthfulness"
+                "text_type": "text",
+                "type_of_class": "topic"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.classification.multi_class.relation",
-    "templates": "templates.classification.multi_class.relation.truthfulness.all",
+    "task": "tasks.classification.multi_class",
+    "templates": "templates.classification.multi_class.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/wsc.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/abstract_algebra.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.498015873015873%*

 * *Differences: {"'__description__'": "'Dataset Card for MMLU\\nDataset Summary\\nMeasuring Massive Multitask "*

 * *                      'Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy '*

 * *                      'Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\\nThis is '*

 * *                      'a massive multitask test consisting of multiple-choice questions from '*

 * *                      'various branches of knowledge. The test spans subjects in the humanities, '*

 * *                      […]*

```diff
@@ -1,54 +1,44 @@
 {
+    "__description__": "Dataset Card for MMLU\nDataset Summary\nMeasuring Massive Multitask Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\nThis is a massive multitask test consisting of multiple-choice questions from various branches of knowledge. The test spans subjects in the humanities, social sciences, hard sciences, and other areas that are important for some people to learn. This covers 57\u2026 See the full description on the dataset page: https://huggingface.co/datasets/cais/mmlu.",
+    "__tags__": {
+        "annotations_creators": "no-annotation",
+        "arxiv": [
+            "2009.03300",
+            "2005.00700",
+            "2005.14165",
+            "2008.02275"
+        ],
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "mit",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": "multiple-choice-qa"
+    },
     "loader": {
-        "name": "wsc",
-        "path": "super_glue",
+        "name": "abstract_algebra",
+        "path": "cais/mmlu",
         "type": "load_hf"
     },
     "preprocess_steps": [
-        "splitters.small_no_test",
         {
-            "mappers": {
-                "label": {
-                    "0": "False",
-                    "1": "True"
-                }
+            "mapper": {
+                "dev": "train"
             },
-            "type": "map_instance_values"
+            "type": "rename_splits"
         },
         {
             "fields": {
-                "choices": [
-                    "False",
-                    "True"
-                ]
+                "topic": "abstract algebra"
             },
             "type": "add_fields"
         }
     ],
-    "task": {
-        "inputs": [
-            "choices",
-            "text",
-            "span1_text",
-            "span2_text"
-        ],
-        "metrics": [
-            "metrics.accuracy"
-        ],
-        "outputs": [
-            "label"
-        ],
-        "type": "form_task"
-    },
-    "templates": {
-        "items": [
-            {
-                "input_format": "Given this sentence: {text} classify if \"{span2_text}\" refers to \"{span1_text}\".",
-                "output_format": "{label}",
-                "type": "input_output_template"
-            }
-        ],
-        "type": "templates_list"
-    },
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/azerbaijani.json` & `unitxt-1.9.0/src/unitxt/catalog/templates/summarization/abstractive/all.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.08333333333333333%*

 * *Differences: {"'items'": "['templates.summarization.abstractive.formal', "*

 * *            "'templates.summarization.abstractive.formal_without_label', "*

 * *            "'templates.summarization.abstractive.casual', "*

 * *            "'templates.summarization.abstractive.professional', "*

 * *            "'templates.summarization.abstractive.instructive', "*

 * *            "'templates.summarization.abstractive.full', "*

 * *            "'templates.summarization.abstractive.one_sentence', "*

 * *            "'templates.summarization.abstractive.passi […]*

```diff
@@ -1,25 +1,15 @@
 {
-    "loader": {
-        "name": "azerbaijani",
-        "path": "GEM/xlsum",
-        "type": "load_hf"
-    },
-    "preprocess_steps": [
-        {
-            "field_to_field": {
-                "target": "summary",
-                "text": "document"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "fields": {
-                "document_type": "document"
-            },
-            "type": "add_fields"
-        }
+    "items": [
+        "templates.summarization.abstractive.formal",
+        "templates.summarization.abstractive.formal_without_label",
+        "templates.summarization.abstractive.casual",
+        "templates.summarization.abstractive.professional",
+        "templates.summarization.abstractive.instructive",
+        "templates.summarization.abstractive.full",
+        "templates.summarization.abstractive.one_sentence",
+        "templates.summarization.abstractive.passive",
+        "templates.summarization.abstractive.write_succinct",
+        "templates.summarization.abstractive.title"
     ],
-    "task": "tasks.summarization.abstractive",
-    "templates": "templates.summarization.abstractive.all",
-    "type": "task_card"
+    "type": "templates_list"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/chinese_traditional.json` & `unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/match.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.038461538461538464%*

 * *Differences: {"'choices_separator'": "'\\n'",*

 * * "'input_format'": "'{context_type}:\\n{context}\\nQuestion:\\n{question}\\nChoices:\\n{choices}'",*

 * * "'instruction'": "'Answer the multiple choice Question about {topic} from one of the Choices "*

 * *                  "(choose from {numerals}) based on the {context_type}.'",*

 * * "'postprocessors'": "['processors.take_first_non_empty_line', 'processors.match_closest_option']",*

 * * "'target_choice_format'": "'{choice_numeral}. {choice_text}'",*

 * * "'target_field'": "'answer'",*

 * * "'target_pr […]*

```diff
@@ -1,25 +1,16 @@
 {
-    "loader": {
-        "name": "chinese_traditional",
-        "path": "GEM/xlsum",
-        "type": "load_hf"
-    },
-    "preprocess_steps": [
-        {
-            "field_to_field": {
-                "target": "summary",
-                "text": "document"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "fields": {
-                "document_type": "document"
-            },
-            "type": "add_fields"
-        }
+    "choices_separator": "\n",
+    "input_format": "{context_type}:\n{context}\nQuestion:\n{question}\nChoices:\n{choices}",
+    "instruction": "Answer the multiple choice Question about {topic} from one of the Choices (choose from {numerals}) based on the {context_type}.",
+    "postprocessors": [
+        "processors.take_first_non_empty_line",
+        "processors.match_closest_option"
     ],
-    "task": "tasks.summarization.abstractive",
-    "templates": "templates.summarization.abstractive.all",
-    "type": "task_card"
+    "target_choice_format": "{choice_numeral}. {choice_text}",
+    "target_field": "answer",
+    "target_prefix": "Answer:\n",
+    "title_fields": [
+        "context_type"
+    ],
+    "type": "multiple_choice_template"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/xlsum/korean.json` & `unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_label/instruction.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.045454545454545456%*

 * *Differences: {"'input_format'": "'Text: {text}'",*

 * * "'instruction'": "'What are the {type_of_classes} expressed in following {text_type}?\\nSelect "*

 * *                  'your answer from the options: {classes}.\\nIf no {type_of_classes} are '*

 * *                  "expressed answer none.'",*

 * * "'labels_field'": "'labels'",*

 * * "'output_format'": "'{labels}'",*

 * * "'postprocessors'": "['processors.take_first_non_empty_line', 'processors.lower_case', "*

 * *                     "'processors.to_list_by_comma', 'processors.remove_none_from_lis […]*

```diff
@@ -1,25 +1,14 @@
 {
-    "loader": {
-        "name": "korean",
-        "path": "GEM/xlsum",
-        "type": "load_hf"
-    },
-    "preprocess_steps": [
-        {
-            "field_to_field": {
-                "target": "summary",
-                "text": "document"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "fields": {
-                "document_type": "document"
-            },
-            "type": "add_fields"
-        }
+    "input_format": "Text: {text}",
+    "instruction": "What are the {type_of_classes} expressed in following {text_type}?\nSelect your answer from the options: {classes}.\nIf no {type_of_classes} are expressed answer none.",
+    "labels_field": "labels",
+    "output_format": "{labels}",
+    "postprocessors": [
+        "processors.take_first_non_empty_line",
+        "processors.lower_case",
+        "processors.to_list_by_comma",
+        "processors.remove_none_from_list"
     ],
-    "task": "tasks.summarization.abstractive",
-    "templates": "templates.summarization.abstractive.all",
-    "type": "task_card"
+    "target_prefix": "The {type_of_classes} is ",
+    "type": "multi_label_template"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/xnli/ar.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/telugu.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4976190476190476%*

 * *Differences: {"'__description__'": "'We present XLSum, a comprehensive and diverse dataset comprising 1.35 "*

 * *                      'million professionally\\nannotated article-summary pairs from BBC, '*

 * *                      'extracted using a set of carefully designed heuristics.\\nThe dataset '*

 * *                      'covers 45 languages ranging from low to high-resource, for many of which '*

 * *                      'no\\npublic dataset is currently available. XL-Sum is highly abstractive, '*

 * *                      'concise,\ […]*

```diff
@@ -1,49 +1,39 @@
 {
+    "__description__": "We present XLSum, a comprehensive and diverse dataset comprising 1.35 million professionally\nannotated article-summary pairs from BBC, extracted using a set of carefully designed heuristics.\nThe dataset covers 45 languages ranging from low to high-resource, for many of which no\npublic dataset is currently available. XL-Sum is highly abstractive, concise,\nand of high quality, as indicated by human and intrinsic evaluation.",
+    "__tags__": {
+        "annotations_creators": "none",
+        "arxiv": "1607.01759",
+        "croissant": true,
+        "language": "und",
+        "language_creators": "unknown",
+        "license": "cc-by-nc-sa-4.0",
+        "multilinguality": "unknown",
+        "region": "us",
+        "size_categories": "unknown",
+        "source_datasets": "original",
+        "task_categories": "summarization"
+    },
     "loader": {
-        "name": "ar",
-        "path": "xnli",
+        "name": "telugu",
+        "path": "GEM/xlsum",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mapper": {
-                "validation_matched": "validation"
-            },
-            "type": "rename_splits"
-        },
-        "splitters.small_no_test",
-        {
             "field_to_field": {
-                "hypothesis": "text_b",
-                "premise": "text_a"
+                "target": "summary",
+                "text": "document"
             },
             "type": "rename_fields"
         },
         {
-            "mappers": {
-                "label": {
-                    "0": "entailment",
-                    "1": "neutral",
-                    "2": "contradiction"
-                }
-            },
-            "type": "map_instance_values"
-        },
-        {
             "fields": {
-                "classes": [
-                    "entailment",
-                    "neutral",
-                    "contradiction"
-                ],
-                "text_a_type": "premise",
-                "text_b_type": "hypothesis",
-                "type_of_relation": "entailment"
+                "document_type": "document"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.classification.multi_class.relation",
-    "templates": "templates.classification.multi_class.relation.all",
+    "task": "tasks.summarization.abstractive",
+    "templates": "templates.summarization.abstractive.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/xnli/bg.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/serbian_latin.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4976190476190476%*

 * *Differences: {"'__description__'": "'We present XLSum, a comprehensive and diverse dataset comprising 1.35 "*

 * *                      'million professionally\\nannotated article-summary pairs from BBC, '*

 * *                      'extracted using a set of carefully designed heuristics.\\nThe dataset '*

 * *                      'covers 45 languages ranging from low to high-resource, for many of which '*

 * *                      'no\\npublic dataset is currently available. XL-Sum is highly abstractive, '*

 * *                      'concise,\ […]*

```diff
@@ -1,49 +1,39 @@
 {
+    "__description__": "We present XLSum, a comprehensive and diverse dataset comprising 1.35 million professionally\nannotated article-summary pairs from BBC, extracted using a set of carefully designed heuristics.\nThe dataset covers 45 languages ranging from low to high-resource, for many of which no\npublic dataset is currently available. XL-Sum is highly abstractive, concise,\nand of high quality, as indicated by human and intrinsic evaluation.",
+    "__tags__": {
+        "annotations_creators": "none",
+        "arxiv": "1607.01759",
+        "croissant": true,
+        "language": "und",
+        "language_creators": "unknown",
+        "license": "cc-by-nc-sa-4.0",
+        "multilinguality": "unknown",
+        "region": "us",
+        "size_categories": "unknown",
+        "source_datasets": "original",
+        "task_categories": "summarization"
+    },
     "loader": {
-        "name": "bg",
-        "path": "xnli",
+        "name": "serbian_latin",
+        "path": "GEM/xlsum",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mapper": {
-                "validation_matched": "validation"
-            },
-            "type": "rename_splits"
-        },
-        "splitters.small_no_test",
-        {
             "field_to_field": {
-                "hypothesis": "text_b",
-                "premise": "text_a"
+                "target": "summary",
+                "text": "document"
             },
             "type": "rename_fields"
         },
         {
-            "mappers": {
-                "label": {
-                    "0": "entailment",
-                    "1": "neutral",
-                    "2": "contradiction"
-                }
-            },
-            "type": "map_instance_values"
-        },
-        {
             "fields": {
-                "classes": [
-                    "entailment",
-                    "neutral",
-                    "contradiction"
-                ],
-                "text_a_type": "premise",
-                "text_b_type": "hypothesis",
-                "type_of_relation": "entailment"
+                "document_type": "document"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.classification.multi_class.relation",
-    "templates": "templates.classification.multi_class.relation.all",
+    "task": "tasks.summarization.abstractive",
+    "templates": "templates.summarization.abstractive.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/xnli/de.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/high_school_us_history.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4976190476190476%*

 * *Differences: {"'__description__'": "'Dataset Card for MMLU\\nDataset Summary\\nMeasuring Massive Multitask "*

 * *                      'Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy '*

 * *                      'Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\\nThis is '*

 * *                      'a massive multitask test consisting of multiple-choice questions from '*

 * *                      'various branches of knowledge. The test spans subjects in the humanities, '*

 * *                      […]*

```diff
@@ -1,49 +1,44 @@
 {
+    "__description__": "Dataset Card for MMLU\nDataset Summary\nMeasuring Massive Multitask Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\nThis is a massive multitask test consisting of multiple-choice questions from various branches of knowledge. The test spans subjects in the humanities, social sciences, hard sciences, and other areas that are important for some people to learn. This covers 57\u2026 See the full description on the dataset page: https://huggingface.co/datasets/cais/mmlu.",
+    "__tags__": {
+        "annotations_creators": "no-annotation",
+        "arxiv": [
+            "2009.03300",
+            "2005.00700",
+            "2005.14165",
+            "2008.02275"
+        ],
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "mit",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": "multiple-choice-qa"
+    },
     "loader": {
-        "name": "de",
-        "path": "xnli",
+        "name": "high_school_us_history",
+        "path": "cais/mmlu",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "validation_matched": "validation"
+                "dev": "train"
             },
             "type": "rename_splits"
         },
-        "splitters.small_no_test",
-        {
-            "field_to_field": {
-                "hypothesis": "text_b",
-                "premise": "text_a"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "mappers": {
-                "label": {
-                    "0": "entailment",
-                    "1": "neutral",
-                    "2": "contradiction"
-                }
-            },
-            "type": "map_instance_values"
-        },
         {
             "fields": {
-                "classes": [
-                    "entailment",
-                    "neutral",
-                    "contradiction"
-                ],
-                "text_a_type": "premise",
-                "text_b_type": "hypothesis",
-                "type_of_relation": "entailment"
+                "topic": "high school us history"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.classification.multi_class.relation",
-    "templates": "templates.classification.multi_class.relation.all",
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/xnli/el.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/human_aging.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4976190476190476%*

 * *Differences: {"'__description__'": "'Dataset Card for MMLU\\nDataset Summary\\nMeasuring Massive Multitask "*

 * *                      'Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy '*

 * *                      'Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\\nThis is '*

 * *                      'a massive multitask test consisting of multiple-choice questions from '*

 * *                      'various branches of knowledge. The test spans subjects in the humanities, '*

 * *                      […]*

```diff
@@ -1,49 +1,44 @@
 {
+    "__description__": "Dataset Card for MMLU\nDataset Summary\nMeasuring Massive Multitask Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\nThis is a massive multitask test consisting of multiple-choice questions from various branches of knowledge. The test spans subjects in the humanities, social sciences, hard sciences, and other areas that are important for some people to learn. This covers 57\u2026 See the full description on the dataset page: https://huggingface.co/datasets/cais/mmlu.",
+    "__tags__": {
+        "annotations_creators": "no-annotation",
+        "arxiv": [
+            "2009.03300",
+            "2005.00700",
+            "2005.14165",
+            "2008.02275"
+        ],
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "mit",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": "multiple-choice-qa"
+    },
     "loader": {
-        "name": "el",
-        "path": "xnli",
+        "name": "human_aging",
+        "path": "cais/mmlu",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "validation_matched": "validation"
+                "dev": "train"
             },
             "type": "rename_splits"
         },
-        "splitters.small_no_test",
-        {
-            "field_to_field": {
-                "hypothesis": "text_b",
-                "premise": "text_a"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "mappers": {
-                "label": {
-                    "0": "entailment",
-                    "1": "neutral",
-                    "2": "contradiction"
-                }
-            },
-            "type": "map_instance_values"
-        },
         {
             "fields": {
-                "classes": [
-                    "entailment",
-                    "neutral",
-                    "contradiction"
-                ],
-                "text_a_type": "premise",
-                "text_b_type": "hypothesis",
-                "type_of_relation": "entailment"
+                "topic": "human aging"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.classification.multi_class.relation",
-    "templates": "templates.classification.multi_class.relation.all",
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/xnli/sw.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/mmlu/moral_scenarios.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4976190476190476%*

 * *Differences: {"'__description__'": "'Dataset Card for MMLU\\nDataset Summary\\nMeasuring Massive Multitask "*

 * *                      'Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy '*

 * *                      'Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\\nThis is '*

 * *                      'a massive multitask test consisting of multiple-choice questions from '*

 * *                      'various branches of knowledge. The test spans subjects in the humanities, '*

 * *                      […]*

```diff
@@ -1,49 +1,44 @@
 {
+    "__description__": "Dataset Card for MMLU\nDataset Summary\nMeasuring Massive Multitask Language Understanding by Dan Hendrycks, Collin Burns, Steven Basart, Andy Zou, Mantas Mazeika, Dawn Song, and Jacob Steinhardt (ICLR 2021).\nThis is a massive multitask test consisting of multiple-choice questions from various branches of knowledge. The test spans subjects in the humanities, social sciences, hard sciences, and other areas that are important for some people to learn. This covers 57\u2026 See the full description on the dataset page: https://huggingface.co/datasets/cais/mmlu.",
+    "__tags__": {
+        "annotations_creators": "no-annotation",
+        "arxiv": [
+            "2009.03300",
+            "2005.00700",
+            "2005.14165",
+            "2008.02275"
+        ],
+        "croissant": true,
+        "language": "en",
+        "language_creators": "expert-generated",
+        "license": "mit",
+        "multilinguality": "monolingual",
+        "region": "us",
+        "size_categories": "10K<n<100K",
+        "source_datasets": "original",
+        "task_categories": "question-answering",
+        "task_ids": "multiple-choice-qa"
+    },
     "loader": {
-        "name": "sw",
-        "path": "xnli",
+        "name": "moral_scenarios",
+        "path": "cais/mmlu",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
             "mapper": {
-                "validation_matched": "validation"
+                "dev": "train"
             },
             "type": "rename_splits"
         },
-        "splitters.small_no_test",
-        {
-            "field_to_field": {
-                "hypothesis": "text_b",
-                "premise": "text_a"
-            },
-            "type": "rename_fields"
-        },
-        {
-            "mappers": {
-                "label": {
-                    "0": "entailment",
-                    "1": "neutral",
-                    "2": "contradiction"
-                }
-            },
-            "type": "map_instance_values"
-        },
         {
             "fields": {
-                "classes": [
-                    "entailment",
-                    "neutral",
-                    "contradiction"
-                ],
-                "text_a_type": "premise",
-                "text_b_type": "hypothesis",
-                "type_of_relation": "entailment"
+                "topic": "moral scenarios"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.classification.multi_class.relation",
-    "templates": "templates.classification.multi_class.relation.all",
+    "task": "tasks.qa.multiple_choice.with_topic",
+    "templates": "templates.qa.multiple_choice.with_topic.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/xnli/vi.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/portuguese.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4976190476190476%*

 * *Differences: {"'__description__'": "'We present XLSum, a comprehensive and diverse dataset comprising 1.35 "*

 * *                      'million professionally\\nannotated article-summary pairs from BBC, '*

 * *                      'extracted using a set of carefully designed heuristics.\\nThe dataset '*

 * *                      'covers 45 languages ranging from low to high-resource, for many of which '*

 * *                      'no\\npublic dataset is currently available. XL-Sum is highly abstractive, '*

 * *                      'concise,\ […]*

```diff
@@ -1,49 +1,39 @@
 {
+    "__description__": "We present XLSum, a comprehensive and diverse dataset comprising 1.35 million professionally\nannotated article-summary pairs from BBC, extracted using a set of carefully designed heuristics.\nThe dataset covers 45 languages ranging from low to high-resource, for many of which no\npublic dataset is currently available. XL-Sum is highly abstractive, concise,\nand of high quality, as indicated by human and intrinsic evaluation.",
+    "__tags__": {
+        "annotations_creators": "none",
+        "arxiv": "1607.01759",
+        "croissant": true,
+        "language": "und",
+        "language_creators": "unknown",
+        "license": "cc-by-nc-sa-4.0",
+        "multilinguality": "unknown",
+        "region": "us",
+        "size_categories": "unknown",
+        "source_datasets": "original",
+        "task_categories": "summarization"
+    },
     "loader": {
-        "name": "vi",
-        "path": "xnli",
+        "name": "portuguese",
+        "path": "GEM/xlsum",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "mapper": {
-                "validation_matched": "validation"
-            },
-            "type": "rename_splits"
-        },
-        "splitters.small_no_test",
-        {
             "field_to_field": {
-                "hypothesis": "text_b",
-                "premise": "text_a"
+                "target": "summary",
+                "text": "document"
             },
             "type": "rename_fields"
         },
         {
-            "mappers": {
-                "label": {
-                    "0": "entailment",
-                    "1": "neutral",
-                    "2": "contradiction"
-                }
-            },
-            "type": "map_instance_values"
-        },
-        {
             "fields": {
-                "classes": [
-                    "entailment",
-                    "neutral",
-                    "contradiction"
-                ],
-                "text_a_type": "premise",
-                "text_b_type": "hypothesis",
-                "type_of_relation": "entailment"
+                "document_type": "document"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.classification.multi_class.relation",
-    "templates": "templates.classification.multi_class.relation.all",
+    "task": "tasks.summarization.abstractive",
+    "templates": "templates.summarization.abstractive.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/xwinogrande/en.json` & `unitxt-1.9.0/src/unitxt/catalog/metrics/rag/answer_correctness.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.1547619047619048%*

 * *Differences: {"'main_score'": "'recall'",*

 * * "'metric'": "'metrics.token_overlap'",*

 * * "'preprocess_steps'": "{0: {'type': 'copy_fields', 'field_to_field': [['ground_truths', "*

 * *                       "'references']], delete: ['fields']}, 1: {'type': 'copy_fields', "*

 * *                       "'field_to_field': [['answer', 'prediction']]}, delete: [2, 0]}",*

 * * "'type'": "'metric_pipeline'",*

 * * 'delete': "['loader', 'task', 'templates']"}*

```diff
@@ -1,37 +1,25 @@
 {
-    "loader": {
-        "name": "en",
-        "path": "Muennighoff/xwinograd",
-        "type": "load_hf"
-    },
+    "main_score": "recall",
+    "metric": "metrics.token_overlap",
     "preprocess_steps": [
         {
-            "fields": [
-                "option1",
-                "option2"
+            "field_to_field": [
+                [
+                    "ground_truths",
+                    "references"
+                ]
             ],
-            "to_field": "choices",
-            "type": "list_field_values"
+            "type": "copy_fields"
         },
         {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
-            "field_to_field": {
-                "sentence": "question"
-            },
-            "type": "rename_fields"
+            "field_to_field": [
+                [
+                    "answer",
+                    "prediction"
+                ]
+            ],
+            "type": "copy_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.open",
-    "templates": "templates.qa.multiple_choice.open.all",
-    "type": "task_card"
+    "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/xwinogrande/jp.json` & `unitxt-1.9.0/src/unitxt/catalog/metrics/rag/recall.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.1547619047619048%*

 * *Differences: {"'main_score'": "'recall'",*

 * * "'metric'": "'metrics.token_overlap'",*

 * * "'preprocess_steps'": "{0: {'type': 'copy_fields', 'field_to_field': [['ground_truths', "*

 * *                       "'references']], delete: ['fields']}, 1: {'type': 'copy_fields', "*

 * *                       "'field_to_field': [['answer', 'prediction']]}, delete: [2, 0]}",*

 * * "'type'": "'metric_pipeline'",*

 * * 'delete': "['loader', 'task', 'templates']"}*

```diff
@@ -1,37 +1,25 @@
 {
-    "loader": {
-        "name": "jp",
-        "path": "Muennighoff/xwinograd",
-        "type": "load_hf"
-    },
+    "main_score": "recall",
+    "metric": "metrics.token_overlap",
     "preprocess_steps": [
         {
-            "fields": [
-                "option1",
-                "option2"
+            "field_to_field": [
+                [
+                    "ground_truths",
+                    "references"
+                ]
             ],
-            "to_field": "choices",
-            "type": "list_field_values"
+            "type": "copy_fields"
         },
         {
-            "fields": {
-                "answer": "int"
-            },
-            "type": "cast_fields"
-        },
-        {
-            "add": -1,
-            "field": "answer",
-            "type": "add_constant"
-        },
-        {
-            "field_to_field": {
-                "sentence": "question"
-            },
-            "type": "rename_fields"
+            "field_to_field": [
+                [
+                    "answer",
+                    "prediction"
+                ]
+            ],
+            "type": "copy_fields"
         }
     ],
-    "task": "tasks.qa.multiple_choice.open",
-    "templates": "templates.qa.multiple_choice.open.all",
-    "type": "task_card"
+    "type": "metric_pipeline"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/cards/yahoo_answers_topics.json` & `unitxt-1.9.0/src/unitxt/catalog/cards/xlsum/chinese_simplified.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4795918367346939%*

 * *Differences: {"'__description__'": "'We present XLSum, a comprehensive and diverse dataset comprising 1.35 "*

 * *                      'million professionally\\nannotated article-summary pairs from BBC, '*

 * *                      'extracted using a set of carefully designed heuristics.\\nThe dataset '*

 * *                      'covers 45 languages ranging from low to high-resource, for many of which '*

 * *                      'no\\npublic dataset is currently available. XL-Sum is highly abstractive, '*

 * *                      'concise,\ […]*

```diff
@@ -1,80 +1,39 @@
 {
+    "__description__": "We present XLSum, a comprehensive and diverse dataset comprising 1.35 million professionally\nannotated article-summary pairs from BBC, extracted using a set of carefully designed heuristics.\nThe dataset covers 45 languages ranging from low to high-resource, for many of which no\npublic dataset is currently available. XL-Sum is highly abstractive, concise,\nand of high quality, as indicated by human and intrinsic evaluation.",
+    "__tags__": {
+        "annotations_creators": "none",
+        "arxiv": "1607.01759",
+        "croissant": true,
+        "language": "und",
+        "language_creators": "unknown",
+        "license": "cc-by-nc-sa-4.0",
+        "multilinguality": "unknown",
+        "region": "us",
+        "size_categories": "unknown",
+        "source_datasets": "original",
+        "task_categories": "summarization"
+    },
     "loader": {
-        "path": "yahoo_answers_topics",
+        "name": "chinese_simplified",
+        "path": "GEM/xlsum",
         "type": "load_hf"
     },
     "preprocess_steps": [
         {
-            "page_size": 9223372036854775807,
-            "type": "shuffle"
-        },
-        {
-            "mix": {
-                "test": "test",
-                "train": "train[87.5%]",
-                "validation": "train[12.5%]"
-            },
-            "type": "split_random_mix"
-        },
-        {
             "field_to_field": {
-                "topic": "label"
+                "target": "summary",
+                "text": "document"
             },
             "type": "rename_fields"
         },
         {
-            "mappers": {
-                "label": {
-                    "0": "Society & Culture",
-                    "1": "Science & Mathematics",
-                    "2": "Health",
-                    "3": "Education & Reference",
-                    "4": "Computers & Internet",
-                    "5": "Sports",
-                    "6": "Business & Finance",
-                    "7": "Entertainment & Music",
-                    "8": "Family & Relationships",
-                    "9": "Politics & Government"
-                }
-            },
-            "type": "map_instance_values"
-        },
-        {
-            "fields": [
-                "question_title",
-                "question_content",
-                "best_answer"
-            ],
-            "to_field": "text",
-            "type": "list_field_values"
-        },
-        {
-            "field": "text",
-            "separator": " ",
-            "to_field": "text",
-            "type": "join_str"
-        },
-        {
             "fields": {
-                "classes": [
-                    "Society & Culture",
-                    "Science & Mathematics",
-                    "Health",
-                    "Education & Reference",
-                    "Computers & Internet",
-                    "Sports",
-                    "Business & Finance",
-                    "Entertainment & Music",
-                    "Family & Relationships",
-                    "Politics & Government"
-                ],
-                "text_type": "text",
-                "type_of_class": "topic"
+                "document_type": "document"
             },
             "type": "add_fields"
         }
     ],
-    "task": "tasks.classification.multi_class",
-    "templates": "templates.classification.multi_class.all",
+    "task": "tasks.summarization.abstractive",
+    "templates": "templates.summarization.abstractive.all",
     "type": "task_card"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/metrics/rag/answer_correctness.json` & `unitxt-1.9.0/src/unitxt/catalog/metrics/rag/bert_recall.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'metric'": "'metrics.bert_score.deberta_large_mnli'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "main_score": "recall",
-    "metric": "metrics.token_overlap",
+    "metric": "metrics.bert_score.deberta_large_mnli",
     "preprocess_steps": [
         {
             "field_to_field": [
                 [
                     "ground_truths",
                     "references"
                 ]
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/metrics/rag/context_correctness.json` & `unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/title.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.045454545454545456%*

 * *Differences: {"'choices_separator'": "'\\n'",*

 * * "'input_format'": "'{context_type}:\\n{context}\\nQuestion:\\n{question}\\nChoices:\\n{choices}'",*

 * * "'instruction'": "'Answer the multiple choice Question from one of the Choices (choose from "*

 * *                  "{numerals}) based on the {context_type}.'",*

 * * "'postprocessors'": "['processors.to_string_stripped', 'processors.first_character']",*

 * * "'target_field'": "'answer'",*

 * * "'target_prefix'": "'Answer:\\n'",*

 * * "'title_fields'": "['context_type']",*

 * * "'type'": "'multiple_choic […]*

```diff
@@ -1,25 +1,15 @@
 {
-    "main_score": "score",
-    "metric": "metrics.mrr",
-    "preprocess_steps": [
-        {
-            "field_to_field": [
-                [
-                    "context_ids",
-                    "prediction"
-                ]
-            ],
-            "type": "copy_fields"
-        },
-        {
-            "field_to_field": [
-                [
-                    "ground_truths_context_ids",
-                    "references"
-                ]
-            ],
-            "type": "copy_fields"
-        }
+    "choices_separator": "\n",
+    "input_format": "{context_type}:\n{context}\nQuestion:\n{question}\nChoices:\n{choices}",
+    "instruction": "Answer the multiple choice Question from one of the Choices (choose from {numerals}) based on the {context_type}.",
+    "postprocessors": [
+        "processors.to_string_stripped",
+        "processors.first_character"
     ],
-    "type": "metric_pipeline"
+    "target_field": "answer",
+    "target_prefix": "Answer:\n",
+    "title_fields": [
+        "context_type"
+    ],
+    "type": "multiple_choice_template"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/metrics/rag/context_relevance.json` & `unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/with_topic/title.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.045454545454545456%*

 * *Differences: {"'choices_separator'": "'\\n'",*

 * * "'input_format'": "'{context_type}:\\n{context}\\nQuestion:\\n{question}\\nChoices:\\n{choices}'",*

 * * "'instruction'": "'Answer the multiple choice Question about {topic} from one of the Choices "*

 * *                  "(choose from {numerals}) based on the {context_type}.'",*

 * * "'postprocessors'": "['processors.to_string_stripped', 'processors.first_character']",*

 * * "'target_field'": "'answer'",*

 * * "'target_prefix'": "'Answer:\\n'",*

 * * "'title_fields'": "['context_type']",*

 * * "'type'": "' […]*

```diff
@@ -1,25 +1,15 @@
 {
-    "main_score": "perplexity",
-    "metric": "metrics.perplexity_q.flan_t5_small",
-    "preprocess_steps": [
-        {
-            "field_to_field": [
-                [
-                    "contexts",
-                    "references"
-                ]
-            ],
-            "type": "copy_fields"
-        },
-        {
-            "field_to_field": [
-                [
-                    "question",
-                    "prediction"
-                ]
-            ],
-            "type": "copy_fields"
-        }
+    "choices_separator": "\n",
+    "input_format": "{context_type}:\n{context}\nQuestion:\n{question}\nChoices:\n{choices}",
+    "instruction": "Answer the multiple choice Question about {topic} from one of the Choices (choose from {numerals}) based on the {context_type}.",
+    "postprocessors": [
+        "processors.to_string_stripped",
+        "processors.first_character"
     ],
-    "type": "metric_pipeline"
+    "target_field": "answer",
+    "target_prefix": "Answer:\n",
+    "title_fields": [
+        "context_type"
+    ],
+    "type": "multiple_choice_template"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/processors/to_span_label_pairs.json` & `unitxt-1.9.0/src/unitxt/catalog/processors/to_span_label_pairs.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/catalog/processors/to_span_label_pairs_surface_only.json` & `unitxt-1.9.0/src/unitxt/catalog/processors/to_span_label_pairs_surface_only.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/catalog/system_prompts/models/labradorite.json` & `unitxt-1.9.0/src/unitxt/catalog/system_prompts/models/labradorite.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/catalog/system_prompts/models/llama.json` & `unitxt-1.9.0/src/unitxt/catalog/system_prompts/models/llama.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/catalog/system_prompts/models/llama2.json` & `unitxt-1.9.0/src/unitxt/catalog/system_prompts/models/llama2.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/all.json` & `unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_class/relation/truthfulness/all.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_label/default.json` & `unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_label/default.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/catalog/templates/classification/multi_label/instruction.json` & `unitxt-1.9.0/src/unitxt/catalog/templates/classification/multi_label/title.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'input_format'": "'{text_type}: {text}'",*

 * * "'target_prefix'": "'{type_of_classes}:\\n'",*

 * * "'title_fields'": "['type_of_classes', 'text_type']"}*

```diff
@@ -1,14 +1,18 @@
 {
-    "input_format": "Text: {text}",
+    "input_format": "{text_type}: {text}",
     "instruction": "What are the {type_of_classes} expressed in following {text_type}?\nSelect your answer from the options: {classes}.\nIf no {type_of_classes} are expressed answer none.",
     "labels_field": "labels",
     "output_format": "{labels}",
     "postprocessors": [
         "processors.take_first_non_empty_line",
         "processors.lower_case",
         "processors.to_list_by_comma",
         "processors.remove_none_from_list"
     ],
-    "target_prefix": "The {type_of_classes} is ",
+    "target_prefix": "{type_of_classes}:\n",
+    "title_fields": [
+        "type_of_classes",
+        "text_type"
+    ],
     "type": "multi_label_template"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/templates/evaluation/preference/default.json` & `unitxt-1.9.0/src/unitxt/catalog/templates/evaluation/preference/default.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/match.json` & `unitxt-1.9.0/src/unitxt/catalog/templates/qa/multiple_choice/with_context/match.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/catalog/templates/qa/multiple_choice/with_context/title.json` & `unitxt-1.9.0/src/unitxt/catalog/templates/selection/by_attribute/default.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.55%*

 * *Differences: {"'choices_field'": "'choices_texts'",*

 * * "'input_format'": "'{choices_text_type}:\\n{choices_texts}'",*

 * * "'instruction'": "'Which of the {choices_text_type} is the most {required_attribute}, please "*

 * *                  "respond with: {numerals}.'",*

 * * "'shuffle_choices'": 'True',*

 * * "'target_field'": "'choice'",*

 * * "'target_prefix'": "'Most {required_attribute}:\\n'",*

 * * "'title_fields'": "['choices_text_type']"}*

```diff
@@ -1,15 +1,17 @@
 {
+    "choices_field": "choices_texts",
     "choices_separator": "\n",
-    "input_format": "{context_type}:\n{context}\nQuestion:\n{question}\nChoices:\n{choices}",
-    "instruction": "Answer the multiple choice Question from one of the Choices (choose from {numerals}) based on the {context_type}.",
+    "input_format": "{choices_text_type}:\n{choices_texts}",
+    "instruction": "Which of the {choices_text_type} is the most {required_attribute}, please respond with: {numerals}.",
     "postprocessors": [
         "processors.to_string_stripped",
         "processors.first_character"
     ],
-    "target_field": "answer",
-    "target_prefix": "Answer:\n",
+    "shuffle_choices": true,
+    "target_field": "choice",
+    "target_prefix": "Most {required_attribute}:\n",
     "title_fields": [
-        "context_type"
+        "choices_text_type"
     ],
     "type": "multiple_choice_template"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/templates/rag/model_response_assessment/llm_as_judge_using_mt_bench_template.json` & `unitxt-1.9.0/src/unitxt/catalog/templates/response_assessment/rating/mt_bench_single_turn.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6%*

 * *Differences: {"'input_format'": '"[Question]\\n{question}\\n\\n[The Start of Assistant\'s '*

 * *                   'Answer]\\n{answer}\\n[The End of Assistant\'s Answer]"',*

 * * "'instruction'": "'Please act as an impartial judge and evaluate the quality of the response "*

 * *                  'provided by an AI assistant to the user question displayed below. Your '*

 * *                  'evaluation should consider factors such as the helpfulness, relevance, '*

 * *                  'accuracy, depth, creativity, and level of detail of the r […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "input_format": "[Question]\n{question}\n\n[The Start of Assistant's Answer]\n{model_output}\n[The End of Assistant's Answer]",
-    "instruction": "Please act as an impartial judge and evaluate the quality of the response provided by an AI assistant to the user question displayed below. Your evaluation should consider factors such as the helpfulness, relevance, accuracy, depth, creativity,  and level of detail of the response. Begin your evaluation by providing a short explanation. Be as objective as possible. After providing your explanation, you must rate the response on a scale of 1 to 10 by strictly following this format: \"[[rating]]\", for example: \"[[5]]\".\n\n",
-    "output_format": "{rating_label}",
+    "input_format": "[Question]\n{question}\n\n[The Start of Assistant's Answer]\n{answer}\n[The End of Assistant's Answer]",
+    "instruction": "Please act as an impartial judge and evaluate the quality of the response provided by an AI assistant to the user question displayed below. Your evaluation should consider factors such as the helpfulness, relevance, accuracy, depth, creativity, and level of detail of the response. Begin your evaluation by providing a short explanation. Be as objective as possible. After providing your explanation, you must rate the response on a scale of 1 to 10 by strictly following this format: \"[[rating]]\", for example: \"Rating: [[5]]\".\n\n",
+    "output_format": "[[{rating}]]",
     "postprocessors": [
-        "processors.extract_mt_bench_judgment"
+        "processors.extract_mt_bench_rating_judgment"
     ],
     "type": "input_output_template"
 }
```

### Comparing `unitxt-1.8.1/src/unitxt/catalog/templates/regression/two_texts/similarity/flan.json` & `unitxt-1.9.0/src/unitxt/catalog/templates/regression/two_texts/similarity/flan.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/catalog/templates/targeted_sentiment_extraction/all.json` & `unitxt-1.9.0/src/unitxt/catalog/templates/targeted_sentiment_extraction/all.json`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/catalog.py` & `unitxt-1.9.0/src/unitxt/catalog.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/collections.py` & `unitxt-1.9.0/src/unitxt/collections.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/collections_operators.py` & `unitxt-1.9.0/src/unitxt/collections_operators.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/dataclass.py` & `unitxt-1.9.0/src/unitxt/dataclass.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/dataset.py` & `unitxt-1.9.0/src/unitxt/dataset.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/dataset_utils.py` & `unitxt-1.9.0/src/unitxt/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/deprecation_utils.py` & `unitxt-1.9.0/src/unitxt/deprecation_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/dialog_operators.py` & `unitxt-1.9.0/src/unitxt/dialog_operators.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/dict_utils.py` & `unitxt-1.9.0/src/unitxt/dict_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/eval_utils.py` & `unitxt-1.9.0/src/unitxt/eval_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/file_utils.py` & `unitxt-1.9.0/src/unitxt/file_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/formats.py` & `unitxt-1.9.0/src/unitxt/formats.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,17 +110,17 @@
                 "target": "2",
                 "source": "Instruction: Solve the math exercises.\n\nInput: 1+2\nOutput: 3\n\nInput: 4-2\nOutput: 2\n\nInput: 1+1\nOutput: ",
             }
 
     """
 
     demos_field: str = "demos"
-    demo_format: str = "{source}\n{target_prefix}{target}\n\n"  #  example: "User: {source}\nAgent: {target}\n\n"
+    demo_format: str = "{source}\\N{target_prefix}{target}\n\n"  #  example: "User: {source}\nAgent: {target}\n\n"
     model_input_format: str = (
-        "{system_prompt}{instruction}{demos}{source}\n{target_prefix}"
+        "{system_prompt}\\N{instruction}\\N{demos}{source}\\N{target_prefix}"
     )
     format_args: Dict[str, str] = OptionalField(default_factory=dict)
 
     @staticmethod
     def _retrieve_field_and_assert_not_none(instance, field_name) -> str:
         if field_name is not None and field_name in instance:
             field_value = instance[field_name]
```

### Comparing `unitxt-1.8.1/src/unitxt/generator_utils.py` & `unitxt-1.9.0/src/unitxt/generator_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/hf_utils.py` & `unitxt-1.9.0/src/unitxt/hf_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/loaders.py` & `unitxt-1.9.0/src/unitxt/loaders.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,26 +23,26 @@
 ------------------------
 """
 import itertools
 import os
 import tempfile
 from pathlib import Path
 from tempfile import TemporaryDirectory
-from typing import Dict, List, Mapping, Optional, Sequence, Union
+from typing import Any, Dict, List, Mapping, Optional, Sequence, Union
 
 import pandas as pd
 from datasets import load_dataset as hf_load_dataset
 from tqdm import tqdm
 
 from .dataclass import InternalField, OptionalField
 from .fusion import FixedFusion
 from .logging_utils import get_logger
 from .operator import SourceOperator
 from .settings_utils import get_settings
-from .stream import MultiStream, Stream
+from .stream import GeneratorStream, MultiStream
 
 logger = get_logger()
 settings = get_settings()
 
 
 class Loader(SourceOperator):
     # The loader_limit an optional parameter used to control the maximum number of instances to load from the the source.
@@ -176,15 +176,15 @@
     def split_limited_load(self, split_name):
         yield from itertools.islice(self._cache[split_name], self.get_limit())
 
     def limited_load(self):
         self.log_limited_loading()
         return MultiStream(
             {
-                name: Stream(
+                name: GeneratorStream(
                     generator=self.split_limited_load, gen_kwargs={"split_name": name}
                 )
                 for name in self._cache.keys()
             }
         )
 
     def process(self):
@@ -236,22 +236,26 @@
 
         yield from self._cache[file]
 
     def process(self):
         if self.streaming:
             return MultiStream(
                 {
-                    name: Stream(generator=self.stream_csv, gen_kwargs={"file": file})
+                    name: GeneratorStream(
+                        generator=self.stream_csv, gen_kwargs={"file": file}
+                    )
                     for name, file in self.files.items()
                 }
             )
 
         return MultiStream(
             {
-                name: Stream(generator=self.load_csv, gen_kwargs={"file": file})
+                name: GeneratorStream(
+                    generator=self.load_csv, gen_kwargs={"file": file}
+                )
                 for name, file in self.files.items()
             }
         )
 
 
 class LoadFromSklearn(Loader):
     dataset_name: str
@@ -468,9 +472,32 @@
 
     """
 
     sources: List[Loader]
 
     def process(self):
         return FixedFusion(
-            origins=self.sources, max_instances_per_origin=self.get_limit()
+            origins=self.sources, max_instances_per_origin_split=self.get_limit()
         ).process()
+
+
+class LoadFromDictionary(Loader):
+    """Allows loading data from dictionary of constants.
+
+    The loader can be used, for example, when debugging or working with small datasets.
+
+    Attributes:
+        data (Dict[str, List[Dict[str, Any]]]): a dictionary of constants from which the data will be loaded
+
+    Examples:
+        data = {
+            "train": {"input": "SomeInput1", "output": "SomeResult1"},
+            "test": {"input": "SomeInput2", "output": "SomeResult2"},
+        }
+        loader = LoadFromDictionary(data=data)
+        multi_stream = loader.process()
+    """
+
+    data: Dict[str, List[Dict[str, Any]]]
+
+    def process(self) -> MultiStream:
+        return MultiStream.from_iterables(self.data)
```

### Comparing `unitxt-1.8.1/src/unitxt/logging_utils.py` & `unitxt-1.9.0/src/unitxt/logging_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/metric.py` & `unitxt-1.9.0/src/unitxt/metric.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/metrics.py` & `unitxt-1.9.0/src/unitxt/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import string
 import uuid
 import warnings
 from abc import ABC, abstractmethod
-from collections import Counter
+from collections import Counter, defaultdict
 from copy import deepcopy
 from dataclasses import field
 from statistics import mean
 from typing import Any, Dict, Generator, List, Optional, Tuple
 
 import evaluate
 import numpy
@@ -911,19 +911,23 @@
                 "score": {
                     "instance": {
                         score_name: group_aggregation_func(
                             score_dict
                             if uses_subgroups
                             else score_dict[default_subgroup_name]
                         )
-                        for score_name, score_dict in group_scores.items()
+                        for score_name, score_dict in group_to_instance_scores[
+                            group_name
+                        ].items()
                     }
                 }
             }
-            for group_scores in group_to_instance_scores.values()
+            for group_name in sorted(
+                group_to_instance_scores.keys()
+            )  # sorted for consistency
         ]
 
     def _set_up_group_mean_aggregation(
         self, instances, reduction_params, reduction_fields
     ):
         group_aggregation_func = reduction_params["agg_func"][1]
         # if treat groups as units
@@ -973,14 +977,48 @@
             )
         }
         result["score"] = result[self.main_score]
         result["score_name"] = self.main_score
         return result
 
 
+class JaccardIndex(InstanceMetric):
+    reduction_map = {"mean": ["jaccard_index"]}
+    main_score = "jaccard_index"
+    ci_scores = ["jaccard_index"]
+
+    prediction_type = "Any"  # string representation is compared
+
+    def compute(
+        self, references: List[Any], prediction: Any, task_data: List[Dict]
+    ) -> dict:
+        if not isinstance(prediction, set):
+            prediction = set(prediction)
+        references = [set(reference) for reference in references]
+
+        result = {
+            self.main_score: max(
+                [
+                    float(
+                        (len(reference.intersection(prediction)))
+                        / (
+                            len(reference)
+                            + len(prediction)
+                            - len(reference.intersection(prediction))
+                        )
+                    )
+                    for reference in references
+                ]
+            )
+        }
+        result["score"] = result[self.main_score]
+        result["score_name"] = self.main_score
+        return result
+
+
 class MaxAccuracy(Accuracy):
     """Calculate the maximal accuracy over all instances as the global score."""
 
     reduction_map = {"max": ["accuracy"]}
 
 
 class UnsortedListExactMatch(InstanceMetric):
@@ -1270,18 +1308,21 @@
     main_score = "f1_binary"
     average = None
     threshold = 0.5
     prediction_type = "Union[float, int]"
     _metric = None
     metric = "f1"
     single_reference_per_prediction = True
+    _requirements_list: List[str] = ["sklearn"]
 
     def prepare(self):
         super().prepare()
-        self._metric = evaluate.load(self.metric)
+        from sklearn import metrics
+
+        self._metric = metrics.precision_recall_fscore_support
 
     def _validate_reference(self, reference):
         super()._validate_reference(reference)
         assert reference[0] in [
             0,
             1,
         ], f"all references of {self.main_score} must by 0 or 1"
@@ -1290,27 +1331,35 @@
         self,
         references: List[List[str]],
         predictions: List[str],
         task_data: List[Dict],
     ) -> dict:
         flattened_int_references = [int(r[0]) for r in references]
         int_predictions = [int(p > self.threshold) for p in predictions]
-
-        result = self._metric.compute(
-            references=flattened_int_references,
-            predictions=int_predictions,
+        precision, recall, f1, _ = self._metric(
+            y_true=flattened_int_references,
+            y_pred=int_predictions,
             labels=[0, 1],
             average=self.average,
         )
-        if isinstance(result[self.metric], numpy.ndarray):
+        if self.average is None:
             return {
-                self.main_score: result[self.metric][1],
-                f"{self.main_score}_neg": result[self.metric][0],
+                "f1_binary": f1[1],
+                "f1_binary_neg": f1[0],
+                "recall_binary": recall[1],
+                "recall_binary_neg": recall[0],
+                "precision_binary": precision[1],
+                "precision_binary_neg": precision[0],
             }
-        return {self.main_score: result[self.metric]}
+        return {"f1_binary": f1, "recall_binary": recall, "precision_binary": precision}
+
+
+class F1BinaryPosOnly(F1Binary):
+    average = "binary"
+    main_score = "f1_binary"
 
 
 class RecallBinary(F1Binary):
     main_score = "recall_binary"
     metric = "recall"
 
 
@@ -3354,48 +3403,53 @@
 
 
 class BinaryMaxF1(F1Binary):
     """Calculate the maximal F1 and the decision threshold that achieves it for a binary task with float predictions."""
 
     main_score = "max_f1_binary"
     single_reference_per_prediction = True
+    average = None
 
     def compute(
         self,
         references: List[List[float]],
         predictions: List[List[float]],
         task_data: List[Dict],
     ) -> dict:
         best_thr = -1
-        best_f1 = -1
+        best_f1 = defaultdict(lambda: -1)
         best_thr_neg = -1
-        best_f1_neg = -1
+        best_f1_neg = defaultdict(lambda: -1)
         thrs = {round(fp, 3) for fp in predictions}
         for thr in thrs:
             new_predictions = [
                 1.0 if float_prediction >= thr else 0.0
                 for float_prediction in predictions
             ]
             f1_results = super().compute(references, new_predictions, task_data)
 
-            f1 = f1_results[self.main_score]
-            if f1 > best_f1:
-                best_f1 = f1
+            f1 = f1_results["f1_binary"]
+            if f1 > best_f1["f1_binary"]:
+                best_f1 = f1_results.copy()
                 best_thr = thr
 
-            f1_neg = f1_results[f"{self.main_score}_neg"]
-            if f1_neg > best_f1_neg:
-                best_f1_neg = f1_neg
+            f1_neg = f1_results["f1_binary_neg"]
+            if f1_neg > best_f1_neg["f1_binary_neg"]:
+                best_f1_neg = f1_results.copy()
                 best_thr_neg = thr
 
         return {
-            self.main_score: best_f1,
+            self.main_score: best_f1["f1_binary"],
             "best_thr_maxf1": best_thr,
-            f"{self.main_score}_neg": best_f1_neg,
+            f"{self.main_score}_neg": best_f1_neg["f1_binary_neg"],
             "best_thr_maxf1_neg": best_thr_neg,
+            "recall_at_max_f1": best_f1["recall_binary"],
+            "recall_at_max_f1_neg": best_f1_neg["recall_binary_neg"],
+            "precision_at_max_f1": best_f1["precision_binary"],
+            "precision_at_max_f1_neg": best_f1_neg["precision_binary_neg"],
         }
 
 
 class BinaryAccuracy(InstanceMetric):
     """Calculate accuracy for a binary task, using 0.5 as the threshold in the case of float predictions."""
 
     reduction_map = {"mean": ["accuracy_binary"]}
```

### Comparing `unitxt-1.8.1/src/unitxt/normalizers.py` & `unitxt-1.9.0/src/unitxt/normalizers.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/operator.py` & `unitxt-1.9.0/src/unitxt/operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from abc import abstractmethod
 from dataclasses import field
 from typing import Any, Dict, Generator, List, Optional, Union
 
 from .artifact import Artifact
 from .dataclass import InternalField, NonPositionalField
-from .stream import MultiStream, Stream
+from .stream import GeneratorStream, MultiStream, Stream
 from .utils import is_module_available
 
 
 class Operator(Artifact):
     pass
 
 
@@ -167,15 +167,17 @@
 
 
 def instance_generator(instance):
     yield instance
 
 
 def stream_single(instance: Dict[str, Any]) -> Stream:
-    return Stream(generator=instance_generator, gen_kwargs={"instance": instance})
+    return GeneratorStream(
+        generator=instance_generator, gen_kwargs={"instance": instance}
+    )
 
 
 class MultiStreamOperator(StreamingOperator):
     """A class representing a multi-stream operator in the streaming system.
 
     A multi-stream operator is a type of `StreamingOperator` that operates on an entire MultiStream object at once. It takes a `MultiStream` as input and produces a `MultiStream` as output. The `process` method should be implemented by subclasses to define the specific operations to be performed on the input `MultiStream`.
     """
@@ -240,15 +242,15 @@
             result[stream_name] = stream
 
         return MultiStream(result)
 
     def _process_single_stream(
         self, stream: Stream, stream_name: Optional[str] = None
     ) -> Stream:
-        return Stream(
+        return GeneratorStream(
             self._process_stream,
             gen_kwargs={"stream": stream, "stream_name": stream_name},
         )
 
     def _is_should_be_processed(self, stream_name):
         if (
             self.apply_to_streams is not None
@@ -441,15 +443,15 @@
     In order to make this efficient and to avoid qudratic complexity, it caches the accessible streams by default.
     """
 
     def __call__(self, multi_stream: Optional[MultiStream] = None) -> MultiStream:
         result = {}
 
         for stream_name, stream in multi_stream.items():
-            stream = Stream(
+            stream = GeneratorStream(
                 self.generator,
                 gen_kwargs={"stream": stream, "multi_stream": multi_stream},
             )
             result[stream_name] = stream
 
         return MultiStream(result)
```

### Comparing `unitxt-1.8.1/src/unitxt/operators.py` & `unitxt-1.9.0/src/unitxt/operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 ------------------------
 """
 import copy
 import operator
 import uuid
 import zipfile
 from abc import abstractmethod
-from collections import Counter
+from collections import Counter, defaultdict
 from copy import deepcopy
 from dataclasses import field
 from itertools import zip_longest
 from random import Random
 from typing import (
     Any,
     Callable,
@@ -71,15 +71,15 @@
     SourceOperator,
     StreamingOperator,
     StreamInitializerOperator,
     StreamInstanceOperator,
 )
 from .random_utils import new_random_generator
 from .settings_utils import get_settings
-from .stream import Stream
+from .stream import GeneratorStream, Stream
 from .text_utils import nested_tuple_to_string
 from .type_utils import isoftype
 from .utils import flatten_dict
 
 settings = get_settings()
 
 
@@ -486,15 +486,15 @@
 
 
 class Augmentor(StreamInstanceOperator):
     """A stream operator that augments the values of either the task input fields before rendering with the template,  or the input passed to the model after rendering of the template.
 
     Args:
         augment_model_input: Whether to augment the input to the model.
-        augment_task_input:  Whether to augment the task input fields.  The specific fields are defined in the FormTask operator.
+        augment_task_input:  Whether to augment the task input fields.  The specific fields are defined in the Task operator.
 
     """
 
     augment_task_input: bool = False
     augment_model_input: bool = False
 
     def verify(self):
@@ -521,15 +521,15 @@
 
     def process(
         self, instance: Dict[str, Any], stream_name: Optional[str] = None
     ) -> Dict[str, Any]:
         if self.augment_task_input:
             assert (
                 len(self._task_input_fields) > 0
-            ), "No augmentable input fields were defined in FormTask, and augmentation was requested. Specify the fields to augment in 'argumentable_inputs' attribute of the FormTask."
+            ), "No augmentable input fields were defined in Task, and augmentation was requested. Specify the fields to augment in 'argumentable_inputs' attribute of the Task."
             fields = self._task_input_fields
             assert not self.augment_model_input
 
         if self.augment_model_input:
             fields = ["source"]
             assert not self.augment_task_input
 
@@ -856,14 +856,59 @@
             zipped = zip_longest(*values)
         else:
             zipped = zip(*values)
         instance[self.to_field] = list(zipped)
         return instance
 
 
+class InterleaveListsToDialogOperator(StreamInstanceOperator):
+    """Interleaves two lists, one of user dialog turns and one of assistant dialog turns, into a single list of tuples, alternating between "user" and "assistant".
+
+     The list of tuples if of format (role, turn_content), where the role label is specified by
+     the 'user_role_label' and 'assistant_role_label' fields (default to "user" and "assistant").
+
+    The user turns and assistant turns field are specified in the arguments.
+     The value of each of the 'fields' is assumed to be a list.
+
+    """
+
+    user_turns_field: str
+    assistant_turns_field: str
+    user_role_label: str = "user"
+    assistant_role_label: str = "assistant"
+    to_field: str
+
+    def process(
+        self, instance: Dict[str, Any], stream_name: Optional[str] = None
+    ) -> Dict[str, Any]:
+        user_turns = instance[self.user_turns_field]
+        assistant_turns = instance[self.assistant_turns_field]
+
+        assert (
+            len(user_turns) == len(assistant_turns)
+            or (len(user_turns) - len(assistant_turns) == 1)
+        ), "user_turns must have either the same length as assistant_turns or one more turn."
+
+        interleaved_dialog = []
+        i, j = 0, 0  # Indices for the user and assistant lists
+        # While either list has elements left, continue interleaving
+        while i < len(user_turns) or j < len(assistant_turns):
+            if i < len(user_turns):
+                interleaved_dialog.append((self.user_role_label, user_turns[i]))
+                i += 1
+            if j < len(assistant_turns):
+                interleaved_dialog.append(
+                    (self.assistant_role_label, assistant_turns[j])
+                )
+                j += 1
+
+        instance[self.to_field] = interleaved_dialog
+        return instance
+
+
 class IndexOf(StreamInstanceOperator):
     """For a given instance, finds the offset of value of field 'index_of', within the value of field 'search_in'."""
 
     search_in: str
     index_of: str
     to_field: str
     use_query: bool = DeprecatedField(
@@ -1556,14 +1601,60 @@
                     stream_name + "_" + nested_tuple_to_string(unique_values)
                 )
                 result[filtered_stream_name] = filtered_streams
 
         return MultiStream(result)
 
 
+class SplitByNestedGroup(MultiStreamOperator):
+    """Splits a MultiStream that is small - for metrics, hence: whole stream can sit in memory, split by the value of field 'group'.
+
+    Args:
+        number_of_fusion_generations: int
+
+    the value in field group is of the form "sourcen/sourcenminus1/..." describing the sources in which the instance sat
+    when these were fused, potentially several phases of fusion. the name of the most recent source sits first in this value.
+    (See BaseFusion and its extensions)
+    number_of_fuaion_generations  specifies the length of the prefix by which to split the stream.
+    E.g. for number_of_fusion_generations = 1, only the most recent fusion in creating this multi_stream, affects the splitting.
+    For number_of_fusion_generations = -1, take the whole history written in this field, ignoring number of generations.
+    """
+
+    field_name_of_group: str = "group"
+    number_of_fusion_generations: int = 1
+
+    def process(self, multi_stream: MultiStream) -> MultiStream:
+        result = defaultdict(list)
+
+        for stream_name, stream in multi_stream.items():
+            for instance in stream:
+                if self.field_name_of_group not in instance:
+                    raise ValueError(
+                        f"Field {self.field_name_of_group} is missing from instance {instance}"
+                    )
+                signature = (
+                    stream_name
+                    + "~"  #  a sign that does not show within group values
+                    + (
+                        "/".join(
+                            instance[self.field_name_of_group].split("/")[
+                                : self.number_of_fusion_generations
+                            ]
+                        )
+                        if self.number_of_fusion_generations >= 0
+                        # for values with a smaller number of generations - take up to their last generation
+                        else instance[self.field_name_of_group]
+                        # for each instance - take all its generations
+                    )
+                )
+                result[signature].append(instance)
+
+        return MultiStream.from_iterables(result)
+
+
 class ApplyStreamOperatorsField(SingleStreamOperator, ArtifactFetcherMixin):
     """Applies stream operators to a stream based on specified fields in each instance.
 
     Args:
         field (str): The field containing the operators to be applied.
         reversed (bool): Whether to apply the operators in reverse order.
     """
@@ -1664,26 +1755,26 @@
     """
 
     streams_to_merge: List[str] = None
     new_stream_name: str = "all"
     add_origin_stream_name: bool = True
     origin_stream_name_field_name: str = "origin"
 
-    def merge(self, multi_stream):
+    def merge(self, multi_stream) -> Generator:
         for stream_name, stream in multi_stream.items():
             if self.streams_to_merge is None or stream_name in self.streams_to_merge:
                 for instance in stream:
                     if self.add_origin_stream_name:
                         instance[self.origin_stream_name_field_name] = stream_name
                     yield instance
 
     def process(self, multi_stream: MultiStream) -> MultiStream:
         return MultiStream(
             {
-                self.new_stream_name: Stream(
+                self.new_stream_name: GeneratorStream(
                     self.merge, gen_kwargs={"multi_stream": multi_stream}
                 )
             }
         )
 
 
 class Shuffle(PagedStreamOperator):
```

### Comparing `unitxt-1.8.1/src/unitxt/parsing_utils.py` & `unitxt-1.9.0/src/unitxt/parsing_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/prepare_utils/card_types.py` & `unitxt-1.9.0/src/unitxt/prepare_utils/card_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict, List, Optional, Union
 
 from ..card import TaskCard
 from ..loaders import Loader
 from ..operator import StreamingOperator
 from ..operators import AddFields, MapInstanceValues, RenameFields
-from ..task import FormTask
+from ..task import Task
 from ..templates import TemplatesDict, TemplatesList
 
 
 def add_classification_choices(label_name, label2string):
     return [
         MapInstanceValues(mappers={label_name: label2string}),
         AddFields(
@@ -21,29 +21,29 @@
 
 def create_2sentences_classification_card(
     loader: Loader,
     label_name: str,
     label2string: Dict,
     inputs: List[str],
     metrics: List[str] = tuple("accuracy"),
-    task: FormTask = None,
+    task: Task = None,
     preprocess_steps: Optional[List[Union[StreamingOperator, str]]] = None,
     templates: Union[TemplatesList, TemplatesDict] = None,
 ) -> TaskCard:
     assert len(inputs) == 2, f"expected only 2 columns as input but received {inputs}"
     sentence1_col = "sentence1"
     sentence2_col = "sentence2"
     preprocess_steps += [
         *add_classification_choices(label_name, label2string),
         RenameFields(
             field_to_field={inputs[0]: sentence1_col, inputs[1]: sentence2_col}
         ),
     ]
     if task is None:
-        task = FormTask(
+        task = Task(
             inputs=["choices", sentence1_col, sentence2_col],
             outputs=[label_name],
             metrics=metrics,
         )
         return TaskCard(
             loader=loader,
             task=task,
@@ -55,27 +55,27 @@
 
 def create_sentence_classification_card(
     loader: Loader,
     label_name: str,
     label2string: Dict,
     inputs: List[str],
     metrics: List[str] = tuple("accuracy"),
-    task: FormTask = None,
+    task: Task = None,
     preprocess_steps: Optional[List[StreamingOperator]] = None,
     templates: Union[TemplatesList, TemplatesDict] = None,
 ) -> TaskCard:
     # TODO labels should be deduced by default
     assert len(inputs) == 1, f"expected only 1 column as input but received {inputs}"
     sentence_col = "sentence1"
     preprocess_steps += [
         *add_classification_choices(label_name, label2string),
         RenameFields(field_to_field={inputs[0]: sentence_col}),
     ]
     if task is None:
-        task = FormTask(
+        task = Task(
             inputs=["choices", sentence_col], outputs=[label_name], metrics=metrics
         )
         return TaskCard(
             loader=loader,
             task=task,
             preprocess_steps=preprocess_steps,
             templates=templates,
```

### Comparing `unitxt-1.8.1/src/unitxt/processors.py` & `unitxt-1.9.0/src/unitxt/processors.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import ast
 import json
 import re
 from difflib import get_close_matches
 from typing import Any, Dict
 
 from .operators import FieldOperator, InstanceFieldOperator
 
@@ -50,22 +51,14 @@
     def process_value(self, text: Any) -> Any:
         matches = super().process_value(text)
         if matches:
             return matches[0]
         return ""
 
 
-class LoadJson(FieldOperator):
-    def process_value(self, text: Any) -> Any:
-        try:
-            return json.loads(text)
-        except json.JSONDecodeError:
-            return []
-
-
 class ListToEmptyEntitiesTuples(FieldOperator):
     def process_value(self, lst: Any) -> Any:
         try:
             return [(str(item), "") for item in lst]
         except json.JSONDecodeError:
             return []
 
@@ -221,14 +214,34 @@
         if "not " + self.string.lower() in text.lower():
             return "not " + self.string.lower()
         if self.string.lower() in text.lower():
             return self.string.lower()
         return text
 
 
-class ExtractMtBenchJudgment(FieldOperator):
+class ExtractMtBenchRatingJudgment(FieldOperator):
     def process_value(self, text: Any) -> Any:
         match = re.search(r"\[\[([\d]+\.?[\d]*)\]\]", text)
         try:
             return float(match.group(1)) / 10
         except:
             return 0.0
+
+
+class ExtractMtBenchLabelJudgment(FieldOperator):
+    def process_value(self, text: Any) -> Any:
+        match = re.search(r"\[\[([^\]]+)\]\]", text)
+        try:
+            return str(match.group(1))
+        except:
+            return "None"
+
+
+class LiteralEval(FieldOperator):
+    def process_value(self, text: Any) -> Any:
+        if text is not None and not isinstance(text, str):
+            raise ValueError(
+                f"LiteralEval: field '{self.field}' is expected to be of 'str' input type, got: {type(text)}"
+            )
+        if text is None or text == "":
+            return text
+        return ast.literal_eval(text.strip())
```

### Comparing `unitxt-1.8.1/src/unitxt/random_utils.py` & `unitxt-1.9.0/src/unitxt/random_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/register.py` & `unitxt-1.9.0/src/unitxt/register.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/schema.py` & `unitxt-1.9.0/src/unitxt/schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,24 +30,32 @@
 
 class ToUnitxtGroup(StreamInstanceOperatorValidator):
     group: str
     metrics: List[str] = None
     postprocessors: List[str] = field(default_factory=lambda: ["to_string_stripped"])
     remove_unnecessary_fields: bool = True
 
-    def _to_lists_of_keys_and_values(self, dict: Dict[str, str]):
-        return {
-            "key": [key for key, _ in dict.items()],
-            "value": [str(value) for _, value in dict.items()],
-        }
+    @staticmethod
+    def artifact_to_jsonable(artifact):
+        if artifact.__id__ is None:
+            return artifact.to_dict()
+        return artifact.__id__
 
     def process(
         self, instance: Dict[str, Any], stream_name: Optional[str] = None
     ) -> Dict[str, Any]:
-        task_data = {**instance["inputs"], **instance["outputs"]}
+        task_data = {
+            **instance["inputs"],
+            **instance["outputs"],
+            "metadata": {
+                "template": self.artifact_to_jsonable(
+                    instance["recipe_metadata"]["template"]
+                )
+            },
+        }
         instance["task_data"] = json.dumps(task_data)
 
         if self.remove_unnecessary_fields:
             keys_to_delete = []
 
             for key in instance.keys():
                 if key not in UNITXT_DATASET_SCHEMA:
```

### Comparing `unitxt-1.8.1/src/unitxt/service/metrics/main.py` & `unitxt-1.9.0/src/unitxt/service/metrics/main.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/service/metrics/tokens.py` & `unitxt-1.9.0/src/unitxt/service/metrics/tokens.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/settings_utils.py` & `unitxt-1.9.0/src/unitxt/settings_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,21 +122,22 @@
     settings.use_only_local_catalogs = (bool, False)
     settings.global_loader_limit = (int, None)
     settings.num_resamples_for_instance_metrics = (int, 1000)
     settings.num_resamples_for_global_metrics = (int, 100)
     settings.max_log_message_size = (int, 100000)
     settings.artifactories = None
     settings.default_recipe = "standard_recipe"
-    settings.default_verbosity = "debug"
+    settings.default_verbosity = "info"
     settings.remote_metrics = []
     settings.allow_passing_data_to_remote_api = (bool, False)
     settings.test_card_disable = (bool, False)
     settings.test_metric_disable = (bool, False)
     settings.metrics_master_key_token = None
     settings.seed = (int, 42)
+    settings.skip_artifacts_prepare_and_verify = (bool, False)
 
 if Constants.is_uninitilized():
     constants = Constants()
     constants.dataset_file = os.path.join(os.path.dirname(__file__), "dataset.py")
     constants.metric_file = os.path.join(os.path.dirname(__file__), "metric.py")
     constants.local_catalog_path = os.path.join(os.path.dirname(__file__), "catalog")
     try:
```

### Comparing `unitxt-1.8.1/src/unitxt/span_lableing_operators.py` & `unitxt-1.9.0/src/unitxt/span_lableing_operators.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/split_utils.py` & `unitxt-1.9.0/src/unitxt/split_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/splitters.py` & `unitxt-1.9.0/src/unitxt/splitters.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,17 +192,20 @@
         if "inputs" not in exemplar:
             raise ValueError(f"'inputs' field is missing from '{exemplar}'.")
         inputs = exemplar["inputs"]
         if self.choices not in inputs:
             raise ValueError(f"'{self.choices}' field is missing from '{inputs}'.")
         choices = inputs[self.choices]
         if not isinstance(choices, list):
-            raise ValueError(
-                f"Unexpected input choices value '{choices}'. Expected a list."
-            )
+            if isinstance(choices, str):
+                choices = [choices]
+            else:
+                raise ValueError(
+                    f"Unexpected input choices value '{choices}'. Expected a list or a string."
+                )
 
         if "outputs" not in exemplar:
             raise ValueError(f"'outputs' field is missing from '{exemplar}'.")
         outputs = exemplar["outputs"]
         if self.labels not in outputs:
             raise ValueError(f"'{self.labels}' field is missing from '{outputs}'.")
```

### Comparing `unitxt-1.8.1/src/unitxt/standard.py` & `unitxt-1.9.0/src/unitxt/standard.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,32 +131,35 @@
         self.finalize = SequentialOperator()
 
         self.steps = [
             self.loading,
             self.metadata,
             self.standardization,
             self.processing,
+            self.metadata,
             self.verblization,
             self.finalize,
         ]
 
         self.inference_instance = SequentialOperator()
 
         self.inference_instance.steps = [
             self.metadata,
             self.processing,
+            self.metadata,
         ]
 
         self.inference_demos = SourceSequentialOperator()
 
         self.inference_demos.steps = [
             self.loading,
             self.metadata,
             self.standardization,
             self.processing,
+            self.metadata,
         ]
 
         self.inference = SequentialOperator()
 
         self.inference.steps = [self.verblization, self.finalize]
 
         self._demos_pool_cache = None
```

### Comparing `unitxt-1.8.1/src/unitxt/stream.py` & `unitxt-1.9.0/src/unitxt/stream.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,60 @@
 import tempfile
-from typing import Dict, Iterable
+from abc import abstractmethod
+from typing import Any, Callable, Dict, Iterable, List
 
 from datasets import Dataset, DatasetDict, IterableDataset, IterableDatasetDict
 
 from .dataclass import Dataclass, OptionalField
 from .generator_utils import CopyingReusableGenerator, ReusableGenerator
 
 
 class Stream(Dataclass):
+    @abstractmethod
+    def __iter__(self):
+        pass
+
+    @abstractmethod
+    def peek(self):
+        pass
+
+    @abstractmethod
+    def take(self, n):
+        pass
+
+
+class ListStream(Stream):
+    instances_list: List[Dict[str, Any]]
+
+    def __iter__(self):
+        return iter(self.instances_list)
+
+    def peek(self):
+        return next(iter(self.instances_list))
+
+    def take(self, n):
+        for i, instance in enumerate(self.instances_list):
+            if i >= n:
+                break
+            yield instance
+
+
+class GeneratorStream(Stream):
     """A class for handling streaming data in a customizable way.
 
     This class provides methods for generating, caching, and manipulating streaming data.
 
     Attributes:
         generator (function): A generator function for streaming data. :no-index:
         gen_kwargs (dict, optional): A dictionary of keyword arguments for the generator function. :no-index:
         caching (bool): Whether the data is cached or not. :no-index:
     """
 
-    generator: callable
-    gen_kwargs: Dict[str, any] = OptionalField(default_factory=dict)
+    generator: Callable
+    gen_kwargs: Dict[str, Any] = OptionalField(default_factory=dict)
     caching: bool = False
     copying: bool = False
 
     def _get_initiator(self):
         """Private method to get the correct initiator based on the streaming and caching attributes.
 
         Returns:
@@ -143,15 +174,15 @@
 
         Returns:
             MultiStream: A MultiStream object.
         """
         assert all(isinstance(v, ReusableGenerator) for v in generators.values())
         return cls(
             {
-                key: Stream(
+                key: GeneratorStream(
                     generator.generator,
                     gen_kwargs=generator.gen_kwargs,
                     caching=caching,
                     copying=copying,
                 )
                 for key, generator in generators.items()
             }
@@ -169,15 +200,15 @@
             copying (bool, optional): Whether the data should be copied or not. Defaults to False.
 
         Returns:
             MultiStream: A MultiStream object.
         """
         return cls(
             {
-                key: Stream(
+                key: GeneratorStream(
                     iterable.__iter__,
                     caching=caching,
                     copying=copying,
                 )
                 for key, iterable in iterables.items()
             }
         )
```

### Comparing `unitxt-1.8.1/src/unitxt/struct_data_operators.py` & `unitxt-1.9.0/src/unitxt/struct_data_operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -543,7 +543,26 @@
         shuffled_header = [header[i] for i in indices]
         shuffled_rows = [[row[i] for i in indices] for row in rows]
 
         table_content["header"] = shuffled_header
         table_content["rows"] = shuffled_rows
 
         return table_content
+
+
+class LoadJson(FieldOperator):
+    failure_value: Any = None
+    allow_failure: bool = False
+
+    def process_value(self, value: str) -> Any:
+        if self.allow_failure:
+            try:
+                return json.loads(value)
+            except json.JSONDecodeError:
+                return self.failure_value
+        else:
+            return json.loads(value)
+
+
+class DumpJson(FieldOperator):
+    def process_value(self, value: str) -> str:
+        return json.dumps(value)
```

### Comparing `unitxt-1.8.1/src/unitxt/system_prompts.py` & `unitxt-1.9.0/src/unitxt/system_prompts.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/templates.py` & `unitxt-1.9.0/src/unitxt/templates.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import json
 from abc import abstractmethod
+from random import random
 from typing import Any, Dict, List, Optional, Tuple, Union
 
+from .artifact import Artifact
 from .collections import ListCollection
 from .dataclass import NonPositionalField
 from .operator import StreamInstanceOperator
 from .random_utils import new_random_generator
 from .type_utils import isoftype
 
 
@@ -44,30 +46,35 @@
             inputs, "input", self.instruction, "instruction", serialize=True
         )
         target_prefix = self.apply_formatting(
             inputs, "input", self.target_prefix, "target_prefix", serialize=True
         )
         return instruction, target_prefix
 
+    def preprocess_inputs_and_outputs(
+        self, inputs: Dict[str, Any], outputs: Dict[str, Any]
+    ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
+        return inputs, outputs
+
     def process(
         self, instance: Dict[str, Any], stream_name: Optional[str] = None
     ) -> Dict[str, Any]:
         if self.skip_rendered_instance:
             if (
                 "source" in instance
                 and "target" in instance
                 and "references" in instance
             ):
                 return instance
 
         inputs = instance.get("inputs")
         outputs = instance.get("outputs")
+        inputs, outputs = self.preprocess_inputs_and_outputs(inputs, outputs)
 
         self.set_titles(inputs)
-
         source = self.inputs_to_source(inputs)
         instruction, target_prefix = self.inputs_to_instruction_and_target_prefix(
             inputs
         )
         target, references = self.outputs_to_target_and_references(outputs)
 
         return {
@@ -146,14 +153,143 @@
         )
         reference = self.apply_formatting(
             outputs, "output", self.reference, "reference", serialize=True
         )
         return target, [reference]
 
 
+class PairwiseChoiceTemplate(InputOutputTemplate):
+    """PairwiseChoiceTemplate.
+
+    Requirements:
+     The answer field value should be of type Literal["choice_a", "choice_b", "tie"]
+
+    Args:
+         choice_a_field (str): The field which contains choice_a value
+         choice_b_field (str): The field which contains choice_b value
+         answer_field (str): The field which contains the answer value.
+           Should be of type Literal["choice_1", "choice_2", "tie"]
+         choice_a_label (str): The label of choice A answer as it is verbalized in the template.
+         choice_b_label (str): The label of choice B answer as it is verbalized in the template.
+         choice_tie_label (str): The label of a tie answer as it should be verbalized in the template.
+         shuffle (bool): whether to shuffle the choices or not. This is done to take into account position bias.
+
+    shuffle: 50% of the time:
+     1) The values of choice_a_field and choice_b_field will be swapped.
+     2) If the values of answer_field is choice_a_label, set it to choice_b_label.
+         Else if the values of answer_field is choice_b_label, set it to choice_a_label.
+         Else if the value of answer_field is choice_tie_label, do nothing.
+
+    """
+
+    choice_a_field: str
+    choice_b_field: str
+    answer_field: str
+    choice_a_label: str
+    choice_b_label: str
+    choice_tie_label: str
+    shuffle: bool
+
+    def verbalize_answer_field(self, outputs: Dict[str, object]):
+        answer = outputs[self.answer_field]
+        assert answer in ["choice_a", "choice_b", "tie"]
+        if answer == "choice_a":
+            outputs[self.answer_field] = self.choice_a_label
+        elif answer == "choice_b":
+            outputs[self.answer_field] = self.choice_b_label
+        else:
+            outputs[self.answer_field] = self.choice_tie_label
+
+        return outputs
+
+    def shuffle_values(self, inputs: Dict[str, object], outputs: Dict[str, object]):
+        outcome = random()  # A float between 0 and 1
+        if outcome <= 0.5:
+            choice_a_value = inputs[self.choice_a_field]
+            choice_b_value = inputs[self.choice_b_field]
+
+            inputs[self.choice_a_field] = choice_a_value
+            inputs[self.choice_b_field] = choice_b_value
+
+            answer = outputs[self.answer_field]
+            assert answer in [
+                self.choice_a_label,
+                self.choice_b_label,
+                self.choice_tie_label,
+            ]
+            if answer == self.choice_a_label:
+                outputs[self.answer_field] = self.choice_b_label
+            elif answer == self.choice_b_label:
+                outputs[self.answer_field] = self.choice_a_label
+
+        return inputs, outputs
+
+    def preprocess_inputs_and_outputs(
+        self, inputs: Dict[str, Any], outputs: Dict[str, Any]
+    ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
+        outputs = self.verbalize_answer_field(outputs)
+        inputs, outputs = self.shuffle_values(inputs, outputs)
+        return inputs, outputs
+
+
+class DialogFieldsData(Artifact):
+    user_role_label: str
+    assistant_role_label: str
+    system_role_label: str
+    dialog_field: str
+
+
+class DialogTemplate(InputOutputTemplate):
+    dialog_fields: List[DialogFieldsData]
+    turns_separator: str = "\n\n"
+    label_separator: str = " "
+
+    def process_dialog(self, inputs: Dict[str, object]):
+        for dialog_fields in self.dialog_fields:
+            dialog = inputs[dialog_fields.dialog_field]
+            # TODO: update isoftype method to support Literal verification and check
+            #  it's List[Tuple[Literal["user", "assistant", "system"], str]] (Issue #799)
+            assert isoftype(dialog, List[Tuple[str, str]])
+
+            user_role_label = dialog_fields.user_role_label
+            assistant_role_label = dialog_fields.assistant_role_label
+            system_role_label = dialog_fields.system_role_label
+
+            dialog_str = ""
+            for i, turn in enumerate(dialog):
+                (turn_type, turn_text) = turn
+                turns_separator = "" if i == 0 else self.turns_separator
+                if turn_type == "user":
+                    dialog_str += f"{turns_separator}{user_role_label}{self.label_separator}{turn_text}"
+                elif turn_type == "assistant":
+                    dialog_str += f"{turns_separator}{assistant_role_label}{self.label_separator}{turn_text}"
+                elif turn_type == "system":
+                    dialog_str += f"{turns_separator}{system_role_label}{self.label_separator}{turn_text}"
+
+            inputs[dialog_fields.dialog_field] = dialog_str
+        return inputs
+
+    def preprocess_inputs_and_outputs(
+        self, inputs: Dict[str, Any], outputs: Dict[str, Any]
+    ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
+        return self.process_dialog(inputs), outputs
+
+
+class DialogPairwiseChoiceTemplate(DialogTemplate, PairwiseChoiceTemplate):
+    def preprocess_inputs_and_outputs(
+        self, inputs: Dict[str, Any], outputs: Dict[str, Any]
+    ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
+        inputs, outputs = DialogTemplate.preprocess_inputs_and_outputs(
+            self, inputs, outputs
+        )
+        return PairwiseChoiceTemplate.preprocess_inputs_and_outputs(
+            self, inputs, outputs
+        )
+
+
 class MultipleChoiceTemplate(Template):
     """Formats the input (that specifies the question), the multiple choices to select the answer from, and specifies the field with the correct answer."""
 
     input_format: str
     target_prefix: str = ""
     choices_field: str = "choices"
     target_field: str = "label"
@@ -324,33 +460,28 @@
     def outputs_to_target_and_references(self, outputs: Dict[str, object]) -> str:
         try:
             gold_class_names = outputs[self.label_field]
         except KeyError as e:
             raise RuntimeError(
                 f"Available outputs are {list(outputs.keys())}, missing required label field: '{self.label_field}'."
             ) from e
-        if not isinstance(gold_class_names, list) or not gold_class_names:
+        if not isinstance(gold_class_names, list):
             raise RuntimeError(
-                f"Unexpected value for gold_class_names: '{gold_class_names}'. Expected a non-empty list."
+                f"Unexpected value for gold_class_names: '{gold_class_names}'. Expecting a list."
             )
         try:
-            queried_class_names = outputs[self.class_field]
+            queried_class_name = outputs[self.class_field]
         except KeyError as e:
             raise RuntimeError(
                 f"Available outputs are {list(outputs.keys())}, missing required class field: '{self.class_field}'."
             ) from e
-        if (
-            not queried_class_names
-            or not isinstance(queried_class_names, list)
-            or not len(queried_class_names) == 1
-        ):
+        if not queried_class_name or not isinstance(queried_class_name, str):
             raise RuntimeError(
-                f"Unexpected value for queried_class_names: '{queried_class_names}'. Expected a list with one item."
+                f"Unexpected value for queried_class_names: '{queried_class_name}'. Expected a string."
             )
-        queried_class_name = queried_class_names[0]
         if queried_class_name in gold_class_names:
             return self.yes_answer, [self.yes_answer]
         return self.no_answer, [self.no_answer]
 
 
 class KeyValTemplate(Template):
     """Generate field 'source' from fields designated as input, and fields 'target' and 'references' from fields designated as output, of the processed instance.
```

### Comparing `unitxt-1.8.1/src/unitxt/test_utils/artifact.py` & `unitxt-1.9.0/src/unitxt/test_utils/artifact.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/test_utils/card.py` & `unitxt-1.9.0/src/unitxt/test_utils/card.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,14 +200,18 @@
         logger.info(
             f"Processed prediction: ({type(result['prediction']).__name__}) {result['prediction']}"
         )
         logger.info(
             f"Processed references: ({type(result['references']).__name__}) {result['references']}"
         )
     logger.info("*" * 80)
+    logger.info("Sample score output:")
+    logger.info(json.dumps(results[0]["score"]["global"], sort_keys=True, indent=4))
+    logger.info("*" * 80)
+
     score_name = results[0]["score"]["global"]["score_name"]
     score = results[0]["score"]["global"]["score"]
 
     if exact_match_score is not None and not math.isclose(score, exact_match_score):
         message = (
             f"The results of running the main metric used in the card ({score_name}) "
             f"over simulated predictions that are equal to the references returns a different score than expected.\n"
```

### Comparing `unitxt-1.8.1/src/unitxt/test_utils/catalog.py` & `unitxt-1.9.0/src/unitxt/test_utils/catalog.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/test_utils/metrics.py` & `unitxt-1.9.0/src/unitxt/test_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/test_utils/operators.py` & `unitxt-1.9.0/src/unitxt/test_utils/operators.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/type_utils.py` & `unitxt-1.9.0/src/unitxt/type_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/ui/__init__.py` & `unitxt-1.9.0/src/unitxt/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/ui/banner.png` & `unitxt-1.9.0/src/unitxt/ui/banner.png`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/ui/gradio_utils.py` & `unitxt-1.9.0/src/unitxt/ui/gradio_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/ui/load_catalog_data.py` & `unitxt-1.9.0/src/unitxt/ui/load_catalog_data.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/ui/run.py` & `unitxt-1.9.0/src/unitxt/ui/run.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/ui/settings.py` & `unitxt-1.9.0/src/unitxt/ui/settings.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/ui/ui_tester.py` & `unitxt-1.9.0/src/unitxt/ui/ui_tester.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/ui/ui_utils.py` & `unitxt-1.9.0/src/unitxt/ui/ui_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/utils.py` & `unitxt-1.9.0/src/unitxt/utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt/validate.py` & `unitxt-1.9.0/src/unitxt/validate.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.8.1/src/unitxt.egg-info/PKG-INFO` & `unitxt-1.9.0/src/unitxt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,130 +1,134 @@
 Metadata-Version: 2.1
 Name: unitxt
-Version: 1.8.1
+Version: 1.9.0
 Summary: Load any mixture of text to text data in one line of code
 Home-page: https://github.com/ibm/unitxt
 Author: IBM Research
 Author-email: elron.bandel@ibm.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: datasets>=2.16.0
 Requires-Dist: evaluate
 Requires-Dist: absl-py
 Requires-Dist: ipadic
 Requires-Dist: scipy
-Provides-Extra: tests
-Requires-Dist: bert_score; extra == "tests"
-Requires-Dist: transformers; extra == "tests"
-Requires-Dist: sentence_transformers; extra == "tests"
-Requires-Dist: ibm-cos-sdk; extra == "tests"
-Requires-Dist: opendatasets; extra == "tests"
-Requires-Dist: httpretty~=1.1.4; extra == "tests"
-Requires-Dist: editdistance; extra == "tests"
-Requires-Dist: rouge-score; extra == "tests"
-Requires-Dist: nltk; extra == "tests"
-Requires-Dist: mecab-python3; extra == "tests"
-Requires-Dist: sacrebleu[ko]; extra == "tests"
-Requires-Dist: scikit-learn; extra == "tests"
-Requires-Dist: jiwer; extra == "tests"
-Requires-Dist: conllu; extra == "tests"
-Requires-Dist: llama-index-core; extra == "tests"
-Requires-Dist: llama-index-llms-openai; extra == "tests"
-Requires-Dist: pytrec-eval; extra == "tests"
-Requires-Dist: SentencePiece; extra == "tests"
-Provides-Extra: service
-Requires-Dist: torch==1.12.1; extra == "service"
-Requires-Dist: fastapi==0.109.0; extra == "service"
-Requires-Dist: uvicorn[standard]==0.27.0.post1; extra == "service"
-Requires-Dist: python-jose[cryptography]==3.3.0; extra == "service"
-Requires-Dist: transformers; extra == "service"
+Provides-Extra: dev
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: tomli; extra == "dev"
+Requires-Dist: codespell; extra == "dev"
+Provides-Extra: ui
+Requires-Dist: gradio; extra == "ui"
+Requires-Dist: transformers; extra == "ui"
 Provides-Extra: base
 Requires-Dist: datasets>=2.16.0; extra == "base"
 Requires-Dist: evaluate; extra == "base"
 Requires-Dist: absl-py; extra == "base"
 Requires-Dist: ipadic; extra == "base"
 Requires-Dist: scipy; extra == "base"
 Provides-Extra: helm
 Requires-Dist: crfm-helm[unitxt]>=0.5.0; extra == "helm"
+Provides-Extra: service
+Requires-Dist: torch==1.12.1; extra == "service"
+Requires-Dist: fastapi==0.109.0; extra == "service"
+Requires-Dist: uvicorn[standard]==0.27.0.post1; extra == "service"
+Requires-Dist: python-jose[cryptography]==3.3.0; extra == "service"
+Requires-Dist: transformers; extra == "service"
 Provides-Extra: docs
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Requires-Dist: piccolo_theme; extra == "docs"
 Requires-Dist: sphinxext-opengraph; extra == "docs"
 Requires-Dist: datasets; extra == "docs"
 Requires-Dist: evaluate; extra == "docs"
 Requires-Dist: nltk; extra == "docs"
 Requires-Dist: sacrebleu; extra == "docs"
 Requires-Dist: absl-py; extra == "docs"
 Requires-Dist: rouge_score; extra == "docs"
 Requires-Dist: scikit-learn; extra == "docs"
 Requires-Dist: jiwer; extra == "docs"
 Requires-Dist: editdistance; extra == "docs"
-Provides-Extra: ui
-Requires-Dist: gradio; extra == "ui"
-Requires-Dist: transformers; extra == "ui"
-Provides-Extra: dev
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: tomli; extra == "dev"
-Requires-Dist: codespell; extra == "dev"
+Provides-Extra: tests
+Requires-Dist: bert_score; extra == "tests"
+Requires-Dist: transformers; extra == "tests"
+Requires-Dist: sentence_transformers; extra == "tests"
+Requires-Dist: ibm-cos-sdk; extra == "tests"
+Requires-Dist: opendatasets; extra == "tests"
+Requires-Dist: httpretty~=1.1.4; extra == "tests"
+Requires-Dist: editdistance; extra == "tests"
+Requires-Dist: rouge-score; extra == "tests"
+Requires-Dist: nltk; extra == "tests"
+Requires-Dist: mecab-python3; extra == "tests"
+Requires-Dist: sacrebleu[ko]; extra == "tests"
+Requires-Dist: scikit-learn; extra == "tests"
+Requires-Dist: jiwer; extra == "tests"
+Requires-Dist: conllu; extra == "tests"
+Requires-Dist: llama-index-core; extra == "tests"
+Requires-Dist: llama-index-llms-openai; extra == "tests"
+Requires-Dist: pytrec-eval; extra == "tests"
+Requires-Dist: SentencePiece; extra == "tests"
+Requires-Dist: openai; extra == "tests"
+Requires-Dist: ibm-generative-ai; extra == "tests"
 Provides-Extra: all
-Requires-Dist: llama-index-core; extra == "all"
-Requires-Dist: nltk; extra == "all"
+Requires-Dist: rouge-score; extra == "all"
+Requires-Dist: ruff; extra == "all"
+Requires-Dist: pytrec-eval; extra == "all"
+Requires-Dist: sphinxext-opengraph; extra == "all"
+Requires-Dist: conllu; extra == "all"
+Requires-Dist: openai; extra == "all"
+Requires-Dist: sacrebleu; extra == "all"
+Requires-Dist: mecab-python3; extra == "all"
+Requires-Dist: ibm-generative-ai; extra == "all"
 Requires-Dist: torch==1.12.1; extra == "all"
+Requires-Dist: ipadic; extra == "all"
 Requires-Dist: codespell; extra == "all"
-Requires-Dist: opendatasets; extra == "all"
 Requires-Dist: absl-py; extra == "all"
-Requires-Dist: conllu; extra == "all"
-Requires-Dist: ruff; extra == "all"
-Requires-Dist: editdistance; extra == "all"
-Requires-Dist: fastapi==0.109.0; extra == "all"
+Requires-Dist: llama-index-llms-openai; extra == "all"
+Requires-Dist: llama-index-core; extra == "all"
+Requires-Dist: piccolo_theme; extra == "all"
+Requires-Dist: nltk; extra == "all"
 Requires-Dist: datasets; extra == "all"
-Requires-Dist: sacrebleu[ko]; extra == "all"
-Requires-Dist: mecab-python3; extra == "all"
-Requires-Dist: sacrebleu; extra == "all"
-Requires-Dist: crfm-helm[unitxt]>=0.5.0; extra == "all"
-Requires-Dist: scikit-learn; extra == "all"
-Requires-Dist: ipadic; extra == "all"
 Requires-Dist: transformers; extra == "all"
-Requires-Dist: datasets>=2.16.0; extra == "all"
-Requires-Dist: uvicorn[standard]==0.27.0.post1; extra == "all"
-Requires-Dist: scipy; extra == "all"
+Requires-Dist: rouge_score; extra == "all"
+Requires-Dist: scikit-learn; extra == "all"
 Requires-Dist: tomli; extra == "all"
-Requires-Dist: piccolo_theme; extra == "all"
-Requires-Dist: SentencePiece; extra == "all"
+Requires-Dist: opendatasets; extra == "all"
+Requires-Dist: uvicorn[standard]==0.27.0.post1; extra == "all"
 Requires-Dist: sphinx_rtd_theme; extra == "all"
-Requires-Dist: pre-commit; extra == "all"
-Requires-Dist: sentence_transformers; extra == "all"
-Requires-Dist: bert_score; extra == "all"
-Requires-Dist: pytrec-eval; extra == "all"
+Requires-Dist: scipy; extra == "all"
+Requires-Dist: fastapi==0.109.0; extra == "all"
 Requires-Dist: httpretty~=1.1.4; extra == "all"
-Requires-Dist: rouge_score; extra == "all"
-Requires-Dist: python-jose[cryptography]==3.3.0; extra == "all"
-Requires-Dist: jiwer; extra == "all"
 Requires-Dist: evaluate; extra == "all"
 Requires-Dist: gradio; extra == "all"
-Requires-Dist: sphinxext-opengraph; extra == "all"
+Requires-Dist: bert_score; extra == "all"
+Requires-Dist: editdistance; extra == "all"
 Requires-Dist: ibm-cos-sdk; extra == "all"
-Requires-Dist: rouge-score; extra == "all"
-Requires-Dist: llama-index-llms-openai; extra == "all"
+Requires-Dist: crfm-helm[unitxt]>=0.5.0; extra == "all"
+Requires-Dist: python-jose[cryptography]==3.3.0; extra == "all"
+Requires-Dist: datasets>=2.16.0; extra == "all"
+Requires-Dist: jiwer; extra == "all"
+Requires-Dist: pre-commit; extra == "all"
+Requires-Dist: sacrebleu[ko]; extra == "all"
+Requires-Dist: SentencePiece; extra == "all"
+Requires-Dist: sentence_transformers; extra == "all"
 
 <div align="center">
     <img src="./assets/banner.png" alt="Image Description" width="100%" />
 </div>
 
 [![Button](https://img.shields.io/badge/Video-pink?style=for-the-badge)](https://unitxt.readthedocs.io/)
 [![Button](https://img.shields.io/badge/Demo-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/docs/demo.html)
 [![Button](https://img.shields.io/badge/Tutorial-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/docs/adding_dataset.html)
 [![Button](https://img.shields.io/badge/Paper-pink?style=for-the-badge)](https://arxiv.org/abs/2401.14019)
 [![Button](https://img.shields.io/badge/Documentation-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/modules.html)
-[![Button](https://img.shields.io/badge/Catalog-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/catalog.html)
-[![Button](https://img.shields.io/badge/Contributors-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/docs/contributors_guide.html)
+[![Button](https://img.shields.io/badge/Catalog-pink?style=for-the-badge)](https://unitxt.readthedocs.io/en/latest/catalog/catalog.__dir__.html)
+[![Button](https://img.shields.io/badge/Contributors-pink?style=for-the-badge)](https://github.com/IBM/unitxt/blob/main/CONTRIBUTING.md)
 [![Button](https://img.shields.io/badge/PyPi-pink?style=for-the-badge)](https://pypi.org/project/unitxt/)
 
 
 In the dynamic landscape of generative NLP, traditional text processing pipelines limit research flexibility and reproducibility, as they are tailored to specific dataset, task, and model combinations. The escalating complexity, involving system prompts, model-specific formats, instructions, and more, calls for a shift to a structured, modular, and customizable solution.
 
  Addressing this need, we present Unitxt, an innovative library for customizable textual data preparation and evaluation tailored to generative language models. Unitxt natively integrates with common libraries like HuggingFace and LM-eval-harness and deconstructs processing flows into modular components, enabling easy customization and sharing between practitioners. These components encompass model-specific formats, task prompts, and many other comprehensive dataset processing definitions. The Unitxt-Catalog centralizes these components, fostering collaboration and exploration in modern textual data workflows. Beyond being a tool, Unitxt is a community-driven platform, empowering users to build, share, and advance their pipelines collaboratively.
```

### Comparing `unitxt-1.8.1/src/unitxt.egg-info/SOURCES.txt` & `unitxt-1.9.0/src/unitxt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -69,25 +69,28 @@
 src/unitxt/catalog/augmentors/no_augmentation.json
 src/unitxt/catalog/cards/20_newsgroups.json
 src/unitxt/catalog/cards/ag_news.json
 src/unitxt/catalog/cards/almost_evil.json
 src/unitxt/catalog/cards/argument_topic.json
 src/unitxt/catalog/cards/atis.json
 src/unitxt/catalog/cards/atta_q.json
+src/unitxt/catalog/cards/attaq_500.json
 src/unitxt/catalog/cards/banking77.json
+src/unitxt/catalog/cards/billsum.json
 src/unitxt/catalog/cards/bold.json
 src/unitxt/catalog/cards/claim_stance_topic.json
 src/unitxt/catalog/cards/cnn_dailymail.json
 src/unitxt/catalog/cards/coedit_error_detection.json
 src/unitxt/catalog/cards/coedit_gec.json
 src/unitxt/catalog/cards/cola.json
 src/unitxt/catalog/cards/copa.json
 src/unitxt/catalog/cards/dart.json
 src/unitxt/catalog/cards/dbpedia_14.json
 src/unitxt/catalog/cards/ethos_binary.json
+src/unitxt/catalog/cards/financebench.json
 src/unitxt/catalog/cards/financial_tweets.json
 src/unitxt/catalog/cards/hellaswag.json
 src/unitxt/catalog/cards/hh_rlhf.json
 src/unitxt/catalog/cards/human_eval.json
 src/unitxt/catalog/cards/law_stack_exchange.json
 src/unitxt/catalog/cards/ledgar.json
 src/unitxt/catalog/cards/mbpp.json
@@ -107,14 +110,15 @@
 src/unitxt/catalog/cards/sciq.json
 src/unitxt/catalog/cards/squad.json
 src/unitxt/catalog/cards/sst2.json
 src/unitxt/catalog/cards/stsb.json
 src/unitxt/catalog/cards/summarize_from_human_feedback.json
 src/unitxt/catalog/cards/tab_fact.json
 src/unitxt/catalog/cards/tablerow_classify.json
+src/unitxt/catalog/cards/tldr.json
 src/unitxt/catalog/cards/toxigen.json
 src/unitxt/catalog/cards/trec.json
 src/unitxt/catalog/cards/unfair_tos.json
 src/unitxt/catalog/cards/wiki_bio.json
 src/unitxt/catalog/cards/wikitq.json
 src/unitxt/catalog/cards/wnli.json
 src/unitxt/catalog/cards/wsc.json
@@ -332,20 +336,27 @@
 src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/eng.json
 src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/fra.json
 src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/jpn.json
 src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/por.json
 src/unitxt/catalog/cards/cohere_for_ai/dolly_machine_translated/spa.json
 src/unitxt/catalog/cards/coqa/completion.json
 src/unitxt/catalog/cards/coqa/qa.json
+src/unitxt/catalog/cards/dynamic_cards_for_llm_judges/rating/single_turn.json
+src/unitxt/catalog/cards/dynamic_cards_for_llm_judges/rating/single_turn_with_reference.json
 src/unitxt/catalog/cards/ffqa_filtered/16k.json
 src/unitxt/catalog/cards/ffqa_filtered/2k.json
 src/unitxt/catalog/cards/ffqa_filtered/4k.json
 src/unitxt/catalog/cards/ffqa_filtered/8k.json
 src/unitxt/catalog/cards/head_qa/en.json
 src/unitxt/catalog/cards/head_qa/es.json
+src/unitxt/catalog/cards/legalbench/abercrombie.json
+src/unitxt/catalog/cards/legalbench/corporate_lobbying.json
+src/unitxt/catalog/cards/legalbench/function_of_decision_section.json
+src/unitxt/catalog/cards/legalbench/international_citizenship_questions.json
+src/unitxt/catalog/cards/legalbench/proa.json
 src/unitxt/catalog/cards/mlsum/de.json
 src/unitxt/catalog/cards/mlsum/es.json
 src/unitxt/catalog/cards/mlsum/fr.json
 src/unitxt/catalog/cards/mlsum/ru.json
 src/unitxt/catalog/cards/mlsum/tu.json
 src/unitxt/catalog/cards/mmlu/abstract_algebra.json
 src/unitxt/catalog/cards/mmlu/anatomy.json
@@ -400,17 +411,27 @@
 src/unitxt/catalog/cards/mmlu/professional_psychology.json
 src/unitxt/catalog/cards/mmlu/public_relations.json
 src/unitxt/catalog/cards/mmlu/security_studies.json
 src/unitxt/catalog/cards/mmlu/sociology.json
 src/unitxt/catalog/cards/mmlu/us_foreign_policy.json
 src/unitxt/catalog/cards/mmlu/virology.json
 src/unitxt/catalog/cards/mmlu/world_religions.json
+src/unitxt/catalog/cards/mt_bench/generation/english_single_turn.json
+src/unitxt/catalog/cards/mt_bench/generation/japanese_single_turn.json
+src/unitxt/catalog/cards/mt_bench/response_assessment/pairwise_comparison/multi_turn_gpt4_judgement.json
+src/unitxt/catalog/cards/mt_bench/response_assessment/pairwise_comparison/multi_turn_with_reference_gpt4_judgement.json
+src/unitxt/catalog/cards/mt_bench/response_assessment/pairwise_comparison/single_turn_gpt4_judgement.json
+src/unitxt/catalog/cards/mt_bench/response_assessment/pairwise_comparison/single_turn_with_reference_gpt4_judgement.json
+src/unitxt/catalog/cards/mt_bench/response_assessment/rating/multi_turn_gpt4_judgement.json
+src/unitxt/catalog/cards/mt_bench/response_assessment/rating/multi_turn_with_reference_gpt4_judgement.json
+src/unitxt/catalog/cards/mt_bench/response_assessment/rating/single_turn_gpt4_judgement.json
+src/unitxt/catalog/cards/mt_bench/response_assessment/rating/single_turn_with_reference_gpt4_judgement.json
 src/unitxt/catalog/cards/multidoc2dial/abstractive.json
 src/unitxt/catalog/cards/multidoc2dial/extractive.json
-src/unitxt/catalog/cards/rag/model_response_assessment/llm_as_judge_using_mt_bench_template.json
+src/unitxt/catalog/cards/rag/response_generation/clapnq.json
 src/unitxt/catalog/cards/reuters21578/ModApte.json
 src/unitxt/catalog/cards/reuters21578/ModHayes.json
 src/unitxt/catalog/cards/reuters21578/ModLewis.json
 src/unitxt/catalog/cards/universal_ner/ceb/gja.json
 src/unitxt/catalog/cards/universal_ner/da/ddt.json
 src/unitxt/catalog/cards/universal_ner/de/pud.json
 src/unitxt/catalog/cards/universal_ner/en/ewt.json
@@ -504,18 +525,21 @@
 src/unitxt/catalog/cards/xwinogrande/ru.json
 src/unitxt/catalog/cards/xwinogrande/zh.json
 src/unitxt/catalog/formats/empty.json
 src/unitxt/catalog/formats/empty_input_output_separator.json
 src/unitxt/catalog/formats/human_assistant.json
 src/unitxt/catalog/formats/llama.json
 src/unitxt/catalog/formats/llama2.json
+src/unitxt/catalog/formats/llama3_chat.json
+src/unitxt/catalog/formats/llama3_chat_with_system_prompt.json
 src/unitxt/catalog/formats/textual_assistant.json
 src/unitxt/catalog/formats/user_agent.json
 src/unitxt/catalog/formats/user_assistant.json
 src/unitxt/catalog/formats/models/alpaca_instruct.json
+src/unitxt/catalog/formats/models/phi_3.json
 src/unitxt/catalog/formats/models/flan/exq_exa.json
 src/unitxt/catalog/formats/models/flan/few_shot.json
 src/unitxt/catalog/formats/models/labradorite/few_shot.json
 src/unitxt/catalog/formats/models/labradorite/zero_shot.json
 src/unitxt/catalog/formats/models/mistral/instruction.json
 src/unitxt/catalog/formats/models/mistral/instruction/with_system_prompt.json
 src/unitxt/catalog/metrics/accuracy.json
@@ -525,14 +549,15 @@
 src/unitxt/catalog/metrics/char_edit_distance.json
 src/unitxt/catalog/metrics/f1_binary.json
 src/unitxt/catalog/metrics/f1_macro.json
 src/unitxt/catalog/metrics/f1_macro_multi_label.json
 src/unitxt/catalog/metrics/f1_micro.json
 src/unitxt/catalog/metrics/f1_micro_multi_label.json
 src/unitxt/catalog/metrics/f1_weighted.json
+src/unitxt/catalog/metrics/jaccard_index.json
 src/unitxt/catalog/metrics/kendalltau_b.json
 src/unitxt/catalog/metrics/kpa.json
 src/unitxt/catalog/metrics/map.json
 src/unitxt/catalog/metrics/matthews_correlation.json
 src/unitxt/catalog/metrics/max_accuracy_binary.json
 src/unitxt/catalog/metrics/max_f1_binary.json
 src/unitxt/catalog/metrics/mrr.json
@@ -561,14 +586,17 @@
 src/unitxt/catalog/metrics/unsorted_list_exact_match.json
 src/unitxt/catalog/metrics/wer.json
 src/unitxt/catalog/metrics/bert_score/deberta_base_mnli.json
 src/unitxt/catalog/metrics/bert_score/deberta_large_mnli.json
 src/unitxt/catalog/metrics/bert_score/deberta_v3_base_mnli_xnli_ml.json
 src/unitxt/catalog/metrics/bert_score/deberta_xlarge_mnli.json
 src/unitxt/catalog/metrics/bert_score/distilbert_base_uncased.json
+src/unitxt/catalog/metrics/llm_as_judge/rating/llama_3_70b_instruct_ibm_genai_template_mt_bench_single_turn.json
+src/unitxt/catalog/metrics/llm_as_judge/rating/llama_3_8b_instruct_ibm_genai_template_mt_bench_single_turn.json
+src/unitxt/catalog/metrics/llm_as_judge/rating/mistral_7b_instruct_v0_2_huggingface_template_mt_bench_single_turn.json
 src/unitxt/catalog/metrics/perplexity/flan_t5_small.json
 src/unitxt/catalog/metrics/perplexity_a/flan_t5_small.json
 src/unitxt/catalog/metrics/perplexity_chat/flan_t5_small.json
 src/unitxt/catalog/metrics/perplexity_nli/t5_nli_mixture.json
 src/unitxt/catalog/metrics/perplexity_q/flan_t5_small.json
 src/unitxt/catalog/metrics/rag/answer_correctness.json
 src/unitxt/catalog/metrics/rag/answer_inference.json
@@ -583,15 +611,18 @@
 src/unitxt/catalog/metrics/rag/faithfulness.json
 src/unitxt/catalog/metrics/rag/k_precision.json
 src/unitxt/catalog/metrics/rag/map.json
 src/unitxt/catalog/metrics/rag/mrr.json
 src/unitxt/catalog/metrics/rag/recall.json
 src/unitxt/catalog/metrics/rag/correctness/llama_index_by_gpt_3_5_turbo.json
 src/unitxt/catalog/metrics/rag/correctness/llama_index_by_mock.json
-src/unitxt/catalog/metrics/rag/model_response_assessment/llm_as_judge_by_flan_t5_large_on_hf_pipeline_using_mt_bench_template.json
+src/unitxt/catalog/metrics/rag/response_generation/correctness/token_overlap.json
+src/unitxt/catalog/metrics/rag/response_generation/correctness/bert_score/deberta_large_mnli.json
+src/unitxt/catalog/metrics/rag/response_generation/correctness/bert_score/deberta_v3_base_mnli_xnli_ml.json
+src/unitxt/catalog/metrics/rag/response_generation/faithfullness/token_overlap.json
 src/unitxt/catalog/metrics/reward/deberta_v3_large_v2.json
 src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_cohens_h_paraphrase_accuracy.json
 src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_cohens_h_paraphrase_string_containment.json
 src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_hedges_g_paraphrase_accuracy.json
 src/unitxt/catalog/metrics/robustness/fixed_group_absval_norm_hedges_g_paraphrase_string_containment.json
 src/unitxt/catalog/metrics/robustness/fixed_group_mean_accuracy.json
 src/unitxt/catalog/metrics/robustness/fixed_group_mean_baseline_accuracy.json
@@ -615,32 +646,36 @@
 src/unitxt/catalog/operators/balancers/qa/by_answer.json
 src/unitxt/catalog/processors/capitalize.json
 src/unitxt/catalog/processors/cast_to_float_return_nan_if_failed.json
 src/unitxt/catalog/processors/cast_to_float_return_zero_if_failed.json
 src/unitxt/catalog/processors/convert_to_boolean.json
 src/unitxt/catalog/processors/dict_of_lists_to_value_key_pairs.json
 src/unitxt/catalog/processors/extract_from_double_brackets.json
-src/unitxt/catalog/processors/extract_mt_bench_judgment.json
+src/unitxt/catalog/processors/extract_mt_bench_label_judgment.json
+src/unitxt/catalog/processors/extract_mt_bench_rating_judgment.json
 src/unitxt/catalog/processors/first_character.json
 src/unitxt/catalog/processors/get_string_after_colon.json
 src/unitxt/catalog/processors/hate_speech_or_not_hate_speech.json
 src/unitxt/catalog/processors/list_to_empty_entity_tuples.json
+src/unitxt/catalog/processors/literal_eval.json
 src/unitxt/catalog/processors/load_json.json
 src/unitxt/catalog/processors/load_json_from_predictions.json
 src/unitxt/catalog/processors/lower_case.json
 src/unitxt/catalog/processors/lower_case_till_punc.json
 src/unitxt/catalog/processors/match_closest_option.json
 src/unitxt/catalog/processors/predictions_yes_1_else_0.json
+src/unitxt/catalog/processors/regex_parser_from_prediction.json
 src/unitxt/catalog/processors/remove_none_from_list.json
 src/unitxt/catalog/processors/stance_to_pro_con.json
 src/unitxt/catalog/processors/str_to_float_format.json
 src/unitxt/catalog/processors/substring.json
 src/unitxt/catalog/processors/take_first_non_empty_line.json
 src/unitxt/catalog/processors/take_first_word.json
 src/unitxt/catalog/processors/to_list_by_comma.json
+src/unitxt/catalog/processors/to_list_by_comma_from_references.json
 src/unitxt/catalog/processors/to_span_label_pairs.json
 src/unitxt/catalog/processors/to_span_label_pairs_surface_only.json
 src/unitxt/catalog/processors/to_string.json
 src/unitxt/catalog/processors/to_string_stripped.json
 src/unitxt/catalog/processors/to_yes_or_none.json
 src/unitxt/catalog/processors/toxic_or_not_toxic.json
 src/unitxt/catalog/processors/yes_no_to_int.json
@@ -660,30 +695,39 @@
 src/unitxt/catalog/tasks/generation.json
 src/unitxt/catalog/tasks/grammatical_error_correction.json
 src/unitxt/catalog/tasks/classification/binary.json
 src/unitxt/catalog/tasks/classification/multi_class.json
 src/unitxt/catalog/tasks/classification/multi_label.json
 src/unitxt/catalog/tasks/classification/binary/zero_or_one.json
 src/unitxt/catalog/tasks/classification/multi_class/relation.json
+src/unitxt/catalog/tasks/classification/multi_class/with_classes_descriptions.json
 src/unitxt/catalog/tasks/completion/abstractive.json
 src/unitxt/catalog/tasks/completion/extractive.json
 src/unitxt/catalog/tasks/completion/multiple_choice.json
 src/unitxt/catalog/tasks/evaluation/preference.json
 src/unitxt/catalog/tasks/ner/all_entity_types.json
 src/unitxt/catalog/tasks/ner/single_entity_type.json
 src/unitxt/catalog/tasks/qa/open.json
 src/unitxt/catalog/tasks/qa/multiple_choice/open.json
 src/unitxt/catalog/tasks/qa/multiple_choice/with_context.json
 src/unitxt/catalog/tasks/qa/multiple_choice/with_topic.json
 src/unitxt/catalog/tasks/qa/multiple_choice/with_context/with_topic.json
 src/unitxt/catalog/tasks/qa/with_context/abstractive.json
 src/unitxt/catalog/tasks/qa/with_context/extractive.json
-src/unitxt/catalog/tasks/rag/model_response_assessment.json
+src/unitxt/catalog/tasks/rag/response_generation.json
 src/unitxt/catalog/tasks/regression/single_text.json
 src/unitxt/catalog/tasks/regression/two_texts.json
+src/unitxt/catalog/tasks/response_assessment/pairwise_comparison/multi_turn.json
+src/unitxt/catalog/tasks/response_assessment/pairwise_comparison/multi_turn_with_reference.json
+src/unitxt/catalog/tasks/response_assessment/pairwise_comparison/single_turn.json
+src/unitxt/catalog/tasks/response_assessment/pairwise_comparison/single_turn_with_reference.json
+src/unitxt/catalog/tasks/response_assessment/rating/multi_turn.json
+src/unitxt/catalog/tasks/response_assessment/rating/multi_turn_with_reference.json
+src/unitxt/catalog/tasks/response_assessment/rating/single_turn.json
+src/unitxt/catalog/tasks/response_assessment/rating/single_turn_with_reference.json
 src/unitxt/catalog/tasks/rewriting/by_attribute.json
 src/unitxt/catalog/tasks/rewriting/paraphrase.json
 src/unitxt/catalog/tasks/selection/by_attribute.json
 src/unitxt/catalog/tasks/span_labeling/extraction.json
 src/unitxt/catalog/tasks/summarization/abstractive.json
 src/unitxt/catalog/tasks/targeted_sentiment_extraction/all_sentiment_classes.json
 src/unitxt/catalog/tasks/targeted_sentiment_extraction/single_sentiment_class.json
@@ -845,22 +889,30 @@
 src/unitxt/catalog/templates/qa/with_context/all.json
 src/unitxt/catalog/templates/qa/with_context/ffqa.json
 src/unitxt/catalog/templates/qa/with_context/question_first.json
 src/unitxt/catalog/templates/qa/with_context/simple.json
 src/unitxt/catalog/templates/qa/with_context/simple2.json
 src/unitxt/catalog/templates/qa/with_context/title.json
 src/unitxt/catalog/templates/qa/with_context/with_type.json
-src/unitxt/catalog/templates/rag/model_response_assessment/llm_as_judge_using_mt_bench_template.json
+src/unitxt/catalog/templates/rag/response_generation/simple.json
 src/unitxt/catalog/templates/regression/single_text/all.json
 src/unitxt/catalog/templates/regression/single_text/simple.json
 src/unitxt/catalog/templates/regression/single_text/title.json
 src/unitxt/catalog/templates/regression/two_texts/all.json
 src/unitxt/catalog/templates/regression/two_texts/simple.json
 src/unitxt/catalog/templates/regression/two_texts/title.json
 src/unitxt/catalog/templates/regression/two_texts/similarity/flan.json
+src/unitxt/catalog/templates/response_assessment/pairwise_comparison/mt_bench_multi_turn_with_reference_with_shuffle.json
+src/unitxt/catalog/templates/response_assessment/pairwise_comparison/mt_bench_multi_turn_with_shuffle.json
+src/unitxt/catalog/templates/response_assessment/pairwise_comparison/mt_bench_single_turn_with_reference_with_shuffle.json
+src/unitxt/catalog/templates/response_assessment/pairwise_comparison/mt_bench_single_turn_with_shuffle.json
+src/unitxt/catalog/templates/response_assessment/rating/mt_bench_multi_turn.json
+src/unitxt/catalog/templates/response_assessment/rating/mt_bench_multi_turn_with_reference.json
+src/unitxt/catalog/templates/response_assessment/rating/mt_bench_single_turn.json
+src/unitxt/catalog/templates/response_assessment/rating/mt_bench_single_turn_with_reference.json
 src/unitxt/catalog/templates/rewriting/by_attribute/all.json
 src/unitxt/catalog/templates/rewriting/by_attribute/default.json
 src/unitxt/catalog/templates/rewriting/paraphrase/all.json
 src/unitxt/catalog/templates/rewriting/paraphrase/default.json
 src/unitxt/catalog/templates/selection/by_attribute/all.json
 src/unitxt/catalog/templates/selection/by_attribute/default.json
 src/unitxt/catalog/templates/span_labeling/extraction/all.json
@@ -907,14 +959,15 @@
 src/unitxt/catalog/templates/translation/directed/formal.json
 src/unitxt/catalog/templates/translation/directed/instructional.json
 src/unitxt/catalog/templates/translation/directed/playful.json
 src/unitxt/catalog/templates/translation/directed/simple.json
 src/unitxt/catalog/templates/translation/directed/title.json
 src/unitxt/prepare_utils/__init__.py
 src/unitxt/prepare_utils/card_types.py
+src/unitxt/prepare_utils/info_annotator.py
 src/unitxt/prepare_utils/instructions.py
 src/unitxt/service/__init__.py
 src/unitxt/service/metrics/__init__.py
 src/unitxt/service/metrics/main.py
 src/unitxt/service/metrics/tokens.py
 src/unitxt/test_utils/__init__.py
 src/unitxt/test_utils/artifact.py
```

### Comparing `unitxt-1.8.1/src/unitxt.egg-info/requires.txt` & `unitxt-1.9.0/src/unitxt.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 datasets>=2.16.0
 evaluate
 absl-py
 ipadic
 scipy
 
 [all]
-llama-index-core
-nltk
+rouge-score
+ruff
+pytrec-eval
+sphinxext-opengraph
+conllu
+openai
+sacrebleu
+mecab-python3
+ibm-generative-ai
 torch==1.12.1
+ipadic
 codespell
-opendatasets
 absl-py
-conllu
-ruff
-editdistance
-fastapi==0.109.0
+llama-index-llms-openai
+llama-index-core
+piccolo_theme
+nltk
 datasets
-sacrebleu[ko]
-mecab-python3
-sacrebleu
-crfm-helm[unitxt]>=0.5.0
-scikit-learn
-ipadic
 transformers
-datasets>=2.16.0
-uvicorn[standard]==0.27.0.post1
-scipy
+scikit-learn
 tomli
-piccolo_theme
-SentencePiece
+opendatasets
+uvicorn[standard]==0.27.0.post1
 sphinx_rtd_theme
-pre-commit
-sentence_transformers
-bert_score
-pytrec-eval
+scipy
+fastapi==0.109.0
 httpretty~=1.1.4
-rouge_score
-python-jose[cryptography]==3.3.0
-jiwer
 evaluate
 gradio
-sphinxext-opengraph
+bert_score
+editdistance
 ibm-cos-sdk
-llama-index-llms-openai
+crfm-helm[unitxt]>=0.5.0
+python-jose[cryptography]==3.3.0
+datasets>=2.16.0
+jiwer
+pre-commit
+sacrebleu[ko]
+SentencePiece
+sentence_transformers
 
 [base]
 datasets>=2.16.0
 evaluate
 absl-py
 ipadic
 scipy
@@ -96,11 +98,13 @@
 scikit-learn
 jiwer
 conllu
 llama-index-core
 llama-index-llms-openai
 pytrec-eval
 SentencePiece
+openai
+ibm-generative-ai
 
 [ui]
 gradio
 transformers
```

