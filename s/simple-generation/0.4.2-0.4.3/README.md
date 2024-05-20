# Comparing `tmp/simple_generation-0.4.2.tar.gz` & `tmp/simple_generation-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_generation-0.4.2.tar", max compression
+gzip compressed data, was "simple_generation-0.4.3.tar", max compression
```

## Comparing `simple_generation-0.4.2.tar` & `simple_generation-0.4.3.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      590 2024-04-17 15:47:25.745257 simple_generation-0.4.2/LICENSE
--rw-r--r--   0        0        0    15122 2024-04-30 11:52:24.409385 simple_generation-0.4.2/README.md
--rw-r--r--   0        0        0      879 2024-04-30 15:14:39.722157 simple_generation-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      225 2024-04-17 15:47:26.249259 simple_generation-0.4.2/simple_generation/__init__.py
--rw-r--r--   0        0        0    20455 2024-04-29 15:27:22.529854 simple_generation-0.4.2/simple_generation/simple_generation.py
--rw-r--r--   0        0        0     4459 2024-04-17 15:47:26.253259 simple_generation-0.4.2/simple_generation/utils.py
--rw-r--r--   0        0        0       36 2024-04-29 15:27:22.537854 simple_generation-0.4.2/simple_generation/vlm/__init__.py
--rw-r--r--   0        0        0     1826 2024-04-30 11:48:57.944947 simple_generation-0.4.2/simple_generation/vlm/utils.py
--rw-r--r--   0        0        0    13209 2024-04-30 14:50:27.934808 simple_generation-0.4.2/simple_generation/vlm/vlm.py
--rw-r--r--   0        0        0    16191 1970-01-01 00:00:00.000000 simple_generation-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      172 2024-05-20 07:37:52.937258 simple_generation-0.4.3/AUTHORS.rst
+-rw-r--r--   0        0        0      590 2024-05-20 07:37:52.937476 simple_generation-0.4.3/LICENSE
+-rw-r--r--   0        0        0    15122 2024-05-20 07:37:52.937748 simple_generation-0.4.3/README.md
+-rw-r--r--   0        0        0      879 2024-05-20 08:04:49.777587 simple_generation-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      225 2024-05-20 08:05:00.050033 simple_generation-0.4.3/simple_generation/__init__.py
+-rw-r--r--   0        0        0    20455 2024-05-20 07:37:52.944794 simple_generation-0.4.3/simple_generation/simple_generation.py
+-rw-r--r--   0        0        0     4459 2024-05-20 07:37:52.944889 simple_generation-0.4.3/simple_generation/utils.py
+-rw-r--r--   0        0        0       36 2024-05-20 07:37:52.944981 simple_generation-0.4.3/simple_generation/vlm/__init__.py
+-rw-r--r--   0        0        0     2062 2024-05-20 07:37:52.945044 simple_generation-0.4.3/simple_generation/vlm/utils.py
+-rw-r--r--   0        0        0    13336 2024-05-20 07:37:52.945176 simple_generation-0.4.3/simple_generation/vlm/vlm.py
+-rw-r--r--   0        0        0    16191 1970-01-01 00:00:00.000000 simple_generation-0.4.3/PKG-INFO
```

### Comparing `simple_generation-0.4.2/LICENSE` & `simple_generation-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_generation-0.4.2/README.md` & `simple_generation-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `simple_generation-0.4.2/pyproject.toml` & `simple_generation-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "simple-generation"
-version = "0.4.2"
+version = "0.4.3"
 description = "A python package to run inference with HuggingFace checkpoints wrapping many convenient features."
 authors = ["Giuseppe Attanasio <giuseppeattanasio6@gmail.com>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-transformers = ">=4.39.3"
+transformers = ">=4.41.0"
 tokenizers = ">=0.13.3"
 accelerate = ">=0.20.3"
 datasets = ">=2.12.0"
 peft = ">=0.3.0"
 bitsandbytes = ">=0.39.1"
 pyopenssl = ">=23.2.0"
 optimum = ">=1.9.0"
```

### Comparing `simple_generation-0.4.2/simple_generation/simple_generation.py` & `simple_generation-0.4.3/simple_generation/simple_generation.py`

 * *Files identical despite different names*

### Comparing `simple_generation-0.4.2/simple_generation/utils.py` & `simple_generation-0.4.3/simple_generation/utils.py`

 * *Files identical despite different names*

### Comparing `simple_generation-0.4.2/simple_generation/vlm/utils.py` & `simple_generation-0.4.3/simple_generation/vlm/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Mapping
 from enum import Enum
 import pdb
 
 
 class VLMType(Enum):
     LLAVA = "LLAVA"
+    LLAVA_NEXT = "LLAVA_NEXT"
     IDEFICS = "IDEFICS"
     IDEFICS2 = "IDEFICS2"
     BLIP2 = "BLIP2"
 
 
 @dataclass
 class VLMCollator:
@@ -21,14 +22,18 @@
     def __call__(self, batch):
         prompts = [x["text"] for x in batch]
         images = [x["image"] for x in batch]
 
         if self.vlm_type == VLMType.LLAVA:
             prompts = [f"USER: <image>\n{p}\nASSISTANT:" for p in prompts]
             batch = self.processor(prompts, images, **self.processor_args)
+        
+        elif self.vlm_type == VLMType.LLAVA_NEXT:
+            prompts = [f"[INST] <image>\n{p} [/INST]" for p in prompts]
+            batch = self.processor(prompts, images, **self.processor_args)
 
         elif self.vlm_type == VLMType.IDEFICS:
             inputs = [
                 [f"User: {p}", i, "<end_of_utterance>", "\nAssistant:"]
                 for p, i in zip(prompts, images)
             ]
             batch = self.processor(inputs, **self.processor_args)
```

### Comparing `simple_generation-0.4.2/simple_generation/vlm/vlm.py` & `simple_generation-0.4.3/simple_generation/vlm/vlm.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,16 @@
         except Exception as e:
             logger.warning("Could not load generation config. Using default one.")
             self.generation_config = DefaultGenerationConfig()
 
         self.config = AutoConfig.from_pretrained(model_name_or_path)
         if self.config.architectures[0] == "LlavaForConditionalGeneration":
             self.vlm_type = VLMType.LLAVA
+        if self.config.architectures[0] == "LlavaNextForConditionalGeneration":
+            self.vlm_type = VLMType.LLAVA_NEXT
         elif self.config.architectures[0] == "IdeficsForVisionText2Text":
             self.vlm_type = VLMType.IDEFICS
         elif self.config.architectures[0] == "Idefics2ForConditionalGeneration":
             self.vlm_type = VLMType.IDEFICS2
         elif self.config.architectures[0] == "Blip2ForConditionalGeneration":
             self.vlm_type = VLMType.BLIP2
         else:
```

### Comparing `simple_generation-0.4.2/PKG-INFO` & `simple_generation-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-generation
-Version: 0.4.2
+Version: 0.4.3
 Summary: A python package to run inference with HuggingFace checkpoints wrapping many convenient features.
 License: Apache Software License 2.0
 Author: Giuseppe Attanasio
 Author-email: giuseppeattanasio6@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -19,15 +19,15 @@
 Requires-Dist: datasets (>=2.12.0)
 Requires-Dist: optimum (>=1.9.0)
 Requires-Dist: peft (>=0.3.0)
 Requires-Dist: pillow (>=10.3.0) ; extra == "vlm"
 Requires-Dist: pyopenssl (>=23.2.0)
 Requires-Dist: scipy (>=1.10.1)
 Requires-Dist: tokenizers (>=0.13.3)
-Requires-Dist: transformers (>=4.39.3)
+Requires-Dist: transformers (>=4.41.0)
 Description-Content-Type: text/markdown
 
 ![Simple Generation Dining](/docs/_static/banner.png)
 
 [![Latest PyPI version](https://img.shields.io/pypi/v/simple-generation.svg)](https://pypi.python.org/pypi/simple-generation)
 [![Documentation Status](https://readthedocs.org/projects/simple-generation/badge/?version=latest)](https://simple-generation.readthedocs.io/en/latest/?version=latest)
 [![downloads badge](https://pepy.tech/badge/simple-generation/month)](https://pepy.tech/project/simple-generation)
```

