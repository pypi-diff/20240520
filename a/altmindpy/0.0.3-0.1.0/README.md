# Comparing `tmp/altmindpy-0.0.3.tar.gz` & `tmp/altmindpy-0.1.0.tar.gz`

## Comparing `altmindpy-0.0.3.tar` & `altmindpy-0.1.0.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/__init__.py
--rw-r--r--   0        0        0    64415 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/_base_client.py
--rw-r--r--   0        0        0    18167 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/_constants.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/_files.py
--rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/_qs.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/_resource.py
--rw-r--r--   0        0        0    28381 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/_response.py
--rw-r--r--   0        0        0    10104 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/_streaming.py
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/_types.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/_utils/__init__.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/lib/.keep
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/resources/__init__.py
--rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/resources/assistants.py
--rw-r--r--   0        0        0     5128 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/resources/experimental.py
--rw-r--r--   0        0        0     8122 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/resources/login.py
--rw-r--r--   0        0        0    19508 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/resources/runs.py
--rw-r--r--   0        0        0    17588 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/resources/threads.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/resources/messages/__init__.py
--rw-r--r--   0        0        0    20011 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/resources/messages/messages.py
--rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/resources/messages/thread.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/resources/users/__init__.py
--rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/resources/users/open.py
--rw-r--r--   0        0        0    20279 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/resources/users/users.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/resources/users/me/__init__.py
--rw-r--r--   0        0        0     8170 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/resources/users/me/me.py
--rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/resources/users/me/password.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/__init__.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/assistant_create_params.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/assistant_delete.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/assistant_list_params.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/assistant_response.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/assistant_update_params.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/assistants_response.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/experimental_stream_params.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/login_access_token_params.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/message_create_params.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/message_delete.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/message_list_params.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/message_response.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/message_update_params.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/run_create_params.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/run_list_params.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/run_response.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/run_update_params.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/runs_response.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/thread_create_params.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/thread_delete.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/thread_list_params.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/thread_response.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/thread_update_params.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/threads_response.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/token.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/user_create_params.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/user_list_params.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/user_update_params.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/users_out.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/messages/__init__.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/messages/thread_list_params.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/shared/__init__.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/shared/messages_response.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/shared/response_message.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/shared/user_out.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/users/__init__.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/users/me_update_params.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/users/open_create_params.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/users/me/__init__.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 altmindpy-0.0.3/src/altmind/types/users/me/password_update_params.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 altmindpy-0.0.3/.gitignore
--rw-r--r--   0        0        0    11337 2020-02-02 00:00:00.000000 altmindpy-0.0.3/LICENSE
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 altmindpy-0.0.3/pyproject.toml
--rw-r--r--   0        0        0    11943 2020-02-02 00:00:00.000000 altmindpy-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/__init__.py
+-rw-r--r--   0        0        0    64415 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_base_client.py
+-rw-r--r--   0        0        0    18167 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_constants.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_files.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_qs.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_resource.py
+-rw-r--r--   0        0        0    28381 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_response.py
+-rw-r--r--   0        0        0    10104 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_streaming.py
+-rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_types.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_utils/__init__.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/lib/.keep
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/__init__.py
+-rw-r--r--   0        0        0    20337 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/assistants.py
+-rw-r--r--   0        0        0     5128 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/experimental.py
+-rw-r--r--   0        0        0     8122 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/login.py
+-rw-r--r--   0        0        0    19508 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/runs.py
+-rw-r--r--   0        0        0    17588 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/threads.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/messages/__init__.py
+-rw-r--r--   0        0        0    20387 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/messages/messages.py
+-rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/messages/thread.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/users/__init__.py
+-rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/users/open.py
+-rw-r--r--   0        0        0    20279 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/users/users.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/users/me/__init__.py
+-rw-r--r--   0        0        0     8170 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/users/me/me.py
+-rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/users/me/password.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/__init__.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/assistant_create_params.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/assistant_delete.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/assistant_list_params.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/assistant_response.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/assistant_update_params.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/assistants_response.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/experimental_stream_params.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/login_access_token_params.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/message_create_params.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/message_delete.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/message_list_params.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/message_response.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/message_update_params.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/run_create_params.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/run_list_params.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/run_response.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/run_update_params.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/runs_response.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/thread_create_params.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/thread_delete.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/thread_list_params.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/thread_response.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/thread_update_params.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/threads_response.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/token.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/user_create_params.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/user_list_params.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/user_update_params.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/users_out.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/messages/__init__.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/messages/thread_list_params.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/shared/__init__.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/shared/messages_response.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/shared/response_message.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/shared/user_out.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/users/__init__.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/users/me_update_params.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/users/open_create_params.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/users/me/__init__.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/users/me/password_update_params.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 altmindpy-0.1.0/.gitignore
+-rw-r--r--   0        0        0    11337 2020-02-02 00:00:00.000000 altmindpy-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 altmindpy-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    11943 2020-02-02 00:00:00.000000 altmindpy-0.1.0/PKG-INFO
```

### Comparing `altmindpy-0.0.3/src/altmind/__init__.py` & `altmindpy-0.1.0/src/altmind/__init__.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/_base_client.py` & `altmindpy-0.1.0/src/altmind/_base_client.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/_client.py` & `altmindpy-0.1.0/src/altmind/_client.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/_compat.py` & `altmindpy-0.1.0/src/altmind/_compat.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/_exceptions.py` & `altmindpy-0.1.0/src/altmind/_exceptions.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/_files.py` & `altmindpy-0.1.0/src/altmind/_files.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/_models.py` & `altmindpy-0.1.0/src/altmind/_models.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/_qs.py` & `altmindpy-0.1.0/src/altmind/_qs.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/_resource.py` & `altmindpy-0.1.0/src/altmind/_resource.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/_response.py` & `altmindpy-0.1.0/src/altmind/_response.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/_streaming.py` & `altmindpy-0.1.0/src/altmind/_streaming.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/_types.py` & `altmindpy-0.1.0/src/altmind/_types.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/_utils/__init__.py` & `altmindpy-0.1.0/src/altmind/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/_utils/_logs.py` & `altmindpy-0.1.0/src/altmind/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/_utils/_proxy.py` & `altmindpy-0.1.0/src/altmind/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/_utils/_sync.py` & `altmindpy-0.1.0/src/altmind/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/_utils/_transform.py` & `altmindpy-0.1.0/src/altmind/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/_utils/_typing.py` & `altmindpy-0.1.0/src/altmind/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/_utils/_utils.py` & `altmindpy-0.1.0/src/altmind/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/resources/__init__.py` & `altmindpy-0.1.0/src/altmind/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/resources/assistants.py` & `altmindpy-0.1.0/src/altmind/resources/assistants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
-from typing import Optional
+from typing import Iterable, Optional
 
 import httpx
 
 from ..types import assistant_list_params, assistant_create_params, assistant_update_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import (
     maybe_transform,
@@ -43,14 +43,15 @@
         self,
         *,
         model: str,
         assistant_metadata: object | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         instructions: Optional[str] | NotGiven = NOT_GIVEN,
         name: Optional[str] | NotGiven = NOT_GIVEN,
+        tools: Iterable[Optional[object]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> AssistantResponse:
@@ -71,14 +72,15 @@
             body=maybe_transform(
                 {
                     "model": model,
                     "assistant_metadata": assistant_metadata,
                     "description": description,
                     "instructions": instructions,
                     "name": name,
+                    "tools": tools,
                 },
                 assistant_create_params.AssistantCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=AssistantResponse,
@@ -122,14 +124,15 @@
         assistant_id: str,
         *,
         model: str,
         assistant_metadata: object | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         instructions: Optional[str] | NotGiven = NOT_GIVEN,
         name: Optional[str] | NotGiven = NOT_GIVEN,
+        tools: Iterable[Optional[object]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> AssistantResponse:
@@ -152,14 +155,15 @@
             body=maybe_transform(
                 {
                     "model": model,
                     "assistant_metadata": assistant_metadata,
                     "description": description,
                     "instructions": instructions,
                     "name": name,
+                    "tools": tools,
                 },
                 assistant_update_params.AssistantUpdateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=AssistantResponse,
@@ -254,14 +258,15 @@
         self,
         *,
         model: str,
         assistant_metadata: object | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         instructions: Optional[str] | NotGiven = NOT_GIVEN,
         name: Optional[str] | NotGiven = NOT_GIVEN,
+        tools: Iterable[Optional[object]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> AssistantResponse:
@@ -282,14 +287,15 @@
             body=await async_maybe_transform(
                 {
                     "model": model,
                     "assistant_metadata": assistant_metadata,
                     "description": description,
                     "instructions": instructions,
                     "name": name,
+                    "tools": tools,
                 },
                 assistant_create_params.AssistantCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=AssistantResponse,
@@ -333,14 +339,15 @@
         assistant_id: str,
         *,
         model: str,
         assistant_metadata: object | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         instructions: Optional[str] | NotGiven = NOT_GIVEN,
         name: Optional[str] | NotGiven = NOT_GIVEN,
+        tools: Iterable[Optional[object]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> AssistantResponse:
@@ -363,14 +370,15 @@
             body=await async_maybe_transform(
                 {
                     "model": model,
                     "assistant_metadata": assistant_metadata,
                     "description": description,
                     "instructions": instructions,
                     "name": name,
+                    "tools": tools,
                 },
                 assistant_update_params.AssistantUpdateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=AssistantResponse,
```

### Comparing `altmindpy-0.0.3/src/altmind/resources/experimental.py` & `altmindpy-0.1.0/src/altmind/resources/experimental.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/resources/login.py` & `altmindpy-0.1.0/src/altmind/resources/login.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/resources/runs.py` & `altmindpy-0.1.0/src/altmind/resources/runs.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/resources/threads.py` & `altmindpy-0.1.0/src/altmind/resources/threads.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/resources/messages/__init__.py` & `altmindpy-0.1.0/src/altmind/resources/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/resources/messages/messages.py` & `altmindpy-0.1.0/src/altmind/resources/messages/messages.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     def with_streaming_response(self) -> MessagesResourceWithStreamingResponse:
         return MessagesResourceWithStreamingResponse(self)
 
     def create(
         self,
         *,
         content: Iterable[message_create_params.Content],
+        tool_calls: Optional[Iterable[object]],
         message_metadata: object | NotGiven = NOT_GIVEN,
         original_role: Optional[Literal["user", "assistant", "system", "tool"]] | NotGiven = NOT_GIVEN,
         role: Optional[Literal["user", "assistant", "system", "tool"]] | NotGiven = NOT_GIVEN,
         thread_id: Optional[int] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
@@ -80,14 +81,15 @@
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._post(
             "/api/v1/messages/",
             body=maybe_transform(
                 {
                     "content": content,
+                    "tool_calls": tool_calls,
                     "message_metadata": message_metadata,
                     "original_role": original_role,
                     "role": role,
                     "thread_id": thread_id,
                 },
                 message_create_params.MessageCreateParams,
             ),
@@ -128,14 +130,15 @@
             cast_to=MessageResponse,
         )
 
     def update(
         self,
         message_id: int,
         *,
+        tool_calls: Optional[Iterable[object]],
         content: Optional[Iterable[message_update_params.Content]] | NotGiven = NOT_GIVEN,
         message_metadata: object | NotGiven = NOT_GIVEN,
         role: Optional[Literal["user", "assistant", "system", "tool"]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -154,14 +157,15 @@
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._patch(
             f"/api/v1/messages/{message_id}",
             body=maybe_transform(
                 {
+                    "tool_calls": tool_calls,
                     "content": content,
                     "message_metadata": message_metadata,
                     "role": role,
                 },
                 message_update_params.MessageUpdateParams,
             ),
             options=make_request_options(
@@ -257,14 +261,15 @@
     def with_streaming_response(self) -> AsyncMessagesResourceWithStreamingResponse:
         return AsyncMessagesResourceWithStreamingResponse(self)
 
     async def create(
         self,
         *,
         content: Iterable[message_create_params.Content],
+        tool_calls: Optional[Iterable[object]],
         message_metadata: object | NotGiven = NOT_GIVEN,
         original_role: Optional[Literal["user", "assistant", "system", "tool"]] | NotGiven = NOT_GIVEN,
         role: Optional[Literal["user", "assistant", "system", "tool"]] | NotGiven = NOT_GIVEN,
         thread_id: Optional[int] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
@@ -285,14 +290,15 @@
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return await self._post(
             "/api/v1/messages/",
             body=await async_maybe_transform(
                 {
                     "content": content,
+                    "tool_calls": tool_calls,
                     "message_metadata": message_metadata,
                     "original_role": original_role,
                     "role": role,
                     "thread_id": thread_id,
                 },
                 message_create_params.MessageCreateParams,
             ),
@@ -333,14 +339,15 @@
             cast_to=MessageResponse,
         )
 
     async def update(
         self,
         message_id: int,
         *,
+        tool_calls: Optional[Iterable[object]],
         content: Optional[Iterable[message_update_params.Content]] | NotGiven = NOT_GIVEN,
         message_metadata: object | NotGiven = NOT_GIVEN,
         role: Optional[Literal["user", "assistant", "system", "tool"]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -359,14 +366,15 @@
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return await self._patch(
             f"/api/v1/messages/{message_id}",
             body=await async_maybe_transform(
                 {
+                    "tool_calls": tool_calls,
                     "content": content,
                     "message_metadata": message_metadata,
                     "role": role,
                 },
                 message_update_params.MessageUpdateParams,
             ),
             options=make_request_options(
```

### Comparing `altmindpy-0.0.3/src/altmind/resources/messages/thread.py` & `altmindpy-0.1.0/src/altmind/resources/messages/thread.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/resources/users/__init__.py` & `altmindpy-0.1.0/src/altmind/resources/users/__init__.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/resources/users/open.py` & `altmindpy-0.1.0/src/altmind/resources/users/open.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/resources/users/users.py` & `altmindpy-0.1.0/src/altmind/resources/users/users.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/resources/users/me/__init__.py` & `altmindpy-0.1.0/src/altmind/resources/users/me/__init__.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/resources/users/me/me.py` & `altmindpy-0.1.0/src/altmind/resources/users/me/me.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/resources/users/me/password.py` & `altmindpy-0.1.0/src/altmind/resources/users/me/password.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/types/__init__.py` & `altmindpy-0.1.0/src/altmind/types/__init__.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/types/assistant_response.py` & `altmindpy-0.1.0/src/altmind/types/assistant_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
-from typing import Optional
+import builtins
+from typing import List, Optional
 from typing_extensions import Literal
 
 from .._models import BaseModel
 
 __all__ = ["AssistantResponse"]
 
 
@@ -20,7 +21,9 @@
     description: Optional[str] = None
 
     instructions: Optional[str] = None
 
     name: Optional[str] = None
 
     object: Optional[Literal["assistant"]] = None
+
+    tools: Optional[List[Optional[builtins.object]]] = None
```

### Comparing `altmindpy-0.0.3/src/altmind/types/message_create_params.py` & `altmindpy-0.1.0/src/altmind/types/message_create_params.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,20 +8,24 @@
 __all__ = [
     "MessageCreateParams",
     "Content",
     "ContentTextContent",
     "ContentTextContentText",
     "ContentImageFileContent",
     "ContentImageFileContentImageFile",
+    "ContentToolContent",
+    "ContentToolContentTool",
 ]
 
 
 class MessageCreateParams(TypedDict, total=False):
     content: Required[Iterable[Content]]
 
+    tool_calls: Required[Optional[Iterable[object]]]
+
     message_metadata: object
 
     original_role: Optional[Literal["user", "assistant", "system", "tool"]]
 
     role: Optional[Literal["user", "assistant", "system", "tool"]]
 
     thread_id: Optional[int]
@@ -43,8 +47,22 @@
 
 class ContentImageFileContent(TypedDict, total=False):
     image_file: Required[ContentImageFileContentImageFile]
 
     type: Literal["image_file"]
 
 
-Content = Union[ContentTextContent, ContentImageFileContent]
+class ContentToolContentTool(TypedDict, total=False):
+    content: Optional[object]
+
+    name: Optional[str]
+
+    tool_call_id: Optional[str]
+
+
+class ContentToolContent(TypedDict, total=False):
+    tool: Required[ContentToolContentTool]
+
+    type: Literal["tool_output"]
+
+
+Content = Union[ContentTextContent, ContentImageFileContent, ContentToolContent]
```

### Comparing `altmindpy-0.0.3/src/altmind/types/message_response.py` & `altmindpy-0.1.0/src/altmind/types/message_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 __all__ = [
     "MessageResponse",
     "Content",
     "ContentTextContent",
     "ContentTextContentText",
     "ContentImageFileContent",
     "ContentImageFileContentImageFile",
+    "ContentToolContent",
+    "ContentToolContentTool",
 ]
 
 
 class ContentTextContentText(BaseModel):
     value: str
 
 
@@ -31,26 +33,42 @@
 
 class ContentImageFileContent(BaseModel):
     image_file: ContentImageFileContentImageFile
 
     type: Optional[Literal["image_file"]] = None
 
 
-Content = Union[ContentTextContent, ContentImageFileContent]
+class ContentToolContentTool(BaseModel):
+    content: Optional[object] = None
+
+    name: Optional[str] = None
+
+    tool_call_id: Optional[str] = None
+
+
+class ContentToolContent(BaseModel):
+    tool: ContentToolContentTool
+
+    type: Optional[Literal["tool_output"]] = None
+
+
+Content = Union[ContentTextContent, ContentImageFileContent, ContentToolContent]
 
 
 class MessageResponse(BaseModel):
     id: int
 
     content: List[Content]
 
     created_at: int
 
     original_role: Optional[Literal["user", "assistant", "system", "tool"]] = None
 
+    tool_calls: Optional[List[object]] = None
+
     message_metadata: Optional[object] = None
 
     object: Optional[Literal["message"]] = None
 
     role: Optional[Literal["user", "assistant", "system", "tool"]] = None
 
     thread_id: Optional[int] = None
```

### Comparing `altmindpy-0.0.3/src/altmind/types/message_update_params.py` & `altmindpy-0.1.0/src/altmind/types/message_update_params.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,18 +8,22 @@
 __all__ = [
     "MessageUpdateParams",
     "Content",
     "ContentTextContent",
     "ContentTextContentText",
     "ContentImageFileContent",
     "ContentImageFileContentImageFile",
+    "ContentToolContent",
+    "ContentToolContentTool",
 ]
 
 
 class MessageUpdateParams(TypedDict, total=False):
+    tool_calls: Required[Optional[Iterable[object]]]
+
     content: Optional[Iterable[Content]]
 
     message_metadata: object
 
     role: Optional[Literal["user", "assistant", "system", "tool"]]
 
 
@@ -39,8 +43,22 @@
 
 class ContentImageFileContent(TypedDict, total=False):
     image_file: Required[ContentImageFileContentImageFile]
 
     type: Literal["image_file"]
 
 
-Content = Union[ContentTextContent, ContentImageFileContent]
+class ContentToolContentTool(TypedDict, total=False):
+    content: Optional[object]
+
+    name: Optional[str]
+
+    tool_call_id: Optional[str]
+
+
+class ContentToolContent(TypedDict, total=False):
+    tool: Required[ContentToolContentTool]
+
+    type: Literal["tool_output"]
+
+
+Content = Union[ContentTextContent, ContentImageFileContent, ContentToolContent]
```

### Comparing `altmindpy-0.0.3/src/altmind/types/run_create_params.py` & `altmindpy-0.1.0/src/altmind/types/run_create_params.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/src/altmind/types/run_response.py` & `altmindpy-0.1.0/src/altmind/types/run_response.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/LICENSE` & `altmindpy-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `altmindpy-0.0.3/pyproject.toml` & `altmindpy-0.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "altmindpy"
-version = "0.0.3"
+version = "0.1.0"
 description = "The official Python library for the altmind API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Altmind", email = "azzi.leonardo@gmail.com" },
 ]
 dependencies = [
```

### Comparing `altmindpy-0.0.3/PKG-INFO` & `altmindpy-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: altmindpy
-Version: 0.0.3
+Version: 0.1.0
 Summary: The official Python library for the altmind API
 Project-URL: Homepage, https://github.com/AltermindLabs/altmind-python
 Project-URL: Repository, https://github.com/AltermindLabs/altmind-python
 Author-email: Altmind <azzi.leonardo@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
```

