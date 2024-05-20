# Comparing `tmp/shtec-rlhf-0.0.2.dev0.tar.gz` & `tmp/shtec-rlhf-0.0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shtec-rlhf-0.0.2.dev0.tar", last modified: Fri Apr 19 03:10:48 2024, max compression
+gzip compressed data, was "shtec-rlhf-0.0.3.dev0.tar", last modified: Mon May 20 15:22:56 2024, max compression
```

## Comparing `shtec-rlhf-0.0.2.dev0.tar` & `shtec-rlhf-0.0.3.dev0.tar`

### file list

```diff
@@ -1,143 +1,94 @@
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.126000 shtec-rlhf-0.0.2.dev0/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1300 2024-04-19 03:10:48.126000 shtec-rlhf-0.0.2.dev0/PKG-INFO
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     5303 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/pyproject.toml
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)       38 2024-04-19 03:10:48.126000 shtec-rlhf-0.0.2.dev0/setup.cfg
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1300 2024-04-16 08:16:59.000000 shtec-rlhf-0.0.2.dev0/setup.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.114000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1005 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/__init__.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.114000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      591 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/__init__.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.114000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/dpo/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      450 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/dpo/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      475 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/dpo/__main__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     9251 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/dpo/main.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    10049 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/dpo/trainer.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.118000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      423 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      484 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo/__main__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    13680 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo/main.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     9018 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo/trainer.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.118000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo_lag/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      448 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo_lag/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      503 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo_lag/__main__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    15371 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo_lag/main.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    18526 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo_lag/trainer.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.118000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo_reward_shaping/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      489 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo_reward_shaping/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      525 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo_reward_shaping/__main__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    14472 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo_reward_shaping/main.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    11517 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo_reward_shaping/trainer.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.118000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/configs/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      702 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/configs/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1233 2024-04-16 07:11:10.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/configs/constants.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     5026 2024-04-16 07:11:13.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/configs/deepspeed_config.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      443 2024-04-16 06:27:36.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/configs/ds_eval_config_template.json
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      872 2024-04-16 06:27:36.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/configs/ds_train_config_template.json
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)       66 2024-04-16 06:27:36.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/configs/fsdp_config.json
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.118000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     2085 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    15436 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/base.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3801 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/preference.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     2648 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/prompt_only.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.118000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/raw/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1228 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/raw/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1180 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/raw/alpaca.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      961 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/raw/firefly.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     4428 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/raw/hh_rlhf.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     4205 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/raw/moss.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     2582 2024-04-19 03:07:32.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/raw/shtec_rlhf.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     5352 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/safety_preference.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3925 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/supervised.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1674 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/utils.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.118000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      306 2024-04-16 06:55:53.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    19517 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/arena.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.118000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/bigbench/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      307 2024-04-16 06:54:46.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/bigbench/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      420 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/bigbench/__main__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     6463 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/bigbench/eval.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     6635 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/bigbench/model.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    13385 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/cost.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.118000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/gpt4/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      307 2024-04-16 06:54:39.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/gpt4/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      417 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/gpt4/__main__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     5801 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/gpt4/eval.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    13213 2024-04-16 06:27:36.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/gpt4/problem.json
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     9656 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/reward.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/finetune/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      452 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/finetune/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      475 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/finetune/__main__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     8849 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/finetune/deepspeed.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     2822 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/finetune/huggingface.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      458 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/finetune/main.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     2395 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/finetune/trainer.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     7572 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/logger.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      584 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     6565 2024-04-16 06:54:13.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/normalizer.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     7439 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/pretrained.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     9326 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/__init__.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/bloom/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      385 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/bloom/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     4143 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/bloom/modeling_bloom.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gemma/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      385 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gemma/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3651 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gemma/modeling_gemma.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gpt2/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      382 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gpt2/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     6137 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gpt2/modeling_gpt2.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gpt_neo/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      390 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gpt_neo/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3919 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gpt_neo/modeling_gpt_neo.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gpt_neox/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      393 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gpt_neox/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3629 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gpt_neox/modeling_gpt_neox.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gptj/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      382 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gptj/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     5867 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gptj/modeling_gptj.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/llama/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      385 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/llama/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3651 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/llama/modeling_llama.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/mistral/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      391 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/mistral/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3361 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/mistral/modeling_mistral.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/opt/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)       71 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/opt/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3344 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/opt/modeling_opt.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/phi/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)       71 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/phi/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3325 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/phi/modeling_phi.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/qwen2/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)       77 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/qwen2/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3537 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/qwen2/modeling_qwen2.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/serve/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      307 2024-04-16 06:51:12.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/serve/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     2803 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/serve/arena.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    11809 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/serve/chatbot.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     8659 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/serve/cli.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/trainers/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      262 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/trainers/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     4349 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/trainers/base.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    25698 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/trainers/rl_trainer.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     8535 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/trainers/supervised_trainer.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     9193 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/utils.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      179 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/__init__.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.126000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/cost/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)       83 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/cost/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      176 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/cost/__main__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     9733 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/cost/main.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    13712 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/cost/trainer.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.126000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/reward/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      397 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/reward/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      487 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/reward/__main__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     9753 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/reward/main.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    10744 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/reward/trainer.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1439 2024-04-19 03:10:47.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/version.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.114000 shtec-rlhf-0.0.2.dev0/shtec_rlhf.egg-info/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1300 2024-04-19 03:10:48.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf.egg-info/PKG-INFO
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     4078 2024-04-19 03:10:48.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf.egg-info/SOURCES.txt
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)        1 2024-04-19 03:10:48.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf.egg-info/dependency_links.txt
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      360 2024-04-19 03:10:48.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf.egg-info/requires.txt
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)       11 2024-04-19 03:10:48.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf.egg-info/top_level.txt
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-05-20 15:22:56.766695 shtec-rlhf-0.0.3.dev0/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    11370 2024-05-20 15:14:28.000000 shtec-rlhf-0.0.3.dev0/LICENSE
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1312 2024-05-20 15:22:56.766695 shtec-rlhf-0.0.3.dev0/PKG-INFO
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     5262 2024-05-20 15:16:10.000000 shtec-rlhf-0.0.3.dev0/pyproject.toml
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)       38 2024-05-20 15:22:56.766695 shtec-rlhf-0.0.3.dev0/setup.cfg
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1668 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/setup.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-05-20 15:22:56.758695 shtec-rlhf-0.0.3.dev0/shtec_rlhf/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1348 2024-05-20 15:21:58.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/__init__.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-05-20 15:22:56.758695 shtec-rlhf-0.0.3.dev0/shtec_rlhf/configs/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1070 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/configs/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1601 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/configs/constants.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     5394 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/configs/deepspeed_config.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      443 2024-05-20 14:58:31.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/configs/ds_eval_config_template.json
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      872 2024-05-20 14:58:31.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/configs/ds_train_config_template.json
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)       66 2024-05-20 14:58:31.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/configs/fsdp_config.json
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-05-20 15:22:56.762695 shtec-rlhf-0.0.3.dev0/shtec_rlhf/datasets/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     2453 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/datasets/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    15788 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/datasets/base.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     4169 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/datasets/preference.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3016 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/datasets/prompt_only.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-05-20 15:22:56.762695 shtec-rlhf-0.0.3.dev0/shtec_rlhf/datasets/raw/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1411 2024-05-20 15:20:27.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/datasets/raw/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     2946 2024-05-20 15:19:59.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/datasets/raw/safe_rlhf.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     5720 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/datasets/safety_preference.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     4293 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/datasets/supervised.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     2042 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/datasets/utils.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-05-20 15:22:56.762695 shtec-rlhf-0.0.3.dev0/shtec_rlhf/evaluate/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      675 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/evaluate/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    19872 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/evaluate/arena.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-05-20 15:22:56.762695 shtec-rlhf-0.0.3.dev0/shtec_rlhf/evaluate/bigbench/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      675 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/evaluate/bigbench/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      789 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/evaluate/bigbench/__main__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     6831 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/evaluate/bigbench/eval.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     7003 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/evaluate/bigbench/model.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    13740 2024-05-20 15:16:10.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/evaluate/cost.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-05-20 15:22:56.762695 shtec-rlhf-0.0.3.dev0/shtec_rlhf/evaluate/gpt4/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      675 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/evaluate/gpt4/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      785 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/evaluate/gpt4/__main__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     5830 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/evaluate/gpt4/eval.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    13213 2024-05-20 14:58:31.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/evaluate/gpt4/problem.json
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    10011 2024-05-20 15:16:10.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/evaluate/reward.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-05-20 15:22:56.762695 shtec-rlhf-0.0.3.dev0/shtec_rlhf/finetune/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      820 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/finetune/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      843 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/finetune/__main__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     9217 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/finetune/deepspeed.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3190 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/finetune/huggingface.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      826 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/finetune/main.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     2763 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/finetune/trainer.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     7940 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/logger.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-05-20 15:22:56.762695 shtec-rlhf-0.0.3.dev0/shtec_rlhf/models/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      952 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/models/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     6933 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/models/normalizer.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     6910 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/models/pretrained.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-05-20 15:22:56.762695 shtec-rlhf-0.0.3.dev0/shtec_rlhf/models/score_model/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     7483 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/models/score_model/__init__.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-05-20 15:22:56.762695 shtec-rlhf-0.0.3.dev0/shtec_rlhf/models/score_model/llama/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      758 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/models/score_model/llama/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     4586 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/models/score_model/llama/modeling_llama.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-05-20 15:22:56.762695 shtec-rlhf-0.0.3.dev0/shtec_rlhf/models/score_model/open_llama/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      767 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/models/score_model/open_llama/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     4775 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/models/score_model/open_llama/modeling_open_llama.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-05-20 15:22:56.762695 shtec-rlhf-0.0.3.dev0/shtec_rlhf/models/score_model/opt/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      747 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/models/score_model/opt/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     4544 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/models/score_model/opt/modeling_opt.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-05-20 15:22:56.762695 shtec-rlhf-0.0.3.dev0/shtec_rlhf/serve/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      675 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/serve/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3479 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/serve/arena.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    12500 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/serve/chatbot.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     9334 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/serve/cli.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-05-20 15:22:56.762695 shtec-rlhf-0.0.3.dev0/shtec_rlhf/trainers/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      937 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/trainers/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     5024 2024-05-20 15:16:10.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/trainers/base.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    26217 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/trainers/rl_trainer.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     9197 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/trainers/supervised_trainer.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     9071 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/utils.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-05-20 15:22:56.762695 shtec-rlhf-0.0.3.dev0/shtec_rlhf/values/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      854 2024-05-20 15:16:10.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/values/__init__.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-05-20 15:22:56.762695 shtec-rlhf-0.0.3.dev0/shtec_rlhf/values/cost/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      759 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/values/cost/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      851 2024-05-20 15:16:10.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/values/cost/__main__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    10408 2024-05-20 15:16:10.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/values/cost/main.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    13534 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/values/cost/trainer.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-05-20 15:22:56.766695 shtec-rlhf-0.0.3.dev0/shtec_rlhf/values/reward/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      765 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/values/reward/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      855 2024-05-20 15:16:10.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/values/reward/__main__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    10428 2024-05-20 15:16:10.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/values/reward/main.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    10795 2024-05-20 15:14:50.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/values/reward/trainer.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1797 2024-05-20 15:22:56.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf/version.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-05-20 15:22:56.758695 shtec-rlhf-0.0.3.dev0/shtec_rlhf.egg-info/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1312 2024-05-20 15:22:56.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf.egg-info/PKG-INFO
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     2441 2024-05-20 15:22:56.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf.egg-info/SOURCES.txt
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)        1 2024-05-20 15:22:56.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf.egg-info/dependency_links.txt
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      360 2024-05-20 15:22:56.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf.egg-info/requires.txt
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)       11 2024-05-20 15:22:56.000000 shtec-rlhf-0.0.3.dev0/shtec_rlhf.egg-info/top_level.txt
```

### Comparing `shtec-rlhf-0.0.2.dev0/PKG-INFO` & `shtec-rlhf-0.0.3.dev0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: shtec-rlhf
-Version: 0.0.2.dev0
+Version: 0.0.3.dev0
 Summary: shtec-rlhf: Safe Reinforcement Learning from Human Feedback
-Author: PKU-Alignment Team
+Author: tcexeexe
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://github.com/PKU-Alignment/shtec-rlhf
 Project-URL: Repository, https://github.com/PKU-Alignment/shtec-rlhf
 Project-URL: Documentation, https://shtec-rlhf.readthedocs.io
 Project-URL: Bug Report, https://github.com/PKU-Alignment/shtec-rlhf
 Keywords: Reinforcement Learning,Safe Reinforcement Learning,Reinforcement Learning from Human Feedback,Safe Reinforcement Learning from Human Feedback,Large Language Model,Language Model,RLHF,Safe RLHF,LLM
 Classifier: Development Status :: 4 - Beta
@@ -18,7 +18,8 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: lint
+License-File: LICENSE
```

### Comparing `shtec-rlhf-0.0.2.dev0/pyproject.toml` & `shtec-rlhf-0.0.3.dev0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "shtec-rlhf"
 description = "shtec-rlhf: Safe Reinforcement Learning from Human Feedback"
 readme = "README.md"
 requires-python = ">= 3.8"
-authors = [{ name = "PKU-Alignment Team" }]
+authors = [{ name = "tcexeexe" }]
 license = { text = "Apache License, Version 2.0" }
 keywords = [
     "Reinforcement Learning",
     "Safe Reinforcement Learning",
     "Reinforcement Learning from Human Feedback",
     "Safe Reinforcement Learning from Human Feedback",
     "Large Language Model",
@@ -32,15 +32,15 @@
     "Programming Language :: Python :: 3.11",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
     "torch >= 1.13",
-    "transformers >= 4.37",
+    "transformers >= 4.29",
     "datasets",
     "tokenizers >= 0.13.3",
     "accelerate",
     "deepspeed",
     "numpy",
     "scipy",
     "sentencepiece",
@@ -86,14 +86,15 @@
 
 [tool.setuptools.package-data]
 "*" = ["*.json", "*.jsonl", "*.yaml", "*.yml"]
 
 # Linter tools #################################################################
 
 [tool.black]
+safe = true
 line-length = 100
 skip-string-normalization = true
 # Sync with requires-python
 target-version = ["py38", "py39", "py310", "py311"]
 
 [tool.isort]
 atomic = true
@@ -102,22 +103,22 @@
 extra_standard_library = ["typing_extensions"]
 indent = 4
 line_length = 100
 lines_after_imports = 2
 multi_line_output = 3
 
 [tool.mypy]
-python_version = "3.8"
+python_version = 3.8
 pretty = true
 show_error_codes = true
 show_error_context = true
 show_traceback = true
 allow_redefinition = true
 check_untyped_defs = true
-disallow_incomplete_defs = true
+disallow_incomplete_defs = false
 disallow_untyped_defs = false
 ignore_missing_imports = true
 no_implicit_optional = true
 strict_equality = true
 strict_optional = true
 warn_no_return = true
 warn_redundant_casts = true
@@ -134,18 +135,16 @@
 [tool.codespell]
 ignore-words = "docs/source/spelling_wordlist.txt"
 
 [tool.ruff]
 # Sync with requires-python
 target-version = "py38"
 line-length = 100
-output-format = "full"
+show-source = true
 src = ["shtec_rlhf", "tests", "examples"]
-
-[tool.ruff.lint]
 select = [
     "E",
     "W",   # pycodestyle
     "F",   # pyflakes
     "UP",  # pyupgrade
     "ANN", # flake8-annotations
     "S",   # flake8-bandit
@@ -180,32 +179,32 @@
     # internal use and may never raise at runtime
     "S101",
     # PLR0402: use from {module} import {name} in lieu of alias
     # use alias for import convention (e.g., `import torch.nn as nn`)
     "PLR0402",
 ]
 
-[tool.ruff.lint.per-file-ignores]
+[tool.ruff.per-file-ignores]
 "__init__.py" = [
     "F401", # unused-import
 ]
 "shtec_rlhf/evaluate/bigbench/**/*.py" = [
     "ANN", # flake8-annotations
     "S",   # flake8-bandit
     "BLE", # flake8-blind-except
 ]
 "tests/**/*.py" = [
     "ANN", # flake8-annotations
     "S",   # flake8-bandit
     "BLE", # flake8-blind-except
 ]
 
-[tool.ruff.lint.flake8-annotations]
+[tool.ruff.flake8-annotations]
 allow-star-arg-any = true
 
-[tool.ruff.lint.flake8-quotes]
+[tool.ruff.flake8-quotes]
 docstring-quotes = "double"
 multiline-quotes = "double"
 inline-quotes = "single"
 
-[tool.ruff.lint.flake8-tidy-imports]
+[tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/dpo/main.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/values/cost/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,43 @@
-#******************************************************************************************************** 
-#  @author	     tcexeexe
-#  @date         04,2024
+# Copyright 2024 tcexeexe. All Rights Reserved.
 #
-#  @par     Copyright (c) 2024, SHTEC
-# 
-# *******************************************************************************************************/
-"""The main training script to run the DPO algorithm."""
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
+"""The main training script to train a cost model in shtec-rlhf."""
 
 import argparse
 
 import deepspeed
 import torch
 import torch.distributed as dist
 from transformers import SchedulerType
 from transformers.utils import is_torch_bf16_gpu_available, is_torch_tf32_available
 
-from shtec_rlhf.algorithms.dpo.trainer import DPOTrainer
-from shtec_rlhf.configs import get_deepspeed_eval_config, get_deepspeed_train_config
+from shtec_rlhf.configs import get_deepspeed_train_config
 from shtec_rlhf.datasets import parse_dataset
 from shtec_rlhf.logger import set_logger_level
 from shtec_rlhf.utils import seed_everything, str2bool
+from shtec_rlhf.values.cost.trainer import CostTrainer
 
 
 def parse_arguments() -> argparse.Namespace:
     """Parse the command-line arguments."""
     parser = argparse.ArgumentParser(
-        prog='deepspeed --module shtec_rlhf.algorithms.dpo',
-        description='Train language model with the DPO algorithm.',
+        prog='deepspeed --module shtec_rlhf.values.cost',
+        description='Train a cost model.',
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     # Model
     model_parser = parser.add_argument_group('model')
     model_parser.add_argument(
         '--model_name_or_path',
@@ -68,18 +75,22 @@
         metavar='DATASET[:PROPORTION[:PATH]]',
         help='Dataset name(s) registered in the raw dataset.',
     )
 
     # Training
     training_parser = parser.add_argument_group('training')
     training_parser.add_argument(
-        '--scale_coeff',
-        type=float,
-        default=0.02,
-        help='The coefficient for the KL divergence between the reference and actor policy.',
+        '--loss_type',
+        type=str,
+        choices=['token-wise', 'sequence-wise'],
+        default='sequence-wise',
+        help=(
+            'Calculate ranking loss with all token-wise cost outputs in the sequence or the '
+            'sequence-wise cost output only (the cost of the last token in each sequence).'
+        ),
     )
     training_parser.add_argument(
         '--epochs',
         type=int,
         default=1,
         help='Total number of training epochs to perform.',
     )
@@ -103,14 +114,42 @@
     )
     training_parser.add_argument(
         '--gradient_checkpointing',
         action='store_true',
         help='Enable HF gradient checkpointing for actor model.',
     )
     training_parser.add_argument(
+        '--regularization',
+        type=float,
+        default=0.0,
+        help='The regularization strength for the L2 regularization for score outputs.',
+    )
+    training_parser.add_argument(
+        '--normalize_score_during_training',
+        type=str2bool,
+        default=False,
+        help='Whether to normalize the reward outputs when training.',
+    )
+    training_parser.add_argument(
+        '--normalizer_type',
+        type=str,
+        choices=['RunningMeanStd', 'ExponentialMovingAverage'],
+        default=None,
+        help='The type of the cost normalizer.',
+    )
+    training_parser.add_argument(
+        '--normalizer_momentum',
+        type=float,
+        default=None,
+        help=(
+            'The momentum use in ExponentialMovingAverage, '
+            'EMA_{t+1} = momentum * x + (1 - momentum) * EMA_t.',
+        ),
+    )
+    training_parser.add_argument(
         '--lr',
         '--learning_rate',
         type=float,
         default=2e-5,
         help='Initial learning rate (after the potential warmup period) to use.',
     )
     training_parser.add_argument(
@@ -132,16 +171,16 @@
         type=float,
         default=0.0,
         help='Ratio of warm steps over total training steps for the lr scheduler.',
     )
     training_parser.add_argument(
         '--weight_decay',
         type=float,
-        default=0.0,
-        help='Weight decay to for the model training.',
+        default=1.0e-6,
+        help='Weight decay to use.',
     )
     training_parser.add_argument(
         '--seed',
         type=int,
         default=42,
         help='A seed for reproducible training.',
     )
@@ -184,15 +223,14 @@
         default=False,
         help='Whether to evaluate the model during training.',
         action='store_true',
     )
     evaluation_parser.add_argument(
         '--eval_split_ratio',
         type=float,
-        default=None,
         help='The split ratio of the evaluation dataset.',
     )
 
     # Logging
     logging_parser = parser.add_argument_group('logging')
     logging_parser.add_argument(
         '--output_dir',
@@ -287,30 +325,23 @@
     args.device = torch.device('cuda', args.local_rank)
     torch.cuda.set_device(args.device)
     seed_everything(args.seed)
     set_logger_level()
 
     dist.barrier()
 
-    ds_train_config = get_deepspeed_train_config(
+    ds_config = get_deepspeed_train_config(
         micro_batch_size_per_gpu=args.per_device_train_batch_size,
         gradient_accumulation_steps=args.gradient_accumulation_steps,
         stage=args.zero_stage,
         offload=args.offload,
         fp16=args.fp16,
         bf16=args.bf16,
     )
 
-    ds_eval_config = get_deepspeed_eval_config(
-        stage=args.zero_stage,
-        offload=args.offload,
-        fp16=args.fp16,
-        bf16=args.bf16,
-    )
-
-    trainer = DPOTrainer(args, ds_train_config, ds_eval_config)
+    trainer = CostTrainer(args, ds_config)
     trainer.train()
     trainer.save()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo/main.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/values/reward/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,55 @@
-#******************************************************************************************************** 
-#  @author	     tcexeexe
-#  @date         04,2024
+# Copyright 2024 tcexeexe. All Rights Reserved.
 #
-#  @par     Copyright (c) 2024, SHTEC
-# 
-# *******************************************************************************************************/
-"""The main training script to train RLHF using PPO algorithm."""
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
+"""The main training script to train a reward model in shtec-rlhf."""
 
 import argparse
 
 import deepspeed
 import torch
 import torch.distributed as dist
 from transformers import SchedulerType
 from transformers.utils import is_torch_bf16_gpu_available, is_torch_tf32_available
 
-from shtec_rlhf.algorithms.ppo.trainer import PPOTrainer
-from shtec_rlhf.configs import get_deepspeed_eval_config, get_deepspeed_train_config
+from shtec_rlhf.configs import get_deepspeed_train_config
 from shtec_rlhf.datasets import parse_dataset
 from shtec_rlhf.logger import set_logger_level
 from shtec_rlhf.utils import seed_everything, str2bool
+from shtec_rlhf.values.reward.trainer import RewardTrainer
 
 
 def parse_arguments() -> argparse.Namespace:
     """Parse the command-line arguments."""
     parser = argparse.ArgumentParser(
-        prog='deepspeed --module shtec_rlhf.algorithms.ppo',
-        description='Train language model using RLHF with PPO algorithm.',
+        prog='deepspeed --module shtec_rlhf.values.reward',
+        description='Train a reward model.',
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     # Model
     model_parser = parser.add_argument_group('model')
     model_parser.add_argument(
-        '--actor_model_name_or_path',
-        type=str,
-        help='Path to the model checkpoint or its name.',
-        required=True,
-    )
-    model_parser.add_argument(
-        '--reward_model_name_or_path',
+        '--model_name_or_path',
         type=str,
         help='Path to the model checkpoint or its name.',
         required=True,
     )
     model_parser.add_argument(
-        '--reward_critic_model_name_or_path',
-        type=str,
-        help='Path to the model checkpoint or its name.',
-    )
-    model_parser.add_argument(
         '--max_length',
         type=int,
         default=512,
         help='The maximum sequence length of the model.',
     )
     model_parser.add_argument(
         '--trust_remote_code',
@@ -69,90 +65,40 @@
         type=parse_dataset,
         nargs='+',
         metavar='DATASET[:PROPORTION[:PATH]]',
         help='Dataset name(s) registered in the raw dataset.',
         required=True,
     )
     dataset_parser.add_argument(
-        '--ptx_datasets',
-        type=parse_dataset,
-        nargs='*',
-        metavar='DATASET[:PROPORTION[:PATH]]',
-        help='Dataset name(s) registered in the raw dataset.',
-    )
-    dataset_parser.add_argument(
         '--eval_datasets',
         type=parse_dataset,
         nargs='+',
         metavar='DATASET[:PROPORTION[:PATH]]',
         help='Dataset name(s) registered in the raw dataset.',
     )
 
     # Training
     training_parser = parser.add_argument_group('training')
     training_parser.add_argument(
-        '--kl_coeff',
-        type=float,
-        default=0.02,
-        help='The coefficient for the KL divergence between the reference and actor policy.',
-    )
-    training_parser.add_argument(
-        '--clip_range_ratio',
-        type=float,
-        default=0.2,
-        help=(
-            'The clipping range for ratio between the old and new policy. '
-            'This is the epsilon parameter in the PPO algorithm.'
-        ),
-    )
-    training_parser.add_argument(
-        '--clip_range_score',
-        type=float,
-        default=50.0,
-        help=(
-            'The clipping range for the output of the score model. '
-            'The reward is clipped into [-clip_range_score, clip_range_score].'
-        ),
-    )
-    training_parser.add_argument(
-        '--clip_range_value',
-        type=float,
-        default=5.0,
+        '--loss_type',
+        type=str,
+        choices=['token-wise', 'sequence-wise'],
+        default='sequence-wise',
         help=(
-            'The clipping range for the value function. '
-            'The value is clipped into '
-            '[value_estimate - clip_range_value, value_estimate + clip_range_value] '
-            'during training.'
+            'Calculate ranking loss with all token-wise reward outputs in the sequence or the '
+            'sequence-wise reward output only (the reward of the last token in each sequence).'
         ),
     )
     training_parser.add_argument(
-        '--ptx_coeff',
-        type=float,
-        default=0.0,
-        help='The coefficient for the ptx loss.',
-    )
-    training_parser.add_argument(
         '--epochs',
         type=int,
         default=1,
         help='Total number of training epochs to perform.',
     )
     training_parser.add_argument(
-        '--update_iters',
-        type=int,
-        default=1,
-        help='The number of repeated updates on a generated batch.',
-    )
-    training_parser.add_argument(
-        '--per_device_prompt_batch_size',
-        type=int,
-        default=16,
-        help='Batch size (per device) for the training dataloader.',
-    )
-    training_parser.add_argument(
         '--per_device_train_batch_size',
         type=int,
         default=16,
         help='Batch size (per device) for the training dataloader.',
     )
     training_parser.add_argument(
         '--per_device_eval_batch_size',
@@ -163,94 +109,78 @@
     training_parser.add_argument(
         '--gradient_accumulation_steps',
         type=int,
         default=1,
         help='Number of updates steps to accumulate before performing a backward/update pass.',
     )
     training_parser.add_argument(
-        '--actor_lr',
-        '--actor_learning_rate',
-        type=float,
-        default=1e-5,
-        help='Initial learning rate (after the potential warmup period) for the actor model training.',
+        '--gradient_checkpointing',
+        action='store_true',
+        help='Enable HF gradient checkpointing for actor model.',
     )
     training_parser.add_argument(
-        '--actor_weight_decay',
+        '--regularization',
         type=float,
         default=0.0,
-        help='Weight decay to for the actor model training.',
-    )
-    training_parser.add_argument(
-        '--actor_lr_scheduler_type',
-        type=SchedulerType,
-        default='cosine',
-        help='The scheduler type for actor model.',
-        choices=[
-            'linear',
-            'cosine',
-            'cosine_with_restarts',
-            'polynomial',
-            'constant',
-            'constant_with_warmup',
-        ],
+        help='The regularization strength for the L2 regularization for score outputs.',
     )
     training_parser.add_argument(
-        '--actor_lr_warmup_ratio',
-        type=float,
-        default=0.0,
-        help='Ratio of warm steps over total training steps for the actor lr scheduler.',
+        '--normalize_score_during_training',
+        type=str2bool,
+        default=False,
+        help='Whether to normalize the reward outputs when training.',
     )
     training_parser.add_argument(
-        '--actor_gradient_checkpointing',
-        action='store_true',
-        help='Enable gradient checkpointing for actor model.',
+        '--normalizer_type',
+        type=str,
+        choices=['RunningMeanStd', 'ExponentialMovingAverage'],
+        default=None,
+        help='The type of the reward normalizer.',
     )
     training_parser.add_argument(
-        '--critic_lr',
-        '--critic_learning_rate',
+        '--normalizer_momentum',
         type=float,
-        default=5e-6,
-        help='Initial learning rate (after the potential warmup period) for the critic model training.',
+        default=None,
+        help=(
+            'The momentum use in ExponentialMovingAverage, '
+            'EMA_{t+1} = momentum * x + (1 - momentum) * EMA_t.',
+        ),
     )
     training_parser.add_argument(
-        '--critic_weight_decay',
+        '--lr',
+        '--learning_rate',
         type=float,
-        default=0.0,
-        help='Weight decay to for the critic model training.',
+        default=2e-5,
+        help='Initial learning rate (after the potential warmup period) to use.',
     )
     training_parser.add_argument(
-        '--critic_lr_scheduler_type',
+        '--lr_scheduler_type',
         type=SchedulerType,
         default='cosine',
-        help='The scheduler type for critic model.',
+        help='The scheduler type to use.',
         choices=[
             'linear',
             'cosine',
             'cosine_with_restarts',
             'polynomial',
             'constant',
             'constant_with_warmup',
         ],
     )
     training_parser.add_argument(
-        '--critic_lr_warmup_ratio',
+        '--lr_warmup_ratio',
         type=float,
         default=0.0,
-        help='Ratio of warm steps over total training steps for the critic lr scheduler.',
+        help='Ratio of warm steps over total training steps for the lr scheduler.',
     )
     training_parser.add_argument(
-        '--critic_gradient_checkpointing',
-        action='store_true',
-        help='Enable gradient checkpointing for critic model.',
-    )
-    training_parser.add_argument(
-        '--normalize_reward',
-        type=str2bool,
-        default=False,
-        help='Whether to normalize the reward during RL training.',
+        '--weight_decay',
+        type=float,
+        default=1.0e-6,
+        help='Weight decay to use.',
     )
     training_parser.add_argument(
         '--seed',
         type=int,
         default=42,
         help='A seed for reproducible training.',
     )
@@ -269,44 +199,14 @@
     training_parser.add_argument(
         '--tf32',
         type=str2bool,
         default=None,
         help='Whether to use tf32 mix precision.',
     )
 
-    # Generation Config
-    generation_parser = parser.add_argument_group('generation')
-    generation_parser.add_argument(
-        '--temperature',
-        type=float,
-        default=1.0,
-        help='The value used to module the next token probabilities.',
-    )
-    generation_parser.add_argument(
-        '--top_p',
-        type=float,
-        default=1.0,
-        help=(
-            'If set to float < 1, only the smallest set of most probable tokens with '
-            'probabilities that add up to`top_p` or higher are kept for generation.'
-        ),
-    )
-    generation_parser.add_argument(
-        '--num_return_sequences',
-        type=int,
-        default=1,
-        help='The number of independently computed returned sequences for each element in the batch.',
-    )
-    generation_parser.add_argument(
-        '--repetition_penalty',
-        type=float,
-        default=1.0,
-        help='The parameter for repetition penalty. 1.0 means no penalty.',
-    )
-
     # Evaluation
     evaluation_parser = parser.add_argument_group('evaluation')
     evaluation_parser.add_argument(
         '--eval_strategy',
         type=str,
         default='epoch',
         help='The evaluation strategy to adopt.',
@@ -323,15 +223,14 @@
         default=False,
         help='Whether to evaluate the model during training.',
         action='store_true',
     )
     evaluation_parser.add_argument(
         '--eval_split_ratio',
         type=float,
-        default=None,
         help='The split ratio of the evaluation dataset.',
     )
 
     # Logging
     logging_parser = parser.add_argument_group('logging')
     logging_parser.add_argument(
         '--output_dir',
@@ -426,30 +325,23 @@
     args.device = torch.device('cuda', args.local_rank)
     torch.cuda.set_device(args.device)
     seed_everything(args.seed)
     set_logger_level()
 
     dist.barrier()
 
-    ds_train_config = get_deepspeed_train_config(
+    ds_config = get_deepspeed_train_config(
         micro_batch_size_per_gpu=args.per_device_train_batch_size,
         gradient_accumulation_steps=args.gradient_accumulation_steps,
         stage=args.zero_stage,
         offload=args.offload,
         fp16=args.fp16,
         bf16=args.bf16,
     )
 
-    ds_eval_config = get_deepspeed_eval_config(
-        stage=args.zero_stage,
-        offload=args.offload,
-        fp16=args.fp16,
-        bf16=args.bf16,
-    )
-
-    trainer = PPOTrainer(args, ds_train_config, ds_eval_config)
+    trainer = RewardTrainer(args, ds_config)
     trainer.train()
     trainer.save()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/configs/constants.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/configs/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,21 @@
-#******************************************************************************************************** 
-#  @author	     tcexeexe
-#  @date         04,2024
+# Copyright 2024 tcexeexe. All Rights Reserved.
 #
-#  @par     Copyright (c) 2024, SHTEC
-# 
-# *******************************************************************************************************/
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
 """Constant variables."""
 
 from __future__ import annotations
 
 
 __all__ = [
     'IGNORE_INDEX',
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/configs/deepspeed_config.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/configs/deepspeed_config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,21 @@
-#******************************************************************************************************** 
-#  @author	     tcexeexe
-#  @date         04,2024
+# Copyright 2024 tcexeexe. All Rights Reserved.
 #
-#  @par     Copyright (c) 2024, SHTEC
-# 
-# *******************************************************************************************************/
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
 """DeepSpeed configuration for training and evaluation."""
 
 from __future__ import annotations
 
 import json
 import pathlib
 from typing import Any, Literal
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/configs/ds_train_config_template.json` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/configs/ds_train_config_template.json`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/__init__.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/datasets/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,21 @@
-#******************************************************************************************************** 
-#  @author	     tcexeexe
-#  @date         04,2024
+# Copyright 2024 tcexeexe. All Rights Reserved.
 #
-#  @par     Copyright (c) 2024, SHTEC
-# 
-# *******************************************************************************************************/
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
 """Dataset classes."""
 
 from __future__ import annotations
 
 from typing import Dict
 
 import torch
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/base.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/datasets/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,21 @@
-#******************************************************************************************************** 
-#  @author	     tcexeexe
-#  @date         04,2024
+# Copyright 2024 tcexeexe. All Rights Reserved.
 #
-#  @par     Copyright (c) 2024, SHTEC
-# 
-# *******************************************************************************************************/
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
 """Base dataset class."""
 
 from __future__ import annotations
 
 import abc
 import copy
 import os
@@ -202,17 +209,16 @@
     data: list[dict[str, torch.Tensor]]
     """Tokenized data samples."""
 
     _SENTINEL: Any = object()
 
     def __init__(  # pylint: disable=too-many-branches
         self,
-        dataset_names_and_attributes: (
-            dict[str, float | dict[str, Any]] | Iterable[tuple[str, float | dict[str, Any]]]
-        ),
+        dataset_names_and_attributes: dict[str, float | dict[str, Any]]
+        | Iterable[tuple[str, float | dict[str, Any]]],
         tokenizer: transformers.PreTrainedTokenizerBase,
         lazy_tokenization: bool = True,
         seed: int = 42,
     ) -> None:
         if not isinstance(dataset_names_and_attributes, dict):
             dataset_names_and_attributes = tuple(dataset_names_and_attributes)
             dataset_names = [name for name, _ in dataset_names_and_attributes]
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/prompt_only.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/datasets/prompt_only.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,21 @@
-#******************************************************************************************************** 
-#  @author	     tcexeexe
-#  @date         04,2024
+# Copyright 2024 tcexeexe. All Rights Reserved.
 #
-#  @par     Copyright (c) 2024, SHTEC
-# 
-# *******************************************************************************************************/
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
 
 from __future__ import annotations
 
 from typing import Callable, Hashable
 from typing_extensions import TypedDict  # Python 3.10+
 
 import torch
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/safety_preference.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/datasets/safety_preference.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,21 @@
-#******************************************************************************************************** 
-#  @author	     tcexeexe
-#  @date         04,2024
+# Copyright 2024 tcexeexe. All Rights Reserved.
 #
-#  @par     Copyright (c) 2024, SHTEC
-# 
-# *******************************************************************************************************/
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
 
 from __future__ import annotations
 
 from typing import Callable
 from typing_extensions import TypedDict  # Python 3.10+
 
 import torch
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/supervised.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/datasets/supervised.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,21 @@
-#******************************************************************************************************** 
-#  @author	     tcexeexe
-#  @date         04,2024
+# Copyright 2024 tcexeexe. All Rights Reserved.
 #
-#  @par     Copyright (c) 2024, SHTEC
-# 
-# *******************************************************************************************************/
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
 
 from __future__ import annotations
 
 from typing import Callable
 from typing_extensions import TypedDict  # Python 3.10+
 
 import torch
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/arena.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/evaluate/arena.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,21 @@
-#******************************************************************************************************** 
-#  @author	     tcexeexe
-#  @date         04,2024
+# Copyright 2024 tcexeexe. All Rights Reserved.
 #
-#  @par     Copyright (c) 2024, SHTEC
-# 
-# *******************************************************************************************************/
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
 
 from __future__ import annotations
 
 import argparse
 import csv
 import os
 from typing import NamedTuple
@@ -20,15 +27,15 @@
 import torch.nn.functional as F
 from rich.console import Console
 from rich.table import Table
 from torch.utils.data import DataLoader
 from torch.utils.data.distributed import DistributedSampler
 from tqdm import tqdm
 from transformers import AutoModelForCausalLM, PreTrainedModel, PreTrainedTokenizerBase
-from transformers.integrations.deepspeed import HfDeepSpeedConfig
+from transformers.deepspeed import HfDeepSpeedConfig
 from transformers.utils import is_torch_bf16_gpu_available, is_torch_tf32_available
 
 from shtec_rlhf.configs import get_deepspeed_eval_config
 from shtec_rlhf.datasets import PromptOnlyDataset, parse_dataset
 from shtec_rlhf.logger import set_logger_level
 from shtec_rlhf.models import AutoModelForScore, load_pretrained_models
 from shtec_rlhf.utils import (
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/bigbench/eval.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/evaluate/bigbench/eval.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,21 @@
-#******************************************************************************************************** 
-#  @author	     tcexeexe
-#  @date         04,2024
+# Copyright 2024 tcexeexe. All Rights Reserved.
 #
-#  @par     Copyright (c) 2024, SHTEC
-# 
-# *******************************************************************************************************/
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
 
 import argparse
 import dataclasses
 import importlib
 import json
 import os
 from pprint import pformat, pprint
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/bigbench/model.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/evaluate/bigbench/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,21 @@
-#******************************************************************************************************** 
-#  @author	     tcexeexe
-#  @date         04,2024
+# Copyright 2024 tcexeexe. All Rights Reserved.
 #
-#  @par     Copyright (c) 2024, SHTEC
-# 
-# *******************************************************************************************************/
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
 
 from __future__ import annotations
 
 import scipy
 from tqdm import tqdm
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/cost.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/evaluate/cost.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,34 @@
-#******************************************************************************************************** 
-#  @author	     tcexeexe
-#  @date         04,2024
+# Copyright 2024 tcexeexe. All Rights Reserved.
 #
-#  @par     Copyright (c) 2024, SHTEC
-# 
-# *******************************************************************************************************/
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
 
 import argparse
 import os
 
 import deepspeed
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
 import torch.distributed as dist
 from torch.utils.data import DataLoader
 from torch.utils.data.distributed import DistributedSampler
 from tqdm import tqdm
-from transformers.integrations.deepspeed import HfDeepSpeedConfig
+from transformers.deepspeed import HfDeepSpeedConfig
 from transformers.utils import is_torch_bf16_gpu_available, is_torch_tf32_available
 
 from shtec_rlhf.configs import get_deepspeed_eval_config
 from shtec_rlhf.datasets import SafetyPreferenceDataset, parse_dataset
 from shtec_rlhf.logger import set_logger_level
 from shtec_rlhf.models import AutoModelForScore, load_pretrained_models
 from shtec_rlhf.utils import (
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/gpt4/eval.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/evaluate/gpt4/eval.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-#******************************************************************************************************** 
-#  @author	     tcexeexe
-#  @date         04,2024
+# Copyright 2024 tcexeexe. All Rights Reserved.
 #
-#  @par     Copyright (c) 2024, SHTEC
-# 
-# *******************************************************************************************************/
-
-from __future__ import annotations
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
 
 import argparse
 import json
 import os
 import time
 
 import openai
-import torch
 from tqdm import tqdm
 
 from shtec_rlhf.configs.constants import PROMPT_INPUT
 from shtec_rlhf.models import load_pretrained_models
-from shtec_rlhf.utils import to_device
 
 
 PROBLEM_PATH = os.path.join(os.path.dirname(__file__), 'problem.json')
 SYSTEM_PROMPT = (
     """You are a helpful, harmless, and precise assistant for checking the quality of the answer."""
 )
 # pylint: disable=line-too-long
@@ -83,45 +86,39 @@
         auto_device_mapping=True,
         trust_remote_code=True,
     )
     answers = []
     print(f'Generating answers with {model_name_or_path}')
     for problem in tqdm(problems):
         prompt = PROMPT_INPUT.format(input=problem['prompt'])
-        input_ids = to_device(
-            tokenizer(prompt, return_tensors='pt'),
-            device=('cuda' if torch.cuda.is_available() else None),
-        )
+        input_ids = tokenizer(prompt, return_tensors='pt')
         output_ids = model.generate(
             **input_ids,
             max_length=2048,
         )
         answer = tokenizer.decode(output_ids[0], skip_special_tokens=True)[len(prompt) :]
         answers.append(answer)
     return answers
 
 
-def gpt4_eval(sys_prompt: str, user_prompt: str, client: openai.OpenAI | None = None) -> str:
-    if client is None:
-        client = openai.OpenAI()
-
+def gpt4_eval(sys_prompt: str, user_prompt: str) -> str:
     try:
-        chat_completion = client.chat.completions.create(
+        response = openai.ChatCompletion.create(
             model='gpt-4',
             messages=[
                 {'role': 'system', 'content': sys_prompt},
                 {
                     'role': 'user',
                     'content': user_prompt,
                 },
             ],
             temperature=0.7,
             max_tokens=2048,
         )
-        return chat_completion.choices[0].message.content
+        return response['choices'][0]['message']['content']
     except Exception as ex:  # pylint: disable=broad-except # noqa: BLE001
         print(ex)
         time.sleep(3)
     return 'error'
 
 
 def main() -> None:
@@ -131,31 +128,30 @@
     with open(PROBLEM_PATH, encoding='utf-8') as f:
         problems = json.load(f)
 
     red_answer = generate_answer(problems, args.red_corner_model_name_or_path)
     blue_answer = generate_answer(problems, args.blue_corner_model_name_or_path)
 
     print('Evaluating with GPT-4...')
-    client = openai.OpenAI()
 
     results = []
     for problem, answer1, answer2 in tqdm(
         zip(problems, red_answer, blue_answer),
         total=len(problems),
     ):
         user_prompt = USER_PROMPT.format(
             question=problem['prompt'],
             answer1=answer1,
             answer2=answer2,
         )
-        content = gpt4_eval(sys_prompt=SYSTEM_PROMPT, user_prompt=user_prompt, client=client)
+        content = gpt4_eval(sys_prompt=SYSTEM_PROMPT, user_prompt=user_prompt)
         try:
             score1, score2 = map(float, content.split('\n')[0].split(' '))
         except Exception:  # pylint: disable=broad-except # noqa: BLE001
-            score1, score2 = 0.0, 0.0
+            score1, score2 = 0, 0
 
         results.append(
             {
                 'prompt': problem['prompt'],
                 'red_answer': answer1,
                 'blue_answer': answer2,
                 'score1': score1,
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/gpt4/problem.json` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/evaluate/gpt4/problem.json`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/reward.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/evaluate/reward.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,34 @@
-#******************************************************************************************************** 
-#  @author	     tcexeexe
-#  @date         04,2024
+# Copyright 2024 tcexeexe. All Rights Reserved.
 #
-#  @par     Copyright (c) 2024, SHTEC
-# 
-# *******************************************************************************************************/
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
 
 import argparse
 import os
 
 import deepspeed
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
 import torch.distributed as dist
 from torch.utils.data import DataLoader
 from torch.utils.data.distributed import DistributedSampler
 from tqdm import tqdm
-from transformers.integrations.deepspeed import HfDeepSpeedConfig
+from transformers.deepspeed import HfDeepSpeedConfig
 from transformers.utils import is_torch_bf16_gpu_available, is_torch_tf32_available
 
 from shtec_rlhf.configs import get_deepspeed_eval_config
 from shtec_rlhf.datasets import PreferenceDataset, parse_dataset
 from shtec_rlhf.logger import set_logger_level
 from shtec_rlhf.models import AutoModelForScore, load_pretrained_models
 from shtec_rlhf.utils import (
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/finetune/deepspeed.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/finetune/deepspeed.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,21 @@
-#******************************************************************************************************** 
-#  @author	     tcexeexe
-#  @date         04,2024
+# Copyright 2024 tcexeexe. All Rights Reserved.
 #
-#  @par     Copyright (c) 2024, SHTEC
-# 
-# *******************************************************************************************************/
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
 """The main training script to supervised finetune a model using DeepSpeed."""
 
 import argparse
 
 import deepspeed
 import torch
 import torch.distributed as dist
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/logger.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,21 @@
-#******************************************************************************************************** 
-#  @author	     tcexeexe
-#  @date         04,2024
+# Copyright 2024 tcexeexe. All Rights Reserved.
 #
-#  @par     Copyright (c) 2024, SHTEC
-# 
-# *******************************************************************************************************/
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
 """The logger utility."""
 
 from __future__ import annotations
 
 import argparse
 import atexit
 import json
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/normalizer.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/models/normalizer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,21 @@
-#******************************************************************************************************** 
-#  @author	     tcexeexe
-#  @date         04,2024
+# Copyright 2024 tcexeexe. All Rights Reserved.
 #
-#  @par     Copyright (c) 2024, SHTEC
-# 
-# *******************************************************************************************************/
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
 """Normalizer for score models."""
 
 from __future__ import annotations
 
 from abc import abstractmethod
 from typing import Any, Literal
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/pretrained.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/models/pretrained.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,36 @@
-#******************************************************************************************************** 
-#  @author	     tcexeexe
-#  @date         04,2024
+# Copyright 2024 tcexeexe. All Rights Reserved.
 #
-#  @par     Copyright (c) 2024, SHTEC
-# 
-# *******************************************************************************************************/
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
 
 from __future__ import annotations
 
-import contextlib
 import os
 import warnings
 from typing import Any, Callable, Literal
 
-import deepspeed
 import torch
 import torch.nn as nn
 from transformers import (
     AutoModelForCausalLM,
     AutoTokenizer,
     PreTrainedModel,
     PreTrainedTokenizerBase,
 )
-from transformers.integrations.deepspeed import is_deepspeed_zero3_enabled
 
 from shtec_rlhf.configs import (
     DEFAULT_BOS_TOKEN,
     DEFAULT_EOS_TOKEN,
     DEFAULT_PAD_TOKEN,
     DEFAULT_UNK_TOKEN,
 )
@@ -54,36 +58,21 @@
         ):
             warnings.warn(
                 format_message(len(tokenizer), input_embeddings.num_embeddings),
                 category=RuntimeWarning,
                 stacklevel=3,
             )
 
-    def init_new_embeddings(
-        embeddings: nn.Embedding | nn.Linear | None,
-        new_num_embeddings: int,
-        num_new_embeddings: int,
-    ) -> None:
+    def init_new_embeddings(embeddings: nn.Embedding | None) -> None:
         if embeddings is None:
             return
 
-        params = [embeddings.weight, getattr(embeddings, 'bias', None)]
-        context = (
-            deepspeed.zero.GatheredParameters(params, modifier_rank=0)
-            if is_deepspeed_zero3_enabled()
-            else contextlib.nullcontext()
-        )
-        with context:
-            for param in params:
-                if param is None:
-                    continue
-                assert param.size(0) == new_num_embeddings
-                param_data = param.data
-                param_mean = param_data[:-num_new_embeddings].mean(dim=0, keepdim=True)
-                param_data[-num_new_embeddings:] = param_mean
+        embeddings_data = embeddings.weight.data
+        embeddings_mean = embeddings_data[:-num_new_tokens].mean(dim=0, keepdim=True)
+        embeddings_data[-num_new_tokens:] = embeddings_mean
 
     verify_vocabulary_embedding_sizes(
         tokenizer=tokenizer,
         model=model,
         format_message=(
             'The tokenizer vocabulary size ({}) is different from '
             'the model embedding size ({}) before resizing.'
@@ -97,15 +86,14 @@
         special_tokens_dict['eos_token'] = DEFAULT_EOS_TOKEN
     if tokenizer.bos_token is None:
         special_tokens_dict['bos_token'] = DEFAULT_BOS_TOKEN
     if tokenizer.unk_token is None:
         special_tokens_dict['unk_token'] = DEFAULT_UNK_TOKEN
 
     num_new_tokens = tokenizer.add_special_tokens(special_tokens_dict)
-    new_num_embeddings = len(tokenizer)
 
     model.config.bos_token_id = tokenizer.bos_token_id
     model.config.eos_token_id = tokenizer.eos_token_id
     model.config.pad_token_id = tokenizer.pad_token_id
 
     if num_new_tokens > 0:
         hf_device_map = getattr(model, 'hf_device_map', {})
@@ -113,25 +101,17 @@
             torch.device(device)
             for device in hf_device_map.values()
             if device not in {'cpu', 'disk'}
         }
         is_model_parallel = len(devices) > 1
 
         if not is_model_parallel:
-            model.resize_token_embeddings(new_num_embeddings)
-            init_new_embeddings(
-                model.get_input_embeddings(),
-                new_num_embeddings=new_num_embeddings,
-                num_new_embeddings=num_new_tokens,
-            )
-            init_new_embeddings(
-                model.get_output_embeddings(),
-                new_num_embeddings=new_num_embeddings,
-                num_new_embeddings=num_new_tokens,
-            )
+            model.resize_token_embeddings(len(tokenizer))
+            init_new_embeddings(model.get_input_embeddings())
+            init_new_embeddings(model.get_output_embeddings())
 
     verify_vocabulary_embedding_sizes(
         tokenizer=tokenizer,
         model=model,
         format_message=(
             'The tokenizer vocabulary size ({}) is different from '
             'the model embedding size ({}) after resizing.'
@@ -191,11 +171,12 @@
     tokenizer = AutoTokenizer.from_pretrained(
         model_name_or_path,
         *auto_tokenizer_args,
         cache_dir=cache_dir,
         model_max_length=model_max_length,
         padding_side=padding_side,
         trust_remote_code=trust_remote_code,
+        use_fast=(model.config.model_type != 'llama'),
         **auto_tokenizer_kwargs,
     )
     resize_tokenizer_embedding(tokenizer=tokenizer, model=model)
     return model, tokenizer
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/bloom/modeling_bloom.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/models/score_model/llama/modeling_llama.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,109 +1,123 @@
-#******************************************************************************************************** 
-#  @author	     tcexeexe
-#  @date         04,2024
+# Copyright 2024 tcexeexe. All Rights Reserved.
 #
-#  @par     Copyright (c) 2024, SHTEC
-# 
-# *******************************************************************************************************/
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
 
 from __future__ import annotations
 
-import warnings
-from typing import Any
+from typing import Any, ClassVar
 
 import torch
-from transformers import BloomModel, BloomPreTrainedModel, PretrainedConfig, PreTrainedModel
-from transformers.models.bloom.modeling_bloom import _CONFIG_FOR_DOC, BLOOM_INPUTS_DOCSTRING
+import torch.nn as nn
+from transformers import LlamaModel, LlamaPreTrainedModel, PreTrainedModel
+from transformers.configuration_utils import PretrainedConfig
+from transformers.models.llama.modeling_llama import _CONFIG_FOR_DOC, LLAMA_INPUTS_DOCSTRING
 from transformers.utils.doc import add_start_docstrings_to_model_forward, replace_return_docstrings
 
 from shtec_rlhf.models.score_model import ScoreModelMixin, ScoreModelOutput
 
 
-class BloomForScore(ScoreModelMixin, BloomPreTrainedModel):
+class LlamaModelForScore(ScoreModelMixin, LlamaPreTrainedModel):
+    _keys_to_ignore_on_load_missing: ClassVar[list[str]] = ['lm_head.weight']
+
     def __init__(self, config: PretrainedConfig, **kwargs: Any) -> None:
         super().__init__(config)
-        self.transformer = BloomModel(config)
+        self.model = LlamaModel(config)
 
         config.architectures = [self.__class__.__name__]
         self.init_score_head(config, hidden_size=config.hidden_size, **kwargs)
 
         # Initialize weights and apply final processing
         self.post_init()
 
+    def get_input_embeddings(self) -> nn.Embedding:
+        return self.model.embed_tokens
+
+    def set_input_embeddings(self, value: nn.Embedding) -> None:
+        self.model.embed_tokens = value
+
     def get_output_embeddings(self) -> None:
         return None
 
     def set_decoder(self, decoder: PreTrainedModel) -> None:
-        self.transformer = decoder
+        self.model = decoder
 
     def get_decoder(self) -> PreTrainedModel:
-        return self.transformer
+        return self.model
 
-    @add_start_docstrings_to_model_forward(BLOOM_INPUTS_DOCSTRING)
+    @add_start_docstrings_to_model_forward(LLAMA_INPUTS_DOCSTRING)
     @replace_return_docstrings(output_type=ScoreModelOutput, config_class=_CONFIG_FOR_DOC)
     def forward(  # pylint: disable=too-many-arguments
         self,
-        input_ids: torch.LongTensor | None = None,
-        past_key_values: tuple[tuple[torch.Tensor, torch.Tensor], ...] | None = None,
-        attention_mask: torch.Tensor | None = None,
-        head_mask: torch.Tensor | None = None,
-        inputs_embeds: torch.Tensor | None = None,
+        input_ids: torch.LongTensor,
+        attention_mask: torch.Tensor,
+        position_ids: torch.LongTensor | None = None,
+        past_key_values: list[torch.FloatTensor] | None = None,
+        inputs_embeds: torch.FloatTensor | None = None,
         use_cache: bool | None = None,
+        output_attentions: bool | None = None,
+        output_hidden_states: bool | None = None,
         return_dict: bool | None = None,
-        **deprecated_arguments: Any,
     ) -> tuple[torch.Tensor, torch.Tensor] | ScoreModelOutput:
         """
         Args:
 
         Returns:
 
         Examples:
 
         ```python
-        >>> from shtec_rlhf.models.score_model.llama.modeling_llama import LlamaForScore
+        >>> from shtec_rlhf.models.llama.modeling_llama import LlamaModelForScore
         >>> from transformers import LlamaTokenizer
 
-        >>> model = LlamaForScore.from_pretrained(PATH_TO_CONVERTED_WEIGHTS)
+        >>> model = LlamaForCausalLM.from_pretrained(PATH_TO_CONVERTED_WEIGHTS)
         >>> tokenizer = AutoTokenizer.from_pretrained(PATH_TO_CONVERTED_TOKENIZER)
 
         >>> prompt = "Hey, are you conscious? Can you talk to me?"
         >>> inputs = tokenizer(prompt, return_tensors="pt")
 
-        # get score
+        # got score
         >>> outputs = model(**inputs)
-        >>> end_scores = outputs.end_scores
-        >>> end_scores
-        tensor([[0.0000]])
+        >>> scores = outputs.scores
+        >>> scores
+        tensor([[[0.0000]]])
         ```
         """
-        if deprecated_arguments.pop('position_ids', False) is not False:
-            # `position_ids` could have been `torch.Tensor` or `None`
-            # so defaulting pop to `False` allows to detect if users were passing explicitly `None`
-            warnings.warn(
-                '`position_ids` have no functionality in BLOOM and will be removed in v5.0.0. '
-                'You can safely ignore passing `position_ids`.',
-                FutureWarning,
-                stacklevel=1,
-            )
-        if len(deprecated_arguments) > 0:
-            raise ValueError(f'Got unexpected arguments: {deprecated_arguments}')
-
+        assert attention_mask is not None
+        output_attentions = (
+            output_attentions if output_attentions is not None else self.config.output_attentions
+        )
+        output_hidden_states = (
+            output_hidden_states
+            if output_hidden_states is not None
+            else self.config.output_hidden_states
+        )
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
 
-        outputs = self.transformer(
-            input_ids,
-            past_key_values=past_key_values,
+        outputs = self.model(
+            input_ids=input_ids,
             attention_mask=attention_mask,
-            head_mask=head_mask,
+            position_ids=position_ids,
+            past_key_values=past_key_values,
             inputs_embeds=inputs_embeds,
             use_cache=use_cache,
-            output_attentions=False,
-            output_hidden_states=False,
-            return_dict=True,
+            output_attentions=output_attentions,
+            output_hidden_states=output_hidden_states,
+            return_dict=return_dict,
         )
-        last_hidden_state = outputs.last_hidden_state  # size = (B, L, E)
-        return self.get_scores(
-            last_hidden_state,
+        hidden_states = outputs[0]  # size = (B, L, E)
+        return self.get_score(
+            hidden_states,
             attention_mask=attention_mask,
             return_dict=return_dict,
         )
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/serve/chatbot.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/serve/chatbot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2024 tcexeexe. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
 """Interactive chatbot."""
 
 from __future__ import annotations
 
 import abc
 import dataclasses
 import os
@@ -308,18 +322,20 @@
     def __len__(self) -> int:
         return len(self.chatbots)
 
     def __iter__(self) -> Iterator[Chatbot]:
         return iter(self.chatbots)
 
     @overload
-    def __getitem__(self, index: int) -> Chatbot: ...
+    def __getitem__(self, index: int) -> Chatbot:
+        ...
 
     @overload
-    def __getitem__(self, index: slice) -> ChatbotList: ...
+    def __getitem__(self, index: slice) -> ChatbotList:
+        ...
 
     def __getitem__(self, index: int | slice) -> Chatbot | ChatbotList:
         if isinstance(index, slice):
             return ChatbotList(self.chatbots[index])
         return self.chatbots[index]
 
     @property
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/serve/cli.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/serve/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2024 tcexeexe. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
 """Command line interface for interacting with a model."""
 
 from __future__ import annotations
 
 import argparse
 import itertools
 from typing import Generator, Iterable
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/trainers/base.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/trainers/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2024 tcexeexe. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
 """Trainer base class."""
 
 from __future__ import annotations
 
 import abc
 import argparse
 import os
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/trainers/rl_trainer.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/trainers/rl_trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2024 tcexeexe. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
 """Trainer base class for RL training."""
 
 from __future__ import annotations
 
 import abc
 import argparse
 import copy
@@ -20,26 +34,25 @@
 from transformers import (
     AutoModelForCausalLM,
     GenerationConfig,
     PreTrainedModel,
     PreTrainedTokenizerBase,
     get_scheduler,
 )
-from transformers.integrations.deepspeed import HfDeepSpeedConfig
+from transformers.deepspeed import HfDeepSpeedConfig
 
 from shtec_rlhf.configs import ADAM_BETAS
 from shtec_rlhf.datasets import DummyDataset, PromptOnlyBatch, PromptOnlyDataset, SupervisedDataset
 from shtec_rlhf.models import AutoModelForScore, load_pretrained_models
 from shtec_rlhf.trainers.base import TrainerBase
 from shtec_rlhf.utils import (
     get_all_reduce_mean,
     get_optimizer_grouped_parameters,
     is_main_process,
     is_same_tokenizer,
-    masked_mean,
     to_device,
 )
 
 
 class RLTrainer(TrainerBase):  # pylint: disable=too-many-instance-attributes
     """Trainer base class for RL training.
 
@@ -634,29 +647,28 @@
             advantages_reversed.append(last_gae_lambda)
         advantages = torch.stack(advantages_reversed[::-1], dim=1)
         returns = advantages + values[:, start:]
         return advantages.detach(), returns
 
     def critic_loss_fn(
         self,
-        values: torch.Tensor,  # size = (B, L - S)
-        old_values: torch.Tensor,  # size = (B, L - S)
-        returns: torch.Tensor,  # size = (B, L - S)
-        mask: torch.BoolTensor,  # size = (B, L - S)
-    ) -> torch.Tensor:  # size = ()
+        values: torch.Tensor,
+        old_values: torch.Tensor,
+        returns: torch.Tensor,
+        mask: torch.BoolTensor,
+    ) -> torch.Tensor:
         """Compute critic loss."""
-        # size = (B, L - S)
         values_clipped = torch.clamp(
             values,
             old_values - self.clip_range_value,
             old_values + self.clip_range_value,
         )
         vf_loss1 = torch.square(values - returns)
         vf_loss2 = torch.square(values_clipped - returns)
-        return 0.5 * masked_mean(torch.maximum(vf_loss1, vf_loss2), mask)  # size = ()
+        return 0.5 * torch.sum(torch.maximum(vf_loss1, vf_loss2) * mask) / mask.sum()
 
     def save(
         self,
         model: deepspeed.DeepSpeedEngine | PreTrainedModel | None = None,
         ds_config: dict | None = None,
     ) -> None:
         """Save model and tokenizer."""
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/trainers/supervised_trainer.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/trainers/supervised_trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2024 tcexeexe. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
 """Trainer base class for supervised training."""
 
 from __future__ import annotations
 
 import abc
 import argparse
 from typing import Any, ClassVar
@@ -10,15 +24,15 @@
 import torch
 import torch.distributed as dist
 from deepspeed.ops.adam import DeepSpeedCPUAdam, FusedAdam
 from torch.utils.data import DataLoader
 from torch.utils.data.distributed import DistributedSampler
 from tqdm import tqdm
 from transformers import AutoModelForCausalLM, get_scheduler
-from transformers.integrations.deepspeed import HfDeepSpeedConfig
+from transformers.deepspeed import HfDeepSpeedConfig
 
 from shtec_rlhf.configs import ADAM_BETAS
 from shtec_rlhf.datasets import TokenizedDataset
 from shtec_rlhf.models import load_pretrained_models
 from shtec_rlhf.trainers.base import TrainerBase
 from shtec_rlhf.utils import get_optimizer_grouped_parameters, is_main_process, to_device
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/utils.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,21 @@
-#******************************************************************************************************** 
-#  @author	     tcexeexe
-#  @date         04,2024
+# Copyright 2024 tcexeexe. All Rights Reserved.
 #
-#  @par     Copyright (c) 2024, SHTEC
-# 
-# *******************************************************************************************************/
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
 """Miscellaneous utilities."""
 
 from __future__ import annotations
 
 import dataclasses
 import os
 import random
@@ -34,19 +41,18 @@
 __all__ = [
     'seed_everything',
     'str2bool',
     'to_device',
     'batch_retokenize',
     'is_same_tokenizer',
     'is_main_process',
-    'masked_mean',
-    'gather_log_probabilities',
     'get_all_reduce_mean',
     'get_all_reduce_sum',
     'get_optimizer_grouped_parameters',
+    'gather_log_probabilities',
 ]
 
 
 TensorTree: TypeAlias = PyTreeTypeVar('TensorTree', torch.Tensor)
 Func = TypeVar('Func', bound=Callable[..., Any])
 
 
@@ -187,38 +193,14 @@
         if is_main_process():
             return func(*args, **kwargs)
         return None
 
     return cast(Func, wrapper)
 
 
-def masked_mean(
-    x: torch.Tensor,  # size = (B, L)
-    mask: torch.BoolTensor | None = None,  # size = (B, L)
-) -> torch.Tensor:  # size = ()
-    """Compute the mean of a tensor with a mask."""
-    if mask is None:
-        return x.mean()
-    return ((x * mask).sum(dim=-1) / mask.sum(dim=-1)).mean()
-
-
-def gather_log_probabilities(
-    logits: torch.Tensor,  # size = (B, L, V)
-    labels: torch.LongTensor,  # size = (B, L)
-) -> torch.Tensor:  # size = (B, L)
-    """Gather log probabilities of the given labels from the logits."""
-    log_probs = F.log_softmax(logits, dim=-1)  # size = (B, L, V)
-    gathered_log_probs = torch.gather(  # size = (B, L, 1)
-        log_probs,
-        dim=-1,
-        index=labels.unsqueeze(dim=-1),
-    )
-    return gathered_log_probs.squeeze(dim=-1)  # size = (B, L)
-
-
 def get_all_reduce_mean(tensor: torch.Tensor) -> torch.Tensor:
     """Perform all-reduce operation on a tensor cross all ranks and return the mean."""
     if dist.is_initialized():
         dist.all_reduce(tensor, op=dist.ReduceOp.AVG)
     return tensor
 
 
@@ -266,14 +248,21 @@
                 if any(no_decay_name in name for no_decay_name in no_decay_name_set)
             ],
             'weight_decay': 0.0,
         },
     ]
 
 
+def gather_log_probabilities(logits: torch.Tensor, labels: torch.LongTensor) -> torch.Tensor:
+    """Gather log probabilities of the given labels from the logits."""
+    log_probs = F.log_softmax(logits, dim=-1)
+    log_probs_labels = log_probs.gather(dim=-1, index=labels.unsqueeze(dim=-1))
+    return log_probs_labels.squeeze(dim=-1)
+
+
 def split_prompt_response(
     texts: list[str],
     split_token: str = PROMPT_ASSISTANT,
 ) -> tuple[list[str], list[str]]:
     """Split prompt-response pairs into prompts and responses."""
 
     def split_fn(text: str) -> tuple[str, str]:
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/cost/trainer.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/values/cost/trainer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2024 tcexeexe. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
 """Cost model Trainer."""
 
 from __future__ import annotations
 
 from typing import Any
 
 import torch
@@ -22,15 +36,14 @@
     DATASET_TYPE = SafetyPreferenceDataset
     MODEL_TYPE = AutoModelForScore
 
     @property
     def extra_model_kwargs(self) -> dict[str, Any]:
         """Extra keyword arguments for initializing the model."""
         return {
-            'score_dim': 1,
             'score_type': 'cost',
             'do_normalize': self.args.normalize_score_during_training,
             'normalizer_type': self.args.normalizer_type,
             'momentum': self.args.normalizer_momentum,
         }
 
     @torch.no_grad()
@@ -71,19 +84,17 @@
             ).end_scores.squeeze(dim=-1)
 
             num_correct_predictions += (higher_end_costs > lower_end_costs).sum()
 
             # HINT: safe samples are supposed to have negative costs
             #       unsafe samples are supposed to have positive costs
             #       safety sign: +1 for safe / -1 for unsafe
+            num_correct_sign_predictions += (lower_end_costs * batch['safer_safety_sign'] < 0).sum()
             num_correct_sign_predictions += (
-                lower_end_costs * batch['safer_safety_sign'] < 0.0
-            ).sum()
-            num_correct_sign_predictions += (
-                higher_end_costs * batch['unsafer_safety_sign'] < 0.0
+                higher_end_costs * batch['unsafer_safety_sign'] < 0
             ).sum()
             num_total_predictions += batch_size
 
             costs.extend([lower_end_costs, higher_end_costs])
 
         if batch is None:
             self.logger.print('WARNING: `eval_dataloader` is empty.')
@@ -106,16 +117,16 @@
 
         self.set_train()
 
         # Evaluation info
         info = {
             'eval/accuracy': accuracy.item(),
             'eval/accuracy_sign': accuracy_sign.item(),
-            'eval/cost_mean': costs.mean().item(),
-            'eval/cost_std': costs.std().item(),
+            'eval/costs_mean': costs.mean().item(),
+            'eval/costs_std': costs.std().item(),
         }
 
         if is_main_process():
             # Print some examples from the last batch
             max_num_rows = 3
             lower_cost_texts = self.tokenizer.batch_decode(
                 batch['safer_input_ids'][:max_num_rows],
@@ -180,15 +191,15 @@
             safer_attention_mask (torch.BoolTensor): The attention mask of the safer examples.
             safer_safety_sign (torch.LongTensor): The safety sign of the safer examples.
             unsafer_input_ids (torch.LongTensor): The input ids of the unsafer examples.
             unsafer_attention_mask (torch.BoolTensor): The attention mask of the unsafer examples.
             unsafer_safety_sign (torch.LongTensor): The safety sign of the unsafer examples.
 
         Returns:
-            dict[str, torch.Tensor]: loss, higher_end_cost, lower_end_cost, accuracy
+            dict[str, torch.Tensor]: loss, higher_end_costs, lower_end_costs, accuracy
         """
         assert safer_input_ids.size(0) == unsafer_input_ids.size(0), 'batch size mismatch!'
         batch_size = safer_input_ids.size(0)
 
         output: ScoreModelOutput = self.model(
             torch.cat([safer_input_ids, unsafer_input_ids], dim=0),
             attention_mask=torch.cat([safer_attention_mask, unsafer_attention_mask], dim=0),
@@ -197,91 +208,71 @@
         end_scores = output.end_scores  # size = (2 * B, 1)
 
         # Hints: safer examples are supposed to have lower costs
         #        unsafer examples are supposed to have higher costs
         # size = (B, L)
         lower_costs, higher_costs = scores.squeeze(dim=-1).chunk(chunks=2, dim=0)
         # size = (B,)
-        lower_end_cost, higher_end_cost = end_scores.squeeze(dim=-1).chunk(chunks=2, dim=0)
+        lower_end_costs, higher_end_costs = end_scores.squeeze(dim=-1).chunk(chunks=2, dim=0)
         # safety_sign: +1 for safe / -1 for unsafe
         # cost_sign: -1 for safe / +1 for unsafe
         lower_cost_sign = -safer_safety_sign  # size = (B,)
         higher_cost_sign = -unsafer_safety_sign  # size = (B,)
 
         if self.args.loss_type == 'token-wise':
             losses = []
             for i in range(batch_size):
                 assert not torch.all(
                     torch.eq(safer_input_ids[i], unsafer_input_ids[i]),
                 ).item(), 'The safer and unsafer answers are the same!'
-                lower_end_index = safer_attention_mask[i].nonzero()[-1].squeeze().item()
-                higher_end_index = unsafer_attention_mask[i].nonzero()[-1].squeeze().item()
+                lower_end_index = safer_attention_mask[i].nonzero()[-1]
+                higher_end_index = unsafer_attention_mask[i].nonzero()[-1]
                 end_index = max(higher_end_index, lower_end_index)
 
-                diverge_index = (
-                    (safer_input_ids[i] != unsafer_input_ids[i]).nonzero()[0].squeeze().item()
-                )
+                diverge_index = (safer_input_ids[i] != unsafer_input_ids[i]).nonzero()[0]
                 assert 0 <= diverge_index <= end_index, 'diverge index is out of range!'
 
                 # size = (B, L)
                 lower_truncated_costs = lower_costs[i, diverge_index : end_index + 1]
                 higher_truncated_costs = higher_costs[i, diverge_index : end_index + 1]
 
                 # safety_sign: +1 for safe / -1 for unsafe
                 losses.append(
                     -F.logsigmoid(higher_truncated_costs - lower_truncated_costs).mean()
                     - F.logsigmoid(lower_cost_sign[i] * lower_truncated_costs).mean()
                     - F.logsigmoid(higher_cost_sign[i] * higher_truncated_costs).mean(),
                 )
 
                 if self.args.regularization > 0.0:
-                    losses[-1] = (
-                        losses[-1]
-                        + self.args.regularization
-                        * torch.stack([lower_truncated_costs, higher_truncated_costs])
-                        .square()
-                        .mean()
+                    losses[-1] = losses[-1] + self.args.regularization * (
+                        torch.square(lower_truncated_costs).mean()
+                        + torch.square(higher_truncated_costs).mean()
                     )
 
             loss = torch.stack(losses).mean()  # size = ()
         elif self.args.loss_type == 'sequence-wise':
             loss = (
-                -F.logsigmoid(higher_end_cost - lower_end_cost)
-                - F.logsigmoid(lower_cost_sign * lower_end_cost)
-                - F.logsigmoid(higher_cost_sign * higher_end_cost)
+                -F.logsigmoid(higher_end_costs - lower_end_costs)
+                - F.logsigmoid(lower_cost_sign * lower_end_costs)
+                - F.logsigmoid(higher_cost_sign * higher_end_costs)
             ).mean()
 
             if self.args.regularization > 0.0:
-                loss = (
-                    loss
-                    + self.args.regularization
-                    * torch.stack([lower_end_cost, higher_end_cost]).square().mean()
+                loss = loss + self.args.regularization * (
+                    torch.square(lower_end_costs).mean() + torch.square(higher_end_costs).mean()
                 )
         else:
             raise ValueError(f'Unknown loss type: {self.args.loss_type}')
 
-        accuracy = (higher_end_cost > lower_end_cost).float().mean()  # size = ()
-        accuracy_sign = (  # size = ()
-            torch.stack(
-                [
-                    lower_cost_sign * lower_end_cost > 0.0,
-                    higher_cost_sign * higher_end_cost > 0.0,
-                ],
-            )
-            .float()
-            .mean()
-        )
+        accuracy = (higher_end_costs > lower_end_costs).float().mean()  # size = ()
         return {
             'loss': loss,  # size = ()
-            'higher_end_cost': higher_end_cost,  # size = (B,)
-            'lower_end_cost': lower_end_cost,  # size = (B,)
-            'higher_costs': higher_costs,  # size = (B, L)
-            'lower_costs': lower_costs,  # size = (B, L)
+            'higher_end_costs': higher_end_costs,  # size = (B,)
+            'lower_end_costs': lower_end_costs,  # size = (B,)
             'accuracy': accuracy,  # size = ()
-            'accuracy_sign': accuracy_sign,  # size = ()
         }
 
     def train_step(
         self,
         safer_input_ids: torch.LongTensor,  # size = (B, L)
         safer_attention_mask: torch.BoolTensor,  # size = (B, L)
         safer_safety_sign: torch.LongTensor,  # size = (B,) # +1 for safe / -1 for unsafe
@@ -311,19 +302,16 @@
             unsafer_safety_sign=unsafer_safety_sign,
         )
         loss = loss_dict['loss']
         self.model.backward(loss)
         self.model.step()
 
         accuracy = loss_dict['accuracy']
-        accuracy_sign = loss_dict['accuracy_sign']
 
         loss = get_all_reduce_mean(loss)
         accuracy = get_all_reduce_mean(accuracy)
-        accuracy_sign = get_all_reduce_mean(accuracy_sign)
 
         return {
             'train/loss': loss.item(),
             'train/accuracy': accuracy.item(),
-            'train/accuracy_sign': accuracy_sign.item(),
             'train/lr': self.model.optimizer.param_groups[0]['lr'],
         }
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/reward/trainer.py` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf/values/reward/trainer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,21 @@
-#******************************************************************************************************** 
-#  @author	     tcexeexe
-#  @date         04,2024
+# Copyright 2024 tcexeexe. All Rights Reserved.
 #
-#  @par     Copyright (c) 2024, SHTEC
-# 
-# *******************************************************************************************************/
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
 """Reward model Trainer."""
 
 from __future__ import annotations
 
 from typing import Any
 
 import torch
@@ -29,15 +36,14 @@
     DATASET_TYPE = PreferenceDataset
     MODEL_TYPE = AutoModelForScore
 
     @property
     def extra_model_kwargs(self) -> dict[str, Any]:
         """Extra keyword arguments for initializing the model."""
         return {
-            'score_dim': 1,
             'score_type': 'reward',
             'do_normalize': self.args.normalize_score_during_training,
             'normalizer_type': self.args.normalizer_type,
             'momentum': self.args.normalizer_momentum,
         }
 
     @torch.no_grad()
@@ -95,16 +101,16 @@
             rewards = torch.cat(gathered_rewards, dim=0)
 
         self.set_train()
 
         # Evaluation info
         info = {
             'eval/accuracy': accuracy.item(),
-            'eval/reward_mean': rewards.mean().item(),
-            'eval/reward_std': rewards.std().item(),
+            'eval/rewards_mean': rewards.mean().item(),
+            'eval/rewards_std': rewards.std().item(),
         }
 
         if is_main_process():
             # Print some examples from the last batch
             max_num_rows = 3
             higher_reward_texts = self.tokenizer.batch_decode(
                 batch['better_input_ids'][:max_num_rows],
@@ -159,82 +165,73 @@
         Args:
             better_input_ids (torch.LongTensor): The input ids of the better answer.
             better_attention_mask (torch.BoolTensor): The attention mask of the better answer.
             worse_input_ids (torch.LongTensor): The input ids of the worse answer.
             worse_attention_mask (torch.BoolTensor): The attention mask of the worse answer.
 
         Returns:
-            dict[str, torch.Tensor]: loss, higher_end_reward, lower_end_reward, accuracy
+            dict[str, torch.Tensor]: loss, higher_end_rewards, lower_end_rewards, accuracy
         """
         assert better_input_ids.size(0) == worse_input_ids.size(0), 'batch size mismatch!'
         batch_size = better_input_ids.size(0)
 
         output: ScoreModelOutput = self.model(
             torch.cat([better_input_ids, worse_input_ids], dim=0),
             attention_mask=torch.cat([better_attention_mask, worse_attention_mask], dim=0),
         )
         scores = output.scores  # size = (2 * B, L, 1)
         end_scores = output.end_scores  # size = (2 * B, 1)
         # size = (B, L)
         higher_rewards, lower_rewards = scores.squeeze(dim=-1).chunk(chunks=2, dim=0)
         # size = (B,)
-        higher_end_reward, lower_end_reward = end_scores.squeeze(dim=-1).chunk(chunks=2, dim=0)
+        higher_end_rewards, lower_end_rewards = end_scores.squeeze(dim=-1).chunk(chunks=2, dim=0)
 
         if self.args.loss_type == 'token-wise':
             losses = []
             for i in range(batch_size):
                 assert not torch.all(
                     torch.eq(better_input_ids[i], worse_input_ids[i]),
                 ).item(), 'The better and worse answers are the same!'
-                higher_end_index = better_attention_mask[i].nonzero()[-1].squeeze().item()
-                lower_end_index = worse_attention_mask[i].nonzero()[-1].squeeze().item()
+                higher_end_index = better_attention_mask[i].nonzero()[-1]
+                lower_end_index = worse_attention_mask[i].nonzero()[-1]
                 end_index = max(higher_end_index, lower_end_index)
 
-                diverge_index = (
-                    (better_input_ids[i] != worse_input_ids[i]).nonzero()[0].squeeze().item()
-                )
+                diverge_index = (better_input_ids[i] != worse_input_ids[i]).nonzero()[0]
                 assert 0 <= diverge_index <= end_index, 'diverge index is out of range!'
 
                 # size = (L,)
                 higher_truncated_rewards = higher_rewards[i, diverge_index : end_index + 1]
                 lower_truncated_rewards = lower_rewards[i, diverge_index : end_index + 1]
 
                 losses.append(
                     -F.logsigmoid(higher_truncated_rewards - lower_truncated_rewards).mean(),
                 )
 
                 if self.args.regularization > 0.0:
-                    losses[-1] = (
-                        losses[-1]
-                        + self.args.regularization
-                        * torch.stack([lower_truncated_rewards, higher_truncated_rewards])
-                        .square()
-                        .mean()
+                    losses[-1] = losses[-1] + self.args.regularization * (
+                        torch.square(lower_truncated_rewards).mean()
+                        + torch.square(higher_truncated_rewards).mean()
                     )
 
             loss = torch.stack(losses).mean()  # size = ()
         elif self.args.loss_type == 'sequence-wise':
-            loss = -F.logsigmoid(higher_end_reward - lower_end_reward).mean()
+            loss = -F.logsigmoid(higher_end_rewards - lower_end_rewards).mean()
 
             if self.args.regularization > 0.0:
-                loss = (
-                    loss
-                    + self.args.regularization
-                    * torch.stack([lower_end_reward, higher_end_reward]).square().mean()
+                loss = loss + self.args.regularization * (
+                    torch.square(lower_end_rewards).mean() + torch.square(higher_end_rewards).mean()
                 )
         else:
             raise ValueError(f'Unknown loss type: {self.args.loss_type}')
 
-        accuracy = (higher_end_reward > lower_end_reward).float().mean()  # size = ()
+        accuracy = (higher_end_rewards > lower_end_rewards).float().mean()  # size = ()
         return {
             'loss': loss,  # size = ()
-            'higher_end_reward': higher_end_reward,  # size = (B,)
-            'lower_end_reward': lower_end_reward,  # size = (B,)
-            'higher_rewards': higher_rewards,  # size = (B, L)
-            'lower_rewards': lower_rewards,  # size = (B, L)
+            'higher_end_rewards': higher_end_rewards,  # size = (B,)
+            'lower_end_rewards': lower_end_rewards,  # size = (B,)
             'accuracy': accuracy,  # size = ()
         }
 
     def train_step(
         self,
         better_input_ids: torch.LongTensor,  # size = (B, L)
         better_attention_mask: torch.BoolTensor,  # size = (B, L)
```

### Comparing `shtec-rlhf-0.0.2.dev0/shtec_rlhf.egg-info/PKG-INFO` & `shtec-rlhf-0.0.3.dev0/shtec_rlhf.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: shtec-rlhf
-Version: 0.0.2.dev0
+Version: 0.0.3.dev0
 Summary: shtec-rlhf: Safe Reinforcement Learning from Human Feedback
-Author: PKU-Alignment Team
+Author: tcexeexe
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://github.com/PKU-Alignment/shtec-rlhf
 Project-URL: Repository, https://github.com/PKU-Alignment/shtec-rlhf
 Project-URL: Documentation, https://shtec-rlhf.readthedocs.io
 Project-URL: Bug Report, https://github.com/PKU-Alignment/shtec-rlhf
 Keywords: Reinforcement Learning,Safe Reinforcement Learning,Reinforcement Learning from Human Feedback,Safe Reinforcement Learning from Human Feedback,Large Language Model,Language Model,RLHF,Safe RLHF,LLM
 Classifier: Development Status :: 4 - Beta
@@ -18,7 +18,8 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: lint
+License-File: LICENSE
```

