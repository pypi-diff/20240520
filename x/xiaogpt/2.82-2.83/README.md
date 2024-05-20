# Comparing `tmp/xiaogpt-2.82.tar.gz` & `tmp/xiaogpt-2.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaogpt-2.82.tar", last modified: Sat May 18 04:09:29 2024, max compression
+gzip compressed data, was "xiaogpt-2.83.tar", last modified: Mon May 20 10:52:11 2024, max compression
```

## Comparing `xiaogpt-2.82.tar` & `xiaogpt-2.83.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1063 2024-05-18 04:09:17.607524 xiaogpt-2.82/LICENSE
--rw-r--r--   0        0        0    23909 2024-05-18 04:09:17.607524 xiaogpt-2.82/README.md
--rw-r--r--   0        0        0     3861 2024-05-18 04:09:29.003477 xiaogpt-2.82/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-18 04:09:17.607524 xiaogpt-2.82/xiaogpt/__init__.py
--rw-r--r--   0        0        0       61 2024-05-18 04:09:17.607524 xiaogpt-2.82/xiaogpt/__main__.py
--rw-r--r--   0        0        0     1160 2024-05-18 04:09:17.607524 xiaogpt-2.82/xiaogpt/bot/__init__.py
--rw-r--r--   0        0        0     1467 2024-05-18 04:09:17.607524 xiaogpt-2.82/xiaogpt/bot/base_bot.py
--rw-r--r--   0        0        0     3660 2024-05-18 04:09:17.607524 xiaogpt-2.82/xiaogpt/bot/chatgptapi_bot.py
--rw-r--r--   0        0        0     2773 2024-05-18 04:09:17.607524 xiaogpt-2.82/xiaogpt/bot/doubao_bot.py
--rw-r--r--   0        0        0     2516 2024-05-18 04:09:17.607524 xiaogpt-2.82/xiaogpt/bot/gemini_bot.py
--rw-r--r--   0        0        0     1825 2024-05-18 04:09:17.607524 xiaogpt-2.82/xiaogpt/bot/glm_bot.py
--rw-r--r--   0        0        0     1944 2024-05-18 04:09:17.607524 xiaogpt-2.82/xiaogpt/bot/langchain_bot.py
--rw-r--r--   0        0        0      708 2024-05-18 04:09:17.607524 xiaogpt-2.82/xiaogpt/bot/llama_bot.py
--rw-r--r--   0        0        0      822 2024-05-18 04:09:17.607524 xiaogpt-2.82/xiaogpt/bot/moonshot_bot.py
--rw-r--r--   0        0        0     3657 2024-05-18 04:09:17.607524 xiaogpt-2.82/xiaogpt/bot/qwen_bot.py
--rw-r--r--   0        0        0      784 2024-05-18 04:09:17.607524 xiaogpt-2.82/xiaogpt/bot/yi_bot.py
--rw-r--r--   0        0        0     5711 2024-05-18 04:09:17.607524 xiaogpt-2.82/xiaogpt/cli.py
--rw-r--r--   0        0        0     6734 2024-05-18 04:09:17.607524 xiaogpt-2.82/xiaogpt/config.py
--rw-r--r--   0        0        0     2616 2024-05-18 04:09:17.607524 xiaogpt-2.82/xiaogpt/langchain/callbacks.py
--rw-r--r--   0        0        0     1495 2024-05-18 04:09:17.607524 xiaogpt-2.82/xiaogpt/langchain/chain.py
--rw-r--r--   0        0        0     6372 2024-05-18 04:09:17.611523 xiaogpt-2.82/xiaogpt/langchain/examples/email/mail_box.py
--rw-r--r--   0        0        0     1561 2024-05-18 04:09:17.611523 xiaogpt-2.82/xiaogpt/langchain/examples/email/mail_summary_tools.py
--rw-r--r--   0        0        0      145 2024-05-18 04:09:17.611523 xiaogpt-2.82/xiaogpt/tts/__init__.py
--rw-r--r--   0        0        0     4656 2024-05-18 04:09:17.611523 xiaogpt-2.82/xiaogpt/tts/base.py
--rw-r--r--   0        0        0     1095 2024-05-18 04:09:17.611523 xiaogpt-2.82/xiaogpt/tts/mi.py
--rw-r--r--   0        0        0     1058 2024-05-18 04:09:17.611523 xiaogpt-2.82/xiaogpt/tts/tetos.py
--rw-r--r--   0        0        0     2072 2024-05-18 04:09:17.611523 xiaogpt-2.82/xiaogpt/utils.py
--rw-r--r--   0        0        0    16524 2024-05-18 04:09:17.611523 xiaogpt-2.82/xiaogpt/xiaogpt.py
--rw-r--r--   0        0        0    29678 1970-01-01 00:00:00.000000 xiaogpt-2.82/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-20 10:52:02.458185 xiaogpt-2.83/LICENSE
+-rw-r--r--   0        0        0    23909 2024-05-20 10:52:02.458185 xiaogpt-2.83/README.md
+-rw-r--r--   0        0        0     3861 2024-05-20 10:52:11.946170 xiaogpt-2.83/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/__init__.py
+-rw-r--r--   0        0        0       61 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/__main__.py
+-rw-r--r--   0        0        0     1160 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/bot/__init__.py
+-rw-r--r--   0        0        0     1467 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/bot/base_bot.py
+-rw-r--r--   0        0        0     3660 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/bot/chatgptapi_bot.py
+-rw-r--r--   0        0        0     2773 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/bot/doubao_bot.py
+-rw-r--r--   0        0        0     2516 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/bot/gemini_bot.py
+-rw-r--r--   0        0        0     1825 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/bot/glm_bot.py
+-rw-r--r--   0        0        0     1944 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/bot/langchain_bot.py
+-rw-r--r--   0        0        0      708 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/bot/llama_bot.py
+-rw-r--r--   0        0        0      822 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/bot/moonshot_bot.py
+-rw-r--r--   0        0        0     3657 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/bot/qwen_bot.py
+-rw-r--r--   0        0        0      784 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/bot/yi_bot.py
+-rw-r--r--   0        0        0     5711 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/cli.py
+-rw-r--r--   0        0        0     6734 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/config.py
+-rw-r--r--   0        0        0     2616 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/langchain/callbacks.py
+-rw-r--r--   0        0        0     1495 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/langchain/chain.py
+-rw-r--r--   0        0        0     6372 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/langchain/examples/email/mail_box.py
+-rw-r--r--   0        0        0     1561 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/langchain/examples/email/mail_summary_tools.py
+-rw-r--r--   0        0        0      145 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/tts/__init__.py
+-rw-r--r--   0        0        0     4665 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/tts/base.py
+-rw-r--r--   0        0        0     1095 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/tts/mi.py
+-rw-r--r--   0        0        0     1058 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/tts/tetos.py
+-rw-r--r--   0        0        0     2072 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/utils.py
+-rw-r--r--   0        0        0    16525 2024-05-20 10:52:02.458185 xiaogpt-2.83/xiaogpt/xiaogpt.py
+-rw-r--r--   0        0        0    29678 1970-01-01 00:00:00.000000 xiaogpt-2.83/PKG-INFO
```

### Comparing `xiaogpt-2.82/LICENSE` & `xiaogpt-2.83/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.82/README.md` & `xiaogpt-2.83/README.md`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.82/pyproject.toml` & `xiaogpt-2.83/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "dashscope>=1.10.0",
     "tetos>=0.2.1",
     "groq>=0.5.0",
     "pyyaml>=6.0.1",
     "langchain-community>=0.0.38",
 ]
 dynamic = []
-version = "2.82"
+version = "2.83"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/yihong0618/xiaogpt"
```

### Comparing `xiaogpt-2.82/xiaogpt/bot/__init__.py` & `xiaogpt-2.83/xiaogpt/bot/__init__.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.82/xiaogpt/bot/base_bot.py` & `xiaogpt-2.83/xiaogpt/bot/base_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.82/xiaogpt/bot/chatgptapi_bot.py` & `xiaogpt-2.83/xiaogpt/bot/chatgptapi_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.82/xiaogpt/bot/doubao_bot.py` & `xiaogpt-2.83/xiaogpt/bot/doubao_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.82/xiaogpt/bot/gemini_bot.py` & `xiaogpt-2.83/xiaogpt/bot/gemini_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.82/xiaogpt/bot/glm_bot.py` & `xiaogpt-2.83/xiaogpt/bot/glm_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.82/xiaogpt/bot/langchain_bot.py` & `xiaogpt-2.83/xiaogpt/bot/langchain_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.82/xiaogpt/bot/llama_bot.py` & `xiaogpt-2.83/xiaogpt/bot/llama_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.82/xiaogpt/bot/moonshot_bot.py` & `xiaogpt-2.83/xiaogpt/bot/moonshot_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.82/xiaogpt/bot/qwen_bot.py` & `xiaogpt-2.83/xiaogpt/bot/qwen_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.82/xiaogpt/bot/yi_bot.py` & `xiaogpt-2.83/xiaogpt/bot/yi_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.82/xiaogpt/cli.py` & `xiaogpt-2.83/xiaogpt/cli.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.82/xiaogpt/config.py` & `xiaogpt-2.83/xiaogpt/config.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.82/xiaogpt/langchain/callbacks.py` & `xiaogpt-2.83/xiaogpt/langchain/callbacks.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.82/xiaogpt/langchain/chain.py` & `xiaogpt-2.83/xiaogpt/langchain/chain.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.82/xiaogpt/langchain/examples/email/mail_box.py` & `xiaogpt-2.83/xiaogpt/langchain/examples/email/mail_box.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.82/xiaogpt/langchain/examples/email/mail_summary_tools.py` & `xiaogpt-2.83/xiaogpt/langchain/examples/email/mail_summary_tools.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.82/xiaogpt/tts/base.py` & `xiaogpt-2.83/xiaogpt/tts/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
                 if finished.is_set():
                     break
                 else:
                     await asyncio.sleep(0.1)
                     continue
             logger.debug("Playing URL %s (%s seconds)", url, duration)
             await asyncio.gather(
-                self.mina_service.play_by_url(self.device_id, url),
+                self.mina_service.play_by_url(self.device_id, url, _type=1),
                 self.wait_for_duration(duration),
             )
         await task
 
     def _start_http_server(self):
         # set the port range
         port_range = range(8050, 8090)
```

### Comparing `xiaogpt-2.82/xiaogpt/tts/mi.py` & `xiaogpt-2.83/xiaogpt/tts/mi.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.82/xiaogpt/tts/tetos.py` & `xiaogpt-2.83/xiaogpt/tts/tetos.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.82/xiaogpt/utils.py` & `xiaogpt-2.83/xiaogpt/utils.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.82/xiaogpt/xiaogpt.py` & `xiaogpt-2.83/xiaogpt/xiaogpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,23 +321,23 @@
         task.cancel()
 
     async def get_if_xiaoai_is_playing(self):
         playing_info = await self.mina_service.player_get_status(self.device_id)
         # WTF xiaomi api
         is_playing = (
             json.loads(playing_info.get("data", {}).get("info", "{}")).get("status", -1)
-            >= 1
+            == 1
         )
         return is_playing
 
     async def stop_if_xiaoai_is_playing(self):
         is_playing = await self.get_if_xiaoai_is_playing()
         if is_playing:
             # stop it
-            await self.mina_service.player_stop(self.device_id)
+            await self.mina_service.player_pause(self.device_id)
 
     async def wakeup_xiaoai(self):
         return await miio_command(
             self.miio_service,
             self.config.mi_did,
             f"{self.config.wakeup_command} {WAKEUP_KEYWORD} 0",
         )
```

### Comparing `xiaogpt-2.82/PKG-INFO` & `xiaogpt-2.83/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaogpt
-Version: 2.82
+Version: 2.83
 Summary: Play ChatGPT or other LLM with xiaomi AI speaker
 Author-Email: yihong0618 <zouzou0208@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/yihong0618/xiaogpt
```

