# Comparing `tmp/nonebot_plugin_with_ai_agents-0.1.8.tar.gz` & `tmp/nonebot_plugin_with_ai_agents-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_with_ai_agents-0.1.8.tar", max compression
+gzip compressed data, was "nonebot_plugin_with_ai_agents-0.1.9.tar", max compression
```

## Comparing `nonebot_plugin_with_ai_agents-0.1.8.tar` & `nonebot_plugin_with_ai_agents-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      510 2024-05-08 08:28:49.886180 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/__init__.py
--rw-r--r--   0        0        0      743 2024-05-08 16:28:31.442912 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/handler.py
--rw-r--r--   0        0        0        2 2024-05-06 07:05:33.777069 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/__init__.py
--rw-r--r--   0        0        0     4623 2024-05-08 15:59:57.148477 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/agents.py
--rw-r--r--   0        0        0     3266 2024-05-08 16:32:46.821602 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/central_brain.py
--rw-r--r--   0        0        0     1083 2024-05-08 09:54:00.100650 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/config.py
--rw-r--r--   0        0        0      131 2024-05-06 07:05:33.778077 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/llms/__init__.py
--rw-r--r--   0        0        0      520 2024-05-08 14:21:20.414475 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/llms/base.py
--rw-r--r--   0        0        0     2277 2024-05-07 11:13:28.157800 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/llms/dashscope.py
--rw-r--r--   0        0        0     1942 2024-05-07 11:13:28.219069 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/llms/glm.py
--rw-r--r--   0        0        0     2046 2024-05-07 11:13:28.141789 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/llms/openai.py
--rw-r--r--   0        0        0       19 2024-05-08 15:39:53.681731 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/mem_stores.py
--rw-r--r--   0        0        0     1727 2024-05-08 16:28:10.356972 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/services.py
--rw-r--r--   0        0        0        0 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/utils/__init__.py
--rw-r--r--   0        0        0     4576 2024-05-08 16:32:46.840606 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/utils/prompts.py
--rw-r--r--   0        0        0     3358 2024-05-07 10:03:19.714495 nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/utils/retrievers.py
--rw-r--r--   0        0        0      679 2024-05-08 16:35:10.830362 nonebot_plugin_with_ai_agents-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     7057 2024-05-08 16:30:07.456483 nonebot_plugin_with_ai_agents-0.1.8/README.md
--rw-r--r--   0        0        0     7842 1970-01-01 00:00:00.000000 nonebot_plugin_with_ai_agents-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      510 2024-05-08 08:28:49.886180 nonebot_plugin_with_ai_agents-0.1.9/nonebot_plugin_with_ai_agents/__init__.py
+-rw-r--r--   0        0        0      743 2024-05-08 16:28:31.442912 nonebot_plugin_with_ai_agents-0.1.9/nonebot_plugin_with_ai_agents/handler.py
+-rw-r--r--   0        0        0        2 2024-05-06 07:05:33.777069 nonebot_plugin_with_ai_agents-0.1.9/nonebot_plugin_with_ai_agents/llm/__init__.py
+-rw-r--r--   0        0        0     4623 2024-05-08 15:59:57.148477 nonebot_plugin_with_ai_agents-0.1.9/nonebot_plugin_with_ai_agents/llm/agents.py
+-rw-r--r--   0        0        0     3649 2024-05-08 17:02:55.852198 nonebot_plugin_with_ai_agents-0.1.9/nonebot_plugin_with_ai_agents/llm/central_brain.py
+-rw-r--r--   0        0        0     1083 2024-05-08 09:54:00.100650 nonebot_plugin_with_ai_agents-0.1.9/nonebot_plugin_with_ai_agents/llm/config.py
+-rw-r--r--   0        0        0      131 2024-05-06 07:05:33.778077 nonebot_plugin_with_ai_agents-0.1.9/nonebot_plugin_with_ai_agents/llm/llms/__init__.py
+-rw-r--r--   0        0        0      520 2024-05-08 14:21:20.414475 nonebot_plugin_with_ai_agents-0.1.9/nonebot_plugin_with_ai_agents/llm/llms/base.py
+-rw-r--r--   0        0        0     2277 2024-05-07 11:13:28.157800 nonebot_plugin_with_ai_agents-0.1.9/nonebot_plugin_with_ai_agents/llm/llms/dashscope.py
+-rw-r--r--   0        0        0     1942 2024-05-07 11:13:28.219069 nonebot_plugin_with_ai_agents-0.1.9/nonebot_plugin_with_ai_agents/llm/llms/glm.py
+-rw-r--r--   0        0        0     2046 2024-05-07 11:13:28.141789 nonebot_plugin_with_ai_agents-0.1.9/nonebot_plugin_with_ai_agents/llm/llms/openai.py
+-rw-r--r--   0        0        0       19 2024-05-08 15:39:53.681731 nonebot_plugin_with_ai_agents-0.1.9/nonebot_plugin_with_ai_agents/llm/mem_stores.py
+-rw-r--r--   0        0        0     1727 2024-05-08 16:28:10.356972 nonebot_plugin_with_ai_agents-0.1.9/nonebot_plugin_with_ai_agents/llm/services.py
+-rw-r--r--   0        0        0        0 2024-05-06 07:05:33.780198 nonebot_plugin_with_ai_agents-0.1.9/nonebot_plugin_with_ai_agents/llm/utils/__init__.py
+-rw-r--r--   0        0        0     4582 2024-05-08 17:00:00.373440 nonebot_plugin_with_ai_agents-0.1.9/nonebot_plugin_with_ai_agents/llm/utils/prompts.py
+-rw-r--r--   0        0        0     3358 2024-05-07 10:03:19.714495 nonebot_plugin_with_ai_agents-0.1.9/nonebot_plugin_with_ai_agents/llm/utils/retrievers.py
+-rw-r--r--   0        0        0      679 2024-05-08 17:06:01.389518 nonebot_plugin_with_ai_agents-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     7057 2024-05-08 16:30:07.456483 nonebot_plugin_with_ai_agents-0.1.9/README.md
+-rw-r--r--   0        0        0     7842 1970-01-01 00:00:00.000000 nonebot_plugin_with_ai_agents-0.1.9/PKG-INFO
```

### Comparing `nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/handler.py` & `nonebot_plugin_with_ai_agents-0.1.9/nonebot_plugin_with_ai_agents/handler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/agents.py` & `nonebot_plugin_with_ai_agents-0.1.9/nonebot_plugin_with_ai_agents/llm/agents.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/central_brain.py` & `nonebot_plugin_with_ai_agents-0.1.9/nonebot_plugin_with_ai_agents/llm/central_brain.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,38 +38,48 @@
         return "WITH_AI_AGENTS 大模型获取失败，请检查配置。配置文档参考：https://github.com/yejue/nonebot-plugin-with-ai-agents"
 
     # 将用户提问发送到大模型分类器，获取分类列表
     prompt = prompts.get_classifier_prompt(question=raw_question)
     s = prompts.get_classifier_master_prompt()
     classifier_res = await llm.ask_model(question=prompt, system_prompt=s)
     print(f"raw_classifier_res: {classifier_res}")
-    classifier_res = json.loads(classifier_res)
+
+    try:
+        classifier_res = json.loads(classifier_res)
+    except Exception as e:
+        print(e)
+        return "WITH_AI_AGENTS 模型处理失败，试着换点更优秀的模型吧"
+
     print(f"智脑分类结果：{classifier_res}")
 
     # 遍历分类列表，向 agents 发送任务并获取 context
     agent_data = ""
 
-    for num in classifier_res:
-        if int(num) == 1:    # 提取页面内容
-            agent_data += await agents.type1.summarize_weblink_content(llm=llm, question=raw_question) + "\n"
-        elif int(num) == 2:  # 联网搜索能力
-            agent_data += await agents.type2.get_search_result(llm=llm, question=raw_question)
-        elif int(num) == 3:  # 某地天气
-            pass
-        elif int(num) == 4:  # 执行指令
-            # agent_data += await agents.type4.get_command_result(llm=llm, question=raw_question)
-            pass
-        elif int(num) == 5:  # who are you
-            agent_data += agents.type5.get_who_you_are() + "\n"
-        elif int(num) == 6:  # 功能列表
-            agent_data += agents.type6.get_ai_abilities() + "\n"
-
-    # 携带 context 向大模型提问 raw_question
-    assemble_prompt = prompts.get_assemble_prompt(question=raw_question, agent_data=agent_data)
-    print("assemble_prompt", assemble_prompt)
+    if len(classifier_res) == 1 and classifier_res[0] == 7:
+        assemble_prompt = raw_question
+        print("assemble_prompt", assemble_prompt)
+    else:
+        for num in classifier_res:
+            if int(num) == 1:    # 提取页面内容
+                agent_data += await agents.type1.summarize_weblink_content(llm=llm, question=raw_question) + "\n"
+            elif int(num) == 2:  # 联网搜索能力
+                agent_data += await agents.type2.get_search_result(llm=llm, question=raw_question)
+            elif int(num) == 3:  # 某地天气
+                pass
+            elif int(num) == 4:  # 执行指令
+                # agent_data += await agents.type4.get_command_result(llm=llm, question=raw_question)
+                pass
+            elif int(num) == 5:  # who are you
+                agent_data += agents.type5.get_who_you_are() + "\n"
+            elif int(num) == 6:  # 功能列表
+                agent_data += agents.type6.get_ai_abilities() + "\n"
+
+        # 携带 context 向大模型提问 raw_question
+        assemble_prompt = prompts.get_assemble_prompt(question=raw_question, agent_data=agent_data)
+        print("assemble_prompt", assemble_prompt)
 
     # Chat History 策略获取
     chat_history_list = ChatService.get_strategically_chat_history(assemble_prompt, max_length=llm.max_length)
 
     s = prompts.get_kurisu_prompt()
     assemble_res = await llm.ask_model(question=assemble_prompt, system_prompt=s, message_history=chat_history_list)
```

### Comparing `nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/config.py` & `nonebot_plugin_with_ai_agents-0.1.9/nonebot_plugin_with_ai_agents/llm/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/llms/base.py` & `nonebot_plugin_with_ai_agents-0.1.9/nonebot_plugin_with_ai_agents/llm/llms/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/llms/dashscope.py` & `nonebot_plugin_with_ai_agents-0.1.9/nonebot_plugin_with_ai_agents/llm/llms/dashscope.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/llms/glm.py` & `nonebot_plugin_with_ai_agents-0.1.9/nonebot_plugin_with_ai_agents/llm/llms/glm.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/llms/openai.py` & `nonebot_plugin_with_ai_agents-0.1.9/nonebot_plugin_with_ai_agents/llm/llms/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/services.py` & `nonebot_plugin_with_ai_agents-0.1.9/nonebot_plugin_with_ai_agents/llm/services.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/utils/prompts.py` & `nonebot_plugin_with_ai_agents-0.1.9/nonebot_plugin_with_ai_agents/llm/utils/prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     '''
     return prompt
 
 
 def get_kurisu_prompt():
 
     prompt = """
-    你是实验小助手 Kurisu，这个名字来源于《命运石之门》女主角牧濑红莉栖。
+    你是小助手 Kurisu，牧濑红莉栖。偶尔在回复的末尾新开一行添加一点符号表情。
     在回答中尽量少的使用非常规的字符，同时不要超过400字
     注意，在回复中不要提及上述的任何事情，不要复述
     """
     return prompt
 
 
 def get_rikka_prompt():
```

### Comparing `nonebot_plugin_with_ai_agents-0.1.8/nonebot_plugin_with_ai_agents/llm/utils/retrievers.py` & `nonebot_plugin_with_ai_agents-0.1.9/nonebot_plugin_with_ai_agents/llm/utils/retrievers.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.8/pyproject.toml` & `nonebot_plugin_with_ai_agents-0.1.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-with-ai-agents"
-version = "0.1.8"
+version = "0.1.9"
 description = "nonebot_plugin_with_ai_agents 是一个基于基本原理实现的 AI Agents（智能体），拥有联网搜索能力、页面内容提取并学习回答等功能"
 authors = ["yejue <1145331931@qq.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nonebot2 = "^2.0"
```

### Comparing `nonebot_plugin_with_ai_agents-0.1.8/README.md` & `nonebot_plugin_with_ai_agents-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_with_ai_agents-0.1.8/PKG-INFO` & `nonebot_plugin_with_ai_agents-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-with-ai-agents
-Version: 0.1.8
+Version: 0.1.9
 Summary: nonebot_plugin_with_ai_agents 是一个基于基本原理实现的 AI Agents（智能体），拥有联网搜索能力、页面内容提取并学习回答等功能
 Author: yejue
 Author-email: 1145331931@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-with-ai-agents Version: 0.1.8
+Metadata-Version: 2.1 Name: nonebot-plugin-with-ai-agents Version: 0.1.9
 Summary: nonebot_plugin_with_ai_agents æ¯ä¸ä¸ªåºäºåºæ¬åçå®ç°ç AI
 Agentsï¼æºè½ä½ï¼ï¼æ¥æèç½æç´¢è½åãé¡µé¢åå®¹æåå¹¶å­¦ä¹ åç­ç­åè½
 Author: yejue Author-email: 1145331931@qq.com Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

