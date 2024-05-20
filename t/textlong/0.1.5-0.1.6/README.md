# Comparing `tmp/textlong-0.1.5.tar.gz` & `tmp/textlong-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textlong-0.1.5.tar", max compression
+gzip compressed data, was "textlong-0.1.6.tar", max compression
```

## Comparing `textlong-0.1.5.tar` & `textlong-0.1.6.tar`

### file list

```diff
@@ -1,34 +1,37 @@
--rw-r--r--   0        0        0     1066 2024-05-17 12:44:59.600013 textlong-0.1.5/LICENSE
--rw-r--r--   0        0        0     1604 2024-05-18 06:08:22.626599 textlong-0.1.5/README.md
--rw-r--r--   0        0        0      880 2024-05-18 09:48:11.407830 textlong-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-17 12:44:59.600533 textlong-0.1.5/textlong/.pypirc
--rw-r--r--   0        0        0      340 2024-05-18 02:21:59.329892 textlong-0.1.5/textlong/__init__.py
--rw-r--r--   0        0        0       22 2024-05-18 09:48:16.664063 textlong-0.1.5/textlong/__version__.py
--rw-r--r--   0        0        0        0 2024-05-17 12:44:59.601026 textlong-0.1.5/textlong/agents/__init__.py
--rw-r--r--   0        0        0     2722 2024-05-17 12:44:59.601163 textlong-0.1.5/textlong/agents/base.py
--rw-r--r--   0        0        0     7036 2024-05-17 12:44:59.601410 textlong-0.1.5/textlong/agents/prompt.py
--rw-r--r--   0        0        0     2370 2024-05-18 02:24:33.016543 textlong-0.1.5/textlong/ai.py
--rw-r--r--   0        0        0     6780 2024-05-17 12:44:59.601940 textlong-0.1.5/textlong/base.py
--rw-r--r--   0        0        0     2511 2024-05-18 03:48:42.318437 textlong-0.1.5/textlong/command.py
--rw-r--r--   0        0        0        0 2024-05-18 02:40:06.723540 textlong-0.1.5/textlong/docs/__init__.py
--rw-r--r--   0        0        0     3557 2024-05-18 03:57:52.669524 textlong-0.1.5/textlong/docs/writing_help.py
--rw-r--r--   0        0        0        0 2024-05-17 12:44:59.602426 textlong-0.1.5/textlong/document_loaders/__init__.py
--rw-r--r--   0        0        0     8955 2024-05-17 12:44:59.602748 textlong-0.1.5/textlong/document_loaders/base.py
--rw-r--r--   0        0        0       57 2024-05-17 12:44:59.602930 textlong-0.1.5/textlong/langgraph/__init__.py
--rw-r--r--   0        0        0     5269 2024-05-17 12:44:59.603160 textlong-0.1.5/textlong/langgraph/tools_calling.py
--rw-r--r--   0        0        0       77 2024-05-17 12:44:59.603326 textlong-0.1.5/textlong/memory/__init__.py
--rw-r--r--   0        0        0    10213 2024-05-17 12:44:59.603589 textlong-0.1.5/textlong/memory/base.py
--rw-r--r--   0        0        0     3839 2024-05-17 12:44:59.603829 textlong-0.1.5/textlong/memory/history.py
--rw-r--r--   0        0        0     3131 2024-05-17 12:44:59.603975 textlong-0.1.5/textlong/memory/memory_manager.py
--rw-r--r--   0        0        0     9693 2024-05-18 09:28:36.074535 textlong-0.1.5/textlong/node.py
--rw-r--r--   0        0        0      121 2024-05-18 02:19:48.770966 textlong-0.1.5/textlong/prompts/__init__.py
--rw-r--r--   0        0        0      936 2024-05-17 12:44:59.604351 textlong-0.1.5/textlong/prompts/main.py
--rw-r--r--   0        0        0      385 2024-05-17 12:44:59.604603 textlong-0.1.5/textlong/prompts/translate.py
--rw-r--r--   0        0        0     6442 2024-05-18 03:59:57.327185 textlong-0.1.5/textlong/prompts/writing_prompt.py
--rw-r--r--   0        0        0        0 2024-05-17 12:44:59.604711 textlong-0.1.5/textlong/retrievers/__init__.py
--rw-r--r--   0        0        0     2999 2024-05-17 12:44:59.604917 textlong-0.1.5/textlong/retrievers/base.py
--rw-r--r--   0        0        0     5358 2024-05-18 09:41:35.737286 textlong-0.1.5/textlong/serialize.py
--rw-r--r--   0        0        0     1949 2024-05-18 09:26:30.600466 textlong-0.1.5/textlong/state.py
--rw-r--r--   0        0        0     2026 2024-05-17 15:18:37.918040 textlong-0.1.5/textlong/tree.py
--rw-r--r--   0        0        0     2438 2024-05-18 03:33:05.691759 textlong-0.1.5/textlong/writing.py
--rw-r--r--   0        0        0     2505 1970-01-01 00:00:00.000000 textlong-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-17 12:44:59.600013 textlong-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1604 2024-05-18 06:08:22.626599 textlong-0.1.6/README.md
+-rw-r--r--   0        0        0      950 2024-05-19 15:38:35.384814 textlong-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-17 12:44:59.600533 textlong-0.1.6/textlong/.pypirc
+-rw-r--r--   0        0        0      530 2024-05-19 15:14:28.297461 textlong-0.1.6/textlong/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-19 15:38:43.220033 textlong-0.1.6/textlong/__version__.py
+-rw-r--r--   0        0        0        0 2024-05-17 12:44:59.601026 textlong-0.1.6/textlong/agents/__init__.py
+-rw-r--r--   0        0        0     2722 2024-05-17 12:44:59.601163 textlong-0.1.6/textlong/agents/base.py
+-rw-r--r--   0        0        0     7036 2024-05-17 12:44:59.601410 textlong-0.1.6/textlong/agents/prompt.py
+-rw-r--r--   0        0        0     2370 2024-05-19 07:03:51.711272 textlong-0.1.6/textlong/ai.py
+-rw-r--r--   0        0        0     6780 2024-05-17 12:44:59.601940 textlong-0.1.6/textlong/base.py
+-rw-r--r--   0        0        0     2511 2024-05-18 03:48:42.318437 textlong-0.1.6/textlong/command.py
+-rw-r--r--   0        0        0      304 2024-05-19 00:35:41.802269 textlong-0.1.6/textlong/config.py
+-rw-r--r--   0        0        0        0 2024-05-18 02:40:06.723540 textlong-0.1.6/textlong/docs/__init__.py
+-rw-r--r--   0        0        0     3591 2024-05-19 12:16:37.280829 textlong-0.1.6/textlong/docs/writing_help.py
+-rw-r--r--   0        0        0        0 2024-05-17 12:44:59.602426 textlong-0.1.6/textlong/document_loaders/__init__.py
+-rw-r--r--   0        0        0     8955 2024-05-17 12:44:59.602748 textlong-0.1.6/textlong/document_loaders/base.py
+-rw-r--r--   0        0        0       57 2024-05-17 12:44:59.602930 textlong-0.1.6/textlong/langgraph/__init__.py
+-rw-r--r--   0        0        0     5269 2024-05-17 12:44:59.603160 textlong-0.1.6/textlong/langgraph/tools_calling.py
+-rw-r--r--   0        0        0       77 2024-05-17 12:44:59.603326 textlong-0.1.6/textlong/memory/__init__.py
+-rw-r--r--   0        0        0    10213 2024-05-17 12:44:59.603589 textlong-0.1.6/textlong/memory/base.py
+-rw-r--r--   0        0        0     3839 2024-05-17 12:44:59.603829 textlong-0.1.6/textlong/memory/history.py
+-rw-r--r--   0        0        0     3131 2024-05-17 12:44:59.603975 textlong-0.1.6/textlong/memory/memory_manager.py
+-rw-r--r--   0        0        0    10875 2024-05-19 08:17:29.283447 textlong-0.1.6/textlong/node.py
+-rw-r--r--   0        0        0     6673 2024-05-19 15:21:55.942882 textlong-0.1.6/textlong/projects.py
+-rw-r--r--   0        0        0      121 2024-05-18 02:19:48.770966 textlong-0.1.6/textlong/prompts/__init__.py
+-rw-r--r--   0        0        0     4187 2024-05-19 14:26:02.963118 textlong-0.1.6/textlong/prompts/hub.py
+-rw-r--r--   0        0        0      936 2024-05-17 12:44:59.604351 textlong-0.1.6/textlong/prompts/main.py
+-rw-r--r--   0        0        0      385 2024-05-17 12:44:59.604603 textlong-0.1.6/textlong/prompts/translate.py
+-rw-r--r--   0        0        0     6114 2024-05-19 14:26:40.868005 textlong-0.1.6/textlong/prompts/writing_prompt.py
+-rw-r--r--   0        0        0        0 2024-05-17 12:44:59.604711 textlong-0.1.6/textlong/retrievers/__init__.py
+-rw-r--r--   0        0        0     2999 2024-05-17 12:44:59.604917 textlong-0.1.6/textlong/retrievers/base.py
+-rw-r--r--   0        0        0     3213 2024-05-19 07:30:31.509304 textlong-0.1.6/textlong/serialize.py
+-rw-r--r--   0        0        0     1949 2024-05-18 09:26:30.600466 textlong-0.1.6/textlong/state.py
+-rw-r--r--   0        0        0     1983 2024-05-19 15:29:28.868426 textlong-0.1.6/textlong/tree.py
+-rw-r--r--   0        0        0     3563 2024-05-19 15:30:49.311152 textlong-0.1.6/textlong/writing.py
+-rw-r--r--   0        0        0     2503 1970-01-01 00:00:00.000000 textlong-0.1.6/PKG-INFO
```

### Comparing `textlong-0.1.5/LICENSE` & `textlong-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `textlong-0.1.5/README.md` & `textlong-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `textlong-0.1.5/pyproject.toml` & `textlong-0.1.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 [tool.poetry]
 name = "textlong"
-version = "0.1.5"
+version = "0.1.6"
 description = "A framework designed to produce long-texts with GPT or other large language models."
 authors = ["arcstep <43801@qq.com>"]
 homepage = "https://github.com/arcstep/textlong"
 repository = "https://github.com/arcstep/textlong.git"
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 pydantic = ">=1,<3"
-langchain = "^0.1.20"
-langchain-community = "^0.0.38"
+langchain = ">=0.1.0,<0.3.0"
 python-dotenv = "^1.0.1"
 python-statemachine = "^2.2.0"
 pydot = "^2.0.0"
+langchain-community = ">=0.0.38,<0.3.0"
 
 [tool.poetry.group.dev.dependencies]
 asyncio = "^3.4.3"
 setuptools = "^69.1.0"
 poetry2setup = "^1.1.0"
 ipykernel = "^6.29.2"
 pytest = "^8.0.1"
 pydantic = "1.10.13"
 docx2txt = "^0.8"
 pypdf = "^4.1.0"
 markdown = "^3.6"
+langchain-openai = "^0.1.7"
+langchain-zhipu = "^4.1.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.poetry.packages]]
 include = "textlong/**/*"
```

### Comparing `textlong-0.1.5/textlong/agents/base.py` & `textlong-0.1.6/textlong/agents/base.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.5/textlong/agents/prompt.py` & `textlong-0.1.6/textlong/agents/prompt.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.5/textlong/ai.py` & `textlong-0.1.6/textlong/ai.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                 from langchain_openai import ChatOpenAI
                 self.llm = ChatOpenAI(model_name="gpt-4-turbo")
             else:
                 raise BaseException("您必须指定一个LLM，或者配置正确的环境变量：ZHIPUAI_API_KEY！")
         else:
             self.llm = llm
 
-        self.memory = memory or ConversationBufferWindowMemory(k=20, return_messages=True)
+        self.memory = memory or ConversationBufferWindowMemory(k=10, return_messages=True)
 
         self.retry_max: int = 5
 
     def ask_ai(self, task, prompt=None, return_json: bool=False):
         """AI推理"""
 
         prompt = prompt or create_writing_help_prompt()
```

### Comparing `textlong-0.1.5/textlong/base.py` & `textlong-0.1.6/textlong/base.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.5/textlong/command.py` & `textlong-0.1.6/textlong/command.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.5/textlong/docs/writing_help.py` & `textlong-0.1.6/textlong/docs/writing_help.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 WRITING_HELP = """
-# 这是一个关于textlong和WritingTask的使用指南
+# `textlong`包使用指南
 
-## 基本介绍
-`textlong`是一个基于大语言模型的长文本生成框架，是一个python包。
-主要特点是通过将生成任务拆解为树形层次结构的任务提纲，再为提纲中的每个子任务生成文本，以便合成超长的文本结果。
+`textlong`是一个python包, 基于大语言模型的AI工作, 可用于长文写作、长文理解等任务。
 
-本文介绍的WritingTask模块就是专门负责生成任务的。
+## `WritingTask`模块。
 
-## 如何使用
+`WritingTask`模块专门负责生成任务。
+其工作方式是将写作任务拆解为写作提纲和子任务，再执行每个子任务，最后合成完整文本。
 
-### invoke方法
+### 写作功能
+
+#### 创建写作项目
+
+```python
+from textlong import 
+```
+
+#### invoke方法
 最灵活的方法是调用WritingTask的invoke方法。
 
-第一步，你应当准备好访问大语言模型所需的APIKEY，你可以选择你喜欢的任何LLM，如ChatGPT、智谱AI等，
+第一步，你应当准备好访问大语言模型所需的APIKEY，你可以选择你喜欢的任何LLM,如ChatGPT、智谱AI等，
 默认支持的是智谱AI。
 
 第二步，你要在代码中创建`WritingTask`对象。
 
 **使用默认的智谱AI:**
 
 ```python
 from textlong import WritingTask
 task = WritingTask()
+```
 
 **使用ChatGPT:**
 
 ```python
 from textlong import WritingTask
 from langchain_openai import ChatOpenAI
 
@@ -37,33 +45,32 @@
 以下是一个简单的代码示范，使用task命令让AI生成800字的信；
 紧接着，代码ok命令将生成的内容保存。
 
 ```python
 task.invoke("task 致孩子的一封信, 800字")
 task.invoke("ok")
 ```
-### auto_write方法
+#### auto_write方法
 使用auto_write方法可以在生成任务后自动执行ok命令，自动生成和确认所有子任务，直至全文创作完毕。
 
 ```python
 task.auto_write("task 致孩子的一封信, 800字")
 ```
 
-### repl_write方法
+#### repl_write方法
 如果你希望精细控制，还可以使用repl_write方法。
 
 ```python
 task.repl_write("task 致孩子的一封信, 800字")
 ```
 
 repl_write会进入一个控制台循环，这通常是在`Jupyter Notes`或命令行终端的环境中。
 在控制台循环中，你可以不断输入`ok`指令，直至完成，也可以选择其他指令，执行重新生成、修改扩写指南等任务。
 
-
-## 命令清单
+### invoke和repl中可用的命令清单
 
 这些命令并非shell脚本，而是在WritingTask的invoke方法中的参数。
 一般的使用方法例如：`writingTaskObj.invoke("<命令名称> <可选的参数>")`
 
 **注意: [ ] 表示该命令尚未完成开发; [x] 表示已经完成开发、可以正常使用。**
 
 - [x] `help` 向AI寻求帮助：优化提示语为对指令的说明
```

### Comparing `textlong-0.1.5/textlong/document_loaders/base.py` & `textlong-0.1.6/textlong/document_loaders/base.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.5/textlong/langgraph/tools_calling.py` & `textlong-0.1.6/textlong/langgraph/tools_calling.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.5/textlong/memory/base.py` & `textlong-0.1.6/textlong/memory/base.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.5/textlong/memory/history.py` & `textlong-0.1.6/textlong/memory/history.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.5/textlong/memory/memory_manager.py` & `textlong-0.1.6/textlong/memory/memory_manager.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.5/textlong/node.py` & `textlong-0.1.6/textlong/node.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,69 +1,80 @@
 from typing import Any, Dict, Iterator, List, Optional, Union
 from langchain_core.runnables import Runnable
 from langchain.prompts import ChatPromptTemplate, MessagesPlaceholder
 from langchain_core.output_parsers import JsonOutputParser
 from .serialize import ContentSerialize
 from .state import ContentState
 from .command import BaseCommand
-from .prompts import (
-    create_writing_help_prompt,
-    create_writing_init_prompt,
-    create_writing_todo_prompt,
-)
 from .ai import BaseAI
 import datetime
 import random
 
 class ContentNode(ContentState, ContentSerialize, BaseCommand):
     """
     树形结构的内容存储节点，段落内容保存在叶子节点，而提纲保存在children的列表中。
     """
 
     def __init__(
         self,
+        ## self
         type: str="unknown",
         words_limit: int=500,
         words_advice: int=None,
         title: str=None,
         howto: str=None,
-        summarise: str=None,
-        text: str=None,
+        ## AI
         last_ai_reply_json: Dict[str, Any]={},
-        is_draft=False,
+        is_draft: bool=False,
         llm=None,
+        memory=None,
+        ## ContentState
         state=None,
+        ## 段落
+        summarise: str=None,
+        text: str=None,
+        ## prompt
+        help_prompt=None,
+        init_prompt=None,
+        outline_prompt=None,
+        paragraph_prompt=None,
+        ## project_id, index, parent 等
         **kwargs,
     ):
+
+        BaseCommand.__init__(self)
+        ContentSerialize.__init__(self, **kwargs)
         if state:
             ContentState.__init__(self, start_value=state)
         else:
             ContentState.__init__(self)
 
-        ContentSerialize.__init__(self, **kwargs)
-
+        # self
         self.type = type
-
-        # 如果超出这个段落字数就拆分为提纲
         self.words_limit = words_limit
-
-        # 扩写指南
         self.words_advice = words_advice
         self.title = title
         self.howto = howto
 
         # 段落
         self.summarise = summarise
         self.text = text
+        
+        # prompt
+        self.help_prompt = help_prompt
+        self.init_prompt = init_prompt
+        self.outline_prompt = outline_prompt
+        self.paragraph_prompt = paragraph_prompt
 
         # 最后的AI回复
         self.last_ai_reply_json = last_ai_reply_json
-        self.is_draft: bool = is_draft
-        self.ai = BaseAI(llm)
+        self.is_draft = is_draft
+        self.ai = BaseAI(llm, memory)
 
+    # 指令清单
     howto_commands = ["title", "words_advice", "howto"]
     result_commands = ["summarise", "text"]
     state_commands = ["state", "memory", "ok", "todo", "modi", "task"]
 
     # inherit
     @property
     def commands(self) -> List[str]:
@@ -115,37 +126,45 @@
         return "help"
 
     def help_ai(self, task: str=None):
         """向AI询问，获得生成结果"""
 
         default_task = "有哪些命令可以使用？"
 
-        prompt = create_writing_help_prompt()
+        prompt = self.help_prompt
         chat = self.ai.ask_ai(task or default_task, prompt, return_json=False)
 
         return chat
 
     def ask_ai(self, task: str=None):
         """向AI询问，获得生成结果"""
 
         default_task = "请开始。"
 
         if self.state == "init":
-            prompt = create_writing_init_prompt()
+            prompt = self.init_prompt
 
-        elif self.state == "todo":
-            prompt = create_writing_todo_prompt(
+        elif self.state == "todo" and self.type == "outline":
+            prompt = self.outline_prompt.partial(
+                title=self.title,
+                content_type=self.type,
+                words_limit=self.words_limit,
+                words_advice=self.words_advice,
+                howto=self.howto,
+                outline_exist=self.root.get_outlines()
+            )
+        elif self.state == "todo" and self.type == "paragraph":
+            prompt = self.paragraph_prompt.partial(
                 title=self.title,
                 content_type=self.type,
                 words_limit=self.words_limit,
                 words_advice=self.words_advice,
                 howto=self.howto,
                 outline_exist=self.root.get_outlines()
             )
-
         else:
             raise NotImplementedError(f"<{self.id}> 对象在状态[{self.state}]没有指定提示语模板")
 
         json = self.ai.ask_ai(task or default_task, prompt, return_json=True)
         self.last_ai_reply_json = json
         self.is_draft = True
 
@@ -195,15 +214,22 @@
                         type=type,
                         title=title,
                         howto=howto,
                         words_advice=words_advice,
                         last_ai_reply_json=item,
                         is_draft=False,
                         item_class=ContentNode,
+
+                        ## 以下这些属性将会继承父节点的配置
+                        help_prompt=self.help_prompt,
+                        init_prompt=self.init_prompt,
+                        outline_prompt=self.outline_prompt,
+                        paragraph_prompt=self.paragraph_prompt,
                         llm=self.ai.llm,
+                        memory=self.ai.memory,
                     )
                     node.edit()
 
             elif self.type == "paragraph":
                 self.reply_json_validator(self.last_ai_reply_json, ["内容摘要", "详细内容"])
                 self.summarise = self.last_ai_reply_json["内容摘要"]
                 self.text = self.last_ai_reply_json["详细内容"]
@@ -259,19 +285,21 @@
     def content(self) -> Dict[str, Union[str, int]]:
         return {
             "id": self.id,
             "type": self.type,
             "state": self.state,
             "is_complete": self.is_complete,
             "is_draft": self.is_draft,
+            "words_limit": self.words_limit,
             "words_advice": self.words_advice,
             "title": self.title or "",
             "howto": self.howto or "",
-            "summarise": self.summarise or None,
+            "summarise": self.summarise or "",
             "text": self.text or "",
+            "last_ai_reply_json": self.last_ai_reply_json,
         }
 
     def get_outlines(self) -> List[Dict[str, Union[str, int]]]:
         """获得大纲清单"""
         outlines = [
             f"{x['id']} {x['title']} \n  扩写指南 >>> {x['howto']}\n  内容摘要 >>> {x['summarise']}"
             for x in self.all_content
```

### Comparing `textlong-0.1.5/textlong/prompts/main.py` & `textlong-0.1.6/textlong/prompts/main.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.5/textlong/prompts/writing_prompt.py` & `textlong-0.1.6/textlong/prompts/writing_prompt.py`

 * *Files 19% similar despite different names*

```diff
@@ -86,86 +86,72 @@
 _AUTO_OUTLINE_OR_PARAGRAPH_PROMPT = """
 你现在的任务是编写《{{title}}》，字数大约为{{words_advice}}字。
 扩写依据为：{{howto}}
 注意，你所写的内容是下面总提纲的一部份：
 {{outline_exist}}
 """
 
-
 def create_writing_help_prompt(system_prompt:str = None):
     """咨询系统如何使用"""
 
     prompt = ChatPromptTemplate.from_messages([
         ("system", system_prompt or HELP_SYSTEM_PROMPT),
         ("ai", "我有哪些资料可以参考？"),
         ("human", "你的资料如下：\n{{doc}}"),
         MessagesPlaceholder(variable_name="history"),
         ("human", "{{task}}"),
-    ], template_format="jinja2").partial(
+    ], template_format="mustache").partial(
         doc=WRITING_HELP
     )
     
     return prompt
 
-def create_writing_init_prompt(main_prompt=None, task_prompt=None, output_format=None, json_instruction=None):
-
+def create_writing_init_prompt():
+    main_prompt = MAIN_PROMPT
+    task_prompt = _INIT_TASK
+    output_prompt = _INIT_FORMAT
+    json_instruction = _JSON_INSTRUCTION 
+    
     prompt = ChatPromptTemplate.from_messages([
-        ("system", main_prompt or MAIN_PROMPT),
+        ("system", main_prompt),
         ("ai", "OK"),
         MessagesPlaceholder(variable_name="history"),
         ("human", "{{task}}"),
-    ], template_format="jinja2").partial(
+    ], template_format="mustache").partial(
         # 任务指南
-        task_instruction=task_prompt or _INIT_TASK,
+        task_instruction=task_prompt,
         # 输出格式要求
-        output_format=output_format or _INIT_FORMAT,
+        output_format=output_prompt,
         # JSON严格控制
-        json_instruction=json_instruction or _JSON_INSTRUCTION,
+        json_instruction=json_instruction,
     )
 
     return prompt
 
-def create_writing_todo_prompt(
-    title: str,
-    content_type: str="paragraph",
-    words_limit: int=500,
-    words_advice: int=500,
-    howto: str=None,
-    outline_exist: List[Any]=None,
-    main_prompt: str=None,
-    auto_prompt: str=None,
-    json_instruction: str=None,
-):
+def create_writing_todo_prompt(content_type: str="paragraph"):
     main_prompt = MAIN_PROMPT
     auto_prompt = _AUTO_OUTLINE_OR_PARAGRAPH_PROMPT
     json_instruction = _JSON_INSTRUCTION 
 
     if content_type == "outline":
         task_prompt   = _OUTLINE_TASK
         output_format = _OUTLINE_FORMAT
-    else:
+    elif content_type == "paragraph":
         task_prompt   = _PARAGRAPH_TASK
         output_format = _PARAGRAPH_FORMAT
+    else:
+        raise ValueError(f"content_type只能是 [outline|paragraph], 无法支持[{content_type}]")
 
     prompt = ChatPromptTemplate.from_messages([
         ("system", main_prompt),
         ("ai", "有什么具体要求？"),
         ("human", auto_prompt),
         ("ai", "OK"),
         MessagesPlaceholder(variable_name="history"),
         ("human", "{{task}}")
-    ], template_format="jinja2").partial(
-        # 字数限制
-        words_limit=words_limit,
-        words_advice=words_advice,
-        # 写作要求
-        title=title,
-        outline_exist=outline_exist,
+    ], template_format="mustache").partial(
         task_instruction=task_prompt,
-        howto=howto,
-        # 输出格式要求
         output_format=output_format,
-        # JSON严格控制
         json_instruction=json_instruction,
     )
 
     return prompt
```

### Comparing `textlong-0.1.5/textlong/retrievers/base.py` & `textlong-0.1.6/textlong/retrievers/base.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.5/textlong/state.py` & `textlong-0.1.6/textlong/state.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.5/textlong/tree.py` & `textlong-0.1.6/textlong/tree.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 from typing import Any, Dict, Iterator, List, Optional, Union
 from .node import ContentNode
 from .command import BaseCommand
 
 class ContentTree(BaseCommand):
     """内容管理树。"""
 
-    def __init__(
-        self,
-        todo_node: Optional[ContentNode]=None,
-        llm=None,
-        **kwargs
-    ):
-        super().__init__(**kwargs)
-
-        self.todo_node = ContentNode(llm=llm) if todo_node == None else todo_node
+    def __init__(self, node=None, **kwargs):
+        BaseCommand.__init__(self)
+        if node:
+            self.todo_node = node
+        else:
+            self.todo_node = ContentNode(**kwargs)
 
     @property
     def root(self):
         return self.todo_node.root
 
     # inherit
     @property
```

### Comparing `textlong-0.1.5/PKG-INFO` & `textlong-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: textlong
-Version: 0.1.5
+Version: 0.1.6
 Summary: A framework designed to produce long-texts with GPT or other large language models.
 Home-page: https://github.com/arcstep/textlong
 License: MIT
 Author: arcstep
 Author-email: 43801@qq.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: langchain (>=0.1.20,<0.2.0)
-Requires-Dist: langchain-community (>=0.0.38,<0.0.39)
+Requires-Dist: langchain (>=0.1.0,<0.3.0)
+Requires-Dist: langchain-community (>=0.0.38,<0.3.0)
 Requires-Dist: pydantic (>=1,<3)
 Requires-Dist: pydot (>=2.0.0,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: python-statemachine (>=2.2.0,<3.0.0)
 Project-URL: Repository, https://github.com/arcstep/textlong.git
 Description-Content-Type: text/markdown
```

