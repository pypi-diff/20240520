# Comparing `tmp/eras-0.2.5.tar.gz` & `tmp/eras-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eras-0.2.5.tar", last modified: Mon May 20 00:26:09 2024, max compression
+gzip compressed data, was "eras-0.2.6.tar", last modified: Mon May 20 00:36:06 2024, max compression
```

## Comparing `eras-0.2.5.tar` & `eras-0.2.6.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:26:09.426791 eras-0.2.5/
--rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.2.5/LICENSE
--rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.2.5/MANIFEST.in
--rw-r--r--   0 jason      (501) staff       (20)     1558 2024-05-20 00:26:09.426201 eras-0.2.5/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)      935 2024-05-20 00:26:03.000000 eras-0.2.5/README.md
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:26:09.398789 eras-0.2.5/eras/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.2.5/eras/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:26:09.400575 eras-0.2.5/eras/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.2.5/eras/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:26:09.402410 eras-0.2.5/eras/agents/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.2.5/eras/agents/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:26:09.404615 eras-0.2.5/eras/agents/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.2.5/eras/agents/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.2.5/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.2.5/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.2.5/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.2.5/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     5501 2024-05-19 20:31:04.000000 eras-0.2.5/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.2.5/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.2.5/eras/agents/llama_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.2.5/eras/agents/llama_terminal_command_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.2.5/eras/agents/llm_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     4742 2024-05-20 00:18:13.000000 eras-0.2.5/eras/agents/terminal_llama_agent.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:26:09.405773 eras-0.2.5/eras/config/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.2.5/eras/config/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:26:09.406935 eras-0.2.5/eras/config/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.2.5/eras/config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1478 2024-05-19 19:36:31.000000 eras-0.2.5/eras/config/__pycache__/config.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.2.5/eras/config/__pycache__/config.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)      442 2024-05-19 19:31:13.000000 eras-0.2.5/eras/config/config.py
--rw-r--r--   0 jason      (501) staff       (20)     4716 2024-05-20 00:00:06.000000 eras-0.2.5/eras/config/post_install.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:26:09.407659 eras-0.2.5/eras/decorators/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.2.5/eras/decorators/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:26:09.408703 eras-0.2.5/eras/decorators/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.2.5/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.2.5/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.2.5/eras/decorators/chatgpt_tool_data.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:26:09.410131 eras-0.2.5/eras/factories/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.2.5/eras/factories/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:26:09.412484 eras-0.2.5/eras/factories/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.2.5/eras/factories/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.2.5/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.2.5/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3256 2024-05-19 20:31:34.000000 eras-0.2.5/eras/factories/__pycache__/message_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.2.5/eras/factories/__pycache__/message_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.2.5/eras/factories/function_details_factory.py
--rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.2.5/eras/factories/message_factory.py
--rw-r--r--   0 jason      (501) staff       (20)      670 2024-05-19 23:14:52.000000 eras-0.2.5/eras/main.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:26:09.414857 eras-0.2.5/eras/models/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.2.5/eras/models/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:26:09.418557 eras-0.2.5/eras/models/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.2.5/eras/models/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4345 2024-05-19 20:31:18.000000 eras-0.2.5/eras/models/__pycache__/conversation.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.2.5/eras/models/__pycache__/conversation.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1453 2024-05-19 20:34:55.000000 eras-0.2.5/eras/models/__pycache__/function_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.2.5/eras/models/__pycache__/function_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.2.5/eras/models/__pycache__/message.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.2.5/eras/models/__pycache__/message.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.2.5/eras/models/conversation.py
--rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.2.5/eras/models/function_details.py
--rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.2.5/eras/models/message.py
--rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.2.5/eras/models/transaction.py
--rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-19 02:17:49.000000 eras-0.2.5/eras/run.ipynb
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:26:09.419451 eras-0.2.5/eras/services/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.2.5/eras/services/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:26:09.420758 eras-0.2.5/eras/services/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.2.5/eras/services/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2837 2024-05-19 20:31:04.000000 eras-0.2.5/eras/services/__pycache__/shell_command_service.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.2.5/eras/services/__pycache__/shell_command_service.cpython-39.pyc
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:26:09.422499 eras-0.2.5/eras/services/llm_callable_functions/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.2.5/eras/services/llm_callable_functions/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:26:09.425276 eras-0.2.5/eras/services/llm_callable_functions/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.2.5/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.2.5/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.2.5/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.2.5/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.2.5/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.2.5/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.2.5/eras/services/llm_callable_functions/callable_function_service_base.py
--rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.2.5/eras/services/llm_callable_functions/terminal_command.py
--rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.2.5/eras/services/llm_callable_functions/user_details.py
--rw-r--r--   0 jason      (501) staff       (20)     2150 2024-05-20 00:18:39.000000 eras-0.2.5/eras/services/shell_command_service.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:26:09.400329 eras-0.2.5/eras.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)     1558 2024-05-20 00:26:09.000000 eras-0.2.5/eras.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     3200 2024-05-20 00:26:09.000000 eras-0.2.5/eras.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-20 00:26:09.000000 eras-0.2.5/eras.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-20 00:26:09.000000 eras-0.2.5/eras.egg-info/entry_points.txt
--rw-r--r--   0 jason      (501) staff       (20)       68 2024-05-20 00:26:09.000000 eras-0.2.5/eras.egg-info/requires.txt
--rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-20 00:26:09.000000 eras-0.2.5/eras.egg-info/top_level.txt
--rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-20 00:26:09.426896 eras-0.2.5/setup.cfg
--rw-r--r--   0 jason      (501) staff       (20)     2549 2024-05-20 00:26:03.000000 eras-0.2.5/setup.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:36:06.323593 eras-0.2.6/
+-rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.2.6/LICENSE
+-rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.2.6/MANIFEST.in
+-rw-r--r--   0 jason      (501) staff       (20)     1582 2024-05-20 00:36:06.323206 eras-0.2.6/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)      959 2024-05-20 00:35:22.000000 eras-0.2.6/README.md
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:36:06.300861 eras-0.2.6/eras/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.2.6/eras/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:36:06.302849 eras-0.2.6/eras/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.2.6/eras/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:36:06.304688 eras-0.2.6/eras/agents/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.2.6/eras/agents/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:36:06.307083 eras-0.2.6/eras/agents/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.2.6/eras/agents/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.2.6/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.2.6/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.2.6/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.2.6/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     5501 2024-05-19 20:31:04.000000 eras-0.2.6/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.2.6/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.2.6/eras/agents/llama_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.2.6/eras/agents/llama_terminal_command_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.2.6/eras/agents/llm_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     4742 2024-05-20 00:18:13.000000 eras-0.2.6/eras/agents/terminal_llama_agent.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:36:06.308143 eras-0.2.6/eras/config/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.2.6/eras/config/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:36:06.309093 eras-0.2.6/eras/config/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.2.6/eras/config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1478 2024-05-19 19:36:31.000000 eras-0.2.6/eras/config/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.2.6/eras/config/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      442 2024-05-19 19:31:13.000000 eras-0.2.6/eras/config/config.py
+-rw-r--r--   0 jason      (501) staff       (20)     4716 2024-05-20 00:00:06.000000 eras-0.2.6/eras/config/post_install.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:36:06.309655 eras-0.2.6/eras/decorators/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.2.6/eras/decorators/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:36:06.310326 eras-0.2.6/eras/decorators/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.2.6/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.2.6/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.2.6/eras/decorators/chatgpt_tool_data.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:36:06.311151 eras-0.2.6/eras/factories/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.2.6/eras/factories/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:36:06.312836 eras-0.2.6/eras/factories/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.2.6/eras/factories/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.2.6/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.2.6/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3256 2024-05-19 20:31:34.000000 eras-0.2.6/eras/factories/__pycache__/message_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.2.6/eras/factories/__pycache__/message_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.2.6/eras/factories/function_details_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.2.6/eras/factories/message_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)      670 2024-05-19 23:14:52.000000 eras-0.2.6/eras/main.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:36:06.314339 eras-0.2.6/eras/models/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.2.6/eras/models/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:36:06.316841 eras-0.2.6/eras/models/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.2.6/eras/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4345 2024-05-19 20:31:18.000000 eras-0.2.6/eras/models/__pycache__/conversation.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.2.6/eras/models/__pycache__/conversation.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1453 2024-05-19 20:34:55.000000 eras-0.2.6/eras/models/__pycache__/function_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.2.6/eras/models/__pycache__/function_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.2.6/eras/models/__pycache__/message.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.2.6/eras/models/__pycache__/message.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.2.6/eras/models/conversation.py
+-rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.2.6/eras/models/function_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.2.6/eras/models/message.py
+-rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.2.6/eras/models/transaction.py
+-rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-19 02:17:49.000000 eras-0.2.6/eras/run.ipynb
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:36:06.317583 eras-0.2.6/eras/services/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.2.6/eras/services/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:36:06.318761 eras-0.2.6/eras/services/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.2.6/eras/services/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2837 2024-05-19 20:31:04.000000 eras-0.2.6/eras/services/__pycache__/shell_command_service.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.2.6/eras/services/__pycache__/shell_command_service.cpython-39.pyc
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:36:06.320313 eras-0.2.6/eras/services/llm_callable_functions/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.2.6/eras/services/llm_callable_functions/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:36:06.322560 eras-0.2.6/eras/services/llm_callable_functions/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.2.6/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.2.6/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.2.6/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.2.6/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.2.6/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.2.6/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.2.6/eras/services/llm_callable_functions/callable_function_service_base.py
+-rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.2.6/eras/services/llm_callable_functions/terminal_command.py
+-rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.2.6/eras/services/llm_callable_functions/user_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     2150 2024-05-20 00:18:39.000000 eras-0.2.6/eras/services/shell_command_service.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-20 00:36:06.302490 eras-0.2.6/eras.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)     1582 2024-05-20 00:36:06.000000 eras-0.2.6/eras.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     3200 2024-05-20 00:36:06.000000 eras-0.2.6/eras.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-20 00:36:06.000000 eras-0.2.6/eras.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-20 00:36:06.000000 eras-0.2.6/eras.egg-info/entry_points.txt
+-rw-r--r--   0 jason      (501) staff       (20)       68 2024-05-20 00:36:06.000000 eras-0.2.6/eras.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-20 00:36:06.000000 eras-0.2.6/eras.egg-info/top_level.txt
+-rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-20 00:36:06.323711 eras-0.2.6/setup.cfg
+-rw-r--r--   0 jason      (501) staff       (20)     2549 2024-05-20 00:35:57.000000 eras-0.2.6/setup.py
```

### Comparing `eras-0.2.5/PKG-INFO` & `eras-0.2.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.2.5
+Version: 0.2.6
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,15 +31,15 @@
 
 # Use
 The first use of Eras will prompt you to enter an OpenAI key, which it will save to your profile as `ERAS_OPENAI_KEY`
 
 The first use will also prompt you to allow accessibility features for Terminal.app, which is required to allow Eras to populate
 the terminal with the shell command.
 
-![img.png](img.png)
+![img.png](https://i.imgur.com/y3OLDuG.png)
 
 
 When you ask Eras a question, it will use AI to create a shell command, then populate your next terminal line with the command, so all you have to do is review and press enter.
 
 ## Examples
 ```
 % eras list files
```

### Comparing `eras-0.2.5/README.md` & `eras-0.2.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # Use
 The first use of Eras will prompt you to enter an OpenAI key, which it will save to your profile as `ERAS_OPENAI_KEY`
 
 The first use will also prompt you to allow accessibility features for Terminal.app, which is required to allow Eras to populate
 the terminal with the shell command.
 
-![img.png](img.png)
+![img.png](https://i.imgur.com/y3OLDuG.png)
 
 
 When you ask Eras a question, it will use AI to create a shell command, then populate your next terminal line with the command, so all you have to do is review and press enter.
 
 ## Examples
 ```
 % eras list files
```

### Comparing `eras-0.2.5/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc` & `eras-0.2.6/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc` & `eras-0.2.6/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc` & `eras-0.2.6/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc` & `eras-0.2.6/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc` & `eras-0.2.6/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc` & `eras-0.2.6/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/agents/llama_functions_agent.py` & `eras-0.2.6/eras/agents/llama_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/agents/llama_terminal_command_functions_agent.py` & `eras-0.2.6/eras/agents/llama_terminal_command_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/agents/llm_functions_agent.py` & `eras-0.2.6/eras/agents/llm_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/agents/terminal_llama_agent.py` & `eras-0.2.6/eras/agents/terminal_llama_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/config/__pycache__/config.cpython-311.pyc` & `eras-0.2.6/eras/config/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/config/__pycache__/config.cpython-39.pyc` & `eras-0.2.6/eras/config/__pycache__/config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/config/post_install.py` & `eras-0.2.6/eras/config/post_install.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc` & `eras-0.2.6/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/decorators/chatgpt_tool_data.py` & `eras-0.2.6/eras/decorators/chatgpt_tool_data.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/factories/__pycache__/function_details_factory.cpython-311.pyc` & `eras-0.2.6/eras/factories/__pycache__/function_details_factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/factories/__pycache__/function_details_factory.cpython-39.pyc` & `eras-0.2.6/eras/factories/__pycache__/function_details_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/factories/__pycache__/message_factory.cpython-311.pyc` & `eras-0.2.6/eras/factories/__pycache__/message_factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/factories/__pycache__/message_factory.cpython-39.pyc` & `eras-0.2.6/eras/factories/__pycache__/message_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/factories/function_details_factory.py` & `eras-0.2.6/eras/factories/function_details_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/factories/message_factory.py` & `eras-0.2.6/eras/factories/message_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/main.py` & `eras-0.2.6/eras/main.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/models/__pycache__/conversation.cpython-311.pyc` & `eras-0.2.6/eras/models/__pycache__/conversation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/models/__pycache__/conversation.cpython-39.pyc` & `eras-0.2.6/eras/models/__pycache__/conversation.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/models/__pycache__/function_details.cpython-311.pyc` & `eras-0.2.6/eras/models/__pycache__/function_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/models/__pycache__/function_details.cpython-39.pyc` & `eras-0.2.6/eras/models/__pycache__/function_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/models/__pycache__/message.cpython-311.pyc` & `eras-0.2.6/eras/models/__pycache__/message.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/models/__pycache__/message.cpython-39.pyc` & `eras-0.2.6/eras/models/__pycache__/message.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/models/conversation.py` & `eras-0.2.6/eras/models/conversation.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/models/function_details.py` & `eras-0.2.6/eras/models/function_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/models/message.py` & `eras-0.2.6/eras/models/message.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/models/transaction.py` & `eras-0.2.6/eras/models/transaction.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/run.ipynb` & `eras-0.2.6/eras/run.ipynb`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/services/__pycache__/shell_command_service.cpython-311.pyc` & `eras-0.2.6/eras/services/__pycache__/shell_command_service.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/services/__pycache__/shell_command_service.cpython-39.pyc` & `eras-0.2.6/eras/services/__pycache__/shell_command_service.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc` & `eras-0.2.6/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc` & `eras-0.2.6/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc` & `eras-0.2.6/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc` & `eras-0.2.6/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc` & `eras-0.2.6/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc` & `eras-0.2.6/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/services/llm_callable_functions/callable_function_service_base.py` & `eras-0.2.6/eras/services/llm_callable_functions/callable_function_service_base.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/services/llm_callable_functions/terminal_command.py` & `eras-0.2.6/eras/services/llm_callable_functions/terminal_command.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/services/llm_callable_functions/user_details.py` & `eras-0.2.6/eras/services/llm_callable_functions/user_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras/services/shell_command_service.py` & `eras-0.2.6/eras/services/shell_command_service.py`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/eras.egg-info/PKG-INFO` & `eras-0.2.6/eras.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.2.5
+Version: 0.2.6
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,15 +31,15 @@
 
 # Use
 The first use of Eras will prompt you to enter an OpenAI key, which it will save to your profile as `ERAS_OPENAI_KEY`
 
 The first use will also prompt you to allow accessibility features for Terminal.app, which is required to allow Eras to populate
 the terminal with the shell command.
 
-![img.png](img.png)
+![img.png](https://i.imgur.com/y3OLDuG.png)
 
 
 When you ask Eras a question, it will use AI to create a shell command, then populate your next terminal line with the command, so all you have to do is review and press enter.
 
 ## Examples
 ```
 % eras list files
```

### Comparing `eras-0.2.5/eras.egg-info/SOURCES.txt` & `eras-0.2.6/eras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eras-0.2.5/setup.py` & `eras-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 #         print('Calling post_install.py')
 #         post_install_script = os.path.join(os.path.dirname(__file__), 'eras', 'post_install.py')
 #         # Run the post_install.py script in a new interactive shell
 #         subprocess.run([sys.executable, post_install_script], check=True, stdin=sys.stdin, stdout=sys.stdout)
 
 setup(
     name='eras',
-    version='0.2.5',
+    version='0.2.6',
     include_package_data=True,
     packages=find_packages(include=["eras", "eras.*"]),
     package_data={
         '': ['*.txt', '*.rst'],
         'eras': ['*.md'],
     },
     install_requires=[
```

