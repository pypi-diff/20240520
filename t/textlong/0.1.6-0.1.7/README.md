# Comparing `tmp/textlong-0.1.6.tar.gz` & `tmp/textlong-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textlong-0.1.6.tar", max compression
+gzip compressed data, was "textlong-0.1.7.tar", max compression
```

## Comparing `textlong-0.1.6.tar` & `textlong-0.1.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1066 2024-05-17 12:44:59.600013 textlong-0.1.6/LICENSE
--rw-r--r--   0        0        0     1604 2024-05-18 06:08:22.626599 textlong-0.1.6/README.md
--rw-r--r--   0        0        0      950 2024-05-19 15:38:35.384814 textlong-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-17 12:44:59.600533 textlong-0.1.6/textlong/.pypirc
--rw-r--r--   0        0        0      530 2024-05-19 15:14:28.297461 textlong-0.1.6/textlong/__init__.py
--rw-r--r--   0        0        0       22 2024-05-19 15:38:43.220033 textlong-0.1.6/textlong/__version__.py
--rw-r--r--   0        0        0        0 2024-05-17 12:44:59.601026 textlong-0.1.6/textlong/agents/__init__.py
--rw-r--r--   0        0        0     2722 2024-05-17 12:44:59.601163 textlong-0.1.6/textlong/agents/base.py
--rw-r--r--   0        0        0     7036 2024-05-17 12:44:59.601410 textlong-0.1.6/textlong/agents/prompt.py
--rw-r--r--   0        0        0     2370 2024-05-19 07:03:51.711272 textlong-0.1.6/textlong/ai.py
--rw-r--r--   0        0        0     6780 2024-05-17 12:44:59.601940 textlong-0.1.6/textlong/base.py
--rw-r--r--   0        0        0     2511 2024-05-18 03:48:42.318437 textlong-0.1.6/textlong/command.py
--rw-r--r--   0        0        0      304 2024-05-19 00:35:41.802269 textlong-0.1.6/textlong/config.py
--rw-r--r--   0        0        0        0 2024-05-18 02:40:06.723540 textlong-0.1.6/textlong/docs/__init__.py
--rw-r--r--   0        0        0     3591 2024-05-19 12:16:37.280829 textlong-0.1.6/textlong/docs/writing_help.py
--rw-r--r--   0        0        0        0 2024-05-17 12:44:59.602426 textlong-0.1.6/textlong/document_loaders/__init__.py
--rw-r--r--   0        0        0     8955 2024-05-17 12:44:59.602748 textlong-0.1.6/textlong/document_loaders/base.py
--rw-r--r--   0        0        0       57 2024-05-17 12:44:59.602930 textlong-0.1.6/textlong/langgraph/__init__.py
--rw-r--r--   0        0        0     5269 2024-05-17 12:44:59.603160 textlong-0.1.6/textlong/langgraph/tools_calling.py
--rw-r--r--   0        0        0       77 2024-05-17 12:44:59.603326 textlong-0.1.6/textlong/memory/__init__.py
--rw-r--r--   0        0        0    10213 2024-05-17 12:44:59.603589 textlong-0.1.6/textlong/memory/base.py
--rw-r--r--   0        0        0     3839 2024-05-17 12:44:59.603829 textlong-0.1.6/textlong/memory/history.py
--rw-r--r--   0        0        0     3131 2024-05-17 12:44:59.603975 textlong-0.1.6/textlong/memory/memory_manager.py
--rw-r--r--   0        0        0    10875 2024-05-19 08:17:29.283447 textlong-0.1.6/textlong/node.py
--rw-r--r--   0        0        0     6673 2024-05-19 15:21:55.942882 textlong-0.1.6/textlong/projects.py
--rw-r--r--   0        0        0      121 2024-05-18 02:19:48.770966 textlong-0.1.6/textlong/prompts/__init__.py
--rw-r--r--   0        0        0     4187 2024-05-19 14:26:02.963118 textlong-0.1.6/textlong/prompts/hub.py
--rw-r--r--   0        0        0      936 2024-05-17 12:44:59.604351 textlong-0.1.6/textlong/prompts/main.py
--rw-r--r--   0        0        0      385 2024-05-17 12:44:59.604603 textlong-0.1.6/textlong/prompts/translate.py
--rw-r--r--   0        0        0     6114 2024-05-19 14:26:40.868005 textlong-0.1.6/textlong/prompts/writing_prompt.py
--rw-r--r--   0        0        0        0 2024-05-17 12:44:59.604711 textlong-0.1.6/textlong/retrievers/__init__.py
--rw-r--r--   0        0        0     2999 2024-05-17 12:44:59.604917 textlong-0.1.6/textlong/retrievers/base.py
--rw-r--r--   0        0        0     3213 2024-05-19 07:30:31.509304 textlong-0.1.6/textlong/serialize.py
--rw-r--r--   0        0        0     1949 2024-05-18 09:26:30.600466 textlong-0.1.6/textlong/state.py
--rw-r--r--   0        0        0     1983 2024-05-19 15:29:28.868426 textlong-0.1.6/textlong/tree.py
--rw-r--r--   0        0        0     3563 2024-05-19 15:30:49.311152 textlong-0.1.6/textlong/writing.py
--rw-r--r--   0        0        0     2503 1970-01-01 00:00:00.000000 textlong-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-17 12:44:59.600013 textlong-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1604 2024-05-18 06:08:22.626599 textlong-0.1.7/README.md
+-rw-r--r--   0        0        0      950 2024-05-20 01:52:35.288407 textlong-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-17 12:44:59.600533 textlong-0.1.7/textlong/.pypirc
+-rw-r--r--   0        0        0      605 2024-05-20 01:52:14.392217 textlong-0.1.7/textlong/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-20 01:52:27.691763 textlong-0.1.7/textlong/__version__.py
+-rw-r--r--   0        0        0        0 2024-05-17 12:44:59.601026 textlong-0.1.7/textlong/agents/__init__.py
+-rw-r--r--   0        0        0     2722 2024-05-17 12:44:59.601163 textlong-0.1.7/textlong/agents/base.py
+-rw-r--r--   0        0        0     7036 2024-05-17 12:44:59.601410 textlong-0.1.7/textlong/agents/prompt.py
+-rw-r--r--   0        0        0     2370 2024-05-19 07:03:51.711272 textlong-0.1.7/textlong/ai.py
+-rw-r--r--   0        0        0     6780 2024-05-17 12:44:59.601940 textlong-0.1.7/textlong/base.py
+-rw-r--r--   0        0        0     2511 2024-05-18 03:48:42.318437 textlong-0.1.7/textlong/command.py
+-rw-r--r--   0        0        0      304 2024-05-19 00:35:41.802269 textlong-0.1.7/textlong/config.py
+-rw-r--r--   0        0        0        0 2024-05-18 02:40:06.723540 textlong-0.1.7/textlong/docs/__init__.py
+-rw-r--r--   0        0        0     3591 2024-05-19 12:16:37.280829 textlong-0.1.7/textlong/docs/writing_help.py
+-rw-r--r--   0        0        0        0 2024-05-17 12:44:59.602426 textlong-0.1.7/textlong/document_loaders/__init__.py
+-rw-r--r--   0        0        0     8955 2024-05-17 12:44:59.602748 textlong-0.1.7/textlong/document_loaders/base.py
+-rw-r--r--   0        0        0       57 2024-05-17 12:44:59.602930 textlong-0.1.7/textlong/langgraph/__init__.py
+-rw-r--r--   0        0        0     5269 2024-05-17 12:44:59.603160 textlong-0.1.7/textlong/langgraph/tools_calling.py
+-rw-r--r--   0        0        0       77 2024-05-17 12:44:59.603326 textlong-0.1.7/textlong/memory/__init__.py
+-rw-r--r--   0        0        0     8113 2024-05-20 01:45:32.350495 textlong-0.1.7/textlong/memory/base.py
+-rw-r--r--   0        0        0     3839 2024-05-17 12:44:59.603829 textlong-0.1.7/textlong/memory/history.py
+-rw-r--r--   0        0        0     2708 2024-05-20 01:50:58.318560 textlong-0.1.7/textlong/memory/memory_manager.py
+-rw-r--r--   0        0        0    10875 2024-05-19 08:17:29.283447 textlong-0.1.7/textlong/node.py
+-rw-r--r--   0        0        0     6673 2024-05-19 15:21:55.942882 textlong-0.1.7/textlong/projects.py
+-rw-r--r--   0        0        0      121 2024-05-18 02:19:48.770966 textlong-0.1.7/textlong/prompts/__init__.py
+-rw-r--r--   0        0        0     4187 2024-05-19 14:26:02.963118 textlong-0.1.7/textlong/prompts/hub.py
+-rw-r--r--   0        0        0      936 2024-05-17 12:44:59.604351 textlong-0.1.7/textlong/prompts/main.py
+-rw-r--r--   0        0        0      385 2024-05-17 12:44:59.604603 textlong-0.1.7/textlong/prompts/translate.py
+-rw-r--r--   0        0        0     6114 2024-05-19 14:26:40.868005 textlong-0.1.7/textlong/prompts/writing_prompt.py
+-rw-r--r--   0        0        0        0 2024-05-17 12:44:59.604711 textlong-0.1.7/textlong/retrievers/__init__.py
+-rw-r--r--   0        0        0     2999 2024-05-17 12:44:59.604917 textlong-0.1.7/textlong/retrievers/base.py
+-rw-r--r--   0        0        0     3213 2024-05-19 07:30:31.509304 textlong-0.1.7/textlong/serialize.py
+-rw-r--r--   0        0        0     1949 2024-05-18 09:26:30.600466 textlong-0.1.7/textlong/state.py
+-rw-r--r--   0        0        0     1983 2024-05-19 15:29:28.868426 textlong-0.1.7/textlong/tree.py
+-rw-r--r--   0        0        0     3563 2024-05-19 15:30:49.311152 textlong-0.1.7/textlong/writing.py
+-rw-r--r--   0        0        0     2503 1970-01-01 00:00:00.000000 textlong-0.1.7/PKG-INFO
```

### Comparing `textlong-0.1.6/LICENSE` & `textlong-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `textlong-0.1.6/README.md` & `textlong-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `textlong-0.1.6/pyproject.toml` & `textlong-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "textlong"
-version = "0.1.6"
+version = "0.1.7"
 description = "A framework designed to produce long-texts with GPT or other large language models."
 authors = ["arcstep <43801@qq.com>"]
 homepage = "https://github.com/arcstep/textlong"
 repository = "https://github.com/arcstep/textlong.git"
 license = "MIT"
 readme = "README.md"
```

### Comparing `textlong-0.1.6/textlong/__init__.py` & `textlong-0.1.7/textlong/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 
 from textlong.agents.base import (
     PROMPT_REACT,
     PROMPT_COT,
     create_reason_agent,
 )
 
+from textlong.memory import (
+    MemoryManager,
+    WithMemoryBinding,
+)
+
 from textlong.writing import WritingTask
 
 from .projects import (
     create_project,
     list_projects,
     is_content_exist,
     is_prompts_exist,
```

### Comparing `textlong-0.1.6/textlong/agents/base.py` & `textlong-0.1.7/textlong/agents/base.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.6/textlong/agents/prompt.py` & `textlong-0.1.7/textlong/agents/prompt.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.6/textlong/ai.py` & `textlong-0.1.7/textlong/ai.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.6/textlong/base.py` & `textlong-0.1.7/textlong/base.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.6/textlong/command.py` & `textlong-0.1.7/textlong/command.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.6/textlong/docs/writing_help.py` & `textlong-0.1.7/textlong/docs/writing_help.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.6/textlong/document_loaders/base.py` & `textlong-0.1.7/textlong/document_loaders/base.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.6/textlong/langgraph/tools_calling.py` & `textlong-0.1.7/textlong/langgraph/tools_calling.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.6/textlong/memory/base.py` & `textlong-0.1.7/textlong/memory/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -62,28 +62,23 @@
         memory_manager: MemoryManager,
         *,
         input_messages_key: Optional[str] = "input",
         output_messages_key: Optional[str] = None,
         history_messages_key: Optional[str] = "history",
         **kwargs: Any,
     ) -> None:
-        # 提取记忆 _enter_memory / _aenter_memory
-        history_chain: Runnable = RunnableLambda(
-            self._enter_memory, self._aenter_memory
-        ).with_config(run_name="load_history")
-        messages_key = history_messages_key or input_messages_key
-        if messages_key:
-            history_chain = RunnablePassthrough.assign(
-                **{messages_key: history_chain}
-            ).with_config(run_name="insert_history")
+        # 提取记忆 _current_history / _acurrent_history
+        history_chain = RunnablePassthrough.assign(
+            **{history_messages_key: RunnableLambda(self._current_history, self._acurrent_history)}
+        ).with_config(run_name="insert_history")
 
-        # 写入记忆 _exit_memory
+        # 写入记忆 _update_history
         bound = (
-            history_chain | runnable.with_listeners(on_end=self._exit_memory)
-        ).with_config(run_name="WithMemoryBinding")
+            history_chain | runnable
+        ).with_listeners(on_end=self._update_history)
 
         # 构造 config.configurable 中的参数，可以被 Runnable 自举
         _config_specs = [
             ConfigurableFieldSpec(
                 id="session_id",
                 annotation=str,
                 name="Session ID",
@@ -115,34 +110,29 @@
     ) -> Type[BaseModel]:
         super_schema = super().get_input_schema(config)
         if super_schema.__custom_root_type__ or not super_schema.schema().get(
             "properties"
         ):
             from langchain_core.messages import BaseMessage
 
-            fields: Dict = {}
-            if self.input_messages_key and self.history_messages_key:
-                fields[self.input_messages_key] = (
-                    Union[str, BaseMessage, Sequence[BaseMessage]],
-                    ...,
-                )
-            elif self.input_messages_key:
-                fields[self.input_messages_key] = (Sequence[BaseMessage], ...)
-            else:
-                fields["__root__"] = (Sequence[BaseMessage], ...)
+            fields = {self.input_messages_key: (
+                Union[str, BaseMessage, Sequence[BaseMessage]],
+                ...,
+            )}
             return create_model(
                 "RunnableWithChatHistoryInput",
                 **fields,
             )
         else:
             return super_schema
 
     def _get_input_messages(
         self, input_val: Union[str, BaseMessage, Sequence[BaseMessage]]
     ) -> List[BaseMessage]:
+        """从Runnable的输入中，提取要保存的部份"""
         from langchain_core.messages import BaseMessage
 
         if isinstance(input_val, str):
             from langchain_core.messages import HumanMessage
 
             return [HumanMessage(content=input_val)]
         elif isinstance(input_val, BaseMessage):
@@ -154,67 +144,65 @@
                 f"Expected str, BaseMessage, List[BaseMessage], or Tuple[BaseMessage]. "
                 f"Got {input_val}."
             )
 
     def _get_output_messages(
         self, output_val: Union[str, BaseMessage, Sequence[BaseMessage], dict]
     ) -> List[BaseMessage]:
+        """从Runnable的输出中，提取要保存的部份"""
         from langchain_core.messages import BaseMessage
 
-        # 如果output_val是字典就取其中的output键或指定名字的键
+        # 对于AgentExcutor
         if isinstance(output_val, dict):
             output_val = output_val[self.output_messages_key or "output"]
 
+        # 对于字符串
         if isinstance(output_val, str):
             from langchain_core.messages import AIMessage
 
             return [AIMessage(content=output_val)]
+        
+        # 对于BaseMessage
         elif isinstance(output_val, BaseMessage):
             return [output_val]
+
+        # 对于字符串列表、包含字符串的元组
         elif isinstance(output_val, (list, tuple)):
             return list(output_val)
+
         else:
             raise ValueError()
 
-    def _enter_memory(self, input: Any, config: RunnableConfig) -> List[BaseMessage]:
+    def _current_history(self, input: Any, config: RunnableConfig) -> List[BaseMessage]:
         memory = config["configurable"]["memory"]
-        # 提取记忆中应当插入到提示语中的部份
-        if self.history_messages_key:
-            return memory.buffer_as_messages
-        else:
-            input_val = (
-                input if not self.input_messages_key else input[self.input_messages_key]
-            )
-            return memory.buffer_as_messages + self._get_input_messages(input_val)
+        return memory.buffer_as_messages
 
-    async def _aenter_memory(
+    async def _acurrent_history(
         self, input: Dict[str, Any], config: RunnableConfig
     ) -> List[BaseMessage]:
-        return await run_in_executor(config, self._enter_memory, input, config)
+        return await run_in_executor(config, self._current_history, input, config)
 
-    def _exit_memory(self, run: Run, config: RunnableConfig) -> None:
+    def _update_history(self, run: Run, config: RunnableConfig) -> None:
+        """
+        退出时，将输入和输出通过chat_memory保存。
+        """
         memory = config["configurable"]["memory"]
-        hist = memory.chat_memory
+        store = memory.chat_memory
 
-        # Get the input messages
-        inputs = load(run.inputs)
-        input_val = inputs[self.input_messages_key or "input"]
+        # 获得输入
+        inputs = run.inputs
+        input_val = inputs[self.input_messages_key]
         input_messages = self._get_input_messages(input_val)
+        print("input_messages:", input_messages)
 
-        # If historic messages were prepended to the input messages, remove them to
-        # avoid adding duplicate messages to history.
-        if not self.history_messages_key:
-            input_messages = input_messages[len(hist.messages) :]
-
-        # Get the output messages
-        output_val = load(run.outputs)
+        # 获得输出
+        output_val = run.outputs
         output_messages = self._get_output_messages(output_val)
-        hist.add_messages(input_messages + output_messages)
-        
-        # print("_exit_memory", hist)
+        store.add_messages(input_messages + output_messages)
+        print("store:", store)
 
     def _merge_configs(self, *configs: Optional[RunnableConfig]) -> RunnableConfig:
         config = super()._merge_configs(*configs)
         expected_keys = [field_spec.id for field_spec in self.history_factory_config]
 
         configurable = config.get("configurable", {})
 
@@ -229,36 +217,12 @@
             raise ValueError(
                 f"Missing keys {sorted(missing_keys)} in config['configurable'] "
                 f"Expected keys are {sorted(expected_keys)}."
                 f"When using via .invoke() or .stream(), pass in a config; "
                 f"e.g., chain.invoke({example_input}, {example_config})"
             )
 
-        parameter_names = _get_parameter_names(self.memory_manager.get_longterm_memory_factory)
-
-        if len(expected_keys) == 1:
-            # 如果configurable中只有一个参数，无论其是否session_id，都当作位置参数传递给记忆体
-            # 所有记忆体的实现中，都应当将第1个位置参数当作session_id使用
-            memory = self.memory_manager.get_shorterm_memory(configurable[expected_keys[0]])
-        else:
-            # 如果有configurable中有多个参数，就当作键值参数传递给记忆体
-            # 在记忆体的实现中，都应当支持按匹配的键值参数来保存和提取记忆历史
-            # 这在一定程度上提供了定制记忆体的可能性
-            if set(expected_keys) != set(parameter_names):
-                raise ValueError(
-                    f"Expected keys {sorted(expected_keys)} do not match parameter "
-                    f"names {sorted(parameter_names)} of memory_writing."
-                )
-
-            memory = self.memory_manager.get_shorterm_memory(
-                **{key: configurable[key] for key in expected_keys}
-            )
+        memory = self.memory_manager.get_memory_factory(configurable["session_id"])
         config["configurable"]["memory"] = memory
         # print("_merge_configs:", memory)
         
         return config
-
-
-def _get_parameter_names(callable_: GetSessionHistoryCallable) -> List[str]:
-    """提取 callable_ 的键值参数"""
-    sig = inspect.signature(callable_)
-    return list(sig.parameters.keys())
```

### Comparing `textlong-0.1.6/textlong/memory/history.py` & `textlong-0.1.7/textlong/memory/history.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.6/textlong/memory/memory_manager.py` & `textlong-0.1.7/textlong/memory/memory_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,66 @@
 from typing import Callable, Optional
 from langchain.memory import ConversationBufferMemory
 from langchain.memory.chat_memory import BaseChatMemory
+from langchain.memory import ConversationBufferWindowMemory
 from langchain_core.messages import BaseMessage
 from langchain_core.chat_history import BaseChatMessageHistory
 from langchain_community.chat_message_histories import ChatMessageHistory
 from typing import Any, Dict, Union, List
 from copy import deepcopy
 
 class MemoryManager:
-    """实现记忆的工厂类，将短期记忆和持久化记忆绑定在一起管理。
-    
+    """
+    实现记忆窗口和持久化捆绑管理。
+
     默认将记忆存储在内存中，但可以替换为redis存储等持久化方案；
     也支持按对话轮次、Token数、知识图谱等管理短期记忆。
     """
 
     # 短期记忆管理，用于记忆模板
-    _shorterm_memory: BaseChatMemory
-    
-    # 为每一个session_id单独建立记忆管理器
-    _shorterm_memory_store: dict[str, BaseChatMemory] = {}
-
-    # 基于内存的记忆存储
-    _history_in_memory: dict[str, ChatMessageHistory] = {}
+    _memory: BaseChatMemory
+    _memory_dict: dict[str, BaseChatMemory] = {}
 
     # 记忆存储的回调函数，要求使用 session_id 位置参数
-    get_longterm_memory_factory: Callable[[str], BaseChatMessageHistory]
+    get_store_factory: Callable[[str], BaseChatMessageHistory]
 
     def __init__(
         self,
-        longterm_memory_factory: Optional[Callable[[str], BaseChatMessageHistory]] = None,
-        shorterm_memory: Optional[BaseChatMemory] = None
+        store_factory: Optional[Callable[[str], BaseChatMessageHistory]] = None,
+        memory: Optional[BaseChatMemory] = None
     ) -> None:
-        # 默认使用内存保存长期记忆
-        # 可更换保存到redis、文件、数据库等
-        if longterm_memory_factory is None:
-            self.get_longterm_memory_factory = self._get_history_in_memory
+        self.get_store_factory = store_factory or self._get_history_in_memory
+        self._memory = memory or ConversationBufferWindowMemory(k=20, return_messages=True)
+
+    def get_memory(self, session_id: str = "default") -> List[BaseMessage]:
+        """返回短期内存记忆"""
+        if session_id in self._memory_dict:
+            memory = self._memory_dict[session_id]
+            return memory.buffer_as_messages
         else:
-            self.get_longterm_memory_factory = longterm_memory_factory
+            return []
 
-        # 默认使用内存保存窗口记忆
-        # 可更换为使用限定对话窗口、限定总Token数等
-        if shorterm_memory is None:
-            self._shorterm_memory = ConversationBufferMemory()
+    def get_store(self, session_id: str = "default") -> List[BaseMessage]:
+        """返回长期记忆存储"""
+        if session_id in self._memory_dict:
+            memory = self._memory_dict[session_id]
+            return memory.chat_memory.messages
         else:
-            self._shorterm_memory = shorterm_memory
+            return []    
+
+    # 结合 session_id 构造记忆对象
+    def get_memory_factory(self, session_id: str = "default") -> BaseChatMemory:
+        if session_id not in self._memory_dict:
+            store = self.get_store_factory(session_id)
+            self._memory_dict[session_id] = deepcopy(self._memory)
+            self._memory_dict[session_id].chat_memory = store
 
-    # 返回短期记忆的消息列表
-    def shorterm_messages(self, session_id: str = "default") -> List[BaseMessage]:
-        memory = self.get_shorterm_memory(session_id)
-        return memory.buffer_as_messages
-
-    # 返回长期记忆的消息列表
-    def longterm_messages(self, session_id: str = "default") -> List[BaseMessage]:
-        memory = self.get_shorterm_memory(session_id)
-        return memory.chat_memory.messages
-
-    # 返回记忆管理器对象
-    def get_shorterm_memory(self, session_id: str = "default") -> BaseChatMemory:
-        if session_id not in self._shorterm_memory_store:
-            history = self.get_longterm_memory_factory(session_id)
-            self._shorterm_memory_store[session_id] = deepcopy(self._shorterm_memory)
-            self._shorterm_memory_store[session_id].chat_memory = history
+        return self._memory_dict[session_id]
 
-        return self._shorterm_memory_store[session_id]
+    # 基于内存的记忆存储
+    _store_in_memory: dict[str, ChatMessageHistory] = {}
 
     def _get_history_in_memory(self, session_id: str) -> BaseChatMessageHistory:
         """默认的基于内存的记忆"""
-        if session_id not in self._history_in_memory:
-            self._history_in_memory[session_id] = ChatMessageHistory()
-        return self._history_in_memory[session_id]
+        if session_id not in self._store_in_memory:
+            self._store_in_memory[session_id] = ChatMessageHistory()
+        return self._store_in_memory[session_id]
```

### Comparing `textlong-0.1.6/textlong/node.py` & `textlong-0.1.7/textlong/node.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.6/textlong/projects.py` & `textlong-0.1.7/textlong/projects.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.6/textlong/prompts/hub.py` & `textlong-0.1.7/textlong/prompts/hub.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.6/textlong/prompts/main.py` & `textlong-0.1.7/textlong/prompts/main.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.6/textlong/prompts/writing_prompt.py` & `textlong-0.1.7/textlong/prompts/writing_prompt.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.6/textlong/retrievers/base.py` & `textlong-0.1.7/textlong/retrievers/base.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.6/textlong/serialize.py` & `textlong-0.1.7/textlong/serialize.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.6/textlong/state.py` & `textlong-0.1.7/textlong/state.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.6/textlong/tree.py` & `textlong-0.1.7/textlong/tree.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.6/textlong/writing.py` & `textlong-0.1.7/textlong/writing.py`

 * *Files identical despite different names*

### Comparing `textlong-0.1.6/PKG-INFO` & `textlong-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textlong
-Version: 0.1.6
+Version: 0.1.7
 Summary: A framework designed to produce long-texts with GPT or other large language models.
 Home-page: https://github.com/arcstep/textlong
 License: MIT
 Author: arcstep
 Author-email: 43801@qq.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

