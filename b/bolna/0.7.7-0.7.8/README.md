# Comparing `tmp/bolna-0.7.7.tar.gz` & `tmp/bolna-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bolna-0.7.7.tar", last modified: Tue May  7 18:45:57 2024, max compression
+gzip compressed data, was "bolna-0.7.8.tar", last modified: Mon May 20 14:36:33 2024, max compression
```

## Comparing `bolna-0.7.7.tar` & `bolna-0.7.8.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.910877 bolna-0.7.7/
--rw-r--r--   0 xan        (501) staff       (20)    34522 2024-03-11 19:09:56.000000 bolna-0.7.7/LICENSE
--rw-r--r--   0 xan        (501) staff       (20)    48383 2024-05-07 18:45:57.910668 bolna-0.7.7/PKG-INFO
--rw-r--r--   0 xan        (501) staff       (20)     7456 2024-04-24 13:49:22.000000 bolna-0.7.7/README.md
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.898979 bolna-0.7.7/bolna/
--rw-r--r--   0 xan        (501) staff       (20)      330 2024-05-07 18:45:43.000000 bolna-0.7.7/bolna/__init__.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.900712 bolna-0.7.7/bolna/agent_manager/
--rw-r--r--   0 xan        (501) staff       (20)      124 2024-01-07 06:26:49.000000 bolna-0.7.7/bolna/agent_manager/__init__.py
--rw-r--r--   0 xan        (501) staff       (20)     3040 2024-05-07 18:42:57.000000 bolna-0.7.7/bolna/agent_manager/assistant_manager.py
--rw-r--r--   0 xan        (501) staff       (20)      174 2024-01-07 16:40:54.000000 bolna-0.7.7/bolna/agent_manager/base_manager.py
--rw-r--r--   0 xan        (501) staff       (20)    82616 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/agent_manager/task_manager.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.902626 bolna-0.7.7/bolna/agent_types/
--rw-r--r--   0 xan        (501) staff       (20)      300 2024-03-22 13:50:32.000000 bolna-0.7.7/bolna/agent_types/__init__.py
--rw-r--r--   0 xan        (501) staff       (20)      176 2024-01-07 16:40:54.000000 bolna-0.7.7/bolna/agent_types/base_agent.py
--rw-r--r--   0 xan        (501) staff       (20)     1353 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/agent_types/contextual_conversational_agent.py
--rw-r--r--   0 xan        (501) staff       (20)      590 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/agent_types/extraction_agent.py
--rw-r--r--   0 xan        (501) staff       (20)     6673 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/agent_types/graph_based_conversational_agent.py
--rw-r--r--   0 xan        (501) staff       (20)      843 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/agent_types/summarization_agent.py
--rw-r--r--   0 xan        (501) staff       (20)     1460 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/agent_types/zapier_agent.py
--rw-r--r--   0 xan        (501) staff       (20)     1807 2024-01-19 12:02:21.000000 bolna-0.7.7/bolna/assistant.py
--rw-r--r--   0 xan        (501) staff       (20)      937 2024-03-22 13:50:32.000000 bolna-0.7.7/bolna/constants.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.903714 bolna-0.7.7/bolna/helpers/
--rw-r--r--   0 xan        (501) staff       (20)        0 2023-12-23 18:13:48.000000 bolna-0.7.7/bolna/helpers/__init__.py
--rw-r--r--   0 xan        (501) staff       (20)     9978 2024-03-22 13:50:32.000000 bolna-0.7.7/bolna/helpers/analytics_helpers.py
--rw-r--r--   0 xan        (501) staff       (20)        0 2024-01-12 18:42:30.000000 bolna-0.7.7/bolna/helpers/cache_helpers.py
--rw-r--r--   0 xan        (501) staff       (20)      548 2024-01-07 16:40:54.000000 bolna-0.7.7/bolna/helpers/logger_config.py
--rw-r--r--   0 xan        (501) staff       (20)    18542 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/helpers/utils.py
--rw-r--r--   0 xan        (501) staff       (20)     3929 2024-03-22 13:50:32.000000 bolna-0.7.7/bolna/helpers/vad.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.904348 bolna-0.7.7/bolna/input_handlers/
--rw-r--r--   0 xan        (501) staff       (20)      159 2024-03-22 13:50:32.000000 bolna-0.7.7/bolna/input_handlers/__init__.py
--rw-r--r--   0 xan        (501) staff       (20)     3748 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/input_handlers/default.py
--rw-r--r--   0 xan        (501) staff       (20)     4547 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/input_handlers/telephony.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.904633 bolna-0.7.7/bolna/input_handlers/telephony_providers/
--rw-r--r--   0 xan        (501) staff       (20)      664 2024-03-22 13:50:32.000000 bolna-0.7.7/bolna/input_handlers/telephony_providers/exotel.py
--rw-r--r--   0 xan        (501) staff       (20)      662 2024-03-22 13:50:32.000000 bolna-0.7.7/bolna/input_handlers/telephony_providers/twilio.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.905686 bolna-0.7.7/bolna/llms/
--rw-r--r--   0 xan        (501) staff       (20)       63 2023-12-23 22:38:43.000000 bolna-0.7.7/bolna/llms/__init__.py
--rw-r--r--   0 xan        (501) staff       (20)     3984 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/llms/litellm.py
--rw-r--r--   0 xan        (501) staff       (20)      380 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/llms/llm.py
--rw-r--r--   0 xan        (501) staff       (20)     4346 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/llms/openai_llm.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.896586 bolna-0.7.7/bolna/memory/
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.906361 bolna-0.7.7/bolna/memory/cache/
--rw-r--r--   0 xan        (501) staff       (20)       54 2024-01-12 18:42:30.000000 bolna-0.7.7/bolna/memory/cache/__init__.py
--rw-r--r--   0 xan        (501) staff       (20)      161 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/memory/cache/base_cache.py
--rw-r--r--   0 xan        (501) staff       (20)     1014 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/memory/cache/inmemory_scalar_cache.py
--rw-r--r--   0 xan        (501) staff       (20)     1254 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/memory/cache/vector_cache.py
--rw-r--r--   0 xan        (501) staff       (20)     4673 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/models.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.906774 bolna-0.7.7/bolna/output_handlers/
--rw-r--r--   0 xan        (501) staff       (20)      162 2024-03-22 13:50:32.000000 bolna-0.7.7/bolna/output_handlers/__init__.py
--rw-r--r--   0 xan        (501) staff       (20)     1492 2024-03-22 13:50:32.000000 bolna-0.7.7/bolna/output_handlers/default.py
--rw-r--r--   0 xan        (501) staff       (20)     2028 2024-03-22 13:50:32.000000 bolna-0.7.7/bolna/output_handlers/telephony.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.907060 bolna-0.7.7/bolna/output_handlers/telephony_providers/
--rw-r--r--   0 xan        (501) staff       (20)     1360 2024-03-22 13:50:32.000000 bolna-0.7.7/bolna/output_handlers/telephony_providers/exotel.py
--rw-r--r--   0 xan        (501) staff       (20)     2291 2024-03-30 13:29:33.000000 bolna-0.7.7/bolna/output_handlers/telephony_providers/twilio.py
--rw-r--r--   0 xan        (501) staff       (20)     2781 2024-04-22 11:30:07.000000 bolna-0.7.7/bolna/prompts.py
--rw-r--r--   0 xan        (501) staff       (20)     1673 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/providers.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.908963 bolna-0.7.7/bolna/synthesizer/
--rw-r--r--   0 xan        (501) staff       (20)      306 2024-04-01 19:37:04.000000 bolna-0.7.7/bolna/synthesizer/__init__.py
--rw-r--r--   0 xan        (501) staff       (20)     1096 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/synthesizer/base_synthesizer.py
--rw-r--r--   0 xan        (501) staff       (20)     2786 2024-04-26 13:33:46.000000 bolna-0.7.7/bolna/synthesizer/deepgram_synthesizer.py
--rw-r--r--   0 xan        (501) staff       (20)    10697 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/synthesizer/elevenlabs_synthesizer.py
--rw-r--r--   0 xan        (501) staff       (20)     3483 2024-02-04 09:51:18.000000 bolna-0.7.7/bolna/synthesizer/fourie_synthesizer.py
--rw-r--r--   0 xan        (501) staff       (20)     4287 2024-04-22 11:30:07.000000 bolna-0.7.7/bolna/synthesizer/openai_synthesizer.py
--rw-r--r--   0 xan        (501) staff       (20)     4566 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/synthesizer/polly_synthesizer.py
--rw-r--r--   0 xan        (501) staff       (20)     7100 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/synthesizer/xtts_synthesizer.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.909769 bolna-0.7.7/bolna/transcriber/
--rw-r--r--   0 xan        (501) staff       (20)      100 2024-05-07 18:42:57.000000 bolna-0.7.7/bolna/transcriber/__init__.py
--rw-r--r--   0 xan        (501) staff       (20)    17668 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/transcriber/azure_transcriber.py
--rw-r--r--   0 xan        (501) staff       (20)     2242 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/transcriber/base_transcriber.py
--rw-r--r--   0 xan        (501) staff       (20)    16058 2024-05-07 14:41:36.000000 bolna-0.7.7/bolna/transcriber/deepgram_transcriber.py
--rw-r--r--   0 xan        (501) staff       (20)    18909 2024-04-26 13:37:59.000000 bolna-0.7.7/bolna/transcriber/hume_transcriber.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-07 18:45:57.910198 bolna-0.7.7/bolna.egg-info/
--rw-r--r--   0 xan        (501) staff       (20)    48383 2024-05-07 18:45:57.000000 bolna-0.7.7/bolna.egg-info/PKG-INFO
--rw-r--r--   0 xan        (501) staff       (20)     2031 2024-05-07 18:45:57.000000 bolna-0.7.7/bolna.egg-info/SOURCES.txt
--rw-r--r--   0 xan        (501) staff       (20)        1 2024-05-07 18:45:57.000000 bolna-0.7.7/bolna.egg-info/dependency_links.txt
--rw-r--r--   0 xan        (501) staff       (20)      387 2024-05-07 18:45:57.000000 bolna-0.7.7/bolna.egg-info/requires.txt
--rw-r--r--   0 xan        (501) staff       (20)        6 2024-05-07 18:45:57.000000 bolna-0.7.7/bolna.egg-info/top_level.txt
--rw-r--r--   0 xan        (501) staff       (20)     1164 2024-05-07 18:45:43.000000 bolna-0.7.7/pyproject.toml
--rw-r--r--   0 xan        (501) staff       (20)      370 2024-05-07 18:42:54.000000 bolna-0.7.7/requirements.txt
--rw-r--r--   0 xan        (501) staff       (20)       38 2024-05-07 18:45:57.910916 bolna-0.7.7/setup.cfg
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.279157 bolna-0.7.8/
+-rw-r--r--   0 xan        (501) staff       (20)    34522 2024-05-16 15:44:48.000000 bolna-0.7.8/LICENSE
+-rw-r--r--   0 xan        (501) staff       (20)    50955 2024-05-20 14:36:33.278889 bolna-0.7.8/PKG-INFO
+-rw-r--r--   0 xan        (501) staff       (20)    10028 2024-05-19 09:18:41.000000 bolna-0.7.8/README.md
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.262924 bolna-0.7.8/bolna/
+-rw-r--r--   0 xan        (501) staff       (20)      330 2024-05-20 14:35:00.000000 bolna-0.7.8/bolna/__init__.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.265050 bolna-0.7.8/bolna/agent_manager/
+-rw-r--r--   0 xan        (501) staff       (20)      124 2024-01-07 06:26:49.000000 bolna-0.7.8/bolna/agent_manager/__init__.py
+-rw-r--r--   0 xan        (501) staff       (20)     3138 2024-05-20 13:21:39.000000 bolna-0.7.8/bolna/agent_manager/assistant_manager.py
+-rw-r--r--   0 xan        (501) staff       (20)      174 2024-01-07 16:40:54.000000 bolna-0.7.8/bolna/agent_manager/base_manager.py
+-rw-r--r--   0 xan        (501) staff       (20)    89754 2024-05-20 13:21:39.000000 bolna-0.7.8/bolna/agent_manager/task_manager.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.268221 bolna-0.7.8/bolna/agent_types/
+-rw-r--r--   0 xan        (501) staff       (20)      302 2024-05-18 15:13:13.000000 bolna-0.7.8/bolna/agent_types/__init__.py
+-rw-r--r--   0 xan        (501) staff       (20)      176 2024-01-07 16:40:54.000000 bolna-0.7.8/bolna/agent_types/base_agent.py
+-rw-r--r--   0 xan        (501) staff       (20)     1353 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/agent_types/contextual_conversational_agent.py
+-rw-r--r--   0 xan        (501) staff       (20)      590 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/agent_types/extraction_agent.py
+-rw-r--r--   0 xan        (501) staff       (20)     6673 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/agent_types/graph_based_conversational_agent.py
+-rw-r--r--   0 xan        (501) staff       (20)      843 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/agent_types/summarization_agent.py
+-rw-r--r--   0 xan        (501) staff       (20)     1485 2024-05-18 15:13:13.000000 bolna-0.7.8/bolna/agent_types/webhook_agent.py
+-rw-r--r--   0 xan        (501) staff       (20)     1807 2024-01-19 12:02:21.000000 bolna-0.7.8/bolna/assistant.py
+-rw-r--r--   0 xan        (501) staff       (20)     1256 2024-05-16 17:24:11.000000 bolna-0.7.8/bolna/constants.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.269893 bolna-0.7.8/bolna/helpers/
+-rw-r--r--   0 xan        (501) staff       (20)        0 2023-12-23 18:13:48.000000 bolna-0.7.8/bolna/helpers/__init__.py
+-rw-r--r--   0 xan        (501) staff       (20)     9978 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/helpers/analytics_helpers.py
+-rw-r--r--   0 xan        (501) staff       (20)        0 2024-01-12 18:42:30.000000 bolna-0.7.8/bolna/helpers/cache_helpers.py
+-rw-r--r--   0 xan        (501) staff       (20)      548 2024-01-07 16:40:54.000000 bolna-0.7.8/bolna/helpers/logger_config.py
+-rw-r--r--   0 xan        (501) staff       (20)    18791 2024-05-18 15:13:13.000000 bolna-0.7.8/bolna/helpers/utils.py
+-rw-r--r--   0 xan        (501) staff       (20)     3929 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/helpers/vad.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.270461 bolna-0.7.8/bolna/input_handlers/
+-rw-r--r--   0 xan        (501) staff       (20)      159 2024-05-16 17:24:11.000000 bolna-0.7.8/bolna/input_handlers/__init__.py
+-rw-r--r--   0 xan        (501) staff       (20)     3748 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/input_handlers/default.py
+-rw-r--r--   0 xan        (501) staff       (20)     4617 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/input_handlers/telephony.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.270894 bolna-0.7.8/bolna/input_handlers/telephony_providers/
+-rw-r--r--   0 xan        (501) staff       (20)      664 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/input_handlers/telephony_providers/exotel.py
+-rw-r--r--   0 xan        (501) staff       (20)      662 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/input_handlers/telephony_providers/twilio.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.271918 bolna-0.7.8/bolna/llms/
+-rw-r--r--   0 xan        (501) staff       (20)       63 2023-12-23 22:38:43.000000 bolna-0.7.8/bolna/llms/__init__.py
+-rw-r--r--   0 xan        (501) staff       (20)     4041 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/llms/litellm.py
+-rw-r--r--   0 xan        (501) staff       (20)      380 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/llms/llm.py
+-rw-r--r--   0 xan        (501) staff       (20)     3584 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/llms/openai_llm.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.259442 bolna-0.7.8/bolna/memory/
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.272832 bolna-0.7.8/bolna/memory/cache/
+-rw-r--r--   0 xan        (501) staff       (20)       54 2024-01-12 18:42:30.000000 bolna-0.7.8/bolna/memory/cache/__init__.py
+-rw-r--r--   0 xan        (501) staff       (20)      161 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/memory/cache/base_cache.py
+-rw-r--r--   0 xan        (501) staff       (20)     1014 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/memory/cache/inmemory_scalar_cache.py
+-rw-r--r--   0 xan        (501) staff       (20)     1254 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/memory/cache/vector_cache.py
+-rw-r--r--   0 xan        (501) staff       (20)     5673 2024-05-20 13:21:39.000000 bolna-0.7.8/bolna/models.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.273692 bolna-0.7.8/bolna/output_handlers/
+-rw-r--r--   0 xan        (501) staff       (20)      162 2024-05-16 17:24:11.000000 bolna-0.7.8/bolna/output_handlers/__init__.py
+-rw-r--r--   0 xan        (501) staff       (20)     1492 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/output_handlers/default.py
+-rw-r--r--   0 xan        (501) staff       (20)     2439 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/output_handlers/telephony.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.274111 bolna-0.7.8/bolna/output_handlers/telephony_providers/
+-rw-r--r--   0 xan        (501) staff       (20)     1360 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/output_handlers/telephony_providers/exotel.py
+-rw-r--r--   0 xan        (501) staff       (20)     2291 2024-05-17 09:22:34.000000 bolna-0.7.8/bolna/output_handlers/telephony_providers/twilio.py
+-rw-r--r--   0 xan        (501) staff       (20)     2781 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/prompts.py
+-rw-r--r--   0 xan        (501) staff       (20)     1714 2024-05-17 07:22:52.000000 bolna-0.7.8/bolna/providers.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.276330 bolna-0.7.8/bolna/synthesizer/
+-rw-r--r--   0 xan        (501) staff       (20)      306 2024-05-17 07:22:52.000000 bolna-0.7.8/bolna/synthesizer/__init__.py
+-rw-r--r--   0 xan        (501) staff       (20)     1208 2024-05-18 15:13:13.000000 bolna-0.7.8/bolna/synthesizer/base_synthesizer.py
+-rw-r--r--   0 xan        (501) staff       (20)     2786 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/synthesizer/deepgram_synthesizer.py
+-rw-r--r--   0 xan        (501) staff       (20)    11230 2024-05-16 17:24:11.000000 bolna-0.7.8/bolna/synthesizer/elevenlabs_synthesizer.py
+-rw-r--r--   0 xan        (501) staff       (20)     3483 2024-02-04 09:51:18.000000 bolna-0.7.8/bolna/synthesizer/fourie_synthesizer.py
+-rw-r--r--   0 xan        (501) staff       (20)     4287 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/synthesizer/openai_synthesizer.py
+-rw-r--r--   0 xan        (501) staff       (20)     5577 2024-05-16 17:24:11.000000 bolna-0.7.8/bolna/synthesizer/polly_synthesizer.py
+-rw-r--r--   0 xan        (501) staff       (20)     7100 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/synthesizer/xtts_synthesizer.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.278026 bolna-0.7.8/bolna/transcriber/
+-rw-r--r--   0 xan        (501) staff       (20)      152 2024-05-16 17:24:11.000000 bolna-0.7.8/bolna/transcriber/__init__.py
+-rw-r--r--   0 xan        (501) staff       (20)     2242 2024-05-15 20:50:00.000000 bolna-0.7.8/bolna/transcriber/base_transcriber.py
+-rw-r--r--   0 xan        (501) staff       (20)    16323 2024-05-20 13:21:39.000000 bolna-0.7.8/bolna/transcriber/deepgram_transcriber.py
+-rw-r--r--   0 xan        (501) staff       (20)    18909 2024-04-26 13:37:59.000000 bolna-0.7.8/bolna/transcriber/hume_transcriber.py
+-rw-r--r--   0 xan        (501) staff       (20)    14620 2024-05-16 17:24:11.000000 bolna-0.7.8/bolna/transcriber/whisper_transcriber.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.278275 bolna-0.7.8/bolna.egg-info/
+-rw-r--r--   0 xan        (501) staff       (20)    50955 2024-05-20 14:36:33.000000 bolna-0.7.8/bolna.egg-info/PKG-INFO
+-rw-r--r--   0 xan        (501) staff       (20)     2034 2024-05-20 14:36:33.000000 bolna-0.7.8/bolna.egg-info/SOURCES.txt
+-rw-r--r--   0 xan        (501) staff       (20)        1 2024-05-20 14:36:33.000000 bolna-0.7.8/bolna.egg-info/dependency_links.txt
+-rw-r--r--   0 xan        (501) staff       (20)      387 2024-05-20 14:36:33.000000 bolna-0.7.8/bolna.egg-info/requires.txt
+-rw-r--r--   0 xan        (501) staff       (20)        6 2024-05-20 14:36:33.000000 bolna-0.7.8/bolna.egg-info/top_level.txt
+-rw-r--r--   0 xan        (501) staff       (20)     1164 2024-05-20 14:35:00.000000 bolna-0.7.8/pyproject.toml
+-rw-r--r--   0 xan        (501) staff       (20)      370 2024-05-16 15:44:48.000000 bolna-0.7.8/requirements.txt
+-rw-r--r--   0 xan        (501) staff       (20)       38 2024-05-20 14:36:33.279210 bolna-0.7.8/setup.cfg
```

### Comparing `bolna-0.7.7/LICENSE` & `bolna-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bolna-0.7.7/PKG-INFO` & `bolna-0.7.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bolna
-Version: 0.7.7
+Version: 0.7.8
 Author-email: Prateek Sachan <ps@prateeksachan.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -693,15 +693,15 @@
 Requires-Dist: semantic-router==0.0.37
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 
 <h1 align="center">
 </h1>
 <p align="center">
-  <p align="center"><b>End-to-end open-source voice agents platform</b>: Quickly build LLM based voice driven conversational applications</p>
+  <p align="center"><b>End-to-end open-source voice agents platform</b>: Quickly build voice firsts conversational assistants through a json. </p>
 </p>
 
 <h4 align="center">
   <a href="https://discord.gg/yDfcqreByj">Discord</a> |
   <a href="https://docs.bolna.dev">Docs</a> |
   <a href="https://bolna.dev">Website</a>
 </h4>
@@ -744,42 +744,127 @@
 The setup consists of four containers:
 
 1. Twilio web server: for initiating the calls one will need to set up a [Twilio account]([https://www.twilio.com/docs/usage/tutorials/how-to-use-your-free-trial-account](https://www.twilio.com/docs/messaging/guides/how-to-use-your-free-trial-account))
 2. Bolna server: for creating and handling agents 
 3. `ngrok`: for tunneling. One will need to add the `authtoken` to `ngrok-config.yml`
 4. `redis`: for persisting agents & prompt data
 
-Running `docker-compose up --build` will use the `.env` as the environment file.
+Use docker to build the images using `.env` file as the environment file and run them locally
+1. `docker-compose build --no-cache`: rebuild images
+2. `docker-compose up`: run the build images
 
 Once the docker containers are up, you can now start to create your agents and instruct them to initiate calls.
 
 
 
 ## Creating your agent and invoking calls
 Once you have the above docker setup and running, you can create agents and initiate calls.
-1. Refer to the official [`Agent` API](https://docs.bolna.dev/api-reference/agent/create) to create an agent
-2. Initiate a call via API similar to [`Call` API](https://docs.bolna.dev/api-reference/calls/make) to receive a call
+1. Use the below payload to create an Agent via `http://localhost:5001/agent`
+
+<details>
+<summary>Agent Payload</summary><br>
+
+```yaml
+{
+    "agent_config": {
+        "agent_name": "Alfred",
+        "agent_type": "other",
+        "agent_welcome_message": "Welcome",
+        "tasks": [
+            {
+                "task_type": "conversation",
+                "toolchain": {
+                    "execution": "parallel",
+                    "pipelines": [
+                        [
+                            "transcriber",
+                            "llm",
+                            "synthesizer"
+                        ]
+                    ]
+                },
+                "tools_config": {
+                    "input": {
+                        "format": "pcm",
+                        "provider": "twilio"
+                    },
+                    "llm_agent": {
+                        "agent_flow_type": "streaming",
+                        "family": "openai",
+                        "request_json": true,
+                        "model": "gpt-3.5-turbo-16k",
+                        "use_fallback": true
+                    },
+                    "output": {
+                        "format": "pcm",
+                        "provider": "twilio"
+                    },
+                    "synthesizer": {
+                        "audio_format": "wav",
+                        "provider": "elevenlabs",
+                        "stream": true,
+                        "provider_config": {
+                            "voice": "Meera - high quality, emotive",
+                            "model": "eleven_multilingual_v2",
+                            "voice_id": "TTa58Hl9lmhnQEvhp1WM"
+                        },
+                        "buffer_size": 100.0
+                    },
+                    "transcriber": {
+                        "encoding": "linear16",
+                        "language": "en",
+                        "model": "deepgram",
+                        "stream": true
+                    }
+                },
+                "task_config": {
+                    "hangup_after_silence": 30.0
+                }
+            }
+        ]
+    },
+    "agent_prompts": {
+        "task_1": {
+            "system_prompt": "Ask if they are coming for party tonight"
+        }
+    }
+}
+```
+</details>
+
+2. The response of the previous API will return a uuid as the `agent_id`. Use this `agent_id` to initiate a call via the telephony server running on `8001` port at `http://localhost:8001/call`
+
+<details>
+<summary>Call Payload</summary><br>
+
+```yaml
+{
+    "agent_id": "4c19700b-227c-4c2d-8bgf-42dfe4b240fc",
+    "recipient_phone_number": "+19876543210",
+}
+```
+</details>
 
 
 ## Using your own providers
 You can populate the `.env` file to use your own keys for providers.
 
-<details open>
+<details>
 
 <summary>ASR Providers</summary><br>
 These are the current supported ASRs Providers:
 
 | Provider     | Environment variable to be added in `.env` file |
 |--------------|-------------------------------------------------|
 | Deepgram     | `DEEPGRAM_AUTH_TOKEN`                           |
 
 </details>
 &nbsp;<br>
 
-<details open>
+<details>
 <summary>LLM Providers</summary><br>
 Bolna uses LiteLLM package to support multiple LLM integrations.
 
 These are the current supported LLM Provider Family:
 https://github.com/bolna-ai/bolna/blob/c8a0d1428793d4df29133119e354bc2f85a7ca76/bolna/providers.py#L19-L28
 
 For LiteLLM based LLMs, add either of the following to the `.env` file depending on your use-case:<br><br>
@@ -789,15 +874,15 @@
 
 For LLMs hosted via VLLM, add the following to the `.env` file:<br>
 `VLLM_SERVER_BASE_URL`: URL of the hosted LLM using VLLM
 
 </details>
 &nbsp;<br>
 
-<details open>
+<details>
 
 <summary>TTS Providers</summary><br>
 These are the current supported TTS Providers:
 https://github.com/bolna-ai/bolna/blob/c8a0d1428793d4df29133119e354bc2f85a7ca76/bolna/providers.py#L7-L14
 
 | Provider   | Environment variable to be added in `.env` file  |
 |------------|--------------------------------------------------|
```

### Comparing `bolna-0.7.7/README.md` & `bolna-0.7.8/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <h1 align="center">
 </h1>
 <p align="center">
-  <p align="center"><b>End-to-end open-source voice agents platform</b>: Quickly build LLM based voice driven conversational applications</p>
+  <p align="center"><b>End-to-end open-source voice agents platform</b>: Quickly build voice firsts conversational assistants through a json. </p>
 </p>
 
 <h4 align="center">
   <a href="https://discord.gg/yDfcqreByj">Discord</a> |
   <a href="https://docs.bolna.dev">Docs</a> |
   <a href="https://bolna.dev">Website</a>
 </h4>
@@ -48,42 +48,127 @@
 The setup consists of four containers:
 
 1. Twilio web server: for initiating the calls one will need to set up a [Twilio account]([https://www.twilio.com/docs/usage/tutorials/how-to-use-your-free-trial-account](https://www.twilio.com/docs/messaging/guides/how-to-use-your-free-trial-account))
 2. Bolna server: for creating and handling agents 
 3. `ngrok`: for tunneling. One will need to add the `authtoken` to `ngrok-config.yml`
 4. `redis`: for persisting agents & prompt data
 
-Running `docker-compose up --build` will use the `.env` as the environment file.
+Use docker to build the images using `.env` file as the environment file and run them locally
+1. `docker-compose build --no-cache`: rebuild images
+2. `docker-compose up`: run the build images
 
 Once the docker containers are up, you can now start to create your agents and instruct them to initiate calls.
 
 
 
 ## Creating your agent and invoking calls
 Once you have the above docker setup and running, you can create agents and initiate calls.
-1. Refer to the official [`Agent` API](https://docs.bolna.dev/api-reference/agent/create) to create an agent
-2. Initiate a call via API similar to [`Call` API](https://docs.bolna.dev/api-reference/calls/make) to receive a call
+1. Use the below payload to create an Agent via `http://localhost:5001/agent`
+
+<details>
+<summary>Agent Payload</summary><br>
+
+```yaml
+{
+    "agent_config": {
+        "agent_name": "Alfred",
+        "agent_type": "other",
+        "agent_welcome_message": "Welcome",
+        "tasks": [
+            {
+                "task_type": "conversation",
+                "toolchain": {
+                    "execution": "parallel",
+                    "pipelines": [
+                        [
+                            "transcriber",
+                            "llm",
+                            "synthesizer"
+                        ]
+                    ]
+                },
+                "tools_config": {
+                    "input": {
+                        "format": "pcm",
+                        "provider": "twilio"
+                    },
+                    "llm_agent": {
+                        "agent_flow_type": "streaming",
+                        "family": "openai",
+                        "request_json": true,
+                        "model": "gpt-3.5-turbo-16k",
+                        "use_fallback": true
+                    },
+                    "output": {
+                        "format": "pcm",
+                        "provider": "twilio"
+                    },
+                    "synthesizer": {
+                        "audio_format": "wav",
+                        "provider": "elevenlabs",
+                        "stream": true,
+                        "provider_config": {
+                            "voice": "Meera - high quality, emotive",
+                            "model": "eleven_multilingual_v2",
+                            "voice_id": "TTa58Hl9lmhnQEvhp1WM"
+                        },
+                        "buffer_size": 100.0
+                    },
+                    "transcriber": {
+                        "encoding": "linear16",
+                        "language": "en",
+                        "model": "deepgram",
+                        "stream": true
+                    }
+                },
+                "task_config": {
+                    "hangup_after_silence": 30.0
+                }
+            }
+        ]
+    },
+    "agent_prompts": {
+        "task_1": {
+            "system_prompt": "Ask if they are coming for party tonight"
+        }
+    }
+}
+```
+</details>
+
+2. The response of the previous API will return a uuid as the `agent_id`. Use this `agent_id` to initiate a call via the telephony server running on `8001` port at `http://localhost:8001/call`
+
+<details>
+<summary>Call Payload</summary><br>
+
+```yaml
+{
+    "agent_id": "4c19700b-227c-4c2d-8bgf-42dfe4b240fc",
+    "recipient_phone_number": "+19876543210",
+}
+```
+</details>
 
 
 ## Using your own providers
 You can populate the `.env` file to use your own keys for providers.
 
-<details open>
+<details>
 
 <summary>ASR Providers</summary><br>
 These are the current supported ASRs Providers:
 
 | Provider     | Environment variable to be added in `.env` file |
 |--------------|-------------------------------------------------|
 | Deepgram     | `DEEPGRAM_AUTH_TOKEN`                           |
 
 </details>
 &nbsp;<br>
 
-<details open>
+<details>
 <summary>LLM Providers</summary><br>
 Bolna uses LiteLLM package to support multiple LLM integrations.
 
 These are the current supported LLM Provider Family:
 https://github.com/bolna-ai/bolna/blob/c8a0d1428793d4df29133119e354bc2f85a7ca76/bolna/providers.py#L19-L28
 
 For LiteLLM based LLMs, add either of the following to the `.env` file depending on your use-case:<br><br>
@@ -93,15 +178,15 @@
 
 For LLMs hosted via VLLM, add the following to the `.env` file:<br>
 `VLLM_SERVER_BASE_URL`: URL of the hosted LLM using VLLM
 
 </details>
 &nbsp;<br>
 
-<details open>
+<details>
 
 <summary>TTS Providers</summary><br>
 These are the current supported TTS Providers:
 https://github.com/bolna-ai/bolna/blob/c8a0d1428793d4df29133119e354bc2f85a7ca76/bolna/providers.py#L7-L14
 
 | Provider   | Environment variable to be added in `.env` file  |
 |------------|--------------------------------------------------|
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-  EEnndd--ttoo--eenndd ooppeenn--ssoouurrccee vvooiiccee aaggeennttss ppllaattffoorrmm: Quickly build LLM based voice
-                      driven conversational applications
+   EEnndd--ttoo--eenndd ooppeenn--ssoouurrccee vvooiiccee aaggeennttss ppllaattffoorrmm: Quickly build voice firsts
+                   conversational assistants through a json.
                        ****** _DD_ii_ss_cc_oo_rr_dd || _DD_oo_cc_ss || _WW_ee_bb_ss_ii_tt_ee ******
      ****** _[[_BB_oo_ll_nn_aa_ _ii_ss_ _rr_ee_ll_ee_aa_ss_ee_dd_ _uu_nn_dd_ee_rr_ _tt_hh_ee_ _AA_GG_PP_LL_--_33_.._00_ _ll_ii_cc_ee_nn_ss_ee_.._]]_[[_PP_RR_ss_ _ww_ee_ll_cc_oo_mm_ee_!!_]] ******
 ## Introduction **[Bolna](https://bolna.dev)** is the end-to-end open source
 production ready framework for quickly building LLM based voice driven
 conversational applications. ## Demo https://github.com/bolna-ai/bolna/assets/
 1313096/2237f64f-1c5b-4723-b7e7-d11466e9b226 ## Components Bolna helps you
 create AI Voice Agents which can be instructed to do tasks beginning with: 1.
@@ -18,24 +18,42 @@
 telephony. We have dockerized the setup in `local_setup/`. One will need to
 populate an environment `.env` file from `.env.sample`. The setup consists of
 four containers: 1. Twilio web server: for initiating the calls one will need
 to set up a [Twilio account]([https://www.twilio.com/docs/usage/tutorials/how-
 to-use-your-free-trial-account](https://www.twilio.com/docs/messaging/guides/
 how-to-use-your-free-trial-account)) 2. Bolna server: for creating and handling
 agents 3. `ngrok`: for tunneling. One will need to add the `authtoken` to
-`ngrok-config.yml` 4. `redis`: for persisting agents & prompt data Running
-`docker-compose up --build` will use the `.env` as the environment file. Once
-the docker containers are up, you can now start to create your agents and
-instruct them to initiate calls. ## Creating your agent and invoking calls Once
-you have the above docker setup and running, you can create agents and initiate
-calls. 1. Refer to the official [`Agent` API](https://docs.bolna.dev/api-
-reference/agent/create) to create an agent 2. Initiate a call via API similar
-to [`Call` API](https://docs.bolna.dev/api-reference/calls/make) to receive a
-call ## Using your own providers You can populate the `.env` file to use your
-own keys for providers. ASR Providers
+`ngrok-config.yml` 4. `redis`: for persisting agents & prompt data Use docker
+to build the images using `.env` file as the environment file and run them
+locally 1. `docker-compose build --no-cache`: rebuild images 2. `docker-compose
+up`: run the build images Once the docker containers are up, you can now start
+to create your agents and instruct them to initiate calls. ## Creating your
+agent and invoking calls Once you have the above docker setup and running, you
+can create agents and initiate calls. 1. Use the below payload to create an
+Agent via `http://localhost:5001/agent` Agent Payload
+```yaml { "agent_config": { "agent_name": "Alfred", "agent_type": "other",
+"agent_welcome_message": "Welcome", "tasks": [ { "task_type": "conversation",
+"toolchain": { "execution": "parallel", "pipelines": [ [ "transcriber", "llm",
+"synthesizer" ] ] }, "tools_config": { "input": { "format": "pcm", "provider":
+"twilio" }, "llm_agent": { "agent_flow_type": "streaming", "family": "openai",
+"request_json": true, "model": "gpt-3.5-turbo-16k", "use_fallback": true },
+"output": { "format": "pcm", "provider": "twilio" }, "synthesizer":
+{ "audio_format": "wav", "provider": "elevenlabs", "stream": true,
+"provider_config": { "voice": "Meera - high quality, emotive", "model":
+"eleven_multilingual_v2", "voice_id": "TTa58Hl9lmhnQEvhp1WM" }, "buffer_size":
+100.0 }, "transcriber": { "encoding": "linear16", "language": "en", "model":
+"deepgram", "stream": true } }, "task_config": { "hangup_after_silence": 30.0 }
+} ] }, "agent_prompts": { "task_1": { "system_prompt": "Ask if they are coming
+for party tonight" } } } ``` 2. The response of the previous API will return a
+uuid as the `agent_id`. Use this `agent_id` to initiate a call via the
+telephony server running on `8001` port at `http://localhost:8001/call` Call
+Payload
+```yaml { "agent_id": "4c19700b-227c-4c2d-8bgf-42dfe4b240fc",
+"recipient_phone_number": "+19876543210", } ``` ## Using your own providers You
+can populate the `.env` file to use your own keys for providers. ASR Providers
 These are the current supported ASRs Providers: | Provider | Environment
 variable to be added in `.env` file | |--------------|-------------------------
 ------------------------| | Deepgram | `DEEPGRAM_AUTH_TOKEN` |  
 LLM Providers
 Bolna uses LiteLLM package to support multiple LLM integrations. These are the
 current supported LLM Provider Family: https://github.com/bolna-ai/bolna/blob/
 c8a0d1428793d4df29133119e354bc2f85a7ca76/bolna/providers.py#L19-L28 For LiteLLM
```

### Comparing `bolna-0.7.7/bolna/agent_manager/assistant_manager.py` & `bolna-0.7.8/bolna/agent_manager/assistant_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import time
-import tiktoken
 from .base_manager import BaseManager
 from .task_manager import TaskManager
 from bolna.helpers.logger_config import configure_logger
+from bolna.models import AGENT_WELCOME_MESSAGE
 
 logger = configure_logger(__name__)
 
-enc = tiktoken.get_encoding("cl100k_base")
 
 class AssistantManager(BaseManager):
     def __init__(self, agent_config, ws=None, assistant_id=None, context_data=None, conversation_history=None,
                  connected_through_dashboard=None, cache=None, input_queue=None, output_queue=None, **kwargs):
         super().__init__()
         self.tools = {}
         self.websocket = ws
@@ -22,26 +21,25 @@
         self.run_id = f"{self.assistant_id}#{str(int(time.time() * 1000))}"
         self.connected_through_dashboard = connected_through_dashboard
         self.cache = cache
         self.input_queue = input_queue
         self.output_queue = output_queue
         self.kwargs = kwargs
         self.conversation_history = conversation_history
-
+        self.kwargs['agent_welcome_message'] = agent_config.get('agent_welcome_message', AGENT_WELCOME_MESSAGE)
 
     async def run(self, local=False, run_id=None):
         """
         Run will start all tasks in sequential format
         """
         if run_id:
             self.run_id = run_id
 
         input_parameters = None
         for task_id, task in enumerate(self.tasks):
-
             logger.info(f"Running task {task_id} {task} and sending kwargs {self.kwargs}")
             task_manager = TaskManager(self.agent_config.get("agent_name", self.agent_config.get("assistant_name")),
                                        task_id, task, self.websocket,
                                        context_data=self.context_data, input_parameters=input_parameters,
                                        assistant_id=self.assistant_id, run_id=self.run_id,
                                        connected_through_dashboard=self.connected_through_dashboard,
                                        cache=self.cache, input_queue=self.input_queue, output_queue=self.output_queue,
```

### Comparing `bolna-0.7.7/bolna/agent_manager/task_manager.py` & `bolna-0.7.8/bolna/agent_manager/task_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 import traceback
 import time
 import json
 import uuid
 import copy
 from datetime import datetime
 
+from bolna.constants import ACCIDENTAL_INTERRUPTION_PHRASES
 from bolna.memory.cache.inmemory_scalar_cache import InmemoryScalarCache
 from bolna.memory.cache.vector_cache import VectorCache
 from .base_manager import BaseManager
 from bolna.agent_types import *
 from bolna.providers import *
+from bolna.prompts import *
 from bolna.helpers.utils import calculate_audio_duration, create_ws_data_packet, get_file_names_in_directory, get_raw_audio_bytes, is_valid_md5, \
-    get_required_input_types, format_messages, get_prompt_responses, list_number_of_wav_files_in_directory, resample, save_audio_file_to_s3, update_prompt_with_context, get_md5_hash, clean_json_string, wav_bytes_to_pcm, write_request_logs, yield_chunks_from_memory
+    get_required_input_types, format_messages, get_prompt_responses, resample, save_audio_file_to_s3, update_prompt_with_context, get_md5_hash, clean_json_string, wav_bytes_to_pcm, write_request_logs, yield_chunks_from_memory
 from bolna.helpers.logger_config import configure_logger
-import uvloop
-asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
 from semantic_router import Route
 from semantic_router.layer import RouteLayer
 from semantic_router.encoders import FastEmbedEncoder
 
 asyncio.get_event_loop().set_debug(True)
 logger = configure_logger(__name__)
 
@@ -43,16 +43,14 @@
         self.websocket = ws
         self.task_config = task
         self.context_data = context_data
         self.connected_through_dashboard = connected_through_dashboard
         self.enforce_streaming = kwargs.get("enforce_streaming", False)
         self.callee_silent = True
         self.yield_chunks = yield_chunks
-        self.kwargs["process_interim_results"] = "true" if task.get("optimize_latency", False) is True else "false"
-        logger.info(f"Processing interim results {self.kwargs['process_interim_results'] }")
         # Set up communication queues between processes
         self.audio_queue = asyncio.Queue()
         self.llm_queue = asyncio.Queue()
         self.synthesizer_queue = asyncio.Queue()
         self.transcriber_output_queue = asyncio.Queue()
         self.queues = {
             "transcriber": self.audio_queue,
@@ -86,21 +84,23 @@
             "output": [],
             "metadata": {
                 "started": 0
             }
         }
         #IO HANDLERS
         if task_id == 0:
+            self.default_io = self.task_config["tools_config"]["output"]["provider"] == 'default'
+            logger.info(f"Connected via websocket")
             self.should_record = self.task_config["tools_config"]["output"]["provider"] == 'default' and self.enforce_streaming #In this case, this is a websocket connection and we should record 
             self.__setup_input_handlers(connected_through_dashboard, input_queue, self.should_record)
         self.__setup_output_handlers(connected_through_dashboard, output_queue)
 
         # Agent stuff
         # Need to maintain current conversation history and overall persona/history kinda thing. 
-        # Soon we will maintain a seperate history for this 
+        # Soon we will maintain a separate history for this 
         self.history = [] if conversation_history is None else conversation_history 
         self.interim_history = copy.deepcopy(self.history.copy())
         logger.info(f'History {self.history}')
         self.label_flow = []
 
         # Setup IO SERVICE, TRANSCRIBER, LLM, SYNTHESIZER
         self.llm_task = None
@@ -168,71 +168,93 @@
         #Setup tasks
         self.__setup_tasks(llm)
 
 
         #setup request logs
         self.request_logs = []
 
-        # for long pauses and rushing
-        
         if task_id == 0:
-            self.output_chunk_size = 16384 if self.sampling_rate == 24000 else 4096 #0.5 second chunk size for calls 
+            self.output_chunk_size = 16384 if self.sampling_rate == 24000 else 8192 #0.5 second chunk size for calls 
             # For nitro
             self.nitro = True 
-            self.minimum_wait_duration = self.task_config["tools_config"]["transcriber"]["endpointing"]
-            logger.info(f"minimum wait duration {self.minimum_wait_duration}")
-            self.last_spoken_timestamp = time.time() * 1000
-            self.incremental_delay = task.get("incremental_delay", 100)
-            self.required_delay_before_speaking = max(self.minimum_wait_duration - self.incremental_delay, 0)  #Everytime we get a message we increase it by 100 miliseconds 
-            self.time_since_first_interim_result  = -1
-
-        #Cut conversation
-        self.hang_conversation_after = task.get("hangup_after_silence", 10)
-        self.last_transmitted_timesatamp = 0
-        self.let_remaining_audio_pass_through = False #Will be used to let remaining audio pass through in case of utterenceEnd event and there's still audio left to be sent
-        self.use_llm_to_determine_hangup = task.get("hangup_after_LLMCall", False)
-        self.check_for_completion_prompt = task.get("call_cancellation_prompt", None)
-        if self.check_for_completion_prompt is not None:
-            completion_json_format = {"answer": "A simple Yes or No based on if you should cut the phone or not"}
-            self.check_for_completion_prompt = f"{self.check_for_completion_prompt}\nYour response should be in the following json format\n{completion_json_format}"
-        self.check_for_completion_llm = os.getenv("CHECK_FOR_COMPLETION_LLM")
-        self.time_since_last_spoken_human_word = 0 
-
-        #Handling accidental interruption
-        self.number_of_words_for_interruption = task.get("number_of_words_for_interruption", 3)
-        self.started_transmitting_audio = False
-        #self.interruption_backoff_period = 1000 #task.get("interruption_backoff_period", 300) #this is the amount of time output loop will sleep before sending next audio
-        self.use_llm_for_hanging_up = task.get("hangup_after_LLMCall", False)
-        self.allow_extra_sleep = False #It'll help us to back off as soon as we hear interruption for a while
-
-        # Conversation
-        if task_id == 0:
+            conversation_config = task.get("task_config", {})
+            logger.info(f"Conversation config {conversation_config}")
+            self.kwargs["process_interim_results"] = "true" if conversation_config.get("optimize_latency", False) is True else "false"
+            logger.info(f"Processing interim results {self.kwargs['process_interim_results'] }")
+            # Routes
             self.routes = task['tools_config']['llm_agent'].get("routes", None)
             self.route_layer = None
             if self.routes:
-                self.__setup_routes(self.routes)
-        
-        #Backchanneling
-        self.should_backchannel = task.get("backchanneling", True)
-        self.backchanneling_task = None
-        self.backchanneling_start_delay = task.get("backchanneling_start_delay", 5)
-        self.backchanneling_message_gap = task.get("backchanneling_message_gap", 2) #Amount of duration co routine will sleep
-        if self.should_backchannel:
-            logger.info(f"Should backchannel")
-            self.backchanneling_audios = f'{kwargs.get("backchanneling_audio_location", os.getenv("BACKCHANNELING_PRESETS_DIR"))}/{self.synthesizer_voice.lower()}'
-            #self.num_files = list_number_of_wav_files_in_directory(self.backchanneling_audios)
-            try:
-                self.filenames = get_file_names_in_directory(self.backchanneling_audios)
-                logger.info(f"Backchanneling audio location {self.backchanneling_audios}")
-            except Exception as e:
-                logger.info(f"Something went wrong an putting should backchannel to false")
-                self.should_backchannel = False
-        else:
-            logger.info(f"Not setting up backchanneling")
-            self.backchanneling_audio_map = []
+                start_time = time.time()
+                routes_meta = self.kwargs.get('routes', None)
+                if self.kwargs['routes']:
+                    self.route_encoder = routes_meta["route_encoder"]
+                    self.vector_caches = routes_meta["vector_caches"]
+                    self.route_responses_dict = routes_meta["route_responses_dict"]
+                    self.route_layer = routes_meta["route_layer"]
+                    logger.info(f"Time to setup routes from warrmed up cache {time.time() - start_time}")
+                else:
+                    self.__setup_routes(self.routes)
+                    logger.info(f"Time to setup routes {time.time() - start_time}")
+
+
+        # for long pauses and rushing
+            if conversation_config is not None:
+                self.minimum_wait_duration = self.task_config["tools_config"]["transcriber"]["endpointing"]
+                logger.info(f"minimum wait duration {self.minimum_wait_duration}")
+                self.last_spoken_timestamp = time.time() * 1000
+                self.incremental_delay = conversation_config.get("incremental_delay", 100)
+                logger.info(f"incremental_delay - {self.incremental_delay}")
+                self.required_delay_before_speaking = max(self.minimum_wait_duration - self.incremental_delay, 0)  #Everytime we get a message we increase it by 100 miliseconds 
+                self.time_since_first_interim_result  = -1
+
+                #Cut conversation
+                self.hang_conversation_after = conversation_config.get("hangup_after_silence", 10)
+                logger.info(f"hangup_after_silence {self.hang_conversation_after}")
+                self.last_transmitted_timesatamp = 0
+                self.let_remaining_audio_pass_through = False #Will be used to let remaining audio pass through in case of utterenceEnd event and there's still audio left to be sent
+                self.use_llm_to_determine_hangup = conversation_config.get("hangup_after_LLMCall", False)
+                self.check_for_completion_prompt = conversation_config.get("call_cancellation_prompt", None)
+                if self.check_for_completion_prompt is not None:
+                    completion_json_format = {"answer": "A simple Yes or No based on if you should cut the phone or not"}
+                    self.check_for_completion_prompt = f"{self.check_for_completion_prompt}\nYour response should be in the following json format\n{completion_json_format}"
+                self.check_for_completion_llm = os.getenv("CHECK_FOR_COMPLETION_LLM")
+                self.time_since_last_spoken_human_word = 0 
+
+                #Handling accidental interruption
+                self.number_of_words_for_interruption = conversation_config.get("number_of_words_for_interruption", 3)
+                self.started_transmitting_audio = False
+                self.accidental_interruption_phrases = set(ACCIDENTAL_INTERRUPTION_PHRASES)
+                #self.interruption_backoff_period = 1000 #conversation_config.get("interruption_backoff_period", 300) #this is the amount of time output loop will sleep before sending next audio
+                self.use_llm_for_hanging_up = conversation_config.get("hangup_after_LLMCall", False)
+                self.allow_extra_sleep = False #It'll help us to back off as soon as we hear interruption for a while
+
+                #Backchanneling
+                self.should_backchannel = conversation_config.get("backchanneling", False)
+                self.backchanneling_task = None
+                self.backchanneling_start_delay = conversation_config.get("backchanneling_start_delay", 5)
+                self.backchanneling_message_gap = conversation_config.get("backchanneling_message_gap", 2) #Amount of duration co routine will sleep
+                if self.should_backchannel and not connected_through_dashboard and task_id == 0:
+                    logger.info(f"Should backchannel")
+                    self.backchanneling_audios = f'{kwargs.get("backchanneling_audio_location", os.getenv("BACKCHANNELING_PRESETS_DIR"))}/{self.synthesizer_voice.lower()}'
+                    #self.num_files = list_number_of_wav_files_in_directory(self.backchanneling_audios)
+                    try:
+                        self.filenames = get_file_names_in_directory(self.backchanneling_audios)
+                        logger.info(f"Backchanneling audio location {self.backchanneling_audios}")
+                    except Exception as e:
+                        logger.info(f"Something went wrong an putting should backchannel to false")
+                        self.should_backchannel = False
+                else:
+                    logger.info(f"Not setting up backchanneling")
+                    self.backchanneling_audio_map = []
+                # Agent welcome message
+                if "agent_welcome_message" in self.kwargs:
+                    logger.info(f"Agent welcome message present {self.kwargs['agent_welcome_message']}")
+                    self.first_message_task = None
+                
             
             
     def __setup_routes(self, routes):
         embedding_model = routes.get("embedding_model", os.getenv("ROUTE_EMBEDDING_MODEL"))
         self.route_encoder = FastEmbedEncoder(name=embedding_model)
 
         routes_list = []
@@ -319,43 +341,48 @@
                 if self.task_config['tools_config']['input']['provider'] == 'default':
                     input_kwargs['queue'] = input_queue
             self.tools["input"] = input_handler_class(**input_kwargs)
         else:
             raise "Other input handlers not supported yet"
 
     def __setup_transcriber(self):
+        
         if self.task_config["tools_config"]["transcriber"] is not None:
+            logger.info("Setting up transcriber")
             provider = "playground" if self.connected_through_dashboard else self.task_config["tools_config"]["input"][
                 "provider"]
             self.task_config["tools_config"]["transcriber"]["input_queue"] = self.audio_queue
             self.task_config['tools_config']["transcriber"]["output_queue"] = self.transcriber_output_queue
             if self.task_config["tools_config"]["transcriber"]["model"] in SUPPORTED_TRANSCRIBER_MODELS.keys():
                 if self.connected_through_dashboard:
                     self.task_config["tools_config"]["transcriber"]["stream"] = True if self.enforce_streaming else False
                     logger.info(f'self.task_config["tools_config"]["transcriber"]["stream"] {self.task_config["tools_config"]["transcriber"]["stream"]} self.enforce_streaming {self.enforce_streaming}')
                 transcriber_class = SUPPORTED_TRANSCRIBER_MODELS.get(
                     self.task_config["tools_config"]["transcriber"]["model"])
                 self.tools["transcriber"] = transcriber_class(provider, **self.task_config["tools_config"]["transcriber"], **self.kwargs)
 
     def __setup_synthesizer(self, llm_config):
-        self.synthesizer_cache = InmemoryScalarCache()
-        
         logger.info(f"Synthesizer config: {self.task_config['tools_config']['synthesizer']}")
         if self._is_conversation_task():
             self.kwargs["use_turbo"] = self.task_config["tools_config"]["transcriber"]["language"] == "en"
         if self.task_config["tools_config"]["synthesizer"] is not None:
+            if "caching" in self.task_config['tools_config']['synthesizer']:
+                caching = self.task_config["tools_config"]["synthesizer"].pop("caching")
+            else:
+                caching = True
+
             self.synthesizer_provider = self.task_config["tools_config"]["synthesizer"].pop("provider")
             synthesizer_class = SUPPORTED_SYNTHESIZER_MODELS.get(self.synthesizer_provider)
             provider_config = self.task_config["tools_config"]["synthesizer"].pop("provider_config")
             self.synthesizer_voice = provider_config["voice"]
             if self.connected_through_dashboard:
                 self.task_config["tools_config"]["synthesizer"]["audio_format"] = "mp3" # Hard code mp3 if we're connected through dashboard
                 self.task_config["tools_config"]["synthesizer"]["stream"] = True if self.enforce_streaming else False #Hardcode stream to be False as we don't want to get blocked by a __listen_synthesizer co-routine
         
-            self.tools["synthesizer"] = synthesizer_class(**self.task_config["tools_config"]["synthesizer"], **provider_config, **self.kwargs, cache = self.synthesizer_cache)
+            self.tools["synthesizer"] = synthesizer_class(**self.task_config["tools_config"]["synthesizer"], **provider_config, **self.kwargs, caching = caching)
             if self.task_config["tools_config"]["llm_agent"] is not None:
                 llm_config["buffer_size"] = self.task_config["tools_config"]["synthesizer"].get('buffer_size')
 
     def __setup_llm(self, llm_config):
         if self.task_config["tools_config"]["llm_agent"] is not None:
             logger.info(f'### PROVIDER {self.task_config["tools_config"]["llm_agent"]["provider"] }')
             if self.task_config["tools_config"]["llm_agent"]["provider"] in SUPPORTED_LLM_PROVIDERS.keys():
@@ -380,17 +407,17 @@
             self.tools["llm_agent"] = ExtractionContextualAgent(llm, prompt=self.system_prompt)
             self.extracted_data = None
         elif self.task_config["task_type"] == "summarization":
             logger.info("Setting up summarization agent")
             self.tools["llm_agent"] = SummarizationContextualAgent(llm, prompt=self.system_prompt)
             self.summarized_data = None
         elif self.task_config["task_type"] == "webhook":
-            zap_url = self.task_config["tools_config"]["api_tools"]["webhookURL"]
-            logger.info(f"Zap URL {zap_url}")
-            self.tools["webhook_agent"] = ZapierAgent(zap_url=zap_url)
+            webhook_url = self.task_config["tools_config"]["api_tools"]["webhookURL"]
+            logger.info(f"Webhook URL {webhook_url}")
+            self.tools["webhook_agent"] = WebhookAgent(webhook_url=webhook_url)
 
         logger.info("prompt and config setup completed")
         
     ########################
     # Helper methods
     ########################
     async def load_prompt(self, assistant_name, task_id, local, **kwargs):
@@ -404,15 +431,16 @@
                 "system_prompt": f'{self.task_config["tools_config"]["llm_agent"]["prompt"]} \n### Date\n Today\'s Date is {today}'
             }
             logger.info(f"Prompt given in llm_agent and hence storing the prompt")
         else:
             prompt_responses = kwargs.get('prompt_responses', None)
             if not prompt_responses:
                 prompt_responses = await get_prompt_responses(assistant_id=self.assistant_id, local=self.is_local)
-            self.prompts = prompt_responses["task_{}".format(task_id + 1)]
+            current_task = "task_{}".format(task_id + 1)
+            self.prompts = self.__prefill_prompts(self.task_config, prompt_responses.get(current_task, None), self.task_config['task_type'])
             if self.task_config["tools_config"]["llm_agent"]['agent_flow_type'] == "preprocessed":
                 self.tools["llm_agent"].load_prompts_and_create_graph(self.prompts)
 
         if "system_prompt" in self.prompts:
             # This isn't a graph based agent
             enriched_prompt = self.prompts["system_prompt"]
             if self.context_data is not None:
@@ -431,25 +459,36 @@
         if len(self.system_prompt['content']) == 0:
             self.history = [] if len(self.history) == 0 else self.history
         else:
             self.history = [self.system_prompt] if len(self.history) == 0 else [self.system_prompt] + self.history
 
         self.interim_history = copy.deepcopy(self.history)
 
+    def __prefill_prompts(self, task, prompt, task_type):
+        if not prompt and task_type in ('extraction', 'summarization'):
+            if task_type == 'extraction':
+                extraction_json = task.get("tools_config").get('llm_agent').get('extraction_json')
+                prompt = EXTRACTION_PROMPT.format(extraction_json)
+                return {"system_prompt": prompt}
+            elif task_type == 'summarization':
+                return {"system_prompt": SUMMARIZATION_PROMPT}
+
+        return prompt
+
     def __process_stop_words(self, text_chunk, meta_info):
          #THis is to remove stop words. Really helpful in smaller 7B models
         if "end_of_llm_stream" in meta_info and meta_info["end_of_llm_stream"] and "user" in text_chunk[-5:].lower():
             if text_chunk[-5:].lower() == "user:":
                 text_chunk = text_chunk[:-5]
             elif text_chunk[-4:].lower() == "user":
                 text_chunk = text_chunk[:-4]
 
-        index = text_chunk.find("AI")
-        if index != -1:
-            text_chunk = text_chunk[index+2:]
+        # index = text_chunk.find("AI")
+        # if index != -1:
+        #     text_chunk = text_chunk[index+2:]
         return text_chunk
     
     async def process_interruption(self):
         logger.info(f"Handling interruption sequenxce ids {self.sequence_ids}")
         await self.__cleanup_downstream_tasks()    
 
     async def __cleanup_downstream_tasks(self):
@@ -463,14 +502,19 @@
             logger.info(f"Cancelling output task")
             self.output_task.cancel()
 
         if self.llm_task is not None:
             logger.info(f"Cancelling LLM Task")
             self.llm_task.cancel()
             self.llm_task = None
+        
+        if self.first_message_task is not None:
+            logger.info("Cancelling first message task")
+            self.first_message_task.cancel()
+            self.first_message_task = None
 
         # self.synthesizer_task.cancel()
         # self.synthesizer_task = asyncio.create_task(self.__listen_synthesizer())
         for task in self.synthesizer_tasks:
             task.cancel()
         
         self.synthesizer_tasks = []
@@ -533,15 +577,15 @@
         if "stream_sid" in message:
             self.stream_sid = message['meta_info']["stream_sid"]
 
     async def _process_followup_task(self, message=None):
         logger.info(f" TASK CONFIG  {self.task_config['task_type']}")
         if self.task_config["task_type"] == "webhook":
             logger.info(f"Input patrameters {self.input_parameters}")
-            logger.info(f"DOING THE POST REQUEST TO ZAPIER WEBHOOK {self.input_parameters['extraction_details']}")
+            logger.info(f"DOING THE POST REQUEST TO WEBHOOK {self.input_parameters['extraction_details']}")
             self.webhook_response = await self.tools["webhook_agent"].execute(self.input_parameters['extraction_details'])
             logger.info(f"Response from the server {self.webhook_response}")
         else:
             message = format_messages(self.input_parameters["messages"])  # Remove the initial system prompt
             self.history.append({
                 'role': 'user',
                 'content': message
@@ -575,28 +619,30 @@
             await asyncio.sleep(5)  # Making sure whatever message was passed is over
 
 
     def __update_preprocessed_tree_node(self):
         logger.info(f"It's a preprocessed flow and hence updating current node")
         self.tools['llm_agent'].update_current_node()
     
-    def __convert_to_request_log(self, message, meta_info, model, component = "transcriber", direction = 'response'):
+    def __convert_to_request_log(self, message, meta_info, model, component = "transcriber", direction = 'response', is_cached = False, engine=None):
         log = dict()
         log['direction'] = direction
         log['data'] = message
         log['leg_id'] = meta_info['request_id'] if "request_id" in meta_info else "1234"
         log['time'] = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         log['component'] = component
         log['sequence_id'] = meta_info['sequence_id']
         log['model'] = model
+        log['cached'] = is_cached
         if component == "transcriber":
             if 'is_final' in meta_info and meta_info['is_final']:
                 log['is_final'] = True
         else:
             log['is_final'] = False #This is logged only for users to know final transcript from the transcriber
+        log['engine'] = engine
         asyncio.create_task(write_request_logs(log, self.run_id))
 
     ##############################################################
     # LLM task
     ##############################################################
     async def _handle_llm_output(self, next_step, text_chunk, should_bypass_synth, meta_info):
 
@@ -616,15 +662,15 @@
 
     async def _process_conversation_preprocessed_task(self, message, sequence, meta_info):
         if self.task_config["tools_config"]["llm_agent"]['agent_flow_type'] == "preprocessed":
             messages = copy.deepcopy(self.history)
             messages.append({'role': 'user', 'content': message['data']})
             logger.info(f"Starting LLM Agent {messages}")
             #Expose get current classification_response method from the agent class and use it for the response log
-            self.__convert_to_request_log(message = format_messages(messages, use_system_prompt= True), meta_info= meta_info, component="llm", direction="request", model=self.task_config["tools_config"]["llm_agent"]["model"])
+            self.__convert_to_request_log(message = format_messages(messages, use_system_prompt= True), meta_info= meta_info, component="llm", direction="request", model=self.task_config["tools_config"]["llm_agent"]["model"], is_cached= True)
             async for next_state in self.tools['llm_agent'].generate(messages, label_flow=self.label_flow):
                 if next_state == "<end_of_conversation>":
                     meta_info["end_of_conversation"] = True
                     self.buffered_output_queue.put_nowait(create_ws_data_packet("<end_of_conversation>", meta_info))
                     return
                 
                 logger.info(f"Text chunk {next_state['text']}")
@@ -634,15 +680,14 @@
             logger.info(f"Interim history after the LLM task {messages}")
             self.llm_response_generated = True
             self.interim_history = copy.deepcopy(messages)
             if self.callee_silent:
                 logger.info("When we got utterance end, maybe LLM was still generating response. So, copying into history")
                 self.history = copy.deepcopy(self.interim_history)
 
-
     async def _process_conversation_formulaic_task(self, message, sequence, meta_info):
         llm_response = ""
         logger.info("Agent flow is formulaic and hence moving smoothly")
         async for text_chunk in self.tools['llm_agent'].generate(self.history):
             if is_valid_md5(text_chunk):
                 self.synthesizer_tasks.append(asyncio.create_task(
                     self._synthesize(create_ws_data_packet(text_chunk, meta_info, is_md5_hash=True))))
@@ -679,42 +724,43 @@
             # If not send the response else get the response from the vector store
             logger.info(f"Vector caches {self.vector_caches}")
             if route in self.vector_caches:
                 logger.info(f"Route {route} has a vector cache")
                 relevant_utterance = self.vector_caches[route].get(message['data'])
                 cache_response = self.route_responses_dict[route][relevant_utterance]
                 self.__convert_to_request_log(message = message['data'], meta_info= meta_info, component="llm", direction="request", model=self.task_config["tools_config"]["llm_agent"]["model"])
-                self.__convert_to_request_log(message = message['data'], meta_info= meta_info, component="llm", direction="response", model=self.task_config["tools_config"]["llm_agent"]["model"])
+                self.__convert_to_request_log(message = message['data'], meta_info= meta_info, component="llm", direction="response", model=self.task_config["tools_config"]["llm_agent"]["model"], is_cached= True)
                 messages = copy.deepcopy(self.history)
                 messages += [{'role': 'user', 'content': message['data']},{'role': 'assistant', 'content': cache_response}]
                 self.interim_history = copy.deepcopy(messages)
                 self.llm_response_generated = True
                 if self.callee_silent:
                     logger.info("##### When we got utterance end, maybe LLM was still generating response. So, copying into history")
                     self.history = copy.deepcopy(self.interim_history)
 
             else:
                 logger.info(f"Route doesn't have a vector cache, and hence simply returning back a given response")
                 cache_response = self.route_responses_dict[route]
             
             logger.info(f"Cached response {cache_response}")
             meta_info['cached'] = True
-            meta_info["end_of_llm_stream"] = True
+            meta_info["end_of_llm_stream"] = True            
                 
             await self._handle_llm_output(next_step, cache_response, should_bypass_synth, meta_info)
             self.llm_processed_request_ids.add(self.current_request_id)
         else:
             messages = copy.deepcopy(self.history)
             messages.append({'role': 'user', 'content': message['data']})
             ### TODO CHECK IF THIS IS EVEN REQUIRED
             self.__convert_to_request_log(message=format_messages(messages, use_system_prompt= True), meta_info= meta_info, component="llm", direction="request", model=self.task_config["tools_config"]["llm_agent"]["model"])
             
             async for llm_message in self.tools['llm_agent'].generate(messages, synthesize=True):
                 text_chunk, end_of_llm_stream = llm_message
                 llm_response += " " + text_chunk
+                logger.info(f"Got a response from LLM {llm_response}")
                 if self.stream:
                     if end_of_llm_stream:
                         meta_info["end_of_llm_stream"] = True
                     text_chunk = self.__process_stop_words(text_chunk, meta_info)
                     logger.info(f"##### O/P from LLM {text_chunk} {llm_response}")
                     await self._handle_llm_output(next_step, text_chunk, should_bypass_synth, meta_info)
                     
@@ -846,15 +892,15 @@
         try:
             while True:
                 message = await self.transcriber_output_queue.get()
                 logger.info(f"##### Message from the transcriber class {message}")
                 if message["data"].strip() == "":
                     continue
                 if message['data'] == "transcriber_connection_closed":
-                    self.transcriber_duration += message['meta_info']["transcriber_duration"]
+                    self.transcriber_duration += message['meta_info']["transcriber_duration"] if message['meta_info'] is not None else 0
                     logger.info("transcriber connection closed")
                     break
 
                 if self.stream:
                     self._set_call_details(message)
                     meta_info = message["meta_info"]
                     sequence = await self.process_transcriber_request(meta_info)
@@ -933,15 +979,15 @@
                             # Hence we transmit quickly 
                             if not self.started_transmitting_audio:
                                 logger.info("##### Haven't started transmitting audio and hence cleaning up downstream tasks")
                                 await self.__cleanup_downstream_tasks()
                             
                             # If we've started transmitting audio this is probably an interruption, so calculate number of words
                             if self.nitro and self.started_transmitting_audio:
-                                if num_words > self.number_of_words_for_interruption:
+                                if num_words > self.number_of_words_for_interruption or message['data'].strip() in self.accidental_interruption_phrases:
                                     #Process interruption only if number of words is higher than the threshold 
                                     logger.info(f"###### Number of words {num_words} is higher than the required number of words for interruption, hence, definitely interrupting")
                                     await self.__cleanup_downstream_tasks()
                                 else:
                                     logger.info(f"Not starting a cleanup because {num_words} number of words are lesser {self.number_of_words_for_interruption} and hence continuing,")
                                     continue
                                     
@@ -1021,15 +1067,17 @@
             if self.stream and self.synthesizer_provider != "polly" and not self.is_an_ivr_call: 
                 logger.info("Opening websocket connection to synthesizer")
                 await self.tools["synthesizer"].open_connection()
             while True:
                 logger.info("Listening to synthesizer")
                 async for message in self.tools["synthesizer"].generate():
                     meta_info = message["meta_info"]
-                    if not self.conversation_ended and message["meta_info"]["sequence_id"] in self.sequence_ids:
+                    is_first_message = 'is_first_message' in meta_info and meta_info['is_first_message']
+                    self.__convert_to_request_log(message = meta_info['text'], meta_info= meta_info, component="synthesizer", direction="response", model = self.synthesizer_provider, is_cached= 'is_cached' in meta_info and meta_info['is_cached'], engine=self.tools['synthesizer'].get_engine())
+                    if is_first_message or (not self.conversation_ended and message["meta_info"]["sequence_id"] in self.sequence_ids):
                         logger.info(f"{message['meta_info']['sequence_id'] } is in sequence ids  {self.sequence_ids} and hence removing the sequence ids ")
                         if self.stream:   
                             if self.synthesizer_provider == "polly":
                                 if message['meta_info']['is_first_chunk']:
                                     first_chunk_generation_timestamp = time.time()
                                     meta_info["synthesizer_first_chunk_latency"] = first_chunk_generation_timestamp - message['meta_info']['synthesizer_start_time']
                                 logger.info(f"Simply Storing in buffered output queue for now")
@@ -1049,24 +1097,22 @@
                                     if meta_info.get('format', '') != 'mulaw':
                                         message['data'] = wav_bytes_to_pcm(message['data'])
                                 
                                 if "is_first_chunk" in message['meta_info'] and message['meta_info']['is_first_chunk']:
                                     first_chunk_generation_timestamp = time.time()
                                     meta_info["synthesizer_first_chunk_latency"] = first_chunk_generation_timestamp - message['meta_info']['synthesizer_start_time']
                                     #self.latency_dict[message['meta_info']["request_id"]]['synthesizer'] = {"first_chunk_generation_latency": first_chunk_generation_timestamp - message['meta_info']['synthesizer_start_time'], "first_chunk_generation_timestamp": first_chunk_generation_timestamp}
-                                
                                 if self.yield_chunks:
                                     number_of_chunks = (len(message['data'])/self.output_chunk_size)
                                     i = 0
                                     for chunk in yield_chunks_from_memory(message['data'], chunk_size=self.output_chunk_size):
-                                        i+=1
                                         self.__enqueue_chunk(chunk, i, number_of_chunks, meta_info)
+                                        i+=1
                                 else:
                                     self.buffered_output_queue.put_nowait(message)
-                            
                         else:
                             logger.info("Stream is not enabled and hence sending entire audio")
                             first_chunk_generation_timestamp = time.time()
                             self.latency_dict[message['meta_info']["request_id"]]['synthesizer'] = {"first_chunk_generation_latency": first_chunk_generation_timestamp - message['meta_info']['synthesizer_start_time'], "first_chunk_generation_timestamp": first_chunk_generation_timestamp}
                             #self.history = copy.deepcopy(self.interim_history)
                             logger.info(f"Changing history")
                             await self.tools["output"].handle(message)
@@ -1076,60 +1122,76 @@
                     await asyncio.sleep(0.3) #Sleeping for 100ms after receiving every chunk so other tasks can execute
 
         except Exception as e:
             traceback.print_exc()
             logger.error(f"Error in synthesizer {e}")
 
     async def __send_preprocessed_audio(self, meta_info, text):
-        #TODO: Either load IVR audio into memory before call or user s3 iter_cunks
-        # This will help with interruption in IVR
-        if self.connected_through_dashboard or self.task_config['tools_config']['output'] == "default":
-            audio_chunk = await get_raw_audio_bytes(text, self.assistant_name,
-                                                            self.task_config["tools_config"]["output"][
-                                                                "format"], local=self.is_local,
-                                                            assistant_id=self.assistant_id)
-            logger.info("Sending preprocessed audio")
-            await self.tools["output"].handle(create_ws_data_packet(audio_chunk, meta_info))
-        else:
-            audio_chunk = await get_raw_audio_bytes( text, self.assistant_name,
-                                                            'pcm', local=self.is_local,
-                                                            assistant_id=self.assistant_id)
-            
-            if not self.buffered_output_queue.empty():
-                logger.info(f"Output queue was not empty and hence emptying it")
-                self.buffered_output_queue = asyncio.Queue()
-
-            if self.yield_chunks:
-                for chunk in yield_chunks_from_memory(audio_chunk, chunk_size=self.output_chunk_size):
-                    logger.debug("Sending chunk to output queue")
-                    message = create_ws_data_packet(chunk, meta_info)
-                    self.buffered_output_queue.put_nowait(message)
+        try:
+            #TODO: Either load IVR audio into memory before call or user s3 iter_cunks
+            # This will help with interruption in IVR
+            if self.connected_through_dashboard or self.task_config['tools_config']['output'] == "default":
+                audio_chunk = await get_raw_audio_bytes(text, self.assistant_name,
+                                                                self.task_config["tools_config"]["output"][
+                                                                    "format"], local=self.is_local,
+                                                                assistant_id=self.assistant_id)
+                logger.info("Sending preprocessed audio")
+                await self.tools["output"].handle(create_ws_data_packet(audio_chunk, meta_info))
             else:
-                message = create_ws_data_packet(audio_chunk, meta_info)
-                logger.info(f"Yield in chunks is false and hence sending a full")
-                self.buffered_output_queue.put_nowait(message)
+                audio_chunk = await get_raw_audio_bytes(text, self.assistant_name,
+                                                                'pcm', local=self.is_local,
+                                                                assistant_id=self.assistant_id)
+                if not self.buffered_output_queue.empty():
+                    logger.info(f"Output queue was not empty and hence emptying it")
+                    self.buffered_output_queue = asyncio.Queue()
+
+                if 'is_first_message' in meta_info:
+                    if audio_chunk is None:
+                        logger.info(f"File doesn't exist in S3. Hence we're synthesizing it from synthesizer")
+                        meta_info['cached'] = False
+                        await self._synthesize(create_ws_data_packet(self.kwargs['agent_welcome_message'], meta_info= meta_info))
+                    else:
+                        logger.info(f"Sending the agent welcome message")
+                        for chunk in yield_chunks_from_memory(audio_chunk, chunk_size=self.output_chunk_size):
+                            logger.debug("Sending chunk to output queue")
+                            message = create_ws_data_packet(chunk, meta_info)
+                            self.buffered_output_queue.put_nowait(message)
+
+                elif self.yield_chunks:
+                    for chunk in yield_chunks_from_memory(audio_chunk, chunk_size=self.output_chunk_size):
+                        logger.debug("Sending chunk to output queue")
+                        message = create_ws_data_packet(chunk, meta_info)
+                        self.buffered_output_queue.put_nowait(message)
+                else:
+                    message = create_ws_data_packet(audio_chunk, meta_info)
+                    logger.info(f"Yield in chunks is false and hence sending a full")
+                    self.buffered_output_queue.put_nowait(message)
+        except Exception as e:
+            traceback.print_exc()
+            logger.error(f"Something went wrong {e}")
 
     async def _synthesize(self, message):
         meta_info = message["meta_info"]
         text = message["data"]
         meta_info["type"] = "audio"
         meta_info["synthesizer_start_time"] = time.time()
         try:
-            if not self.conversation_ended and message["meta_info"]["sequence_id"] in self.sequence_ids:
+            if not self.conversation_ended and ('is_first_message' in meta_info and meta_info['is_first_message'] or message["meta_info"]["sequence_id"] in self.sequence_ids):
                 if meta_info["is_md5_hash"]:
                     logger.info('sending preprocessed audio response to {}'.format(self.task_config["tools_config"]["output"]["provider"]))
                     await self.__send_preprocessed_audio(meta_info, text)
                     
                 elif self.synthesizer_provider in SUPPORTED_SYNTHESIZER_MODELS.keys():
                     # self.sequence_ids.add(meta_info["sequence_id"])
                     # logger.info(f"After adding into sequence id {self.sequence_ids}")
-                    self.__convert_to_request_log(message = text, meta_info= meta_info, component="synthesizer", direction="request", model = self.synthesizer_provider)
+                    self.__convert_to_request_log(message = text, meta_info= meta_info, component="synthesizer", direction="request", model = self.synthesizer_provider, engine=self.tools['synthesizer'].get_engine())
                     logger.info('##### sending text to {} for generation: {} '.format(self.synthesizer_provider, text))
-                    if 'cached' in message['meta_info'] and meta_info['cached'] == True:
+                    if 'cached' in message['meta_info'] and meta_info['cached'] is True:
                         logger.info(f"Cached response and hence sending preprocessed text")
+                        self.__convert_to_request_log(message = text, meta_info= meta_info, component="synthesizer", direction="response", model = self.synthesizer_provider, is_cached= True, engine=self.tools['synthesizer'].get_engine())
                         await self.__send_preprocessed_audio(meta_info, get_md5_hash(text))
                     else:
                         self.synthesizer_characters += len(text)
                         await self.tools["synthesizer"].push(message)
                 else:
                     logger.info("other synthesizer models not supported yet")
             else:
@@ -1138,17 +1200,18 @@
         except Exception as e:
             traceback.print_exc()
             logger.error(f"Error in synthesizer: {e}")
 
     ############################################################
     # Output handling
     ############################################################
-    async def __handle_initial_silence(self):
-        logger.info(f"Checking for initial silence")
-        await asyncio.sleep(5)
+    async def __handle_initial_silence(self, duration = 5):
+        logger.info(f"Checking for initial silence {duration}")
+        await asyncio.sleep(duration)
+        logger.info(f"Woke up from my slumber {self.callee_silent}, {self.history}, {self.interim_history}")
         if self.callee_silent and len(self.history) == 1 and len(self.interim_history) == 1:
             logger.info(f"Calee was silent and hence speaking Hello on callee's behalf")
             meta_info = self.__get_updated_meta_info()
             sequence = meta_info["sequence"]
             next_task = self._get_next_step(sequence, "transcriber")
             await self._handle_transcriber_output(next_task, "Hello", meta_info)
             self.time_since_first_interim_result = (time.time() * 1000) - 1000
@@ -1187,15 +1250,15 @@
                     logger.info(f'prev message is not none and hence getting prev message')
                     message = prev_message
                     prev_message = None
                 logger.info("##### Start response is True and hence starting to speak {} Current sequence ids".format(message['meta_info'], self.sequence_ids))
                 if "end_of_conversation" in message['meta_info']:
                     await self.__process_end_of_conversation()
                 
-                if 'sequence_id' in message['meta_info'] and message["meta_info"]["sequence_id"] in self.sequence_ids:
+                if ('is_first_message' in message['meta_info'] and message['meta_info']['is_first_message']) or ( 'sequence_id' in message['meta_info'] and message["meta_info"]["sequence_id"] in self.sequence_ids):
                     await self.tools["output"].handle(message)                    
                     duration = calculate_audio_duration(len(message["data"]), self.sampling_rate)
                     logger.info(f"Duration of the byte {duration}")
                     self.conversation_recording['output'].append({'data': message['data'], "start_time": time.time(), "duration": duration})
                 else:
                     logger.info(f'{message["meta_info"]["sequence_id"]} is not in {self.sequence_ids} and hence not speaking')
                     continue
@@ -1238,83 +1301,112 @@
                         logger.info("LATENCY METRICS FOR {} are {}".format(message['meta_info']["request_id"], latency_metrics))
                     
                     await asyncio.sleep(duration + 0.1) 
                 else:
                     # Sleep until this particular audio frame is spoken only if the duration for the frame is atleast 500ms
                     if duration > 0:
                         logger.info(f"##### Sleeping for {duration} to maintain quueue on our side {self.sampling_rate}")
-                        await asyncio.sleep(duration - 0.010) #10 milliseconds less
+                        await asyncio.sleep(duration - 0.030) #30 milliseconds less
                         
 
                     
                 self.last_transmitted_timesatamp = time.time()
                 logger.info(f"##### Updating Last transmitted timestamp to {self.last_transmitted_timesatamp}")
                 
         except Exception as e:
             traceback.print_exc()
             logger.error(f'Error in processing message output')
 
+    
     async def __check_for_completion(self):
         while True:
             await asyncio.sleep(2)
-
             if self.last_transmitted_timesatamp == 0:
                 logger.info(f"Last transmitted timestamp is simply 0 and hence continuing")
                 continue
 
             time_since_last_spoken_AI_word = (time.time() - self.last_transmitted_timesatamp) 
             if time_since_last_spoken_AI_word > self.hang_conversation_after and self.time_since_last_spoken_human_word < self.last_transmitted_timesatamp:
                 logger.info(f"{time_since_last_spoken_AI_word} seconds since last spoken time stamp and hence cutting the phone call and last transmitted timestampt ws {self.last_transmitted_timesatamp} and time since last spoken human word {self.time_since_last_spoken_human_word}")
                 await self.__process_end_of_conversation()
                 break
             else:
-                logger.info(f"Only {time_since_last_spoken_AI_word} seconds since last spoken time stamp and hence cutting the phone call and hence not cutting the phone call")
+                logger.info(f"Only {time_since_last_spoken_AI_word} seconds since last spoken time stamp and hence not cutting the phone call")
     
     async def __check_for_backchanneling(self):
         while True:
             if self.callee_speaking and time.time() - self.callee_speaking_start_time > self.backchanneling_start_delay:
                 filename = random.choice(self.filenames)
                 logger.info(f"Should send a random backchanneling words and sending them {filename}")
                 audio = await get_raw_audio_bytes(f"{self.backchanneling_audios}/{filename}", local= True, is_location=True)
                 if not self.connected_through_dashboard and self.task_config['tools_config']['output'] != "default":
                     audio = resample(audio, target_sample_rate= 8000, format="wav")
                 await self.tools["output"].handle(create_ws_data_packet(audio, self.__get_updated_meta_info())) 
             else:
                 logger.info(f"Callee isn't speaking and hence not sending or {time.time() - self.callee_speaking_start_time} is not greater than {self.backchanneling_start_delay}") 
             await asyncio.sleep(self.backchanneling_message_gap) 
+    
+    async def __first_message(self):
+        logger.info(f"Executing the first message task")
+        try:
+            while True:
+                if not self.stream_sid and not self.default_io:
+                    stream_sid = self.tools["input"].get_stream_sid()
+                    if stream_sid is not None:
+                        logger.info(f"Got stream sid and hence sending the first message {stream_sid}")
+                        self.stream_sid = stream_sid
+                        logger.info(f"Generating {self.kwargs.get('agent_welcome_message', None)}")
+                        meta_info={'io': 'twilio', 'is_first_message': True, 'stream_sid': stream_sid, "request_id": str(uuid.uuid4()), "cached": True, "sequence_id": -1, 'format': 'pcm'}
+                        await self._synthesize(create_ws_data_packet(self.kwargs.get('agent_welcome_message', None), meta_info= meta_info))
+                        break
+                    else:
+                        logger.info(f"Stream id is still None, so not passing it")
+                        await asyncio.sleep(0.5) #Sleep for half a second to see if stream id goes past None 
+                elif self.default_io:
+                    logger.info(f"Shouldn't record")
+                    # meta_info={'io': 'default', 'is_first_message': True, "request_id": str(uuid.uuid4()), "cached": True, "sequence_id": -1, 'format': 'wav'}
+                    # await self._synthesize(create_ws_data_packet(self.kwargs['agent_welcome_message'], meta_info= meta_info))
+                    break
+
+        except Exception as e:
+            logger.error(f"Error happeneed {e}")
+
     async def run(self):
         try:
             if self.task_id == 0:
                 # Create transcriber and synthesizer tasks
-                logger.info("starting task_id {}".format(self.task_id))
+                logger.info("starting task_id {}".format(self.task_id))                
                 tasks = [asyncio.create_task(self.tools['input'].handle())]
                 if not self.connected_through_dashboard:
-                    self.background_check_task = asyncio.create_task(self.__handle_initial_silence())
+                    self.background_check_task = asyncio.create_task(self.__handle_initial_silence(duration = 15))
                 if "transcriber" in self.tools:
                     tasks.append(asyncio.create_task(self._listen_transcriber()))
                     self.transcriber_task = asyncio.create_task(self.tools["transcriber"].run())
 
-                if self.connected_through_dashboard and self.task_config['task_type'] == "conversation":
+                if self.connected_through_dashboard and self._is_conversation_task():
                     logger.info(
                         "Since it's connected through dashboard, I'll run listen_llm_tas too in case user wants to simply text")
                     self.llm_queue_task = asyncio.create_task(self._listen_llm_input_queue())
                 
                 if "synthesizer" in self.tools and self._is_conversation_task():
                     logger.info("Starting synthesizer task")
                     try:
                         self.synthesizer_task = asyncio.create_task(self.__listen_synthesizer())
                     except asyncio.CancelledError as e:
                         logger.error(f'Synth task got cancelled {e}')
                         traceback.print_exc()
                 if self._is_conversation_task():
+                    logger.info("Starting the first message task")
                     self.output_task = asyncio.create_task(self.__process_output_loop())
-                    if not self.use_llm_to_determine_hangup and not self.connected_through_dashboard :
-                        self.hangup_task = asyncio.create_task(self.__check_for_completion())
-                    if not self.connected_through_dashboard and self.should_backchannel:
-                        self.backchanneling_task = asyncio.create_task(self.__check_for_backchanneling())
+                    if not self.connected_through_dashboard:
+                        self.first_message_task = asyncio.create_task(self.__first_message())
+                        if not self.use_llm_to_determine_hangup :
+                            self.hangup_task = asyncio.create_task(self.__check_for_completion())
+                        if self.should_backchannel:
+                            self.backchanneling_task = asyncio.create_task(self.__check_for_backchanneling())
                 try:
                     await asyncio.gather(*tasks)
                 except asyncio.CancelledError as e:
                     logger.error(f'task got cancelled {e}')
                     traceback.print_exc()
                 except Exception as e:
                     traceback.print_exc()
@@ -1343,15 +1435,16 @@
             self.handle_cancellation(f"Exception occurred {e}")
             raise Exception(e)
 
         finally:
             # Construct output
             if "synthesizer" in self.tools and self.synthesizer_task is not None:   
                 self.synthesizer_task.cancel()
-            if self.use_llm_to_determine_hangup is False and self._is_conversation_task() and not self.connected_through_dashboard:
+
+            if self._is_conversation_task() and self.use_llm_to_determine_hangup is False and not self.connected_through_dashboard:
                 self.hangup_task.cancel()
             
             if self._is_conversation_task():
                 self.output_task.cancel()
             
             if self._is_conversation_task() and self.backchanneling_task is not None:
                 self.backchanneling_task.cancel()
@@ -1386,8 +1479,8 @@
             logger.info(f"tasks {len(tasks)}")
             for task in tasks:
                 logger.info(f"Cancelling task {task.get_name()}")
                 task.cancel()
             logger.info(message)
         except Exception as e:
             traceback.print_exc()
-            logger.info(e)
+            logger.info(e)
```

### Comparing `bolna-0.7.7/bolna/agent_types/contextual_conversational_agent.py` & `bolna-0.7.8/bolna/agent_types/contextual_conversational_agent.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.7/bolna/agent_types/extraction_agent.py` & `bolna-0.7.8/bolna/agent_types/extraction_agent.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.7/bolna/agent_types/graph_based_conversational_agent.py` & `bolna-0.7.8/bolna/agent_types/graph_based_conversational_agent.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.7/bolna/agent_types/summarization_agent.py` & `bolna-0.7.8/bolna/agent_types/summarization_agent.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.7/bolna/agent_types/zapier_agent.py` & `bolna-0.7.8/bolna/agent_types/webhook_agent.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 import aiohttp
 from .base_agent import BaseAgent
 from bolna.helpers.logger_config import configure_logger
 
 logger = configure_logger(__name__)
 
 
-class ZapierAgent(BaseAgent):
-    def __init__(self, zap_url, payload=None):
+class WebhookAgent(BaseAgent):
+    def __init__(self, webhook_url, payload=None):
         super().__init__()
-        self.zap_url = zap_url
+        self.webhook_url = webhook_url
         self.payload = payload or {}
 
     async def __send_payload(self, payload):
         try:
-            logger.info(f"Sending a zapier post request {payload}")
+            logger.info(f"Sending a webhook post request {payload}")
             async with aiohttp.ClientSession() as session:
                 if payload is not None:
-                    async with session.post(self.zap_url, json=payload) as response:
+                    async with session.post(self.webhook_url, json=payload) as response:
                         if response.status == 200:
                             # need to check if the returned response is json or not
                             #data = await response.json()
                             return True
                         else:
                             logger.error(f"Error: {response.status} - {await response.text()}")
                             return None
                 else:
                     logger.info("Payload was null")
             return None
         except Exception as e:
-            logger.error(f"Something went wrong with webhook {self.zap_url}, {payload}")
-
+            logger.error(f"Something went wrong with webhook {self.webhook_url}, {payload}")
 
     async def execute(self, payload):
-        if not self.zap_url:
+        if not self.webhook_url:
             return None
         response = await self.__send_payload(payload)
         logger.info(f"Response {response}")
         return response
```

### Comparing `bolna-0.7.7/bolna/assistant.py` & `bolna-0.7.8/bolna/assistant.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.7/bolna/helpers/analytics_helpers.py` & `bolna-0.7.8/bolna/helpers/analytics_helpers.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.7/bolna/helpers/logger_config.py` & `bolna-0.7.8/bolna/helpers/logger_config.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.7/bolna/helpers/utils.py` & `bolna-0.7.8/bolna/helpers/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,17 +185,20 @@
     # we are already storing pcm formatted audio in the filler config. No need to encode/decode them further
     audio_data = None
     if local:
         if not is_location:
             file_name = f"{PREPROCESS_DIR}/{agent_name}/{audio_format}/{filename}.{audio_format}"
         else:
             file_name = filename
-        with open(file_name, 'rb') as file:
-            # Read the entire file content into a variable
-            audio_data = file.read()
+        if os.path.isfile(file_name):
+            with open(file_name, 'rb') as file:
+                # Read the entire file content into a variable
+                audio_data = file.read()
+        else:
+            audio_data = None
     else:
         if not is_location:
             object_key = f"{assistant_id}/audio/{filename}.{audio_format}"
         else:
             object_key = filename
             
         logger.info(f"Reading {object_key}")
@@ -401,39 +404,45 @@
 2. Request/Response
 3. conversation_leg_id
 4. data
 5. num_input_tokens
 6. num_output_tokens 
 7. num_characters 
 8. is_final
+9. engine
 '''
+
 async def write_request_logs(message, run_id):
     component_details = [None, None, None, None, None]
     logger.info(f"Message {message}")
+    message_data = message.get('data', '')
+    if message_data is None:
+        message_data = ''
+
     row = [message['time'], message["component"], message["direction"], message["leg_id"], message['sequence_id'], message['model']]
     if message["component"] == "llm":
-        component_details = [message['data'], message.get('input_tokens', 0), message.get('output_tokens', 0), None, None]
+        component_details = [message_data, message.get('input_tokens', 0), message.get('output_tokens', 0), None, message['cached'], None]
     elif message["component"] == "transcriber":
-        component_details = [message['data'], None, None, None, message.get('is_final', False)]
+        component_details = [message_data, None, None, None, False ,message.get('is_final', False)]
     elif message["component"] == "synthesizer":
-        component_details = [message['data'], None, None, len(message['data']), None]
-    
+        component_details = [message_data, None, None, len(message_data), message['cached'], None, message['engine']]
+
     row = row + component_details
-    
-    header = "Time,Component,Direction,Leg ID,Sequence ID,Model,Data,Input Tokens,Output Tokens,Characters,Final Transcript\n"
-    log_string = ','.join(['"' + str(item).replace('"', '""') + '"' if item is not None else '' for item in row]) + '\n'    
+
+    header = "Time,Component,Direction,Leg ID,Sequence ID,Model,Data,Input Tokens,Output Tokens,Characters,Cached,Final Transcript,Engine\n"
+    log_string = ','.join(['"' + str(item).replace('"', '""') + '"' if item is not None else '' for item in row]) + '\n'
     log_dir = f"./logs/{run_id.split('#')[0]}"
-    os.makedirs(log_dir, exist_ok=True) 
+    os.makedirs(log_dir, exist_ok=True)
     log_file_path = f"{log_dir}/{run_id.split('#')[1]}.csv"
     file_exists = os.path.exists(log_file_path)
-    
+
     async with aiofiles.open(log_file_path, mode='a') as log_file:
         if not file_exists:
             await log_file.write(header+log_string)
-        else:    
+        else:
             await log_file.write(log_string)
 
 async def save_audio_file_to_s3(conversation_recording, sampling_rate = 24000, assistant_id = None, run_id = None):
     last_frame_end_time = conversation_recording['output'][0]['start_time']
     logger.info(f"LENGTH OF OUTPUT AUDIO {len(conversation_recording['output'])}")
     initial_gap = (last_frame_end_time - conversation_recording["metadata"]["started"] ) *1000
     logger.info(f"Initial gap {initial_gap}")
```

### Comparing `bolna-0.7.7/bolna/helpers/vad.py` & `bolna-0.7.8/bolna/helpers/vad.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.7/bolna/input_handlers/default.py` & `bolna-0.7.8/bolna/input_handlers/default.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.7/bolna/input_handlers/telephony.py` & `bolna-0.7.8/bolna/input_handlers/telephony.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,18 @@
         self.stream_sid = None
         self.call_sid = None
         self.buffer = []
         self.message_count = 0
         self.mark_set = mark_set
         self.last_media_received = 0
         self.io_provider = None
-
+    
+    def get_stream_sid(self):
+        return self.stream_sid
+    
     async def call_start(self, packet):
         pass
 
     async def process_mark_message(self, packet):
         if packet["mark"]["name"] in self.mark_set:
             self.mark_set.remove(packet["mark"]["name"])
```

### Comparing `bolna-0.7.7/bolna/input_handlers/telephony_providers/exotel.py` & `bolna-0.7.8/bolna/input_handlers/telephony_providers/exotel.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.7/bolna/input_handlers/telephony_providers/twilio.py` & `bolna-0.7.8/bolna/input_handlers/telephony_providers/twilio.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.7/bolna/llms/litellm.py` & `bolna-0.7.8/bolna/llms/litellm.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,24 +23,24 @@
         if self.api_key:
             self.model_args["api_key"] = self.api_key
         if self.api_base:
             self.model_args["api_base"] = self.api_base
         if self.api_version:
             self.model_args["api_version"] = self.api_version
 
-        if "top_k" in kwargs:
-            self.model_args["top_k"] = kwargs["top_k"]
-        if "top_p" in kwargs:
-            self.model_args["top_p"] = kwargs["top_p"]
-        if "stop" in kwargs:
-            self.model_args["stop"] = kwargs["stop"]
-        if "presence_penalty" in kwargs:
-            self.model_args["presence_penalty"] = kwargs["presence_penalty"]
-        if "frequency_penalty" in kwargs:
-            self.model_args["frequency_penalty"] = kwargs["frequency_penalty"]
+        # if "top_k" in kwargs:
+        #     self.model_args["top_k"] = kwargs["top_k"]
+        # if "top_p" in kwargs:
+        #     self.model_args["top_p"] = kwargs["top_p"]
+        # if "stop" in kwargs:
+        #     self.model_args["stop"] = kwargs["stop"]
+        # if "presence_penalty" in kwargs:
+        #     self.model_args["presence_penalty"] = kwargs["presence_penalty"]
+        # if "frequency_penalty" in kwargs:
+        #     self.model_args["frequency_penalty"] = kwargs["frequency_penalty"]
 
         if len(kwargs) != 0:
             if "base_url" in kwargs:
                 self.model_args["api_base"] = kwargs["base_url"]
             if "llm_key" in kwargs:
                 self.model_args["api_key"] = kwargs["llm_key"]
             if "api_version" in kwargs:
@@ -48,15 +48,15 @@
 
     async def generate_stream(self, messages, synthesize=True):
         answer, buffer = "", ""
         model_args = self.model_args.copy()
         model_args["messages"] = messages
         model_args["stream"] = True
 
-        logger.info(f"request to model: {self.model}: {messages}")
+        logger.info(f"request to model: {self.model}: {messages} and model args {model_args}")
         start_time = time.time()
         async for chunk in await litellm.acompletion(**model_args):
             if (text_chunk := chunk['choices'][0]['delta'].content) and not chunk['choices'][0].finish_reason:
                 answer += text_chunk
                 buffer += text_chunk
 
                 if len(buffer) >= self.buffer_size and synthesize:
@@ -70,15 +70,15 @@
 
         if synthesize:
             if buffer != "":
                 yield buffer, True
         else:
             yield answer, True
         self.started_streaming = False
-        logger.info(f"Time to generate response {time.time() - start_time}")
+        logger.info(f"Time to generate response {time.time() - start_time} {answer}")
 
     async def generate(self, messages, stream=False, request_json=False):
         text = ""
         model_args = self.model_args.copy()
         model_args["model"] = self.model
         model_args["messages"] = messages
         model_args["stream"] = stream
```

### Comparing `bolna-0.7.7/bolna/llms/openai_llm.py` & `bolna-0.7.8/bolna/llms/openai_llm.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,47 +15,29 @@
         self.model = model
         self.started_streaming = False
         logger.info(f"Initializing OpenAI LLM with model: {self.model} and maxc tokens {max_tokens}")
         self.max_tokens = max_tokens
         self.temperature = temperature
         self.vllm_model = "vllm" in self.model
         self.model_args = { "max_tokens": self.max_tokens, "temperature": self.temperature, "model": self.model}
-
-        if self.vllm_model:
-            base_url = kwargs.get("base_url", None)
-            if base_url is None:
-                raise Exception("Cannot run a custom LLM without base URL")
+        if model == "Krutrim-spectre-v2":
+            logger.info(f"Connecting to Ola's krutrim model")
+            base_url = kwargs.get("base_url", os.getenv("OLA_KRUTRIM_BASE_URL"))
             api_key=kwargs.get('llm_key', None)
             if api_key is not None and len(api_key) > 0:
                 api_key = api_key
-            else:
-                api_key = "EMPTY"
             self.async_client = AsyncOpenAI( base_url=base_url, api_key= api_key)
-            self.model = self.model[5:]
-            self.model_args["model"] = self.model
-            if "top_k" in kwargs:
-                self.model_args["top_k"] = kwargs["top_k"]
-            logger.info(f"Using VLLM model base_url {base_url} and model {self.model} and api key {api_key}")
         else:
             llm_key = kwargs.get('llm_key', os.getenv('OPENAI_API_KEY'))
             if llm_key != "sk-":
                 llm_key = os.getenv('OPENAI_API_KEY')
             else:
                 llm_key = kwargs['llm_key']
             self.async_client = AsyncOpenAI(api_key=llm_key)
-        
-        if "top_p" in kwargs:
-            self.model_args["top_p"] = kwargs["top_p"]
-        if "stop" in kwargs:
-            self.model_args["stop"] = kwargs["stop"]        
-        if "presence_penalty" in kwargs:
-            self.model_args["presence_penalty"] = kwargs["presence_penalty"]
-        if  "frequency_penalty" in kwargs:
-            self.model_args["frequency_penalty"] = kwargs["frequency_penalty"]
-
+            
     async def generate_stream(self, messages, synthesize=True, request_json=False):
         if len(messages) == 0:
             raise Exception("No messages provided")
         
         response_format = self.get_response_format(request_json)
 
         answer, buffer = "", ""
```

### Comparing `bolna-0.7.7/bolna/memory/cache/inmemory_scalar_cache.py` & `bolna-0.7.8/bolna/memory/cache/inmemory_scalar_cache.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.7/bolna/memory/cache/vector_cache.py` & `bolna-0.7.8/bolna/memory/cache/vector_cache.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.7/bolna/models.py` & `bolna-0.7.8/bolna/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import json
 from typing import Optional, List, Union, Dict
 from pydantic import BaseModel, Field, validator, ValidationError, Json
 from .providers import *
 
+AGENT_WELCOME_MESSAGE = "This call is being recorded for quality assurance and training. Please speak now."
+
 
 def validate_attribute(value, allowed_values):
     if value not in allowed_values:
         raise ValidationError(f"Invalid provider. Supported values: {', '.join(allowed_values)}")
     return value
 
 
@@ -66,40 +68,45 @@
 
 class Synthesizer(BaseModel):
     provider: str
     provider_config: Union[PollyConfig, XTTSConfig, ElevenLabsConfig, OpenAIConfig, FourieConfig, DeepgramConfig]
     stream: bool = False
     buffer_size: Optional[int] = 40  # 40 characters in a buffer
     audio_format: Optional[str] = "pcm"
+    caching: Optional[bool] = True
 
     @validator("provider")
     def validate_model(cls, value):
         return validate_attribute(value, ["polly", "xtts", "elevenlabs", "openai", "deepgram"])
 
 
 class IOModel(BaseModel):
     provider: str
     format: str
 
     @validator("provider")
     def validate_provider(cls, value):
         return validate_attribute(value, ["twilio", "default", "database", "exotel"])
 
+
 # Can be used to route across multiple prompts as well
 class Route(BaseModel):
     route_name: str
     utterances: List[str]
-    response: Union[List[str], str] #If length of responses is less than utterances, a random sentence will be used as a response and if it's equal, respective index will be used to use it as FAQs caching
-    score_threshold: Optional[float] = 0.85 # this is the required threshold for cosine similarity 
+    response: Union[List[
+        str], str]  # If length of responses is less than utterances, a random sentence will be used as a response and if it's equal, respective index will be used to use it as FAQs caching
+    score_threshold: Optional[float] = 0.85  # this is the required threshold for cosine similarity
+
 
 # Routes can be used for FAQs caching, prompt routing, guard rails, agent assist function calling
 class Routes(BaseModel):
     embedding_model: Optional[str] = "Snowflake/snowflake-arctic-embed-l"
     routes: List[Route]
 
+
 class LLM(BaseModel):
     model: Optional[str] = "gpt-3.5-turbo-16k"
     max_tokens: Optional[int] = 100
     agent_flow_type: Optional[str] = "streaming"
     family: Optional[str] = "openai"
     temperature: Optional[float] = 0.1
     request_json: Optional[bool] = False
@@ -108,14 +115,17 @@
     top_p: Optional[float] = 0.9
     min_p: Optional[float] = 0.1
     frequency_penalty: Optional[float] = 0.0
     presence_penalty: Optional[float] = 0.0
     provider: Optional[str] = "openai"
     base_url: Optional[str] = None
     routes: Optional[Routes] = None
+    extraction_details: Optional[str] = None
+    summarization_details: Optional[str] = None
+
 
 class MessagingModel(BaseModel):
     provider: str
     template: str
 
 
 # Need to redefine it
@@ -144,18 +154,33 @@
 
 
 class ToolsChainModel(BaseModel):
     execution: str = Field(..., pattern="^(parallel|sequential)$")
     pipelines: List[List[str]]
 
 
+class ConversationConfig(BaseModel):
+    optimize_latency: Optional[bool] = True  # This will work on in conversation
+    hangup_after_silence: Optional[int] = 10
+    incremental_delay: Optional[int] = 100  # use this to incrementally delay to handle long pauses
+    number_of_words_for_interruption: Optional[
+        int] = 1  # Maybe send half second of empty noise if needed for a while as soon as we get speaking true in nitro, use that to delay
+    interruption_backoff_period: Optional[int] = 100
+    hangup_after_LLMCall: Optional[bool] = False
+    call_cancellation_prompt: Optional[str] = None
+    backchanneling: Optional[bool] = False
+    backchanneling_message_gap: Optional[int] = 5
+    backchanneling_start_delay: Optional[int] = 5
+
+
 class Task(BaseModel):
     tools_config: ToolsConfig
     toolchain: ToolsChainModel
     task_type: Optional[str] = "conversation"  # extraction, summarization, notification
+    task_config: ConversationConfig = dict()
 
 
 class AgentModel(BaseModel):
     agent_name: str
     agent_type: str = "other"
     tasks: List[Task]
- # Usually of the format task_1: { "system_prompt" : "helpful agent" } #For IVR type it should be a basic graph
+    agent_welcome_message: Optional[str] = AGENT_WELCOME_MESSAGE
```

### Comparing `bolna-0.7.7/bolna/output_handlers/default.py` & `bolna-0.7.8/bolna/output_handlers/default.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.7/bolna/output_handlers/telephony.py` & `bolna-0.7.8/bolna/output_handlers/telephony.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,30 +29,36 @@
     async def form_mark_message(self, mark_id):
         pass
 
     async def handle(self, ws_data_packet):
         try:
             audio_chunk = ws_data_packet.get('data')
             meta_info = ws_data_packet.get('meta_info')
-            self.stream_sid = meta_info.get('stream_sid', None)
-
+            if self.stream_sid is None:
+                self.stream_sid = meta_info.get('stream_sid', None)
+            logger.info(f"Sending Message {self.current_request_id} and {self.stream_sid} and  {meta_info}")
             try:
                 if self.current_request_id == meta_info['request_id']:
                     if len(audio_chunk) == 1:
                         audio_chunk += b'\x00'
 
                 if audio_chunk and self.stream_sid and len(audio_chunk) != 1:
+                    
                     audio_format = meta_info.get("format", "wav")
+                    logger.info(f"Sending message {len(audio_chunk)} {audio_format}")
                     media_message = await self.form_media_message(audio_chunk, audio_format)
+                    logger.info(f"Got media message {media_message['streamSid']}")
                     await self.websocket.send_text(json.dumps(media_message))
 
                     mark_id = str(uuid.uuid4())
                     self.mark_set.add(mark_id)
 
                     mark_message = await self.form_mark_message(mark_id)
                     await self.websocket.send_text(json.dumps(mark_message))
+                else:
+                    logger.info("Not sending")
             except Exception as e:
                 traceback.print_exc()
                 logger.error(f'something went wrong while sending message to twilio {e}')
 
         except Exception as e:
             logger.error(f'something went wrong while handling twilio {e}')
```

### Comparing `bolna-0.7.7/bolna/output_handlers/telephony_providers/exotel.py` & `bolna-0.7.8/bolna/output_handlers/telephony_providers/exotel.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.7/bolna/output_handlers/telephony_providers/twilio.py` & `bolna-0.7.8/bolna/output_handlers/telephony_providers/twilio.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.7/bolna/prompts.py` & `bolna-0.7.8/bolna/prompts.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.7/bolna/providers.py` & `bolna-0.7.8/bolna/providers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 from .synthesizer import PollySynthesizer, XTTSSynthesizer, ElevenlabsSynthesizer, OPENAISynthesizer, FourieSynthesizer, DeepgramSynthesizer
-from .transcriber import DeepgramTranscriber
+from .transcriber import DeepgramTranscriber, WhisperTranscriber
 from .input_handlers import DefaultInputHandler, TwilioInputHandler, ExotelInputHandler
 from .output_handlers import DefaultOutputHandler, TwilioOutputHandler, ExotelOutputHandler
 from .llms import OpenAiLLM, LiteLLM
 
 SUPPORTED_SYNTHESIZER_MODELS = {
     'polly': PollySynthesizer,
     'xtts': XTTSSynthesizer,
     'elevenlabs': ElevenlabsSynthesizer,
     'openai': OPENAISynthesizer,
     'fourie': FourieSynthesizer,
     'deepgram': DeepgramSynthesizer
 }
 SUPPORTED_TRANSCRIBER_MODELS = {
     'deepgram': DeepgramTranscriber,
-    'whisper': DeepgramTranscriber #Seperate out a transcriber for https://github.com/bolna-ai/streaming-transcriber-server or build a deepgram compatible proxy
+    'whisper': WhisperTranscriber #Seperate out a transcriber for https://github.com/bolna-ai/streaming-transcriber-server or build a deepgram compatible proxy
 }
 
 SUPPORTED_LLM_PROVIDERS = {
     'openai': OpenAiLLM,
     'cohere': LiteLLM,
     'ollama': LiteLLM,
     'deepinfra': LiteLLM,
     'together': LiteLLM,
     'fireworks': LiteLLM,
     'azure-openai': LiteLLM,
     'perplexity': LiteLLM,
     'vllm': OpenAiLLM,
     'anyscale': LiteLLM,
-    'custom': OpenAiLLM
+    'custom': OpenAiLLM,
+    'ola': OpenAiLLM
 }
 SUPPORTED_INPUT_HANDLERS = {
     'default': DefaultInputHandler,
     'twilio': TwilioInputHandler,
     'exotel': ExotelInputHandler
 }
 SUPPORTED_INPUT_TELEPHONY_HANDLERS = {
```

### Comparing `bolna-0.7.7/bolna/synthesizer/base_synthesizer.py` & `bolna-0.7.8/bolna/synthesizer/base_synthesizer.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,17 +21,23 @@
 
     def push(self, text):
         pass
     
     def synthesize(self, text):
         pass
 
+    def get_synthesized_characters(self):
+        return 0
+
     def resample(self, audio_bytes):
         audio_buffer = io.BytesIO(audio_bytes)
         waveform, orig_sample_rate = torchaudio.load(audio_buffer)
         resampler = torchaudio.transforms.Resample(orig_sample_rate, 8000)
         audio_waveform = resampler(waveform)
         audio_buffer = io.BytesIO()
         torchaudio.save(audio_buffer, audio_waveform, 8000, format="wav")
         audio_buffer.seek(0)
         audio_data = audio_buffer.read()
         return audio_data
+
+    def get_engine(self):
+        return "default"
```

### Comparing `bolna-0.7.7/bolna/synthesizer/deepgram_synthesizer.py` & `bolna-0.7.8/bolna/synthesizer/deepgram_synthesizer.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.7/bolna/synthesizer/elevenlabs_synthesizer.py` & `bolna-0.7.8/bolna/synthesizer/elevenlabs_synthesizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 import websockets
 import base64
 import json
 import aiohttp
 import os
 import traceback
 from collections import deque
+
+from bolna.memory.cache.inmemory_scalar_cache import InmemoryScalarCache
 from .base_synthesizer import BaseSynthesizer
 from bolna.helpers.logger_config import configure_logger
 from bolna.helpers.utils import convert_audio_to_wav, create_ws_data_packet, pcm_to_wav_bytes, resample
 
 
 logger = configure_logger(__name__)
 
 
 class ElevenlabsSynthesizer(BaseSynthesizer):
     def __init__(self, voice, voice_id, model="eleven_multilingual_v1", audio_format="mp3", sampling_rate="16000",
                  stream=False, buffer_size=400, temperature = 0.5, similarity_boost = 0.5, synthesier_key=None, 
-                 cache=None, **kwargs):
+                 caching=True, **kwargs):
         super().__init__(stream)
         self.api_key = os.environ["ELEVENLABS_API_KEY"] if synthesier_key is None else synthesier_key
         self.voice = voice_id
         self.use_turbo = kwargs.get("use_turbo", False)
         self.model = "eleven_turbo_v2" if self.use_turbo else "eleven_multilingual_v2"
         logger.info(f"Using turbo or not {self.model}")
         self.stream = False  # Issue with elevenlabs streaming that we need to always send the text quickly
@@ -35,26 +37,31 @@
         self.api_url = f"https://api.elevenlabs.io/v1/text-to-speech/{self.voice}?optimize_streaming_latency=2&output_format="
         self.first_chunk_generated = False
         self.last_text_sent = False
         self.text_queue = deque()
         self.meta_info = None
         self.temperature = temperature
         self.similarity_boost = similarity_boost
-        self.cache = cache
+        self.caching = caching
+        if self.caching:
+            self.cache = InmemoryScalarCache()
         self.synthesized_characters = 0
 
     # Ensuring we only do wav output for now
     def get_format(self, format, sampling_rate):
         # Eleven labs only allow mp3_44100_64, mp3_44100_96, mp3_44100_128, mp3_44100_192, pcm_16000, pcm_22050,
         # pcm_24000, ulaw_8000
         if self.use_mulaw:
             return "ulaw_8000"
         return f"mp3_44100_128"
 
-    # Don't send EOS signal. Let        
+    def get_engine(self):
+        return self.model
+
+    # Don't send EOS signal. Let
     async def sender(self, text, end_of_llm_stream=False):  # sends text to websocket
         if self.websocket_connection is not None and not self.websocket_connection.open:
             self.connection_open = False
             logger.info(f"Connection was closed and hence opening connection")
             await self.open_connection()
 
         if not self.connection_open:
@@ -182,23 +189,29 @@
                         self.first_chunk_generated = False
 
             else:
                 while True:
                     message = await self.internal_queue.get()
                     logger.info(f"Generating TTS response for message: {message}")
                     meta_info, text = message.get("meta_info"), message.get("data")
-                    if self.cache.get(text):
-                        logger.info(f"Cache hit and hence returning quickly {text}")
-                        message = self.cache.get(text)
+                    if self.caching:
+                        if self.cache.get(text):
+                            logger.info(f"Cache hit and hence returning quickly {text}")
+                            message = self.cache.get(text)
+                            meta_info['is_cached'] = True
+                        else:
+                            c = len(text)
+                            self.synthesized_characters += c
+                            logger.info(f"Not a cache hit {list(self.cache.data_dict)} and hence increasing characters by {c}")
+                            meta_info['is_cached'] = False
+                            audio = await self.__generate_http(text)
+                            self.cache.set(text, audio)
                     else:
-                        c = len(text)
-                        self.synthesized_characters += c
-                        logger.info(f"Not a cache hit {list(self.cache.data_dict)} and hence increasing characters by {c}")
+                        meta_info['is_cached'] = False
                         audio = await self.__generate_http(text)
-                        self.cache.set(text, audio)
                         
                     meta_info['text'] = text
                     if not self.first_chunk_generated:
                         meta_info["is_first_chunk"] = True
                         self.first_chunk_generated = True
 
                     if "end_of_llm_stream" in meta_info and meta_info["end_of_llm_stream"]:
```

### Comparing `bolna-0.7.7/bolna/synthesizer/fourie_synthesizer.py` & `bolna-0.7.8/bolna/synthesizer/fourie_synthesizer.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.7/bolna/synthesizer/openai_synthesizer.py` & `bolna-0.7.8/bolna/synthesizer/openai_synthesizer.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.7/bolna/synthesizer/polly_synthesizer.py` & `bolna-0.7.8/bolna/synthesizer/polly_synthesizer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,77 @@
+import os
 from dotenv import load_dotenv
 from botocore.exceptions import BotoCoreError, ClientError
 from aiobotocore.session import AioSession
 from contextlib import AsyncExitStack
-import audioop
 from bolna.helpers.logger_config import configure_logger
 from bolna.helpers.utils import convert_audio_to_wav, create_ws_data_packet, pcm_to_wav_bytes, resample
+from bolna.memory.cache.inmemory_scalar_cache import InmemoryScalarCache
 from .base_synthesizer import BaseSynthesizer
 
 logger = configure_logger(__name__)
 load_dotenv()
 
 
 class PollySynthesizer(BaseSynthesizer):
     def __init__(self, voice, language, audio_format="pcm", sampling_rate=8000, stream=False, engine="neural",
-                 buffer_size=400, speaking_rate = "100%", volume = "0dB", cache= None, **kwargs):
+                 buffer_size=400, speaking_rate = "100%", volume = "0dB", caching= True, **kwargs):
         super().__init__(stream, buffer_size)
         self.engine = engine
         self.format = self.get_format(audio_format.lower())
         self.voice = voice
         self.language = language
         self.sample_rate = str(sampling_rate)
         self.client = None
         self.first_chunk_generated = False
         self.speaking_rate = speaking_rate
         self.volume = volume
         self.synthesized_characters = 0
-        self.cache = cache
+        self.caching = caching
+        if caching:
+            self.cache = InmemoryScalarCache()
 
     def get_synthesized_characters(self):
         return self.synthesized_characters
     
+    def get_engine(self):
+        return self.engine
+
     def get_format(self, audio_format):
         if audio_format == "pcm":
             return "pcm"
         else:
             return "mp3"
 
     @staticmethod
     async def create_client(service: str, session: AioSession, exit_stack: AsyncExitStack):
-        # creates AWS session from system environment credentials & config
-        return await exit_stack.enter_async_context(session.create_client(service))
+        if os.getenv('AWS_ACCESS_KEY_ID'):
+            return await exit_stack.enter_async_context(session.create_client(
+                service,
+                aws_access_key_id=os.getenv('AWS_ACCESS_KEY_ID'),
+                aws_secret_access_key=os.getenv('AWS_SECRET_ACCESS_KEY'),
+                region_name=os.getenv('AWS_REGION')
+            ))
+        else:
+            return await exit_stack.enter_async_context(session.create_client(service))
 
     async def __generate_http(self, text):
-        self.synthesized_characters += len(text)
         session = AioSession()
         async with AsyncExitStack() as exit_stack:
             polly = await self.create_client("polly", session, exit_stack)
             logger.info(f"Generating TTS response for text: {text}, SampleRate {self.sample_rate} format {self.format}")
             # input = f"""
             # <speak> 
             #     <amazon:auto-breaths volume= "x-loud" frequency="x-high" duration="x-long"> 
             #         <prosody volume="{self.volume}" rate="{self.speaking_rate}"> {text} 
             #         </prosody> 
             #     </amazon:auto-breaths>
             # </speak>
             # """
 
-            logger.info(f"Sending text {input}")
             try:
                 response = await polly.synthesize_speech(
                     Engine=self.engine,
                     Text=text,
                     OutputFormat=self.format,
                     VoiceId=self.voice,
                     LanguageCode=self.language,
@@ -72,30 +83,41 @@
                 return await response["AudioStream"].read()
 
     async def open_connection(self):
         pass
 
     async def synthesize(self, text):
         # This is used for one off synthesis mainly for use cases like voice lab and IVR
-        audio = await self.__generate_http(text)
-
-        return audio
-
+        try:
+            audio = await self.__generate_http(text)
+            if self.format == "mp3":
+                audio = convert_audio_to_wav(audio, source_format="mp3")
+            return audio
+        except Exception as e:
+            logger.error(f"Could not synthesize {e}")
     async def generate(self):
         while True:
             logger.info("Generating TTS response")
             message = await self.internal_queue.get()
             logger.info(f"Generating TTS response for message: {message}")
             meta_info, text = message.get("meta_info"), message.get("data")
-            if self.cache.get(text):
-                logger.info(f"Cache hit and hence returning quickly {text}")
-                message = self.cache[text]
+            if self.caching:
+                logger.info(f"Caching is on")
+                if self.cache.get(text):
+                    logger.info(f"Cache hit and hence returning quickly {text}")
+                    message = self.cache.get(text)
+                else:
+                    logger.info(f"Not a cache hit {list(self.cache.data_dict)}")
+                    self.synthesized_characters += len(text)
+                    message = await self.__generate_http(text)
+                    self.cache.set(text, message)
             else:
-                logger.info(f"Not a cache hit {list(self.cache.data_dict)}")
-            message = await self.__generate_http(text)
+                logger.info(f"No caching present")
+                self.synthesized_characters += len(text)
+                message = await self.__generate_http(text)
             if self.format == "mp3":
                 message = convert_audio_to_wav(message, source_format="mp3")
             if not self.first_chunk_generated:
                 meta_info["is_first_chunk"] = True
                 self.first_chunk_generated = True
             else:
                 meta_info["is_first_chunk"] = False
```

### Comparing `bolna-0.7.7/bolna/synthesizer/xtts_synthesizer.py` & `bolna-0.7.8/bolna/synthesizer/xtts_synthesizer.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.7/bolna/transcriber/azure_transcriber.py` & `bolna-0.7.8/bolna/transcriber/hume_transcriber.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,98 +9,81 @@
 import time
 from urllib.parse import urlencode
 from dotenv import load_dotenv
 from .base_transcriber import BaseTranscriber
 from bolna.helpers.logger_config import configure_logger
 from bolna.helpers.utils import create_ws_data_packet, int2float
 from bolna.helpers.vad import VAD
-import azure.cognitiveservices.speech as speechsdk
+from hume import HumeBatchClient
+
 
 import uvloop
 asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
+
+
 torch.set_num_threads(1)
 
 logger = configure_logger(__name__)
 load_dotenv()
 
 
-class DeepgramTranscriber(BaseTranscriber):
-    def __init__(self, provider, input_queue=None, model='deepgram', stream=True, language="en", endpointing="400",
+class HumeTranscriber(BaseTranscriber):
+    def __init__(self, provider, input_queue=None, model='hume', stream=True, language="en", endpointing="400",
                  sampling_rate="16000", encoding="linear16", output_queue=None, keywords=None,
                  process_interim_results="true", **kwargs):
         logger.info(f"Initializing transcriber")
         super().__init__(input_queue)
         self.endpointing = endpointing
         self.language = language
         self.stream = stream
         self.provider = provider
-        if self.provider not in ('twilio', 'exotel'):
-            raise Exception("Cannot use Azure with any other settings apart from Twilio or Exotel.")
         self.heartbeat_task = None
         self.sender_task = None
         self.model = 'deepgram'
-        self.sampling_rate = 16000
+        self.sampling_rate = sampling_rate
         self.encoding = encoding
         self.api_key = kwargs.get("transcriber_key", os.getenv('DEEPGRAM_AUTH_TOKEN'))
         self.transcriber_output_queue = output_queue
         self.transcription_task = None
-        self.keywords = keywords
+        self.on_device_vad = kwargs.get("on_device_vad", False) if self.stream else False
         logger.info(f"self.stream: {self.stream}")
-        if not self.stream:
-            raise Exception("Can use Azure transcriber only in calls")
+        if self.on_device_vad:
+            self.vad_model = VAD()
+            self.audio = []
+            # logger.info("on_device_vad is TRue")
+            # self.vad_model, self.vad_utils = torch.hub.load(repo_or_dir='snakers4/silero-vad', model='silero_vad', force_reload=False)
+        self.voice_threshold = 0.5
         self.interruption_signalled = False
+        self.sampling_rate = 16000
         if not self.stream:
             self.api_url = f"https://api.deepgram.com/v1/listen?model=nova-2&filler_words=true&language={self.language}"
             self.session = aiohttp.ClientSession()
-            if self.keywords is not None:
-                keyword_string = "&keywords=" + "&keywords=".join(self.keywords.split(","))
-                self.api_url = f"{self.api_url}{keyword_string}"
         self.audio_submitted = False
         self.audio_submission_time = None
         self.num_frames = 0
         self.connection_start_time = None
         self.process_interim_results = process_interim_results
+        # Work on this soon
+        self.last_utterance_time_stamp = time.time()
+        self.utterance_end_task = None
         self.audio_frame_duration = 0.0
 
-        #Message states
-        self.curr_message = ''
-        self.finalized_transcript = ""
-
-
-        self.speech_config = speechsdk.SpeechConfig(subscription=os.getenv("AZURE_SPEECH_KEY"), region=os.getenv("AZURE_SPEECH_REGION"))
-
-        # Setup the audio stream
-        self.audio_format = speechsdk.audio.AudioStreamFormat(samples_per_second=16000,
-                                                        bits_per_sample=8,
-                                                        channels=1, 
-                                                        wave_stream_format=speechsdk.AudioStreamWaveFormat.PCM)
-        self.audio_stream = speechsdk.audio.PushAudioInputStream(stream_format=self.audio_format)
-        self.audio_config = speechsdk.audio.AudioConfig(stream=self.audio_stream)
-        self.speech_recognizer = speechsdk.SpeechRecognizer(speech_config=self.speech_config, audio_config=self.audio_config)
-
-    def __session_stopped_cb(self, evt):
-        print('SESSION STOPPED: {}'.format(evt))
-    
-    def __receive_transcription(self, evt):
-        msg = evt.result.text
-        if msg != "":
-            logger.info(f"Yielding interim-message current_message = {msg}")
-            self.meta_info["include_latency"] = False
-            self.meta_info["utterance_end"] = self.__calculate_utterance_end(msg)
-            self.meta_info["time_received"] = time.time()
-            self.meta_info["transcriber_latency"] = self.meta_info["time_received"] - self.meta_info["utterance_end"]
-            self.transcriber_output_queue.put_nowait(create_ws_data_packet(self.curr_message, self.meta_info))
-        
-
-    def setup(self):
-        self.speech_recognizer.recognizing.connect(lambda evt: print('RECOGNIZING: {}'.format(evt)))
-        self.speech_recognizer.recognized.connect(self.__receive_transcription)
-        self.speech_recognizer.session_started.connect(lambda evt: print('SESSION STARTED: {}'.format(evt)))
-        self.speech_recognizer.session_stopped.connect(self.__session_stopped_cb)
-        self.speech_recognizer.canceled.connect(lambda evt: print('CANCELED {}'.format(evt)))
+    def __get_speaker_transcript(self, data):
+        transcript_words = []
+        if 'channel' in data and 'alternatives' in data['channel']:
+            for alternative in data['channel']['alternatives']:
+                if 'words' in alternative:
+                    for word_info in alternative['words']:
+                        if word_info['speaker'] == 0:
+                            transcript_words.append(word_info['word'])
+
+        return ' '.join(transcript_words)
+
+    def get_hume_ws_url(self):
+        return 'wss://api.hume.ai/v0/evi/chat'
 
     async def send_heartbeat(self, ws):
         try:
             while True:
                 data = {'type': 'KeepAlive'}
                 await ws.send(json.dumps(data))
                 await asyncio.sleep(5)  # Send a heartbeat message every 5 seconds
@@ -143,38 +126,87 @@
             return True  # Indicates end of processing
 
         return False
 
     def get_meta_info(self):
         return self.meta_info
 
+    async def sender(self, ws=None):
+        try:
+            while True:
+                ws_data_packet = await self.input_queue.get()
+                # If audio submitted was false, that means that we're starting the stream now. That's our stream start
+                if not self.audio_submitted:
+                    self.audio_submitted = True
+                    self.audio_submission_time = time.time()
+                end_of_stream = await self._check_and_process_end_of_stream(ws_data_packet, ws)
+                if end_of_stream:
+                    break
+                self.meta_info = ws_data_packet.get('meta_info')
+                start_time = time.time()
+                transcription = await self._get_http_transcription(ws_data_packet.get('data'))
+                transcription['meta_info']["include_latency"] = True
+                transcription['meta_info']["transcriber_latency"] = time.time() - start_time
+                transcription['meta_info']['audio_duration'] = transcription['meta_info']['transcriber_duration']
+                transcription['meta_info']['last_vocal_frame_timestamp'] = start_time
+                yield transcription
+
+            if self.transcription_task is not None:
+                self.transcription_task.cancel()
+        except asyncio.CancelledError:
+            logger.info("Cancelled sender task")
+            return
+        except Exception as e:
+            logger.error('Error while sending: ' + str(e))
+            raise Exception("Something went wrong")
+
+    async def __check_for_vad(self, data):
+        if data is None:
+            return
+        self.audio.append(data)
+        audio_bytes = b''.join(self.audio)
+        audio_int16 = np.frombuffer(audio_bytes, np.int16)
+        frame_np = int2float(audio_int16)
+
+        speech_prob = self.vad_model(torch.from_numpy(frame_np.copy()), self.sampling_rate).item()
+        logger.info(f"Speech probability {speech_prob}")
+        if float(speech_prob) >= float(self.voice_threshold):
+            logger.info(f"It's definitely human voice and hence interrupting {self.meta_info}")
+            self.interruption_signalled = True
+            await self.push_to_transcriber_queue(create_ws_data_packet("INTERRUPTION", self.meta_info))
+            self.audio = []
+
     async def sender_stream(self, ws=None):
         try:
             while True:
                 ws_data_packet = await self.input_queue.get()
                 # Initialise new request
                 if not self.audio_submitted:
                     self.meta_info = ws_data_packet.get('meta_info')
                     self.audio_submitted = True
                     self.audio_submission_time = time.time()
                     self.current_request_id = self.generate_request_id()
                     self.meta_info['request_id'] = self.current_request_id
-                    
 
+                audio_bytes = ws_data_packet['data']
+                if not self.interruption_signalled and self.on_device_vad:
+                    await self.__check_for_vad(audio_bytes)
                 end_of_stream = await self._check_and_process_end_of_stream(ws_data_packet, ws)
                 if end_of_stream:
                     break
                 self.num_frames += 1
-                self.stream.write(ws_data_packet.get('data'))
+                await ws.send(ws_data_packet.get('data'))
 
         except Exception as e:
             logger.error('Error while sending: ' + str(e))
             raise Exception("Something went wrong")
 
     async def receiver(self, ws):
+        curr_message = ""
+        finalized_transcript = ""
         async for msg in ws:
             try:
                 msg = json.loads(msg)
 
                 # If connection_start_time is None, it is the duratons of frame submitted till now minus current time
                 if self.connection_start_time is None:
                     self.connection_start_time = (time.time() - (self.num_frames * self.audio_frame_duration))
@@ -189,119 +221,126 @@
                     return
 
                 # TODO LATENCY STUFF
                 if msg["type"] == "UtteranceEnd":
                     logger.info(
                         "Transcriber Latency: {} for request id {}".format(time.time() - self.audio_submission_time,
                                                                            self.current_request_id))
-                    logger.info(f"Current message during UtteranceEnd {self.curr_message}")
+                    logger.info(f"Current message during UtteranceEnd {curr_message}")
                     self.meta_info["start_time"] = self.audio_submission_time
                     self.meta_info["end_time"] = time.time() - 100
                     self.meta_info['speech_final'] = True
                     self.audio_submitted = False
                     self.meta_info["include_latency"] = True
                     self.meta_info["utterance_end"] = self.connection_start_time + msg['last_word_end']
                     self.meta_info["time_received"] = time.time()
                     self.meta_info["transcriber_latency"] = None
-                    if self.curr_message == "":
+                    if curr_message == "":
                         continue
                     logger.info(f"Signalling the Task manager to start speaking")
-                    yield create_ws_data_packet(self.finalized_transcript, self.meta_info)
-                    self.curr_message = ""
-                    self.finalized_transcript = ""
+                    yield create_ws_data_packet(finalized_transcript, self.meta_info)
+                    curr_message = ""
+                    finalized_transcript = ""
                     continue
 
                 if msg["type"] == "SpeechStarted":
-                    if self.curr_message != "" and not self.process_interim_results:
+                    if curr_message != "" and not self.process_interim_results:
                         logger.info("Current messsage is null and hence inetrrupting")
                         self.meta_info["should_interrupt"] = True
                     elif self.process_interim_results:
                         self.meta_info["should_interrupt"] = False
                     logger.info(f"YIELDING TRANSCRIBER BEGIN")
                     yield create_ws_data_packet("TRANSCRIBER_BEGIN", self.meta_info)
                     await asyncio.sleep(0.05) #Sleep for 50ms to pass the control to task manager
                     continue
 
                 transcript = msg['channel']['alternatives'][0]['transcript']
 
                 if transcript and len(transcript.strip()) == 0 or transcript == "":
                     continue
 
-                # # TODO Remove the need for on_device_vad
-                # # If interim message is not true and curr message is null, send a begin signal
-                # if self.curr_message == "" and msg["is_final"] is False:
-                #     yield create_ws_data_packet("TRANSCRIBER_BEGIN", self.meta_info)
-                #     await asyncio.sleep(0.1)  # Enable taskmanager to interrupt
+                # TODO Remove the need for on_device_vad
+                # If interim message is not true and curr message is null, send a begin signal
+                if curr_message == "" and msg["is_final"] is False:
+                    if not self.on_device_vad:
+                        logger.info("Not on device vad and hence inetrrupting")
+                        self.meta_info["should_interrupt"] = False
+                    yield create_ws_data_packet("TRANSCRIBER_BEGIN", self.meta_info)
+
+                    await asyncio.sleep(0.1)  # Enable taskmanager to interrupt
 
                 if self.process_interim_results == "true":
                     # If we're not processing interim results
                     # Yield current transcript
+                    # curr_message = self.__get_speaker_transcript(msg)
                     # Just yield the current transcript as we do not want to wait for is_final. Is_final is just to make 
-                    self.curr_message = self.finalized_transcript + " " + transcript
-                    logger.info(f"Yielding interim-message current_message = {self.curr_message}")
+                    curr_message = finalized_transcript + " " + transcript
+                    logger.info(f"Yielding interim-message current_message = {curr_message}")
                     self.meta_info["include_latency"] = False
                     self.meta_info["utterance_end"] = self.__calculate_utterance_end(msg)
                     self.meta_info["time_received"] = time.time()
                     self.meta_info["transcriber_latency"] = self.meta_info["time_received"] - self.meta_info[
                         "utterance_end"]
-                    yield create_ws_data_packet(self.curr_message, self.meta_info)
+                    yield create_ws_data_packet(curr_message, self.meta_info)
                     
                     # If is_final is true simply update the finalized transcript
                     if  msg["is_final"] is True:
-                        self.finalized_transcript += " " + transcript  # Just get the whole transcript as there's mismatch at times
+                        finalized_transcript += " " + transcript  # Just get the whole transcript as there's mismatch at times
                         self.meta_info["is_final"] = True
 
                 else:
-                    self.curr_message += " " + transcript
+                    curr_message += " " + transcript
                     # Process interim results is false and hence we need to be dependent on the endpointing
                     if msg["speech_final"] or not self.stream:
                         logger.info(f"Full Transcriber message from speech final {msg}")
-                        yield create_ws_data_packet(self.curr_message, self.meta_info)
-                        logger.info(f"Yielded {self.curr_message}")
-                        logger.info('User: {}'.format(self.curr_message))
+                        yield create_ws_data_packet(curr_message, self.meta_info)
+                        logger.info(f"Yielded {curr_message}")
+                        logger.info('User: {}'.format(curr_message))
 
                         self.interruption_signalled = False
                         if self.audio_submitted == True:
                             logger.info("Transcriber Latency: {} for request id {}".format(
                                 time.time() - self.audio_submission_time, self.current_request_id))
                             self.meta_info["start_time"] = self.audio_submission_time
                             self.meta_info["end_time"] = time.time()
                             self.audio_submitted = False
-                        if self.curr_message != "":
+                        if curr_message != "":
                             self.meta_info["include_latency"] = True
                             self.meta_info["audio_duration"] = msg['start'] + msg['duration']
                             last_spoken_audio_frame = self.__calculate_utterance_end(msg)
                             self.meta_info["audio_start_time"] = self.audio_submission_time
                             transcription_completion_time = time.time()
                             self.meta_info["transcription_completion_time"] = transcription_completion_time
                             self.meta_info[
                                 "transcriber_latency"] = transcription_completion_time - last_spoken_audio_frame  # We subtract first audio wav because user started speaking then. In this case we can calculate actual latency taken by the transcriber
                             self.meta_info["last_vocal_frame_timestamp"] = last_spoken_audio_frame
                         else:
                             self.meta_info["include_latency"] = False
                         self.meta_info["speech_final"] = True
                         yield create_ws_data_packet("TRANSCRIBER_END", self.meta_info)
-                        self.curr_message = ""
+                        curr_message = ""
 
             except Exception as e:
                 traceback.print_exc()
                 logger.error(f"Error while getting transcriptions {e}")
                 self.interruption_signalled = False
                 yield create_ws_data_packet("TRANSCRIBER_END", self.meta_info)
 
     async def push_to_transcriber_queue(self, data_packet):
         await self.transcriber_output_queue.put(data_packet)
 
-    def deepgram_connect(self):
-        websocket_url = self.get_deepgram_ws_url()
+    def hume_connect(self):
+        websocket_url = self.get_hume_ws_url()
         extra_headers = {
-            'Authorization': 'Token {}'.format(os.getenv('DEEPGRAM_AUTH_TOKEN'))
+            "X-Hume-Api-Key": 'nODRW0JT515subWEe4GBGEOyXHoy0xV9ouN5jv6SRoETBolT',
+            "X-Hume-Client-Name": "python_sdk",
+            "X-Hume-Client-Version": "0.5.0",
         }
-        deepgram_ws = websockets.connect(websocket_url, extra_headers=extra_headers)
-        return deepgram_ws
+        hume_ws = websockets.connect(websocket_url, extra_headers=extra_headers)
+        return hume_ws
 
     async def run(self):
         try:
             self.transcription_task = asyncio.create_task(self.transcribe())
         except Exception as e:
             logger.error(f"not working {e}")
     def __calculate_utterance_end(self, data):
@@ -313,24 +352,24 @@
                     utterance_end = self.connection_start_time + final_word['end']
                     logger.info(f"Final word ended at {utterance_end}")
         return utterance_end
 
     async def transcribe(self):
         logger.info(f"STARTED TRANSCRIBING")
         try:
-            async with self.connect() as deepgram_ws:
+            async with self.hume_connect() as hume_ws:
                 if self.stream:
-                    self.sender_task = asyncio.create_task(self.sender_stream(deepgram_ws))
-                    self.heartbeat_task = asyncio.create_task(self.send_heartbeat(deepgram_ws))
-                    async for message in self.receiver(deepgram_ws):
+                    self.sender_task = asyncio.create_task(self.sender_stream(hume_ws))
+                    #self.heartbeat_task = asyncio.create_task(self.send_heartbeat(hume_ws))
+                    async for message in self.receiver(hume_ws):
                         if self.connection_on:
                             await self.push_to_transcriber_queue(message)
                         else:
                             logger.info("closing the deepgram connection")
-                            await self._close(deepgram_ws, data={"type": "CloseStream"})
+                            await self._close(hume_ws, data={"type": "CloseStream"})
                 else:
                     async for message in self.sender():
                         await self.push_to_transcriber_queue(message)
 
             await self.push_to_transcriber_queue(create_ws_data_packet("transcriber_connection_closed", self.meta_info))
         except Exception as e:
             logger.error(f"Error in transcribe: {e}")
```

### Comparing `bolna-0.7.7/bolna/transcriber/base_transcriber.py` & `bolna-0.7.8/bolna/transcriber/base_transcriber.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.7/bolna/transcriber/deepgram_transcriber.py` & `bolna-0.7.8/bolna/transcriber/deepgram_transcriber.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 load_dotenv()
 
 
 class DeepgramTranscriber(BaseTranscriber):
     def __init__(self, provider, input_queue=None, model='deepgram', stream=True, language="en", endpointing="400",
                  sampling_rate="16000", encoding="linear16", output_queue=None, keywords=None,
                  process_interim_results="true", **kwargs):
-        logger.info(f"Initializing transcriber")
+        logger.info(f"Initializing transcriber {kwargs}")
         super().__init__(input_queue)
         self.endpointing = endpointing
         self.language = language
         self.stream = stream
         self.provider = provider
         self.heartbeat_task = None
         self.sender_task = None
@@ -49,15 +49,15 @@
                 self.api_url = f"{self.api_url}{keyword_string}"
         self.audio_submitted = False
         self.audio_submission_time = None
         self.num_frames = 0
         self.connection_start_time = None
         self.process_interim_results = process_interim_results
         self.audio_frame_duration = 0.0
-
+        self.connected_via_dashboard = kwargs.get("enforce_streaming", True)
         #Message states
         self.curr_message = ''
         self.finalized_transcript = ""
 
     def get_deepgram_ws_url(self):
         dg_params = {
             'model': 'nova-2',
@@ -74,14 +74,19 @@
             self.sampling_rate = 8000
             self.audio_frame_duration = 0.2  # With twilio we are sending 200ms at a time
 
             dg_params['encoding'] = self.encoding
             dg_params['sample_rate'] = self.sampling_rate
             dg_params['channels'] = "1"
 
+        elif not self.connected_via_dashboard:
+            dg_params['encoding'] = "linear16"
+            dg_params['sample_rate'] = 16000
+            dg_params['channels'] = "1"
+
         if self.provider == "playground":
             logger.info(f"CONNECTED THROUGH PLAYGROUND")
             self.sampling_rate = 8000
             self.audio_frame_duration = 0.0  # There's no streaming from the playground
 
         if "en" not in self.language:
             dg_params['language'] = self.language
```

### Comparing `bolna-0.7.7/bolna/transcriber/hume_transcriber.py` & `bolna-0.7.8/bolna/transcriber/whisper_transcriber.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,375 +1,340 @@
 import asyncio
+# from asyncio.base_tasks import tasks
 import traceback
 import numpy as np
 import torch
 import websockets
 import os
 import json
-import aiohttp
 import time
-from urllib.parse import urlencode
-from dotenv import load_dotenv
 from .base_transcriber import BaseTranscriber
 from bolna.helpers.logger_config import configure_logger
 from bolna.helpers.utils import create_ws_data_packet, int2float
 from bolna.helpers.vad import VAD
-from hume import HumeBatchClient
-
+from audioop import ulaw2lin, ratecv
+import json
+import os
+import time
+from queue import Queue
+from websockets.exceptions import *
 
 import uvloop
 asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
-
-
 torch.set_num_threads(1)
 
 logger = configure_logger(__name__)
-load_dotenv()
 
 
-class HumeTranscriber(BaseTranscriber):
-    def __init__(self, provider, input_queue=None, model='hume', stream=True, language="en", endpointing="400",
-                 sampling_rate="16000", encoding="linear16", output_queue=None, keywords=None,
-                 process_interim_results="true", **kwargs):
+
+
+class WhisperTranscriber(BaseTranscriber):
+    def __init__(self, provider, input_queue=None, model='whisper', stream=True, language="en", endpointing="400",
+                 sampling_rate="16000", encoding="PCM", output_queue=None, keywords=None,
+                 process_interim_results="true", *args,**kwargs):
         logger.info(f"Initializing transcriber")
         super().__init__(input_queue)
+
         self.endpointing = endpointing
-        self.language = language
-        self.stream = stream
+        self.language:str = language
+        self.stream:bool = True
         self.provider = provider
+
+        #   TASKS
         self.heartbeat_task = None
         self.sender_task = None
-        self.model = 'deepgram'
-        self.sampling_rate = sampling_rate
-        self.encoding = encoding
-        self.api_key = kwargs.get("transcriber_key", os.getenv('DEEPGRAM_AUTH_TOKEN'))
-        self.transcriber_output_queue = output_queue
         self.transcription_task = None
-        self.on_device_vad = kwargs.get("on_device_vad", False) if self.stream else False
-        logger.info(f"self.stream: {self.stream}")
-        if self.on_device_vad:
-            self.vad_model = VAD()
-            self.audio = []
-            # logger.info("on_device_vad is TRue")
-            # self.vad_model, self.vad_utils = torch.hub.load(repo_or_dir='snakers4/silero-vad', model='silero_vad', force_reload=False)
-        self.voice_threshold = 0.5
-        self.interruption_signalled = False
-        self.sampling_rate = 16000
-        if not self.stream:
-            self.api_url = f"https://api.deepgram.com/v1/listen?model=nova-2&filler_words=true&language={self.language}"
-            self.session = aiohttp.ClientSession()
-        self.audio_submitted = False
-        self.audio_submission_time = None
-        self.num_frames = 0
-        self.connection_start_time = None
-        self.process_interim_results = process_interim_results
-        # Work on this soon
-        self.last_utterance_time_stamp = time.time()
-        self.utterance_end_task = None
-        self.audio_frame_duration = 0.0
-
-    def __get_speaker_transcript(self, data):
-        transcript_words = []
-        if 'channel' in data and 'alternatives' in data['channel']:
-            for alternative in data['channel']['alternatives']:
-                if 'words' in alternative:
-                    for word_info in alternative['words']:
-                        if word_info['speaker'] == 0:
-                            transcript_words.append(word_info['word'])
 
-        return ' '.join(transcript_words)
+        # MODEL CONF
+        self.model:str = model
+        self.sampling_rate:int = sampling_rate
+        self.encoding = encoding
+
+        # INPUT/OUPUT queue present in base class
+        self.transcriber_output_queue:Queue = output_queue
+        
+
+        self.keywords = keywords
+        self.interruption_signalled:bool = False
+        self.url:str = os.getenv('WHISPER_URL')
+        
+        # audio submitted
+        self.audio_submission_time:float = None
+        self.num_frames:int = 0
+        self.connection_start_time:float = None
+        self.process_interim_results:bool = True
+        self.audio_frame_duration:float = 0.0
+
+
+        # FLAGS
+        self.speech_started:bool = False
+        self.audio_submitted:bool = False
+
+        #   Message states
+        self.curr_message:str = ''
+        self.commited_list:list = []
+        self.segments_list:list = None
+        self.whole_segment_list:list = []
+        self.seg_ptr:int = -1
+        self.current_seg_ptr:int = -1
+        self.finalized_transcript:str = ""
+    
+    def get_whisper_ws_url(self):
+        return self.url
 
-    def get_hume_ws_url(self):
-        return 'wss://api.hume.ai/v0/evi/chat'
 
     async def send_heartbeat(self, ws):
         try:
             while True:
                 data = {'type': 'KeepAlive'}
                 await ws.send(json.dumps(data))
                 await asyncio.sleep(5)  # Send a heartbeat message every 5 seconds
         except Exception as e:
             logger.error('Error while sending: ' + str(e))
             raise Exception("Something went wrong while sending heartbeats to {}".format(self.model))
 
     async def toggle_connection(self):
         self.connection_on = False
-        if self.heartbeat_task is not None:
-            self.heartbeat_task.cancel()
+        # if self.heartbeat_task is not None:
+        #     self.heartbeat_task.send(b"END_OF_AUDIO")
         self.sender_task.cancel()
 
-    async def _get_http_transcription(self, audio_data):
-        if self.session is None or self.session.closed:
-            self.session = aiohttp.ClientSession()
-
-        headers = {
-            'Authorization': 'Token {}'.format(self.api_key),
-            'Content-Type': 'audio/webm'  # Currently we are assuming this is via browser
-        }
-
-        self.current_request_id = self.generate_request_id()
-        self.meta_info['request_id'] = self.current_request_id
-        start_time = time.time()
-        async with self.session as session:
-            async with session.post(self.api_url, data=audio_data, headers=headers) as response:
-                response_data = await response.json()
-                logger.info(f"response_data {response_data} total time {time.time() - start_time}")
-                transcript = response_data["results"]["channels"][0]["alternatives"][0]["transcript"]
-                logger.info(f"transcript {transcript} total time {time.time() - start_time}")
-                self.meta_info['transcriber_duration'] = response_data["metadata"]["duration"]
-                return create_ws_data_packet(transcript, self.meta_info)
 
+    # TODO: add a server end  process in the server code
     async def _check_and_process_end_of_stream(self, ws_data_packet, ws):
         if 'eos' in ws_data_packet['meta_info'] and ws_data_packet['meta_info']['eos'] is True:
             logger.info("First closing transcription websocket")
-            await self._close(ws, data={"type": "CloseStream"})
+            await self.heartbeat_task.send(b"END_OF_AUDIO")
             logger.info("Closed transcription websocket and now closing transcription task")
             return True  # Indicates end of processing
 
         return False
 
     def get_meta_info(self):
         return self.meta_info
 
-    async def sender(self, ws=None):
-        try:
-            while True:
-                ws_data_packet = await self.input_queue.get()
-                # If audio submitted was false, that means that we're starting the stream now. That's our stream start
-                if not self.audio_submitted:
-                    self.audio_submitted = True
-                    self.audio_submission_time = time.time()
-                end_of_stream = await self._check_and_process_end_of_stream(ws_data_packet, ws)
-                if end_of_stream:
-                    break
-                self.meta_info = ws_data_packet.get('meta_info')
-                start_time = time.time()
-                transcription = await self._get_http_transcription(ws_data_packet.get('data'))
-                transcription['meta_info']["include_latency"] = True
-                transcription['meta_info']["transcriber_latency"] = time.time() - start_time
-                transcription['meta_info']['audio_duration'] = transcription['meta_info']['transcriber_duration']
-                transcription['meta_info']['last_vocal_frame_timestamp'] = start_time
-                yield transcription
-
-            if self.transcription_task is not None:
-                self.transcription_task.cancel()
-        except asyncio.CancelledError:
-            logger.info("Cancelled sender task")
-            return
-        except Exception as e:
-            logger.error('Error while sending: ' + str(e))
-            raise Exception("Something went wrong")
-
-    async def __check_for_vad(self, data):
-        if data is None:
-            return
-        self.audio.append(data)
-        audio_bytes = b''.join(self.audio)
-        audio_int16 = np.frombuffer(audio_bytes, np.int16)
-        frame_np = int2float(audio_int16)
-
-        speech_prob = self.vad_model(torch.from_numpy(frame_np.copy()), self.sampling_rate).item()
-        logger.info(f"Speech probability {speech_prob}")
-        if float(speech_prob) >= float(self.voice_threshold):
-            logger.info(f"It's definitely human voice and hence interrupting {self.meta_info}")
-            self.interruption_signalled = True
-            await self.push_to_transcriber_queue(create_ws_data_packet("INTERRUPTION", self.meta_info))
-            self.audio = []
 
     async def sender_stream(self, ws=None):
         try:
             while True:
                 ws_data_packet = await self.input_queue.get()
                 # Initialise new request
                 if not self.audio_submitted:
                     self.meta_info = ws_data_packet.get('meta_info')
                     self.audio_submitted = True
                     self.audio_submission_time = time.time()
-                    self.current_request_id = self.generate_request_id()
+
+                    # this is init when we connect to server
+                    # self.current_request_id = self.generate_request_id()
+                    
                     self.meta_info['request_id'] = self.current_request_id
 
-                audio_bytes = ws_data_packet['data']
-                if not self.interruption_signalled and self.on_device_vad:
-                    await self.__check_for_vad(audio_bytes)
                 end_of_stream = await self._check_and_process_end_of_stream(ws_data_packet, ws)
                 if end_of_stream:
                     break
                 self.num_frames += 1
-                await ws.send(ws_data_packet.get('data'))
-
+                audio_chunk:bytes = ws_data_packet.get('data')
+                # ulaw is encoding method , this is the inverse function
+                audio_chunk = ulaw2lin(audio_chunk, 2)
+                # convert from 8000 to 16000 HZ
+                audio_chunk = ratecv(audio_chunk, 2, 1, 8000, 16000, None)[0]
+                audio_chunk = self.bytes_to_float_array(audio_chunk).tobytes()
+                await ws.send(audio_chunk)
         except Exception as e:
             logger.error('Error while sending: ' + str(e))
             raise Exception("Something went wrong")
 
     async def receiver(self, ws):
-        curr_message = ""
-        finalized_transcript = ""
         async for msg in ws:
             try:
-                msg = json.loads(msg)
-
+                msg:dict = json.loads(msg)
+                print(msg)
                 # If connection_start_time is None, it is the duratons of frame submitted till now minus current time
                 if self.connection_start_time is None:
                     self.connection_start_time = (time.time() - (self.num_frames * self.audio_frame_duration))
                     logger.info(
                         f"Connecton start time {self.connection_start_time} {self.num_frames} and {self.audio_frame_duration}")
 
                 logger.info(f"###### ######### ############# Message from the transcriber {msg}")
-                if msg['type'] == "Metadata":
+                if "message" in msg and msg["message"] == "DISCONNECT":
                     logger.info(f"Got a summary object {msg}")
                     self.meta_info["transcriber_duration"] = msg["duration"]
                     yield create_ws_data_packet("transcriber_connection_closed", self.meta_info)
+                    self.curr_message:str = ''
+                    self.commited_list:list = []
+                    self.segments_list:list = None
+                    self.whole_segment_list:list = []
+                    self.seg_ptr:int = -1
+                    self.current_seg_ptr:int = -1
+                    self.finalized_transcript:str = ""
                     return
 
                 # TODO LATENCY STUFF
-                if msg["type"] == "UtteranceEnd":
+                if "message" in msg and msg["message"] == "UTTERANCE_END":
+                    logger.info(f"segmeny list{self.segments_list}")
+                    if len(self.segments_list) >= 0:
+                        self.finalized_transcript = self.finalized_transcript + " " + self.segments_list[-1].get("text")
+                    
+
                     logger.info(
                         "Transcriber Latency: {} for request id {}".format(time.time() - self.audio_submission_time,
                                                                            self.current_request_id))
-                    logger.info(f"Current message during UtteranceEnd {curr_message}")
+                    logger.info(f"Current message during UtteranceEnd {self.curr_message}")
                     self.meta_info["start_time"] = self.audio_submission_time
                     self.meta_info["end_time"] = time.time() - 100
                     self.meta_info['speech_final'] = True
                     self.audio_submitted = False
                     self.meta_info["include_latency"] = True
-                    self.meta_info["utterance_end"] = self.connection_start_time + msg['last_word_end']
+                    
+                    self.meta_info["utterance_end"] = self.connection_start_time + float(self.whole_segment_list[-1].get('end'))
                     self.meta_info["time_received"] = time.time()
                     self.meta_info["transcriber_latency"] = None
-                    if curr_message == "":
-                        continue
+                    # if self.curr_message == "":
+                    #     continue
                     logger.info(f"Signalling the Task manager to start speaking")
-                    yield create_ws_data_packet(finalized_transcript, self.meta_info)
-                    curr_message = ""
-                    finalized_transcript = ""
+                    yield create_ws_data_packet(self.finalized_transcript, self.meta_info)
+                    self.curr_message = ""
+                    self.finalized_transcript = ""
                     continue
 
-                if msg["type"] == "SpeechStarted":
-                    if curr_message != "" and not self.process_interim_results:
-                        logger.info("Current messsage is null and hence inetrrupting")
-                        self.meta_info["should_interrupt"] = True
-                    elif self.process_interim_results:
-                        self.meta_info["should_interrupt"] = False
-                    logger.info(f"YIELDING TRANSCRIBER BEGIN")
-                    yield create_ws_data_packet("TRANSCRIBER_BEGIN", self.meta_info)
-                    await asyncio.sleep(0.05) #Sleep for 50ms to pass the control to task manager
-                    continue
 
-                transcript = msg['channel']['alternatives'][0]['transcript']
+                if "segments" in msg:
+                    if not self.speech_started:
+                        self.speech_started = True
+                        if self.curr_message != "" and not self.process_interim_results:
+                            logger.info("Current messsage is null and hence inetrrupting")
+                            self.meta_info["should_interrupt"] = True
+                        elif self.process_interim_results:
+                            self.meta_info["should_interrupt"] = False
+                        logger.info(f"YIELDING TRANSCRIBER BEGIN")
+                        yield create_ws_data_packet("TRANSCRIBER_BEGIN", self.meta_info)
+                        await asyncio.sleep(0.05) #Sleep for 50ms to pass the control to task manager
+                        continue
+                    self.whole_segment_list = self.AddAttributes(msg)
+                    self.segments_list = self.AddComited(self.whole_segment_list)
+
+                transcript:str = self.segments_list[-1].get('text')
+                
 
+                # SKIP if you didn't get any data
                 if transcript and len(transcript.strip()) == 0 or transcript == "":
                     continue
 
-                # TODO Remove the need for on_device_vad
-                # If interim message is not true and curr message is null, send a begin signal
-                if curr_message == "" and msg["is_final"] is False:
-                    if not self.on_device_vad:
-                        logger.info("Not on device vad and hence inetrrupting")
-                        self.meta_info["should_interrupt"] = False
-                    yield create_ws_data_packet("TRANSCRIBER_BEGIN", self.meta_info)
-
-                    await asyncio.sleep(0.1)  # Enable taskmanager to interrupt
-
-                if self.process_interim_results == "true":
-                    # If we're not processing interim results
-                    # Yield current transcript
-                    # curr_message = self.__get_speaker_transcript(msg)
-                    # Just yield the current transcript as we do not want to wait for is_final. Is_final is just to make 
-                    curr_message = finalized_transcript + " " + transcript
-                    logger.info(f"Yielding interim-message current_message = {curr_message}")
+                if self.process_interim_results:
+                    self.curr_message = self.finalized_transcript + " " + transcript
+                    logger.info(f"Yielding interim-message current_message = {self.curr_message}")
                     self.meta_info["include_latency"] = False
                     self.meta_info["utterance_end"] = self.__calculate_utterance_end(msg)
                     self.meta_info["time_received"] = time.time()
                     self.meta_info["transcriber_latency"] = self.meta_info["time_received"] - self.meta_info[
                         "utterance_end"]
-                    yield create_ws_data_packet(curr_message, self.meta_info)
+                    yield create_ws_data_packet(self.curr_message, self.meta_info)
                     
                     # If is_final is true simply update the finalized transcript
-                    if  msg["is_final"] is True:
-                        finalized_transcript += " " + transcript  # Just get the whole transcript as there's mismatch at times
-                        self.meta_info["is_final"] = True
 
-                else:
-                    curr_message += " " + transcript
-                    # Process interim results is false and hence we need to be dependent on the endpointing
-                    if msg["speech_final"] or not self.stream:
-                        logger.info(f"Full Transcriber message from speech final {msg}")
-                        yield create_ws_data_packet(curr_message, self.meta_info)
-                        logger.info(f"Yielded {curr_message}")
-                        logger.info('User: {}'.format(curr_message))
-
-                        self.interruption_signalled = False
-                        if self.audio_submitted == True:
-                            logger.info("Transcriber Latency: {} for request id {}".format(
-                                time.time() - self.audio_submission_time, self.current_request_id))
-                            self.meta_info["start_time"] = self.audio_submission_time
-                            self.meta_info["end_time"] = time.time()
-                            self.audio_submitted = False
-                        if curr_message != "":
-                            self.meta_info["include_latency"] = True
-                            self.meta_info["audio_duration"] = msg['start'] + msg['duration']
-                            last_spoken_audio_frame = self.__calculate_utterance_end(msg)
-                            self.meta_info["audio_start_time"] = self.audio_submission_time
-                            transcription_completion_time = time.time()
-                            self.meta_info["transcription_completion_time"] = transcription_completion_time
-                            self.meta_info[
-                                "transcriber_latency"] = transcription_completion_time - last_spoken_audio_frame  # We subtract first audio wav because user started speaking then. In this case we can calculate actual latency taken by the transcriber
-                            self.meta_info["last_vocal_frame_timestamp"] = last_spoken_audio_frame
-                        else:
-                            self.meta_info["include_latency"] = False
-                        self.meta_info["speech_final"] = True
-                        yield create_ws_data_packet("TRANSCRIBER_END", self.meta_info)
-                        curr_message = ""
+                    if  "segments" in msg and self.seg_ptr > -1:
+                        if self.seg_ptr != self.current_seg_ptr:
+                            self.finalized_transcript += " " + self.segments_list[self.seg_ptr].get("text")  # Just get the whole transcript as there's mismatch at times
+                            self.meta_info["is_final"] = True
+                            self.current_seg_ptr = self.seg_ptr
+                            logger.info(f"final segment {self.finalized_transcript}")
+
+                    # if  msg["is_final"] is True:
+                    #     self.finalized_transcript += " " + transcript  # Just get the whole transcript as there's mismatch at times
+                    #     self.meta_info["is_final"] = True
+
+                
 
             except Exception as e:
                 traceback.print_exc()
                 logger.error(f"Error while getting transcriptions {e}")
                 self.interruption_signalled = False
                 yield create_ws_data_packet("TRANSCRIBER_END", self.meta_info)
 
     async def push_to_transcriber_queue(self, data_packet):
         await self.transcriber_output_queue.put(data_packet)
 
-    def hume_connect(self):
-        websocket_url = self.get_hume_ws_url()
-        extra_headers = {
-            "X-Hume-Api-Key": 'nODRW0JT515subWEe4GBGEOyXHoy0xV9ouN5jv6SRoETBolT',
-            "X-Hume-Client-Name": "python_sdk",
-            "X-Hume-Client-Version": "0.5.0",
-        }
-        hume_ws = websockets.connect(websocket_url, extra_headers=extra_headers)
-        return hume_ws
 
+
+    def whisper_connect(self):
+        websocket_url = self.get_whisper_ws_url()
+        whisper_ws:websockets.connect = websockets.connect(websocket_url)
+        
+        return whisper_ws
+
+
+    # UTILS FUNCTION
+    def __calculate_utterance_end(self, data):
+        utterance_end = None
+        if self.segments_list is not None:
+            # TODO: ASK it
+            utterance_end = self.connection_start_time + float(self.whole_segment_list[-1].get('end'))
+            logger.info(f"Final word ended at {utterance_end}")
+        return utterance_end
+    def AddAttributes(self,segments:dict):
+        segments_list = [seg for seg in segments['segments']]
+        for i,seg in enumerate(segments_list):
+            if seg['text'] in self.commited_list:
+                seg["is_final"] = True
+            else:
+                seg["is_final"] = False
+        return segments_list
+    def AddComited(self, segments):
+        if len(segments) > 1 and len(segments) - self.seg_ptr >= 2:
+            self.seg_ptr += 1
+            self.commited_list.append(segments[self.seg_ptr]['text'])
+            segments[self.seg_ptr]["is_final"] = True  
+        return segments
+    def bytes_to_float_array(self,audio_bytes):
+        raw_data = np.frombuffer(buffer=audio_bytes, dtype=np.int16)
+        return raw_data.astype(np.float32) / 32768.0
+
+    # RUNER FUNCTION
     async def run(self):
+        """
+        its start the transcriber function
+        """
         try:
             self.transcription_task = asyncio.create_task(self.transcribe())
         except Exception as e:
             logger.error(f"not working {e}")
-    def __calculate_utterance_end(self, data):
-        utterance_end = None
-        if 'channel' in data and 'alternatives' in data['channel']:
-            for alternative in data['channel']['alternatives']:
-                if 'words' in alternative:
-                    final_word = alternative['words'][-1]
-                    utterance_end = self.connection_start_time + final_word['end']
-                    logger.info(f"Final word ended at {utterance_end}")
-        return utterance_end
+    
+    
 
+    
+    # TRANSCRIBER
     async def transcribe(self):
         logger.info(f"STARTED TRANSCRIBING")
         try:
-            async with self.hume_connect() as hume_ws:
+            async with self.whisper_connect() as whisper_ws:
+                self.current_request_id = self.generate_request_id()
+                await whisper_ws.send(json.dumps(
+                    {
+                        "uid": self.current_request_id,
+                        "language": "en",
+                        "task": "translate",
+                        "model": "small",
+                        "use_vad": True
+                    }
+                ))
+                logger.info(f"the server is connect to WHISPER {await whisper_ws.recv()}")
                 if self.stream:
-                    self.sender_task = asyncio.create_task(self.sender_stream(hume_ws))
-                    #self.heartbeat_task = asyncio.create_task(self.send_heartbeat(hume_ws))
-                    async for message in self.receiver(hume_ws):
+                    self.sender_task = asyncio.create_task(self.sender_stream(whisper_ws))
+                    # self.heartbeat_task = asyncio.create_task(self.send_heartbeat(whisper_ws))
+                    self.heartbeat_task = whisper_ws
+                    async for message in self.receiver(whisper_ws):
                         if self.connection_on:
                             await self.push_to_transcriber_queue(message)
                         else:
                             logger.info("closing the deepgram connection")
-                            await self._close(hume_ws, data={"type": "CloseStream"})
+                            await self._close(whisper_ws, data={"type": "CloseStream"})
                 else:
                     async for message in self.sender():
                         await self.push_to_transcriber_queue(message)
 
             await self.push_to_transcriber_queue(create_ws_data_packet("transcriber_connection_closed", self.meta_info))
         except Exception as e:
-            logger.error(f"Error in transcribe: {e}")
+            logger.error(f"Error in transcribe: {e}")
+
+
+
+
```

### Comparing `bolna-0.7.7/bolna.egg-info/PKG-INFO` & `bolna-0.7.8/bolna.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bolna
-Version: 0.7.7
+Version: 0.7.8
 Author-email: Prateek Sachan <ps@prateeksachan.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -693,15 +693,15 @@
 Requires-Dist: semantic-router==0.0.37
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 
 <h1 align="center">
 </h1>
 <p align="center">
-  <p align="center"><b>End-to-end open-source voice agents platform</b>: Quickly build LLM based voice driven conversational applications</p>
+  <p align="center"><b>End-to-end open-source voice agents platform</b>: Quickly build voice firsts conversational assistants through a json. </p>
 </p>
 
 <h4 align="center">
   <a href="https://discord.gg/yDfcqreByj">Discord</a> |
   <a href="https://docs.bolna.dev">Docs</a> |
   <a href="https://bolna.dev">Website</a>
 </h4>
@@ -744,42 +744,127 @@
 The setup consists of four containers:
 
 1. Twilio web server: for initiating the calls one will need to set up a [Twilio account]([https://www.twilio.com/docs/usage/tutorials/how-to-use-your-free-trial-account](https://www.twilio.com/docs/messaging/guides/how-to-use-your-free-trial-account))
 2. Bolna server: for creating and handling agents 
 3. `ngrok`: for tunneling. One will need to add the `authtoken` to `ngrok-config.yml`
 4. `redis`: for persisting agents & prompt data
 
-Running `docker-compose up --build` will use the `.env` as the environment file.
+Use docker to build the images using `.env` file as the environment file and run them locally
+1. `docker-compose build --no-cache`: rebuild images
+2. `docker-compose up`: run the build images
 
 Once the docker containers are up, you can now start to create your agents and instruct them to initiate calls.
 
 
 
 ## Creating your agent and invoking calls
 Once you have the above docker setup and running, you can create agents and initiate calls.
-1. Refer to the official [`Agent` API](https://docs.bolna.dev/api-reference/agent/create) to create an agent
-2. Initiate a call via API similar to [`Call` API](https://docs.bolna.dev/api-reference/calls/make) to receive a call
+1. Use the below payload to create an Agent via `http://localhost:5001/agent`
+
+<details>
+<summary>Agent Payload</summary><br>
+
+```yaml
+{
+    "agent_config": {
+        "agent_name": "Alfred",
+        "agent_type": "other",
+        "agent_welcome_message": "Welcome",
+        "tasks": [
+            {
+                "task_type": "conversation",
+                "toolchain": {
+                    "execution": "parallel",
+                    "pipelines": [
+                        [
+                            "transcriber",
+                            "llm",
+                            "synthesizer"
+                        ]
+                    ]
+                },
+                "tools_config": {
+                    "input": {
+                        "format": "pcm",
+                        "provider": "twilio"
+                    },
+                    "llm_agent": {
+                        "agent_flow_type": "streaming",
+                        "family": "openai",
+                        "request_json": true,
+                        "model": "gpt-3.5-turbo-16k",
+                        "use_fallback": true
+                    },
+                    "output": {
+                        "format": "pcm",
+                        "provider": "twilio"
+                    },
+                    "synthesizer": {
+                        "audio_format": "wav",
+                        "provider": "elevenlabs",
+                        "stream": true,
+                        "provider_config": {
+                            "voice": "Meera - high quality, emotive",
+                            "model": "eleven_multilingual_v2",
+                            "voice_id": "TTa58Hl9lmhnQEvhp1WM"
+                        },
+                        "buffer_size": 100.0
+                    },
+                    "transcriber": {
+                        "encoding": "linear16",
+                        "language": "en",
+                        "model": "deepgram",
+                        "stream": true
+                    }
+                },
+                "task_config": {
+                    "hangup_after_silence": 30.0
+                }
+            }
+        ]
+    },
+    "agent_prompts": {
+        "task_1": {
+            "system_prompt": "Ask if they are coming for party tonight"
+        }
+    }
+}
+```
+</details>
+
+2. The response of the previous API will return a uuid as the `agent_id`. Use this `agent_id` to initiate a call via the telephony server running on `8001` port at `http://localhost:8001/call`
+
+<details>
+<summary>Call Payload</summary><br>
+
+```yaml
+{
+    "agent_id": "4c19700b-227c-4c2d-8bgf-42dfe4b240fc",
+    "recipient_phone_number": "+19876543210",
+}
+```
+</details>
 
 
 ## Using your own providers
 You can populate the `.env` file to use your own keys for providers.
 
-<details open>
+<details>
 
 <summary>ASR Providers</summary><br>
 These are the current supported ASRs Providers:
 
 | Provider     | Environment variable to be added in `.env` file |
 |--------------|-------------------------------------------------|
 | Deepgram     | `DEEPGRAM_AUTH_TOKEN`                           |
 
 </details>
 &nbsp;<br>
 
-<details open>
+<details>
 <summary>LLM Providers</summary><br>
 Bolna uses LiteLLM package to support multiple LLM integrations.
 
 These are the current supported LLM Provider Family:
 https://github.com/bolna-ai/bolna/blob/c8a0d1428793d4df29133119e354bc2f85a7ca76/bolna/providers.py#L19-L28
 
 For LiteLLM based LLMs, add either of the following to the `.env` file depending on your use-case:<br><br>
@@ -789,15 +874,15 @@
 
 For LLMs hosted via VLLM, add the following to the `.env` file:<br>
 `VLLM_SERVER_BASE_URL`: URL of the hosted LLM using VLLM
 
 </details>
 &nbsp;<br>
 
-<details open>
+<details>
 
 <summary>TTS Providers</summary><br>
 These are the current supported TTS Providers:
 https://github.com/bolna-ai/bolna/blob/c8a0d1428793d4df29133119e354bc2f85a7ca76/bolna/providers.py#L7-L14
 
 | Provider   | Environment variable to be added in `.env` file  |
 |------------|--------------------------------------------------|
```

### Comparing `bolna-0.7.7/bolna.egg-info/SOURCES.txt` & `bolna-0.7.8/bolna.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 bolna/agent_manager/task_manager.py
 bolna/agent_types/__init__.py
 bolna/agent_types/base_agent.py
 bolna/agent_types/contextual_conversational_agent.py
 bolna/agent_types/extraction_agent.py
 bolna/agent_types/graph_based_conversational_agent.py
 bolna/agent_types/summarization_agent.py
-bolna/agent_types/zapier_agent.py
+bolna/agent_types/webhook_agent.py
 bolna/helpers/__init__.py
 bolna/helpers/analytics_helpers.py
 bolna/helpers/cache_helpers.py
 bolna/helpers/logger_config.py
 bolna/helpers/utils.py
 bolna/helpers/vad.py
 bolna/input_handlers/__init__.py
@@ -53,11 +53,11 @@
 bolna/synthesizer/deepgram_synthesizer.py
 bolna/synthesizer/elevenlabs_synthesizer.py
 bolna/synthesizer/fourie_synthesizer.py
 bolna/synthesizer/openai_synthesizer.py
 bolna/synthesizer/polly_synthesizer.py
 bolna/synthesizer/xtts_synthesizer.py
 bolna/transcriber/__init__.py
-bolna/transcriber/azure_transcriber.py
 bolna/transcriber/base_transcriber.py
 bolna/transcriber/deepgram_transcriber.py
-bolna/transcriber/hume_transcriber.py
+bolna/transcriber/hume_transcriber.py
+bolna/transcriber/whisper_transcriber.py
```

### Comparing `bolna-0.7.7/pyproject.toml` & `bolna-0.7.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bolna"
-version = "0.7.7"
+version = "0.7.8"
 readme = "README.md"
 authors = [
     { name = "Prateek Sachan", email = "ps@prateeksachan.com" }
 ]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU Affero General Public License v3",
@@ -26,15 +26,15 @@
 [tool.setuptools]
 package-dir = {"bolna" = "bolna"}
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
 [tool.bumpver]
-current_version = "0.7.7"
+current_version = "0.7.8"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump bolna version {old_version} -> {new_version}"
 tag_message = "bolna-{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

