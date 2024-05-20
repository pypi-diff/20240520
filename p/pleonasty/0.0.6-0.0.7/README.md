# Comparing `tmp/pleonasty-0.0.6.tar.gz` & `tmp/pleonasty-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pleonasty-0.0.6.tar", last modified: Tue May 14 11:47:53 2024, max compression
+gzip compressed data, was "pleonasty-0.0.7.tar", last modified: Mon May 20 20:05:17 2024, max compression
```

## Comparing `pleonasty-0.0.6.tar` & `pleonasty-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 11:47:53.641718 pleonasty-0.0.6/
--rw-rw-rw-   0        0        0     1089 2024-03-15 19:33:10.000000 pleonasty-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1385 2024-05-14 11:47:53.640718 pleonasty-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      621 2024-03-15 20:09:12.000000 pleonasty-0.0.6/README.MD
--rw-rw-rw-   0        0        0      830 2024-05-14 11:47:31.000000 pleonasty-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-14 11:47:53.641718 pleonasty-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-14 11:47:53.634718 pleonasty-0.0.6/src/
--rw-rw-rw-   0        0        0        0 2024-03-15 19:46:12.000000 pleonasty-0.0.6/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 11:47:53.640718 pleonasty-0.0.6/src/pleonasty.egg-info/
--rw-rw-rw-   0        0        0     1385 2024-05-14 11:47:53.000000 pleonasty-0.0.6/src/pleonasty.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2024-05-14 11:47:53.000000 pleonasty-0.0.6/src/pleonasty.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 11:47:53.000000 pleonasty-0.0.6/src/pleonasty.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2024-05-14 11:47:53.000000 pleonasty-0.0.6/src/pleonasty.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-14 11:47:53.000000 pleonasty-0.0.6/src/pleonasty.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    14839 2024-05-14 11:15:26.000000 pleonasty-0.0.6/src/pleonasty.py
+drwxrwxrwx   0        0        0        0 2024-05-20 20:05:17.017531 pleonasty-0.0.7/
+-rw-rw-rw-   0        0        0     1089 2024-03-15 19:33:10.000000 pleonasty-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1385 2024-05-20 20:05:17.017019 pleonasty-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      621 2024-03-15 20:09:12.000000 pleonasty-0.0.7/README.MD
+-rw-rw-rw-   0        0        0      830 2024-05-20 20:01:36.000000 pleonasty-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-20 20:05:17.017531 pleonasty-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 20:05:17.011737 pleonasty-0.0.7/src/
+-rw-rw-rw-   0        0        0        0 2024-03-15 19:46:12.000000 pleonasty-0.0.7/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 20:05:17.016506 pleonasty-0.0.7/src/pleonasty.egg-info/
+-rw-rw-rw-   0        0        0     1385 2024-05-20 20:05:16.000000 pleonasty-0.0.7/src/pleonasty.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2024-05-20 20:05:16.000000 pleonasty-0.0.7/src/pleonasty.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 20:05:16.000000 pleonasty-0.0.7/src/pleonasty.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2024-05-20 20:05:16.000000 pleonasty-0.0.7/src/pleonasty.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-20 20:05:16.000000 pleonasty-0.0.7/src/pleonasty.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    16483 2024-05-20 20:00:02.000000 pleonasty-0.0.7/src/pleonasty.py
```

### Comparing `pleonasty-0.0.6/LICENSE` & `pleonasty-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pleonasty-0.0.6/PKG-INFO` & `pleonasty-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pleonasty
-Version: 0.0.6
+Version: 0.0.7
 Summary: A very simple abstraction for LLMs to get single responses to a given input.
 Author-email: "Ryan L. Boyd" <ryan@ryanboyd.io>
 Project-URL: Homepage, https://github.com/ryanboyd/pleonasty
 Project-URL: Issues, https://github.com/ryanboyd/pleonasty/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pleonasty-0.0.6/README.MD` & `pleonasty-0.0.7/README.MD`

 * *Files identical despite different names*

### Comparing `pleonasty-0.0.6/pyproject.toml` & `pleonasty-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 build-backend = "setuptools.build_meta"
 
 
 [project]
 
 name = "pleonasty"
 
-version = "0.0.6"
+version = "0.0.7"
 
 authors = [
   { name="Ryan L. Boyd", email="ryan@ryanboyd.io" },
 ]
 
 description = "A very simple abstraction for LLMs to get single responses to a given input."
```

### Comparing `pleonasty-0.0.6/src/pleonasty.egg-info/PKG-INFO` & `pleonasty-0.0.7/src/pleonasty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pleonasty
-Version: 0.0.6
+Version: 0.0.7
 Summary: A very simple abstraction for LLMs to get single responses to a given input.
 Author-email: "Ryan L. Boyd" <ryan@ryanboyd.io>
 Project-URL: Homepage, https://github.com/ryanboyd/pleonasty
 Project-URL: Issues, https://github.com/ryanboyd/pleonasty/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pleonasty-0.0.6/src/pleonasty.py` & `pleonasty-0.0.7/src/pleonasty.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,14 +62,16 @@
                  model: str,
                  tokenizer: str,
                  offload_folder: str,
                  #llm_format: InstructionFormat,
                  hf_token: str = None
                  ):
 
+        self.model_name_str = model
+        self.tokenizer_name_str = tokenizer
         self.result = None
         self.message_context = []
         #self.llm_format = llm_format
 
         if torch.cuda.is_available():
             torch.cuda.empty_cache()
             torch.set_default_device("cuda")
@@ -336,14 +338,51 @@
                 raise MessageContextException("""Your prompt set need to be contained in dictionaries.
                          Each dictionary must have both a "role" and "content" key.""")
 
         return self.tokenizer.apply_chat_template(prompt_messages, 
                                                   tokenize=False,
                                                   add_generation_prompt=True)
 
+    def chat_mode(self, max_length: int = 1000, bot_name: str = "Bot") -> None:
+    
+        # just disabling all warnings for now, as there appear to be many warnings that are not relevant
+        transformers.logging.set_verbosity_error()
+    
+        print("Type 'quit' (without the quotes) to exit chat mode.")
+        text = ""
+        step = 0
+        while True:
+            # take user input
+            text = input(">> You:")
+
+            if text.strip() == "quit":
+                break
+
+            # encode the input and add end of string token
+            input_ids = self.tokenizer.encode(text + self.tokenizer.eos_token, return_tensors="pt")
+            # concatenate new user input with chat history (if there is)
+            bot_input_ids = torch.cat([chat_history_ids, input_ids], dim=-1) if step > 0 else input_ids
+            step += 1
+            # generate a bot response
+            chat_history_ids = self.model.generate(
+                bot_input_ids,
+                max_length=max_length,
+                do_sample=True,
+                top_k=10,
+                temperature=.75,
+                pad_token_id=self.tokenizer.eos_token_id,
+            )
+            #print the output
+            output = self.tokenizer.decode(chat_history_ids[:, bot_input_ids.shape[-1]:][0],
+                                           skip_special_tokens=True)
+            print(f"\r\n{bot_name}: {output.strip('assistant').strip()}\r\n")
+        
+        transformers.logging.set_verbosity_info()
+        return
+
 
 
 # some potential stuff for parsing jsons
 #import ast
 #import json
 #from pprint import pprint
```

