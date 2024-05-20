# Comparing `tmp/eras-0.2.3.tar.gz` & `tmp/eras-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eras-0.2.3.tar", last modified: Sun May 19 23:58:39 2024, max compression
+gzip compressed data, was "eras-0.2.4.tar", last modified: Mon May 20 00:00:26 2024, max compression
```

## Comparing `eras-0.2.3.tar` & `eras-0.2.4.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 23:58:39.439919 eras-0.2.3/
--rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.2.3/LICENSE
--rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.2.3/MANIFEST.in
--rw-r--r--   0 jason      (501) staff       (20)      706 2024-05-19 23:58:39.439603 eras-0.2.3/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)       82 2024-05-19 18:38:38.000000 eras-0.2.3/README.md
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 23:58:39.425842 eras-0.2.3/eras/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.2.3/eras/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 23:58:39.427280 eras-0.2.3/eras/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.2.3/eras/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 23:58:39.428317 eras-0.2.3/eras/agents/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.2.3/eras/agents/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 23:58:39.429813 eras-0.2.3/eras/agents/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.2.3/eras/agents/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.2.3/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.2.3/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.2.3/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.2.3/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     5501 2024-05-19 20:31:04.000000 eras-0.2.3/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.2.3/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.2.3/eras/agents/llama_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.2.3/eras/agents/llama_terminal_command_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.2.3/eras/agents/llm_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     4745 2024-05-19 23:25:55.000000 eras-0.2.3/eras/agents/terminal_llama_agent.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 23:58:39.430399 eras-0.2.3/eras/config/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.2.3/eras/config/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 23:58:39.431031 eras-0.2.3/eras/config/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.2.3/eras/config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1478 2024-05-19 19:36:31.000000 eras-0.2.3/eras/config/__pycache__/config.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.2.3/eras/config/__pycache__/config.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)      442 2024-05-19 19:31:13.000000 eras-0.2.3/eras/config/config.py
--rw-r--r--   0 jason      (501) staff       (20)     4671 2024-05-19 23:58:15.000000 eras-0.2.3/eras/config/post_install.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 23:58:39.431395 eras-0.2.3/eras/decorators/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.2.3/eras/decorators/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 23:58:39.431815 eras-0.2.3/eras/decorators/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.2.3/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.2.3/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.2.3/eras/decorators/chatgpt_tool_data.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 23:58:39.432388 eras-0.2.3/eras/factories/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.2.3/eras/factories/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 23:58:39.433684 eras-0.2.3/eras/factories/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.2.3/eras/factories/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.2.3/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.2.3/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3256 2024-05-19 20:31:34.000000 eras-0.2.3/eras/factories/__pycache__/message_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.2.3/eras/factories/__pycache__/message_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.2.3/eras/factories/function_details_factory.py
--rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.2.3/eras/factories/message_factory.py
--rw-r--r--   0 jason      (501) staff       (20)      670 2024-05-19 23:14:52.000000 eras-0.2.3/eras/main.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 23:58:39.434690 eras-0.2.3/eras/models/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.2.3/eras/models/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 23:58:39.436150 eras-0.2.3/eras/models/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.2.3/eras/models/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4345 2024-05-19 20:31:18.000000 eras-0.2.3/eras/models/__pycache__/conversation.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.2.3/eras/models/__pycache__/conversation.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1453 2024-05-19 20:34:55.000000 eras-0.2.3/eras/models/__pycache__/function_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.2.3/eras/models/__pycache__/function_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.2.3/eras/models/__pycache__/message.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.2.3/eras/models/__pycache__/message.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.2.3/eras/models/conversation.py
--rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.2.3/eras/models/function_details.py
--rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.2.3/eras/models/message.py
--rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.2.3/eras/models/transaction.py
--rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-19 02:17:49.000000 eras-0.2.3/eras/run.ipynb
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 23:58:39.436536 eras-0.2.3/eras/services/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.2.3/eras/services/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 23:58:39.437168 eras-0.2.3/eras/services/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.2.3/eras/services/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2837 2024-05-19 20:31:04.000000 eras-0.2.3/eras/services/__pycache__/shell_command_service.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.2.3/eras/services/__pycache__/shell_command_service.cpython-39.pyc
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 23:58:39.437956 eras-0.2.3/eras/services/llm_callable_functions/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.2.3/eras/services/llm_callable_functions/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 23:58:39.439208 eras-0.2.3/eras/services/llm_callable_functions/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.2.3/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.2.3/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.2.3/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.2.3/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.2.3/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.2.3/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.2.3/eras/services/llm_callable_functions/callable_function_service_base.py
--rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.2.3/eras/services/llm_callable_functions/terminal_command.py
--rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.2.3/eras/services/llm_callable_functions/user_details.py
--rw-r--r--   0 jason      (501) staff       (20)     2046 2024-05-19 23:31:13.000000 eras-0.2.3/eras/services/shell_command_service.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 23:58:39.427075 eras-0.2.3/eras.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)      706 2024-05-19 23:58:39.000000 eras-0.2.3/eras.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     3200 2024-05-19 23:58:39.000000 eras-0.2.3/eras.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-19 23:58:39.000000 eras-0.2.3/eras.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-19 23:58:39.000000 eras-0.2.3/eras.egg-info/entry_points.txt
--rw-r--r--   0 jason      (501) staff       (20)       68 2024-05-19 23:58:39.000000 eras-0.2.3/eras.egg-info/requires.txt
--rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-19 23:58:39.000000 eras-0.2.3/eras.egg-info/top_level.txt
--rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-19 23:58:39.439991 eras-0.2.3/setup.cfg
--rw-r--r--   0 jason      (501) staff       (20)     2549 2024-05-19 23:56:26.000000 eras-0.2.3/setup.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:00:26.757523 eras-0.2.4/
+-rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.2.4/LICENSE
+-rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.2.4/MANIFEST.in
+-rw-r--r--   0 jason      (501) staff       (20)      706 2024-05-20 00:00:26.757202 eras-0.2.4/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)       82 2024-05-19 18:38:38.000000 eras-0.2.4/README.md
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:00:26.742541 eras-0.2.4/eras/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.2.4/eras/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:00:26.744475 eras-0.2.4/eras/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.2.4/eras/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:00:26.745555 eras-0.2.4/eras/agents/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.2.4/eras/agents/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:00:26.747217 eras-0.2.4/eras/agents/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.2.4/eras/agents/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.2.4/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.2.4/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.2.4/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.2.4/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     5501 2024-05-19 20:31:04.000000 eras-0.2.4/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.2.4/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.2.4/eras/agents/llama_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.2.4/eras/agents/llama_terminal_command_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.2.4/eras/agents/llm_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     4745 2024-05-19 23:25:55.000000 eras-0.2.4/eras/agents/terminal_llama_agent.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:00:26.747825 eras-0.2.4/eras/config/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.2.4/eras/config/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:00:26.748477 eras-0.2.4/eras/config/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.2.4/eras/config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1478 2024-05-19 19:36:31.000000 eras-0.2.4/eras/config/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.2.4/eras/config/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      442 2024-05-19 19:31:13.000000 eras-0.2.4/eras/config/config.py
+-rw-r--r--   0 jason      (501) staff       (20)     4716 2024-05-20 00:00:06.000000 eras-0.2.4/eras/config/post_install.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:00:26.748848 eras-0.2.4/eras/decorators/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.2.4/eras/decorators/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:00:26.749263 eras-0.2.4/eras/decorators/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.2.4/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.2.4/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.2.4/eras/decorators/chatgpt_tool_data.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:00:26.749837 eras-0.2.4/eras/factories/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.2.4/eras/factories/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:00:26.750905 eras-0.2.4/eras/factories/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.2.4/eras/factories/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.2.4/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.2.4/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3256 2024-05-19 20:31:34.000000 eras-0.2.4/eras/factories/__pycache__/message_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.2.4/eras/factories/__pycache__/message_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.2.4/eras/factories/function_details_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.2.4/eras/factories/message_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)      670 2024-05-19 23:14:52.000000 eras-0.2.4/eras/main.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:00:26.751912 eras-0.2.4/eras/models/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.2.4/eras/models/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:00:26.753388 eras-0.2.4/eras/models/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.2.4/eras/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4345 2024-05-19 20:31:18.000000 eras-0.2.4/eras/models/__pycache__/conversation.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.2.4/eras/models/__pycache__/conversation.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1453 2024-05-19 20:34:55.000000 eras-0.2.4/eras/models/__pycache__/function_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.2.4/eras/models/__pycache__/function_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.2.4/eras/models/__pycache__/message.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.2.4/eras/models/__pycache__/message.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.2.4/eras/models/conversation.py
+-rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.2.4/eras/models/function_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.2.4/eras/models/message.py
+-rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.2.4/eras/models/transaction.py
+-rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-19 02:17:49.000000 eras-0.2.4/eras/run.ipynb
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:00:26.753786 eras-0.2.4/eras/services/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.2.4/eras/services/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:00:26.754569 eras-0.2.4/eras/services/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.2.4/eras/services/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2837 2024-05-19 20:31:04.000000 eras-0.2.4/eras/services/__pycache__/shell_command_service.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.2.4/eras/services/__pycache__/shell_command_service.cpython-39.pyc
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:00:26.755489 eras-0.2.4/eras/services/llm_callable_functions/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.2.4/eras/services/llm_callable_functions/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:00:26.756796 eras-0.2.4/eras/services/llm_callable_functions/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.2.4/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.2.4/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.2.4/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.2.4/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.2.4/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.2.4/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.2.4/eras/services/llm_callable_functions/callable_function_service_base.py
+-rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.2.4/eras/services/llm_callable_functions/terminal_command.py
+-rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.2.4/eras/services/llm_callable_functions/user_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     2046 2024-05-19 23:31:13.000000 eras-0.2.4/eras/services/shell_command_service.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:00:26.744222 eras-0.2.4/eras.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)      706 2024-05-20 00:00:26.000000 eras-0.2.4/eras.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     3200 2024-05-20 00:00:26.000000 eras-0.2.4/eras.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-20 00:00:26.000000 eras-0.2.4/eras.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-20 00:00:26.000000 eras-0.2.4/eras.egg-info/entry_points.txt
+-rw-r--r--   0 jason      (501) staff       (20)       68 2024-05-20 00:00:26.000000 eras-0.2.4/eras.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-20 00:00:26.000000 eras-0.2.4/eras.egg-info/top_level.txt
+-rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-20 00:00:26.757592 eras-0.2.4/setup.cfg
+-rw-r--r--   0 jason      (501) staff       (20)     2549 2024-05-20 00:00:14.000000 eras-0.2.4/setup.py
```

### Comparing `eras-0.2.3/PKG-INFO` & `eras-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.2.3
+Version: 0.2.4
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eras-0.2.3/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc` & `eras-0.2.4/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc` & `eras-0.2.4/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc` & `eras-0.2.4/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc` & `eras-0.2.4/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc` & `eras-0.2.4/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc` & `eras-0.2.4/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/agents/llama_functions_agent.py` & `eras-0.2.4/eras/agents/llama_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/agents/llama_terminal_command_functions_agent.py` & `eras-0.2.4/eras/agents/llama_terminal_command_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/agents/llm_functions_agent.py` & `eras-0.2.4/eras/agents/llm_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/agents/terminal_llama_agent.py` & `eras-0.2.4/eras/agents/terminal_llama_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/config/__pycache__/config.cpython-311.pyc` & `eras-0.2.4/eras/config/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/config/__pycache__/config.cpython-39.pyc` & `eras-0.2.4/eras/config/__pycache__/config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/config/post_install.py` & `eras-0.2.4/eras/config/post_install.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,16 @@
         openai_key = input("Please enter your OpenAI API key (ERAS_OPENAI_KEY): ").strip()
         if not openai_key:
             print("Error: OpenAI API key cannot be empty.")
             sys.exit(1)
         env_var_command = f"export ERAS_OPENAI_KEY='{openai_key}'"
         os.environ['ERAS_OPENAI_KEY'] = openai_key # DO THIS FOR THE FIRST INSTALL !!!!
         add_env_var_to_shell(env_var_command)
-        print("Environment variable 'ERAS_OPENAI_KEY' added to shell configuration files.")
-        print('Please run source ~/.zshrc or open a new terminal window.')
+        print("Environment variable 'ERAS_OPENAI_KEY' added to shell configuration files.  Reloading .zshrc in this terminal window.")
+        # print('Please run source ~/.zshrc or open a new terminal window.')
         os.system(f'source {os.path.expanduser("~/.zshrc")}')
 
     reload_profile(get_profile_file())  # so the first install works with env vars
     # else:
         # print("Environment variable 'ERAS_OPENAI_KEY' already exists in shell configuration files.")
 
     # if not env_var_exists("ERAS_BASE_URL"):
```

### Comparing `eras-0.2.3/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc` & `eras-0.2.4/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/decorators/chatgpt_tool_data.py` & `eras-0.2.4/eras/decorators/chatgpt_tool_data.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/factories/__pycache__/function_details_factory.cpython-311.pyc` & `eras-0.2.4/eras/factories/__pycache__/function_details_factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/factories/__pycache__/function_details_factory.cpython-39.pyc` & `eras-0.2.4/eras/factories/__pycache__/function_details_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/factories/__pycache__/message_factory.cpython-311.pyc` & `eras-0.2.4/eras/factories/__pycache__/message_factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/factories/__pycache__/message_factory.cpython-39.pyc` & `eras-0.2.4/eras/factories/__pycache__/message_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/factories/function_details_factory.py` & `eras-0.2.4/eras/factories/function_details_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/factories/message_factory.py` & `eras-0.2.4/eras/factories/message_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/main.py` & `eras-0.2.4/eras/main.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/models/__pycache__/conversation.cpython-311.pyc` & `eras-0.2.4/eras/models/__pycache__/conversation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/models/__pycache__/conversation.cpython-39.pyc` & `eras-0.2.4/eras/models/__pycache__/conversation.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/models/__pycache__/function_details.cpython-311.pyc` & `eras-0.2.4/eras/models/__pycache__/function_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/models/__pycache__/function_details.cpython-39.pyc` & `eras-0.2.4/eras/models/__pycache__/function_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/models/__pycache__/message.cpython-311.pyc` & `eras-0.2.4/eras/models/__pycache__/message.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/models/__pycache__/message.cpython-39.pyc` & `eras-0.2.4/eras/models/__pycache__/message.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/models/conversation.py` & `eras-0.2.4/eras/models/conversation.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/models/function_details.py` & `eras-0.2.4/eras/models/function_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/models/message.py` & `eras-0.2.4/eras/models/message.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/models/transaction.py` & `eras-0.2.4/eras/models/transaction.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/run.ipynb` & `eras-0.2.4/eras/run.ipynb`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/services/__pycache__/shell_command_service.cpython-311.pyc` & `eras-0.2.4/eras/services/__pycache__/shell_command_service.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/services/__pycache__/shell_command_service.cpython-39.pyc` & `eras-0.2.4/eras/services/__pycache__/shell_command_service.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc` & `eras-0.2.4/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc` & `eras-0.2.4/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc` & `eras-0.2.4/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc` & `eras-0.2.4/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc` & `eras-0.2.4/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc` & `eras-0.2.4/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/services/llm_callable_functions/callable_function_service_base.py` & `eras-0.2.4/eras/services/llm_callable_functions/callable_function_service_base.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/services/llm_callable_functions/terminal_command.py` & `eras-0.2.4/eras/services/llm_callable_functions/terminal_command.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/services/llm_callable_functions/user_details.py` & `eras-0.2.4/eras/services/llm_callable_functions/user_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras/services/shell_command_service.py` & `eras-0.2.4/eras/services/shell_command_service.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/eras.egg-info/PKG-INFO` & `eras-0.2.4/eras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.2.3
+Version: 0.2.4
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eras-0.2.3/eras.egg-info/SOURCES.txt` & `eras-0.2.4/eras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eras-0.2.3/setup.py` & `eras-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 #         print('Calling post_install.py')
 #         post_install_script = os.path.join(os.path.dirname(__file__), 'eras', 'post_install.py')
 #         # Run the post_install.py script in a new interactive shell
 #         subprocess.run([sys.executable, post_install_script], check=True, stdin=sys.stdin, stdout=sys.stdout)
 
 setup(
     name='eras',
-    version='0.2.3',
+    version='0.2.4',
     include_package_data=True,
     packages=find_packages(include=["eras", "eras.*"]),
     package_data={
         '': ['*.txt', '*.rst'],
         'eras': ['*.md'],
     },
     install_requires=[
```

