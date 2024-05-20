# Comparing `tmp/llama_cpp_agent-0.2.7.tar.gz` & `tmp/llama_cpp_agent-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_cpp_agent-0.2.7.tar", last modified: Tue May 14 05:39:24 2024, max compression
+gzip compressed data, was "llama_cpp_agent-0.2.8.tar", last modified: Mon May 20 21:19:52 2024, max compression
```

## Comparing `llama_cpp_agent-0.2.7.tar` & `llama_cpp_agent-0.2.8.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:39:24.966807 llama_cpp_agent-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-05-14 05:39:24.962807 llama_cpp_agent-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9413 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/ReadMe.md
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 05:39:24.966807 llama_cpp_agent-0.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:39:24.954807 llama_cpp_agent-0.2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:39:24.958807 llama_cpp_agent-0.2.7/src/llama_cpp_agent/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:39:24.958807 llama_cpp_agent-0.2.7/src/llama_cpp_agent/agent_memory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/agent_memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/agent_memory/core_memory_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/agent_memory/event_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/agent_memory/event_memory_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     9662 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/agent_memory/memory_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/agent_memory/retrieval_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    12331 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:39:24.962807 llama_cpp_agent-0.2.7/src/llama_cpp_agent/chat_history/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/chat_history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/chat_history/basic_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/chat_history/chat_history_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/chat_history/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)    10519 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/function_calling.py
--rw-r--r--   0 runner    (1001) docker     (127)    12312 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/function_calling_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:39:24.962807 llama_cpp_agent-0.2.7/src/llama_cpp_agent/gbnf_grammar_generator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/gbnf_grammar_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51567 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/hermes_2_pro_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:39:24.962807 llama_cpp_agent-0.2.7/src/llama_cpp_agent/json_schema_generator/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/json_schema_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11406 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/json_schema_generator/schema_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21017 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/llm_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:39:24.962807 llama_cpp_agent-0.2.7/src/llama_cpp_agent/llm_documentation/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/llm_documentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18378 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/llm_documentation/documentation_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:39:24.962807 llama_cpp_agent-0.2.7/src/llama_cpp_agent/llm_output_settings/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/llm_output_settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32249 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/llm_output_settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/llm_prompt_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    11448 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/messages_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/mixtral_8x22b_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/prompt_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:39:24.962807 llama_cpp_agent-0.2.7/src/llama_cpp_agent/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/providers/llama_cpp_python.py
--rw-r--r--   0 runner    (1001) docker     (127)    13424 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/providers/llama_cpp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/providers/provider_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/providers/tgi_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/providers/vllm_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:39:24.962807 llama_cpp_agent-0.2.7/src/llama_cpp_agent/rag/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/rag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/rag/rag_colbert_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6920 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/structured_output_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-14 05:39:20.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent/text_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 05:39:24.962807 llama_cpp_agent-0.2.7/src/llama_cpp_agent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-05-14 05:39:24.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-14 05:39:24.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 05:39:24.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-14 05:39:24.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 05:39:24.000000 llama_cpp_agent-0.2.7/src/llama_cpp_agent.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:52.549673 llama_cpp_agent-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-05-20 21:19:52.549673 llama_cpp_agent-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9413 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/ReadMe.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 21:19:52.549673 llama_cpp_agent-0.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:52.537673 llama_cpp_agent-0.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:52.541673 llama_cpp_agent-0.2.8/src/llama_cpp_agent/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:52.545673 llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/core_memory_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/event_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/event_memory_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9662 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/memory_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/retrieval_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12331 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:52.545673 llama_cpp_agent-0.2.8/src/llama_cpp_agent/chat_history/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/chat_history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/chat_history/basic_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/chat_history/chat_history_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/chat_history/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10519 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/function_calling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12312 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/function_calling_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:52.545673 llama_cpp_agent-0.2.8/src/llama_cpp_agent/gbnf_grammar_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/gbnf_grammar_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51567 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/hermes_2_pro_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:52.545673 llama_cpp_agent-0.2.8/src/llama_cpp_agent/json_schema_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/json_schema_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11406 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/json_schema_generator/schema_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21328 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/llm_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:52.545673 llama_cpp_agent-0.2.8/src/llama_cpp_agent/llm_documentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/llm_documentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/llm_documentation/documentation_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:52.545673 llama_cpp_agent-0.2.8/src/llama_cpp_agent/llm_output_settings/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/llm_output_settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32298 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/llm_output_settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/llm_prompt_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11425 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/messages_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/mixtral_8x22b_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/prompt_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:52.545673 llama_cpp_agent-0.2.8/src/llama_cpp_agent/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/providers/llama_cpp_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13424 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/providers/llama_cpp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/providers/provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/providers/tgi_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/providers/vllm_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:52.545673 llama_cpp_agent-0.2.8/src/llama_cpp_agent/rag/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/rag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/rag/rag_colbert_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6920 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/structured_output_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/text_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:52.549673 llama_cpp_agent-0.2.8/src/llama_cpp_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-05-20 21:19:52.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-20 21:19:52.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:19:52.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-20 21:19:52.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 21:19:52.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent.egg-info/top_level.txt
```

### Comparing `llama_cpp_agent-0.2.7/LICENSE` & `llama_cpp_agent-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/PKG-INFO` & `llama_cpp_agent-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-cpp-agent
-Version: 0.2.7
+Version: 0.2.8
 Summary: A framework for building LLM based AI agents with llama.cpp.
 Author-email: Maximilian Winter <maximilian.winter.91@gmail.com>
 Project-URL: Homepage, https://github.com/Maximilian-Winter/llama-cpp-agent
 Project-URL: Bug Tracker, https://github.com/Maximilian-Winter/llama-cpp-agent/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llama_cpp_agent-0.2.7/ReadMe.md` & `llama_cpp_agent-0.2.8/ReadMe.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/pyproject.toml` & `llama_cpp_agent-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [  "setuptools>=42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llama-cpp-agent"
-version = "0.2.7"
+version = "0.2.8"
 description = "A framework for building LLM based AI agents with llama.cpp."
 
 readme = "ReadMe.md"
 dependencies = [
     "llama-cpp-python>=0.2.60",
     "pydantic>=2.5.3",
     "requests>=2.31.0",
```

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/agent_memory/core_memory_manager.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/core_memory_manager.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/agent_memory/event_memory.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/event_memory.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/agent_memory/event_memory_manager.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/event_memory_manager.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/agent_memory/memory_tools.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/memory_tools.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/agent_memory/retrieval_memory.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/retrieval_memory.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/chain.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/chain.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/chat_history/basic_chat_history.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/chat_history/basic_chat_history.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/chat_history/chat_history_base.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/chat_history/chat_history_base.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/chat_history/messages.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/chat_history/messages.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/function_calling.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/function_calling.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/function_calling_agent.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/function_calling_agent.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/hermes_2_pro_agent.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/hermes_2_pro_agent.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/json_schema_generator/schema_generator.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/json_schema_generator/schema_generator.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/llm_agent.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/llm_agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -166,16 +166,17 @@
                 llm_samplings_settings=llm_sampling_settings,
             )
 
             def stream_results():
                 full_response_stream = ""
                 for out_stream in completion:
                     out_text = out_stream["choices"][0]["text"]
-                    full_response_stream += text
+                    full_response_stream += out_text
                     yield out_text
+
                 return structured_output_settings.handle_structured_output(
                     full_response_stream
                 )
 
             if llm_sampling_settings.is_streaming():
                 full_response = ""
                 if returns_streaming_generator:
@@ -280,22 +281,24 @@
         )
 
         def stream_results():
             full_response_stream = ""
             for out_stream in completion:
                 out_text = out_stream["choices"][0]["text"]
                 if out_text != self.messages_formatter.eos_token:
-                    full_response_stream += text
+                    full_response_stream += out_text
                     yield out_text
-            self.last_response = full_response
+            if prompt_suffix:
+                full_response_stream = prompt_suffix + full_response_stream
+            self.last_response = full_response_stream
             if add_response_to_chat_history:
                 chat_history.add_message(
                     {
                         "role": response_role,
-                        "content": full_response,
+                        "content": full_response_stream,
                     }
                 )
             return structured_output_settings.handle_structured_output(
                 full_response_stream
             )
 
         if self.provider:
@@ -315,14 +318,16 @@
                             print(text, end="")
                 if streaming_callback is not None:
                     streaming_callback(
                         StreamingResponse(text="", is_last_response=True)
                     )
                 if print_output or self.debug_output:
                     print("")
+                if prompt_suffix:
+                    full_response = prompt_suffix + full_response
                 self.last_response = full_response
                 if add_response_to_chat_history:
                     chat_history.add_message(
                         {
                             "role": response_role,
                             "content": full_response,
                         }
@@ -333,14 +338,16 @@
                 )
             else:
                 text = completion["choices"][0]["text"]
                 if text.strip().endswith(self.messages_formatter.eos_token):
                     text = text.replace(self.messages_formatter.eos_token, "")
                 if print_output or self.debug_output:
                     print(text)
+                if prompt_suffix:
+                    text = prompt_suffix + text
                 self.last_response = text
                 if add_response_to_chat_history:
                     chat_history.add_message(
                         {
                             "role": response_role,
                             "content": text,
                         }
```

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/llm_documentation/documentation_generation.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/llm_documentation/documentation_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,32 +8,33 @@
 
 
 def generate_markdown_documentation(
     pydantic_models: list[type[BaseModel]],
     model_prefix="Model",
     fields_prefix="Fields",
     documentation_with_field_description=True,
+    ordered_json_mode=False,
 ) -> str:
     """
     Generate markdown documentation for a list of Pydantic models.
 
     Args:
         pydantic_models (list[type[BaseModel]]): list of Pydantic model classes.
         model_prefix (str): Prefix for the model section.
         fields_prefix (str): Prefix for the fields section.
         documentation_with_field_description (bool): Include field descriptions in the documentation.
 
     Returns:
         str: Generated text documentation.
     """
-    documentation = "## Functions\n\n"
+    documentation = ""
     pyd_models = [(model, True) for model in pydantic_models]
     for model, add_prefix in pyd_models:
         if add_prefix:
-            documentation += f"### {model_prefix}: {model.__name__}\n"
+            documentation += f"### {model_prefix} {model.__name__}\n"
         else:
             documentation += f"### {model.__name__}\n"
 
         # Handling multi-line model description with proper indentation
 
         class_doc = getdoc(model)
         base_class_doc = getdoc(BaseModel)
@@ -45,14 +46,15 @@
 
         if add_prefix:
             # Indenting the fields section
             documentation += f"{fields_prefix}:\n"
         else:
             documentation += f"Fields:\n"
         if isclass(model) and issubclass(model, BaseModel):
+            count = 1
             for name, field_type in model.__annotations__.items():
                 # if name == "markdown_code_block":
                 #    continue
                 if get_origin(field_type) == list:
                     element_type = get_args(field_type)[0]
                     if isclass(element_type) and issubclass(element_type, BaseModel):
                         pyd_models.append((element_type, False))
@@ -60,15 +62,17 @@
                     element_types = get_args(field_type)
                     for element_type in element_types:
                         if isclass(element_type) and issubclass(
                             element_type, BaseModel
                         ):
                             pyd_models.append((element_type, False))
                 documentation += generate_field_markdown(
-                    name,
+                    name
+                    if not ordered_json_mode
+                    else "{:03}".format(count) + "_" + name,
                     field_type,
                     model,
                     documentation_with_field_description=documentation_with_field_description,
                 )
             if add_prefix:
                 if documentation.endswith(f"{fields_prefix}:\n"):
                     documentation += "none\n"
@@ -105,15 +109,15 @@
         model (type[BaseModel]): Pydantic model class.
         depth (int): Indentation depth in the documentation.
         documentation_with_field_description (bool): Include field descriptions in the documentation.
 
     Returns:
         str: Generated text documentation for the field.
     """
-    indent = "  " * depth
+    indent = ""
 
     field_info = model.model_fields.get(field_name)
     field_description = (
         field_info.description if field_info and field_info.description else ""
     )
 
     if get_origin(field_type) == list:
```

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/llm_output_settings/settings.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/llm_output_settings/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pydantic import BaseModel, Field
 
 from llama_cpp_agent.function_calling import LlamaCppFunctionTool
 from llama_cpp_agent.gbnf_grammar_generator.gbnf_grammar_from_pydantic_models import (
     generate_gbnf_grammar_from_pydantic_models,
 )
 from llama_cpp_agent.json_schema_generator.schema_generator import generate_json_schemas
-from llama_cpp_agent.llm_documentation import generate_text_documentation
+from llama_cpp_agent.llm_documentation import generate_text_documentation, generate_markdown_documentation
 from llama_cpp_agent.output_parser import parse_json_response
 
 
 class LlmStructuredOutputType(Enum):
     """
     Enum for defining different types of structured outputs that can be generated by a Language Model.
     """
@@ -376,30 +376,30 @@
         ):
             json_schema_mode = True
         if self.output_type == LlmStructuredOutputType.no_structured_output:
             raise NotImplementedError(
                 "LlmOutputType: no_structured_output not supported for structured output and function calling!"
             )
         elif self.output_type == LlmStructuredOutputType.object_instance:
-            return generate_text_documentation(
+            return generate_markdown_documentation(
                 self.pydantic_models, ordered_json_mode=json_schema_mode
             ).strip()
         elif self.output_type == LlmStructuredOutputType.list_of_objects:
-            return generate_text_documentation(
+            return generate_markdown_documentation(
                 self.pydantic_models, ordered_json_mode=json_schema_mode
             ).strip()
         elif self.output_type == LlmStructuredOutputType.function_calling:
-            return generate_text_documentation(
+            return generate_markdown_documentation(
                 [tool.model for tool in self.function_tools],
                 model_prefix="Function",
                 fields_prefix="Parameters",
                 ordered_json_mode=json_schema_mode,
             ).strip()
         elif self.output_type == LlmStructuredOutputType.parallel_function_calling:
-            return generate_text_documentation(
+            return generate_markdown_documentation(
                 [tool.model for tool in self.function_tools],
                 model_prefix="Function",
                 fields_prefix="Parameters",
                 ordered_json_mode=json_schema_mode,
             ).strip()
 
     def get_gbnf_grammar(self):
```

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/llm_prompt_template.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/llm_prompt_template.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/messages_formatter.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/messages_formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             elif role == Roles.tool:
                 formatted_messages += self._format_tool_message(content)
                 last_role = Roles.tool
 
         return self._format_response(formatted_messages, last_role, response_role)
 
     def _format_message_content(self, content: str, role: Roles) -> str:
-        if self.strip_prompt and role != Roles.tool:
+        if self.strip_prompt:
             return content.strip()
         return content
 
     def _format_system_message(self, content: str) -> str:
         formatted_message = self.prompt_markers[Roles.system].start + content + self.prompt_markers[Roles.system].end
         self.added_system_prompt = True
         if self.include_sys_prompt_in_first_user_message:
```

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/mixtral_8x22b_agent.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/mixtral_8x22b_agent.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/output_parser.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/prompt_templates.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/prompt_templates.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/prompts.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/providers/llama_cpp_python.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/providers/llama_cpp_python.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/providers/llama_cpp_server.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/providers/llama_cpp_server.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/providers/provider_base.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/providers/provider_base.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/providers/tgi_server.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/providers/tgi_server.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/providers/vllm_server.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/providers/vllm_server.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/rag/rag_colbert_reranker.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/rag/rag_colbert_reranker.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/structured_output_agent.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/structured_output_agent.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent/text_utils.py` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent/text_utils.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent.egg-info/PKG-INFO` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-cpp-agent
-Version: 0.2.7
+Version: 0.2.8
 Summary: A framework for building LLM based AI agents with llama.cpp.
 Author-email: Maximilian Winter <maximilian.winter.91@gmail.com>
 Project-URL: Homepage, https://github.com/Maximilian-Winter/llama-cpp-agent
 Project-URL: Bug Tracker, https://github.com/Maximilian-Winter/llama-cpp-agent/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llama_cpp_agent-0.2.7/src/llama_cpp_agent.egg-info/SOURCES.txt` & `llama_cpp_agent-0.2.8/src/llama_cpp_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

