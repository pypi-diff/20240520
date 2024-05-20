# Comparing `tmp/nonebot_plugin_calc24-0.2.3.tar.gz` & `tmp/nonebot_plugin_calc24-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_calc24-0.2.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_calc24-1.3.3.tar", max compression
```

## Comparing `nonebot_plugin_calc24-0.2.3.tar` & `nonebot_plugin_calc24-1.3.3.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1097 2024-05-17 01:11:38.482498 nonebot_plugin_calc24-0.2.3/LICENSE
--rw-r--r--   0        0        0     3811 2024-05-18 06:23:46.845160 nonebot_plugin_calc24-0.2.3/nonebot_plugin_calc24/__init__.py
--rw-r--r--   0        0        0     5303 2024-05-17 01:11:38.483619 nonebot_plugin_calc24-0.2.3/nonebot_plugin_calc24/calc24_invalid_data.json
--rw-r--r--   0        0        0     1866 2024-05-17 05:53:24.529102 nonebot_plugin_calc24-0.2.3/nonebot_plugin_calc24/xj_calc24.py
--rw-r--r--   0        0        0      701 2024-05-17 06:27:33.366930 nonebot_plugin_calc24-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      592 2024-05-18 06:23:33.596723 nonebot_plugin_calc24-0.2.3/README.md
--rw-r--r--   0        0        0     1538 1970-01-01 00:00:00.000000 nonebot_plugin_calc24-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1097 2024-05-17 01:11:38.482498 nonebot_plugin_calc24-1.3.3/LICENSE
+-rw-r--r--   0        0        0     5006 2024-05-19 12:16:21.577872 nonebot_plugin_calc24-1.3.3/nonebot_plugin_calc24/__init__.py
+-rw-r--r--   0        0        0     7152 2024-05-19 12:10:16.275566 nonebot_plugin_calc24-1.3.3/nonebot_plugin_calc24/calc24-data.json
+-rw-r--r--   0        0        0      860 2024-05-19 12:10:54.744539 nonebot_plugin_calc24-1.3.3/nonebot_plugin_calc24/file_handle.py
+-rw-r--r--   0        0        0     1643 2024-05-19 11:48:12.385393 nonebot_plugin_calc24-1.3.3/nonebot_plugin_calc24/xj_calc24.py
+-rw-r--r--   0        0        0      701 2024-05-19 10:20:40.242743 nonebot_plugin_calc24-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0      592 2024-05-18 06:23:33.596723 nonebot_plugin_calc24-1.3.3/README.md
+-rw-r--r--   0        0        0     1538 1970-01-01 00:00:00.000000 nonebot_plugin_calc24-1.3.3/PKG-INFO
```

### Comparing `nonebot_plugin_calc24-0.2.3/LICENSE` & `nonebot_plugin_calc24-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_calc24-0.2.3/nonebot_plugin_calc24/__init__.py` & `nonebot_plugin_calc24-1.3.3/nonebot_plugin_calc24/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+from .file_handle import file_handle
 from nonebot import on_command, on_message
 from nonebot.rule import to_me
 from nonebot.params import CommandArg
 from nonebot.adapters import Bot, Event
 from nonebot.typing import T_State 
 from nonebot.plugin import PluginMetadata
 from .xj_calc24 import xj_calc24
@@ -13,24 +14,40 @@
     usage="加载插件后使用/calc24或/24点开始游戏，在游戏中可以使用‘退出’退出游戏。",
     type="application",
     homepage="https://github.com/ajdgg/nonebot-plugin-calc24",
 )
 _timers = {}
 _calc24_session = {} 
 _original_array = {}
+
+file_handle = file_handle()
+c_m_data = file_handle.file_reading("calc24-data.json", "continuous-mode")
+    
 async def timeout_task(user_id, task):
     await asyncio.sleep(300) 
     if user_id in _calc24_session and _calc24_session[user_id] == "waiting_for_input":
         del _calc24_session[user_id]
         del _original_array['array']
 calc24 = on_command("24点", rule=to_me(),  priority=10, block=True)  
 @calc24.handle()  
 async def handle_first_receive(bot: Bot, event: Event, state: T_State, args = CommandArg()):  
     if  str(args) == 'help':
-        await calc24.finish("该插件实现的小游戏的游戏规则为一人一题。在插件启动时使用[24点]命令启动游戏。使用加减乘除使给出的数等于24，在游戏进行时可以直接回复[退出]来退出游戏或者[换一题]来更换新的题目。如果在5分钟内未回答会自动退出。")
+        await calc24.finish("该插件实现的小游戏的游戏规则为一人一题。在插件启动时使用[24点]命令启动游戏。使用加减乘除使给出的数等于24，在游戏进行时可以直接回复[退出]来退出游戏或者[换一题]来更换新的题目。如果在5分钟内未回答会自动退出。\n ===指令===\n 24点：开始游戏\n ===游戏进行时===\n 退出：退出游戏\n 换一题：更换新的题目\n ===设置===\n 24点 开启连续模式：开启连续模式\n 24点 退出连续模式：退出连续模式")
+    elif str(args) == '开启连续模式':
+        if c_m_data:
+            await calc24.finish("连续模式已是开启了哦")
+        else:
+            file_handle.file_change("calc24-data.json", "continuous-mode", True)
+            await calc24.finish("连续模式开启")
+    elif str(args) == '退出连续模式':
+        if c_m_data:
+            file_handle.file_change("calc24-data.json", "continuous-mode", False)
+            await calc24.finish("连续模式关闭")
+        else:
+            await calc24.finish("连续模式已是关闭的哦")
     a_data = class_calc24.calc_a_main()
     _original_array['array'] = a_data
     user_id = event.get_user_id()  
     sender_nickname = event.sender.nickname
     await calc24.send(f'{sender_nickname}请计算：\n {str(a_data)}')
     _calc24_session[user_id] = "waiting_for_input"
     task = asyncio.create_task(timeout_task(user_id, asyncio.current_task()))
@@ -60,13 +77,18 @@
         if b_data == 'NO':
             await calc24_input.send('输入无效，请重新输入')
         elif b_data == 'CONTINUOUS_OPERATOR':
             await calc24_input.send('连续操作符，请重新输入')
         elif b_data == 'ERROR':
             await calc24_input.send('答案错误，请重新输入')
         else:
-            a_data = class_calc24.calc_a_main()
-            _original_array['array'] = a_data
-            await calc24.send(f'{sender_nickname}答对了呢，下一题是：{str(a_data)}')
+            if c_m_data:
+                a_data = class_calc24.calc_a_main()
+                _original_array['array'] = a_data
+                await calc24.send(f'{sender_nickname}答对了呢，下一题是：{str(a_data)}')
+            else:
+                del _calc24_session[user_id]
+                del _original_array['array']
+                await calc24_input.finish(f'{sender_nickname}答对了呢，游戏结束')
     _calc24_session[user_id] = "waiting_for_input"
     task = asyncio.create_task(timeout_task(user_id, asyncio.current_task()))
     _timers[user_id] = task
```

### Comparing `nonebot_plugin_calc24-0.2.3/nonebot_plugin_calc24/xj_calc24.py` & `nonebot_plugin_calc24-1.3.3/nonebot_plugin_calc24/xj_calc24.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,14 @@
 import re
-import json
 import random
-from pathlib import Path 
+from .file_handle import file_handle
 
-# 加载无效数据列表
-script_path = Path(__file__).absolute()  
-current_dir = script_path.parent  
-json_file_path = current_dir / "calc24_invalid_data.json"  
+file_handle = file_handle()
 
-
-with json_file_path.open("r", encoding="utf-8") as json_file:  
-    loaded_data = json.load(json_file)  
-    legal_data_array = loaded_data["data"]  
+legal_data_array = file_handle.file_reading("calc24-data.json", "data")
 new_continuous_legal_data = {tuple(arr): None for arr in legal_data_array}
 
 def check_if_in_dict(array):
     key_tuple = tuple(array)
     return key_tuple in new_continuous_legal_data
 
 # 生成随机数函数
```

### Comparing `nonebot_plugin_calc24-0.2.3/pyproject.toml` & `nonebot_plugin_calc24-1.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-calc24"
-version = "0.2.3"
+version = "1.3.3"
 description = "A 24-point game plugin implemented using NoneBot."
 authors = ["AwAjie <139576615+ajdgg@users.noreply.github.com>"]
 license = "LICENSE"
 readme = "README.md"
 homepage = "https://github.com/ajdgg/nonebot-plugin-calc24"
 repository = "https://github.com/ajdgg/nonebot-plugin-calc24"
 documentation = "https://github.com/ajdgg/nonebot-plugin-calc24"
```

### Comparing `nonebot_plugin_calc24-0.2.3/README.md` & `nonebot_plugin_calc24-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_calc24-0.2.3/PKG-INFO` & `nonebot_plugin_calc24-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-calc24
-Version: 0.2.3
+Version: 1.3.3
 Summary: A 24-point game plugin implemented using NoneBot.
 Home-page: https://github.com/ajdgg/nonebot-plugin-calc24
 License: LICENSE
 Keywords: nonebot,nonebot2
 Author: AwAjie
 Author-email: 139576615+ajdgg@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
```

