# Comparing `tmp/telegram_notifier_client-1.2.0.tar.gz` & `tmp/telegram_notifier_client-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_notifier_client-1.2.0.tar", last modified: Mon May  6 06:38:59 2024, max compression
+gzip compressed data, was "telegram_notifier_client-1.2.1.tar", last modified: Mon May 20 14:20:30 2024, max compression
```

## Comparing `telegram_notifier_client-1.2.0.tar` & `telegram_notifier_client-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-05-06 06:38:59.360550 telegram_notifier_client-1.2.0/
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      729 2024-05-06 06:38:59.360550 telegram_notifier_client-1.2.0/PKG-INFO
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      106 2023-11-27 16:14:13.000000 telegram_notifier_client-1.2.0/README.md
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      605 2024-05-06 06:32:49.000000 telegram_notifier_client-1.2.0/pyproject.toml
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)       79 2024-05-06 06:38:59.360550 telegram_notifier_client-1.2.0/setup.cfg
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      396 2024-05-06 06:32:49.000000 telegram_notifier_client-1.2.0/setup.py
-drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-05-06 06:38:59.344550 telegram_notifier_client-1.2.0/src/
-drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-05-06 06:38:59.344550 telegram_notifier_client-1.2.0/src/notifier_client/
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)        0 2023-11-27 16:14:13.000000 telegram_notifier_client-1.2.0/src/notifier_client/__init__.py
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)    20057 2024-05-05 11:18:50.000000 telegram_notifier_client-1.2.0/src/notifier_client/web_app_notifier_client.py
-drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-05-06 06:38:59.360550 telegram_notifier_client-1.2.0/src/telegram_notifier_client.egg-info/
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      729 2024-05-06 06:38:59.000000 telegram_notifier_client-1.2.0/src/telegram_notifier_client.egg-info/PKG-INFO
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      381 2024-05-06 06:38:59.000000 telegram_notifier_client-1.2.0/src/telegram_notifier_client.egg-info/SOURCES.txt
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)        1 2024-05-06 06:38:59.000000 telegram_notifier_client-1.2.0/src/telegram_notifier_client.egg-info/dependency_links.txt
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)       49 2024-05-06 06:38:59.000000 telegram_notifier_client-1.2.0/src/telegram_notifier_client.egg-info/requires.txt
--rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)       16 2024-05-06 06:38:59.000000 telegram_notifier_client-1.2.0/src/telegram_notifier_client.egg-info/top_level.txt
+drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-05-20 14:20:30.018207 telegram_notifier_client-1.2.1/
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      729 2024-05-20 14:20:30.018207 telegram_notifier_client-1.2.1/PKG-INFO
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      106 2023-11-27 16:14:13.000000 telegram_notifier_client-1.2.1/README.md
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      605 2024-05-20 14:08:41.000000 telegram_notifier_client-1.2.1/pyproject.toml
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)       79 2024-05-20 14:20:30.018207 telegram_notifier_client-1.2.1/setup.cfg
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      396 2024-05-20 14:08:41.000000 telegram_notifier_client-1.2.1/setup.py
+drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-05-20 14:20:29.958207 telegram_notifier_client-1.2.1/src/
+drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-05-20 14:20:29.986207 telegram_notifier_client-1.2.1/src/notifier_client/
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)        0 2023-11-27 16:14:13.000000 telegram_notifier_client-1.2.1/src/notifier_client/__init__.py
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)    19860 2024-05-20 14:01:10.000000 telegram_notifier_client-1.2.1/src/notifier_client/web_app_notifier_client.py
+drwxrwxr-x   0 mehdi8    (1000) mehdi8    (1000)        0 2024-05-20 14:20:30.018207 telegram_notifier_client-1.2.1/src/telegram_notifier_client.egg-info/
+-rw-r--r--   0 mehdi8    (1000) mehdi8    (1000)      729 2024-05-20 14:20:29.000000 telegram_notifier_client-1.2.1/src/telegram_notifier_client.egg-info/PKG-INFO
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)      381 2024-05-20 14:20:29.000000 telegram_notifier_client-1.2.1/src/telegram_notifier_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)        1 2024-05-20 14:20:29.000000 telegram_notifier_client-1.2.1/src/telegram_notifier_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)       49 2024-05-20 14:20:29.000000 telegram_notifier_client-1.2.1/src/telegram_notifier_client.egg-info/requires.txt
+-rw-rw-r--   0 mehdi8    (1000) mehdi8    (1000)       16 2024-05-20 14:20:29.000000 telegram_notifier_client-1.2.1/src/telegram_notifier_client.egg-info/top_level.txt
```

### Comparing `telegram_notifier_client-1.2.0/PKG-INFO` & `telegram_notifier_client-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegram_notifier_client
-Version: 1.2.0
+Version: 1.2.1
 Summary: telegram_notifier_client
 Home-page: https://github.com/deusfinance/notifier-client.git
 Author: Metalica
 Author-email: rorschach <rorschach45001@gmail.com>
 Project-URL: Homepage, https://github.com/deusfinance/notifier-client
 Project-URL: Issues, https://github.com/deusfinance/notifier-client/issues
 Keywords: telegram notifier client
```

### Comparing `telegram_notifier_client-1.2.0/pyproject.toml` & `telegram_notifier_client-1.2.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "telegram_notifier_client"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="rorschach", email="rorschach45001@gmail.com" },
 ]
 description = "telegram_notifier_client"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `telegram_notifier_client-1.2.0/src/notifier_client/web_app_notifier_client.py` & `telegram_notifier_client-1.2.1/src/notifier_client/web_app_notifier_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,16 +38,17 @@
     body: str = None
     amend: dict = None
     mentions: str = None
 
     def message(self):
         self.title = prepare_for_html(self.title)
         developers = f'\n👨‍💻    {self.mentions}' if self.mentions else ''
-        self.body = prepare_for_html(f"{self.body[:200]}...") if self.body and (len(self.body) > 200) else self.body
-        self.body = f'\n<b>Body</b>\n<pre><code class="language-python">{self.body}</code></pre>\n' if self.body else ''
+        self.body = f"{self.body[:200]}..." if self.body and (len(self.body) > 200) else self.body
+        self.body = f'\n<b>Body</b>\n<pre><code class="language-python">{prepare_for_html(self.body)}</code></pre>\n' \
+            if self.body else ''
 
         return (f'<blockquote>🔵 <b>Title:</b>    <code class="language-python">{self.title}</code>\n'
                 f'📊 <b>APM Reference:</b>   <code>{self.apm_reference}</code>'
                 f'{developers}</blockquote>\n'
                 f'{self.body}')
 
 
@@ -159,15 +160,15 @@
                           ):
         """
         The send_message_once function is used to notify the user of an error.
 
         :param title: str: Set the title of the notification
         :param apm_reference: str: Reference of the message in the ElasticAPM dashboard
         :param amend: dict: Add additional information to the message
-        :param mentions: tuple: List of the developers that should be mentioned in the message
+        :param mentions: str: string of the developers that should be mentioned in the message
         :param expire: int: Expire time of the message that prevents from sending a repeated message in seconds.
          Default is 2 days. If sets to `0` the message will be sent immediately.
         :param body: str: the body of the message.
         The maximum acceptable length is 200 characters.`Three dots` will replace the rest of the message.
 
         :return: A status code of the request
         """
@@ -194,15 +195,15 @@
 
 class SendNotification:
     def __init__(
             self,
             receiver_id: int,
             server_url: str,
             auth_token: str,
-            retrying_number: int = 5,
+            retrying_number: int = 5,  # FIXME: remove
             telegram_bot_token=None,
             test_env=False,
             test_env_logger: Optional[Logger] = None,
             topic_id: Optional[int] = None,
             max_msg_size: int = 3000
     ):
         """
@@ -217,20 +218,20 @@
                - test_env (bool): Flag indicating if the notification is being sent in a test environment.
                - test_env_logger (logging.Logger, optional): The logger to use in the test environment.
                - topic_id (int, optional):
                - max_msg_size (int): The maximum allowed size for a message to be sent.
            """
         self.receiver_id = receiver_id
         self.server_url = server_url
-        self.retiring_number = retrying_number
+        self.retiring_number = retrying_number  # FIXME: remove
         self.telegram_bot_token = telegram_bot_token
         self.notifier_client = WebAppNotifierClient(self.receiver_id, server_url, auth_token, topic_id)
         self.test_env = test_env
         self.max_msg_size = max_msg_size
-        self.topic_id = topic_id
+        self.topic_id = topic_id if topic_id else None
         if self.test_env:
             if test_env_logger:
                 self.test_env_logger = test_env_logger
             else:
                 logging.basicConfig()
                 logging.getLogger().setLevel(logging.DEBUG)
                 self.test_env_logger = logging
@@ -334,23 +335,21 @@
         """
 
         if self.test_env:
             self.test_env_logger.info(f"{title}: {apm_reference}")
             return
 
         res = 0
-        if mentions:
-            mentions = " ".join(mentions)
+        mentions = " ".join(mentions) if mentions else ""
 
         try:
-            for _ in range(self.retiring_number):
-                res = self.notifier_client.send_message_once(title=title, apm_reference=apm_reference, amend=amend,
-                                                             mentions=mentions, expire=expire, body=body)
-                if self.__check_status(res):
-                    return res
+            res = self.notifier_client.send_message_once(title=title, apm_reference=apm_reference, amend=amend,
+                                                         mentions=mentions, expire=expire, body=body)
+            if self.__check_status(res):
+                return res
 
         except Exception as e:
             logger.exception(f'exception:{e}')
 
         message = PrettifiedMessage(title=title, apm_reference=apm_reference, amend=amend, mentions=mentions, body=body)
         self.__send_emergency_message(message.message(), message.amend)
         return res
@@ -395,22 +394,17 @@
         Returns:
             - Union[int, Optional[Tuple[int, bool]]]: The result of the last message attempt to send.
         """
         message = message.replace('<', '&lt;').replace('>', '&gt;')
         msg_list = self.__split_msg(message, amend, emergency_msg)
         res = 0
         for msg in msg_list:
-            break_flag = False
             try:
-                for _ in range(self.retiring_number):
-                    res = send_func(msg.message(), msg.amend)
-                    if self.__check_status(res):
-                        break_flag = True
-                        break
-                if break_flag:
+                res = send_func(msg.message(), msg.amend)
+                if self.__check_status(res):
                     continue
             except Exception as e:
                 logger.exception(f'exception:{e}')
             self.__send_emergency_message(msg.message(), msg.amend)
         return res
 
     @staticmethod
```

### Comparing `telegram_notifier_client-1.2.0/src/telegram_notifier_client.egg-info/PKG-INFO` & `telegram_notifier_client-1.2.1/src/telegram_notifier_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telegram-notifier-client
-Version: 1.2.0
+Version: 1.2.1
 Summary: telegram_notifier_client
 Home-page: https://github.com/deusfinance/notifier-client.git
 Author: Metalica
 Author-email: rorschach <rorschach45001@gmail.com>
 Project-URL: Homepage, https://github.com/deusfinance/notifier-client
 Project-URL: Issues, https://github.com/deusfinance/notifier-client/issues
 Keywords: telegram notifier client
```

