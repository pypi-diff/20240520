# Comparing `tmp/eras-0.3.0.tar.gz` & `tmp/eras-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eras-0.3.0.tar", last modified: Mon May 20 00:58:29 2024, max compression
+gzip compressed data, was "eras-0.3.1.tar", last modified: Mon May 20 01:16:41 2024, max compression
```

## Comparing `eras-0.3.0.tar` & `eras-0.3.1.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:58:29.793913 eras-0.3.0/
--rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.3.0/LICENSE
--rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.3.0/MANIFEST.in
--rw-r--r--   0 jason      (501) staff       (20)     1864 2024-05-20 00:58:29.793352 eras-0.3.0/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     1241 2024-05-20 00:58:07.000000 eras-0.3.0/README.md
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:58:29.770102 eras-0.3.0/eras/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.3.0/eras/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:58:29.771963 eras-0.3.0/eras/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.3.0/eras/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:58:29.773247 eras-0.3.0/eras/agents/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.3.0/eras/agents/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:58:29.775339 eras-0.3.0/eras/agents/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.3.0/eras/agents/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.3.0/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.3.0/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.3.0/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.3.0/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     5501 2024-05-19 20:31:04.000000 eras-0.3.0/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.3.0/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.3.0/eras/agents/llama_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.3.0/eras/agents/llama_terminal_command_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.3.0/eras/agents/llm_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     4742 2024-05-20 00:18:13.000000 eras-0.3.0/eras/agents/terminal_llama_agent.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:58:29.776510 eras-0.3.0/eras/config/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.3.0/eras/config/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:58:29.777521 eras-0.3.0/eras/config/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.3.0/eras/config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1478 2024-05-19 19:36:31.000000 eras-0.3.0/eras/config/__pycache__/config.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.3.0/eras/config/__pycache__/config.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)      442 2024-05-19 19:31:13.000000 eras-0.3.0/eras/config/config.py
--rw-r--r--   0 jason      (501) staff       (20)     4716 2024-05-20 00:00:06.000000 eras-0.3.0/eras/config/post_install.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:58:29.778046 eras-0.3.0/eras/decorators/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.3.0/eras/decorators/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:58:29.778955 eras-0.3.0/eras/decorators/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.3.0/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.3.0/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.3.0/eras/decorators/chatgpt_tool_data.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:58:29.780196 eras-0.3.0/eras/factories/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.3.0/eras/factories/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:58:29.782328 eras-0.3.0/eras/factories/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.3.0/eras/factories/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.3.0/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.3.0/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3256 2024-05-19 20:31:34.000000 eras-0.3.0/eras/factories/__pycache__/message_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.3.0/eras/factories/__pycache__/message_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.3.0/eras/factories/function_details_factory.py
--rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.3.0/eras/factories/message_factory.py
--rw-r--r--   0 jason      (501) staff       (20)      670 2024-05-19 23:14:52.000000 eras-0.3.0/eras/main.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:58:29.783952 eras-0.3.0/eras/models/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.3.0/eras/models/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:58:29.786670 eras-0.3.0/eras/models/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.3.0/eras/models/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4345 2024-05-19 20:31:18.000000 eras-0.3.0/eras/models/__pycache__/conversation.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.3.0/eras/models/__pycache__/conversation.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1453 2024-05-19 20:34:55.000000 eras-0.3.0/eras/models/__pycache__/function_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.3.0/eras/models/__pycache__/function_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.3.0/eras/models/__pycache__/message.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.3.0/eras/models/__pycache__/message.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.3.0/eras/models/conversation.py
--rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.3.0/eras/models/function_details.py
--rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.3.0/eras/models/message.py
--rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.3.0/eras/models/transaction.py
--rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-19 02:17:49.000000 eras-0.3.0/eras/run.ipynb
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:58:29.787307 eras-0.3.0/eras/services/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.3.0/eras/services/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:58:29.788442 eras-0.3.0/eras/services/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.3.0/eras/services/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2837 2024-05-19 20:31:04.000000 eras-0.3.0/eras/services/__pycache__/shell_command_service.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.3.0/eras/services/__pycache__/shell_command_service.cpython-39.pyc
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:58:29.790082 eras-0.3.0/eras/services/llm_callable_functions/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.3.0/eras/services/llm_callable_functions/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:58:29.792640 eras-0.3.0/eras/services/llm_callable_functions/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.3.0/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.3.0/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.3.0/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.3.0/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.3.0/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.3.0/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.3.0/eras/services/llm_callable_functions/callable_function_service_base.py
--rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.3.0/eras/services/llm_callable_functions/terminal_command.py
--rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.3.0/eras/services/llm_callable_functions/user_details.py
--rw-r--r--   0 jason      (501) staff       (20)     2150 2024-05-20 00:18:39.000000 eras-0.3.0/eras/services/shell_command_service.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:58:29.771652 eras-0.3.0/eras.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)     1864 2024-05-20 00:58:29.000000 eras-0.3.0/eras.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     3200 2024-05-20 00:58:29.000000 eras-0.3.0/eras.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-20 00:58:29.000000 eras-0.3.0/eras.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-20 00:58:29.000000 eras-0.3.0/eras.egg-info/entry_points.txt
--rw-r--r--   0 jason      (501) staff       (20)       68 2024-05-20 00:58:29.000000 eras-0.3.0/eras.egg-info/requires.txt
--rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-20 00:58:29.000000 eras-0.3.0/eras.egg-info/top_level.txt
--rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-20 00:58:29.794023 eras-0.3.0/setup.cfg
--rw-r--r--   0 jason      (501) staff       (20)     2549 2024-05-20 00:58:26.000000 eras-0.3.0/setup.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:16:41.212525 eras-0.3.1/
+-rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.3.1/LICENSE
+-rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.3.1/MANIFEST.in
+-rw-r--r--   0 jason      (501) staff       (20)     1987 2024-05-20 01:16:41.211801 eras-0.3.1/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     1364 2024-05-20 01:16:27.000000 eras-0.3.1/README.md
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:16:41.190156 eras-0.3.1/eras/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.3.1/eras/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:16:41.191788 eras-0.3.1/eras/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.3.1/eras/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:16:41.193119 eras-0.3.1/eras/agents/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.3.1/eras/agents/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:16:41.195563 eras-0.3.1/eras/agents/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.3.1/eras/agents/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.3.1/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.3.1/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.3.1/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.3.1/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     5501 2024-05-19 20:31:04.000000 eras-0.3.1/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.3.1/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.3.1/eras/agents/llama_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.3.1/eras/agents/llama_terminal_command_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.3.1/eras/agents/llm_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     4742 2024-05-20 00:18:13.000000 eras-0.3.1/eras/agents/terminal_llama_agent.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:16:41.196540 eras-0.3.1/eras/config/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.3.1/eras/config/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:16:41.197640 eras-0.3.1/eras/config/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.3.1/eras/config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1478 2024-05-19 19:36:31.000000 eras-0.3.1/eras/config/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.3.1/eras/config/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      442 2024-05-19 19:31:13.000000 eras-0.3.1/eras/config/config.py
+-rw-r--r--   0 jason      (501) staff       (20)     4716 2024-05-20 00:00:06.000000 eras-0.3.1/eras/config/post_install.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:16:41.198354 eras-0.3.1/eras/decorators/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.3.1/eras/decorators/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:16:41.198893 eras-0.3.1/eras/decorators/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.3.1/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.3.1/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.3.1/eras/decorators/chatgpt_tool_data.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:16:41.199701 eras-0.3.1/eras/factories/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.3.1/eras/factories/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:16:41.201156 eras-0.3.1/eras/factories/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.3.1/eras/factories/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.3.1/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.3.1/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3256 2024-05-19 20:31:34.000000 eras-0.3.1/eras/factories/__pycache__/message_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.3.1/eras/factories/__pycache__/message_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.3.1/eras/factories/function_details_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.3.1/eras/factories/message_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)      670 2024-05-19 23:14:52.000000 eras-0.3.1/eras/main.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:16:41.202594 eras-0.3.1/eras/models/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.3.1/eras/models/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:16:41.204856 eras-0.3.1/eras/models/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.3.1/eras/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4345 2024-05-19 20:31:18.000000 eras-0.3.1/eras/models/__pycache__/conversation.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.3.1/eras/models/__pycache__/conversation.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1453 2024-05-19 20:34:55.000000 eras-0.3.1/eras/models/__pycache__/function_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.3.1/eras/models/__pycache__/function_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.3.1/eras/models/__pycache__/message.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.3.1/eras/models/__pycache__/message.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.3.1/eras/models/conversation.py
+-rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.3.1/eras/models/function_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.3.1/eras/models/message.py
+-rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.3.1/eras/models/transaction.py
+-rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-19 02:17:49.000000 eras-0.3.1/eras/run.ipynb
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:16:41.205723 eras-0.3.1/eras/services/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.3.1/eras/services/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:16:41.207022 eras-0.3.1/eras/services/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.3.1/eras/services/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2837 2024-05-19 20:31:04.000000 eras-0.3.1/eras/services/__pycache__/shell_command_service.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.3.1/eras/services/__pycache__/shell_command_service.cpython-39.pyc
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:16:41.208676 eras-0.3.1/eras/services/llm_callable_functions/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.3.1/eras/services/llm_callable_functions/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:16:41.211105 eras-0.3.1/eras/services/llm_callable_functions/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.3.1/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.3.1/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.3.1/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.3.1/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.3.1/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.3.1/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.3.1/eras/services/llm_callable_functions/callable_function_service_base.py
+-rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.3.1/eras/services/llm_callable_functions/terminal_command.py
+-rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.3.1/eras/services/llm_callable_functions/user_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     2150 2024-05-20 00:18:39.000000 eras-0.3.1/eras/services/shell_command_service.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 01:16:41.191560 eras-0.3.1/eras.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)     1987 2024-05-20 01:16:41.000000 eras-0.3.1/eras.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     3200 2024-05-20 01:16:41.000000 eras-0.3.1/eras.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-20 01:16:41.000000 eras-0.3.1/eras.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-20 01:16:41.000000 eras-0.3.1/eras.egg-info/entry_points.txt
+-rw-r--r--   0 jason      (501) staff       (20)       68 2024-05-20 01:16:41.000000 eras-0.3.1/eras.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-20 01:16:41.000000 eras-0.3.1/eras.egg-info/top_level.txt
+-rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-20 01:16:41.212636 eras-0.3.1/setup.cfg
+-rw-r--r--   0 jason      (501) staff       (20)     2549 2024-05-20 01:16:37.000000 eras-0.3.1/setup.py
```

### Comparing `eras-0.3.0/PKG-INFO` & `eras-0.3.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.3.0
+Version: 0.3.1
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,27 +26,27 @@
 
 [![Video Thumbnail](https://img.youtube.com/vi/T7KRDwi5HDo/0.jpg)](https://youtu.be/T7KRDwi5HDo)
 
 
 <video src="./eras-demo.mov" controls></video>
 
 # Install
+```
+% pip install eras
+```
+
+If you get an error about externally-managed-environment it's because you have python installed via homebrew, and need to use pipx instead:
+
 pipx
 ``` 
 brew install pipx
 pipx ensurepath
-pipx install eras
-# you may need to open a new terminal window or source .zshrc
-```
-
-or use a virtual environment
-```
-python -m venv env
-pip install eras
+pipx install eras\
 ```
+With pipx you may need to open a new terminal window or source .zshrc a couple of times.
 
 # Use
 The first use of Eras will prompt you to enter an OpenAI key, which it will save to your profile as `ERAS_OPENAI_KEY`
 
 The first use will also prompt you to allow accessibility features for Terminal.app, which is required to allow Eras to populate
 the terminal with the shell command.
```

### Comparing `eras-0.3.0/README.md` & `eras-0.3.1/eras.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,52 @@
+Metadata-Version: 2.1
+Name: eras
+Version: 0.3.1
+Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
+Home-page: https://github.com/jasonmcaffee/eras
+Author: Jason McAffee
+Author-email: jasonlmcaffee@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: openai==1.26.0
+Requires-Dist: keyboard==0.13.5
+Requires-Dist: python-dotenv==1.0.0
+Requires-Dist: asyncio==3.4.3
+
 # ERAS
 Easily Run AI Shell allows you to run shell commands using natural language.   
 
 No more having to leave the terminal to look up how to run a command!
 
 # Demo
 [Eras Demo](https://youtu.be/T7KRDwi5HDo)
 
 [![Video Thumbnail](https://img.youtube.com/vi/T7KRDwi5HDo/0.jpg)](https://youtu.be/T7KRDwi5HDo)
 
 
 <video src="./eras-demo.mov" controls></video>
 
 # Install
+```
+% pip install eras
+```
+
+If you get an error about externally-managed-environment it's because you have python installed via homebrew, and need to use pipx instead:
+
 pipx
 ``` 
 brew install pipx
 pipx ensurepath
-pipx install eras
-# you may need to open a new terminal window or source .zshrc
-```
-
-or use a virtual environment
-```
-python -m venv env
-pip install eras
+pipx install eras\
 ```
+With pipx you may need to open a new terminal window or source .zshrc a couple of times.
 
 # Use
 The first use of Eras will prompt you to enter an OpenAI key, which it will save to your profile as `ERAS_OPENAI_KEY`
 
 The first use will also prompt you to allow accessibility features for Terminal.app, which is required to allow Eras to populate
 the terminal with the shell command.
```

### Comparing `eras-0.3.0/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc` & `eras-0.3.1/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc` & `eras-0.3.1/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc` & `eras-0.3.1/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc` & `eras-0.3.1/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc` & `eras-0.3.1/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc` & `eras-0.3.1/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/agents/llama_functions_agent.py` & `eras-0.3.1/eras/agents/llama_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/agents/llama_terminal_command_functions_agent.py` & `eras-0.3.1/eras/agents/llama_terminal_command_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/agents/llm_functions_agent.py` & `eras-0.3.1/eras/agents/llm_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/agents/terminal_llama_agent.py` & `eras-0.3.1/eras/agents/terminal_llama_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/config/__pycache__/config.cpython-311.pyc` & `eras-0.3.1/eras/config/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/config/__pycache__/config.cpython-39.pyc` & `eras-0.3.1/eras/config/__pycache__/config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/config/post_install.py` & `eras-0.3.1/eras/config/post_install.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc` & `eras-0.3.1/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/decorators/chatgpt_tool_data.py` & `eras-0.3.1/eras/decorators/chatgpt_tool_data.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/factories/__pycache__/function_details_factory.cpython-311.pyc` & `eras-0.3.1/eras/factories/__pycache__/function_details_factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/factories/__pycache__/function_details_factory.cpython-39.pyc` & `eras-0.3.1/eras/factories/__pycache__/function_details_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/factories/__pycache__/message_factory.cpython-311.pyc` & `eras-0.3.1/eras/factories/__pycache__/message_factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/factories/__pycache__/message_factory.cpython-39.pyc` & `eras-0.3.1/eras/factories/__pycache__/message_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/factories/function_details_factory.py` & `eras-0.3.1/eras/factories/function_details_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/factories/message_factory.py` & `eras-0.3.1/eras/factories/message_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/main.py` & `eras-0.3.1/eras/main.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/models/__pycache__/conversation.cpython-311.pyc` & `eras-0.3.1/eras/models/__pycache__/conversation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/models/__pycache__/conversation.cpython-39.pyc` & `eras-0.3.1/eras/models/__pycache__/conversation.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/models/__pycache__/function_details.cpython-311.pyc` & `eras-0.3.1/eras/models/__pycache__/function_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/models/__pycache__/function_details.cpython-39.pyc` & `eras-0.3.1/eras/models/__pycache__/function_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/models/__pycache__/message.cpython-311.pyc` & `eras-0.3.1/eras/models/__pycache__/message.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/models/__pycache__/message.cpython-39.pyc` & `eras-0.3.1/eras/models/__pycache__/message.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/models/conversation.py` & `eras-0.3.1/eras/models/conversation.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/models/function_details.py` & `eras-0.3.1/eras/models/function_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/models/message.py` & `eras-0.3.1/eras/models/message.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/models/transaction.py` & `eras-0.3.1/eras/models/transaction.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/run.ipynb` & `eras-0.3.1/eras/run.ipynb`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/services/__pycache__/shell_command_service.cpython-311.pyc` & `eras-0.3.1/eras/services/__pycache__/shell_command_service.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/services/__pycache__/shell_command_service.cpython-39.pyc` & `eras-0.3.1/eras/services/__pycache__/shell_command_service.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc` & `eras-0.3.1/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc` & `eras-0.3.1/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc` & `eras-0.3.1/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc` & `eras-0.3.1/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc` & `eras-0.3.1/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc` & `eras-0.3.1/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/services/llm_callable_functions/callable_function_service_base.py` & `eras-0.3.1/eras/services/llm_callable_functions/callable_function_service_base.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/services/llm_callable_functions/terminal_command.py` & `eras-0.3.1/eras/services/llm_callable_functions/terminal_command.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/services/llm_callable_functions/user_details.py` & `eras-0.3.1/eras/services/llm_callable_functions/user_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras/services/shell_command_service.py` & `eras-0.3.1/eras/services/shell_command_service.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/eras.egg-info/SOURCES.txt` & `eras-0.3.1/eras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eras-0.3.0/setup.py` & `eras-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 #         print('Calling post_install.py')
 #         post_install_script = os.path.join(os.path.dirname(__file__), 'eras', 'post_install.py')
 #         # Run the post_install.py script in a new interactive shell
 #         subprocess.run([sys.executable, post_install_script], check=True, stdin=sys.stdin, stdout=sys.stdout)
 
 setup(
     name='eras',
-    version='0.3.0',
+    version='0.3.1',
     include_package_data=True,
     packages=find_packages(include=["eras", "eras.*"]),
     package_data={
         '': ['*.txt', '*.rst'],
         'eras': ['*.md'],
     },
     install_requires=[
```

