# Comparing `tmp/radprompter-1.1.3.tar.gz` & `tmp/radprompter-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radprompter-1.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "radprompter-1.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `radprompter-1.1.3.tar` & `radprompter-1.1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     6148 2024-05-15 00:50:49.718415 radprompter-1.1.3/.DS_Store
--rw-r--r--   0        0        0     3169 2024-05-19 17:32:04.647315 radprompter-1.1.3/.gitignore
--rw-r--r--   0        0        0    11357 2024-05-14 18:23:37.432618 radprompter-1.1.3/LICENSE
--rw-r--r--   0        0        0     2689 2024-05-19 21:37:15.946367 radprompter-1.1.3/README.md
--rw-r--r--   0        0        0    91362 2024-05-19 21:36:28.548393 radprompter-1.1.3/logo.png
--rw-r--r--   0        0        0      705 2024-05-20 13:17:12.301636 radprompter-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      225 2024-05-19 18:13:05.689042 radprompter-1.1.3/radprompter/__init__.py
--rw-r--r--   0        0        0       21 2024-05-20 13:18:03.421131 radprompter-1.1.3/radprompter/__version__.py
--rw-r--r--   0        0        0      146 2024-05-20 02:33:21.208331 radprompter-1.1.3/radprompter/clients/__init__.py
--rw-r--r--   0        0        0      586 2024-05-19 22:16:28.933183 radprompter-1.1.3/radprompter/clients/clients.py
--rw-r--r--   0        0        0     2651 2024-05-20 02:37:42.872389 radprompter-1.1.3/radprompter/clients/huggingface/clients.py
--rw-r--r--   0        0        0     3022 2024-05-19 22:09:18.270492 radprompter-1.1.3/radprompter/clients/openai/clients.py
--rw-r--r--   0        0        0       27 2024-05-14 22:18:09.544596 radprompter-1.1.3/radprompter/prompts/__init__.py
--rw-r--r--   0        0        0     9907 2024-05-19 18:00:58.295860 radprompter-1.1.3/radprompter/prompts/prompts.py
--rw-r--r--   0        0        0     7054 2024-05-19 21:54:55.853203 radprompter-1.1.3/radprompter/radprompter.py
--rw-r--r--   0        0        0     1089 2024-05-14 18:23:37.434577 radprompter-1.1.3/sample_reports/sample_report_1.txt
--rw-r--r--   0        0        0     1388 2024-05-14 18:23:37.434671 radprompter-1.1.3/sample_reports/sample_report_2.txt
--rw-r--r--   0        0        0     1374 2024-05-14 18:23:37.434764 radprompter-1.1.3/sample_reports/sample_report_3.txt
--rw-r--r--   0        0        0     6148 2024-05-19 19:37:48.126029 radprompter-1.1.3/tutorials/.DS_Store
--rw-r--r--   0        0        0    16856 2024-05-20 02:44:22.407044 radprompter-1.1.3/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb
--rw-r--r--   0        0        0      386 2024-05-19 18:49:48.028574 radprompter-1.1.3/tutorials/01_Basic-Usecase/01_Basic-Usecase.toml
--rw-r--r--   0        0        0    17598 2024-05-19 20:43:40.346642 radprompter-1.1.3/tutorials/02_RDP-Templating/02_RDP-Templating.ipynb
--rw-r--r--   0        0        0     1716 2024-05-19 18:34:44.363741 radprompter-1.1.3/tutorials/02_RDP-Templating/02_RDP-Templating.toml
--rw-r--r--   0        0        0    19012 2024-05-19 20:43:59.917234 radprompter-1.1.3/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.ipynb
--rw-r--r--   0        0        0     1884 2024-05-19 19:04:34.358936 radprompter-1.1.3/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.toml
--rw-r--r--   0        0        0    26880 2024-05-19 20:44:10.453045 radprompter-1.1.3/tutorials/04_Using-Schemas/04_Using-Schemas.ipynb
--rw-r--r--   0        0        0     4478 2024-05-19 19:55:16.714928 radprompter-1.1.3/tutorials/04_Using-Schemas/04_Using-Schemas.toml
--rw-r--r--   0        0        0    23827 2024-05-19 20:45:24.923958 radprompter-1.1.3/tutorials/05_Assistant-Prefill/05_Assistant-Prefill.ipynb
--rw-r--r--   0        0        0     3277 2024-05-19 20:44:47.851630 radprompter-1.1.3/tutorials/05_Assistant-Prefill/05_Assistant-Prefill.toml
--rw-r--r--   0        0        0        0 2024-05-15 18:54:34.909069 radprompter-1.1.3/tutorials/README.md
--rw-r--r--   0        0        0     3270 1970-01-01 00:00:00.000000 radprompter-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3179 2024-05-20 13:36:09.252853 radprompter-1.1.5/.gitignore
+-rw-r--r--   0        0        0    11357 2024-05-20 13:12:44.869856 radprompter-1.1.5/LICENSE
+-rw-r--r--   0        0        0     2820 2024-05-20 16:25:04.092868 radprompter-1.1.5/README.md
+-rw-r--r--   0        0        0    91362 2024-05-20 13:12:44.870856 radprompter-1.1.5/logo.png
+-rw-r--r--   0        0        0      705 2024-05-20 13:21:03.040821 radprompter-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0      244 2024-05-20 14:12:23.709526 radprompter-1.1.5/radprompter/__init__.py
+-rw-r--r--   0        0        0       21 2024-05-20 16:23:05.789689 radprompter-1.1.5/radprompter/__version__.py
+-rw-r--r--   0        0        0      146 2024-05-20 13:12:44.874856 radprompter-1.1.5/radprompter/clients/__init__.py
+-rw-r--r--   0        0        0      586 2024-05-20 14:15:49.896582 radprompter-1.1.5/radprompter/clients/clients.py
+-rw-r--r--   0        0        0     3231 2024-05-20 16:16:17.141616 radprompter-1.1.5/radprompter/clients/huggingface/clients.py
+-rw-r--r--   0        0        0     3022 2024-05-20 13:12:44.878856 radprompter-1.1.5/radprompter/clients/openai/clients.py
+-rw-r--r--   0        0        0       27 2024-05-20 13:12:44.879856 radprompter-1.1.5/radprompter/prompts/__init__.py
+-rw-r--r--   0        0        0     9907 2024-05-20 13:12:44.879856 radprompter-1.1.5/radprompter/prompts/prompts.py
+-rw-r--r--   0        0        0     7303 2024-05-20 15:54:59.559882 radprompter-1.1.5/radprompter/radprompter.py
+-rw-r--r--   0        0        0     1089 2024-05-20 13:12:44.882856 radprompter-1.1.5/sample_reports/sample_report_1.txt
+-rw-r--r--   0        0        0     1388 2024-05-20 13:12:44.883856 radprompter-1.1.5/sample_reports/sample_report_2.txt
+-rw-r--r--   0        0        0     1374 2024-05-20 13:12:44.883856 radprompter-1.1.5/sample_reports/sample_report_3.txt
+-rw-r--r--   0        0        0    16552 2024-05-20 13:37:57.069928 radprompter-1.1.5/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb
+-rw-r--r--   0        0        0      386 2024-05-20 13:12:44.887856 radprompter-1.1.5/tutorials/01_Basic-Usecase/01_Basic-Usecase.toml
+-rw-r--r--   0        0        0    17598 2024-05-20 13:12:44.888856 radprompter-1.1.5/tutorials/02_RDP-Templating/02_RDP-Templating.ipynb
+-rw-r--r--   0        0        0     1716 2024-05-20 13:12:44.889856 radprompter-1.1.5/tutorials/02_RDP-Templating/02_RDP-Templating.toml
+-rw-r--r--   0        0        0    19012 2024-05-20 13:12:44.890856 radprompter-1.1.5/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.ipynb
+-rw-r--r--   0        0        0     1884 2024-05-20 13:12:44.891856 radprompter-1.1.5/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.toml
+-rw-r--r--   0        0        0    26880 2024-05-20 13:12:44.892856 radprompter-1.1.5/tutorials/04_Using-Schemas/04_Using-Schemas.ipynb
+-rw-r--r--   0        0        0     4478 2024-05-20 15:54:06.767356 radprompter-1.1.5/tutorials/04_Using-Schemas/04_Using-Schemas.toml
+-rw-r--r--   0        0        0    23843 2024-05-20 16:17:06.473108 radprompter-1.1.5/tutorials/05_JSON-Prefill/05_JSON-Prefill.ipynb
+-rw-r--r--   0        0        0     3277 2024-05-20 13:12:44.895856 radprompter-1.1.5/tutorials/05_JSON-Prefill/05_JSON-Prefill.toml
+-rw-r--r--   0        0        0    17925 2024-05-20 16:22:17.611209 radprompter-1.1.5/tutorials/06_HuggingFace-Client/06_HuggingFace-Client.ipynb
+-rw-r--r--   0        0        0     1922 2024-05-20 16:01:46.474938 radprompter-1.1.5/tutorials/06_HuggingFace-Client/06_HuggingFace-Client.toml
+-rw-r--r--   0        0        0        0 2024-05-20 13:12:44.896856 radprompter-1.1.5/tutorials/README.md
+-rw-r--r--   0        0        0     3401 1970-01-01 00:00:00.000000 radprompter-1.1.5/PKG-INFO
```

### Comparing `radprompter-1.1.3/.gitignore` & `radprompter-1.1.5/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Custom .gitignore for Python projects
 *.log
 output/
 tutorials/*/*.csv
 tutorials/*/*.log
+.DS_Store
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `radprompter-1.1.3/LICENSE` & `radprompter-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.3/README.md` & `radprompter-1.1.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -60,15 +60,16 @@
 
 | Tutorial                    | Description                                         | Notebook                                                                         |
 |-----------------------------|-----------------------------------------------------|----------------------------------------------------------------------------------|
 | 01_Basic-Usecase            | Covers the basic usage of RadPrompter               | [📓](./tutorials/01_Basic-Usecase)     |
 | 02_RDP-Templating           | Introduces the `[PROMPTS]` section and `rdp` operator | [📓](./tutorials/02_RDP-Templating)    |
 | 03_Multiturn-Prompting      | Demonstrates multi-turn prompting                   | [📓](./tutorials/03_Multiturn-Prompting) |
 | 04_Using-Schemas            | Shows how to use schemas for structured output      | [📓](./tutorials/04_Using-Schemas)     |
-| 05_Assistant-Prefill        | Covers using assistant prefills                     | [📓](./tutorials/05_Assistant-Prefill)  |
+| 05_JSON-Prefill        | Covers using assistant prefills                     | [📓](./tutorials/05_JSON-Prefill)  |
+| 06_HuggingFace-Client        | Covers using the new `HuggingFaceClient`                     | [📓](./tutorials/06_HuggingFace-Client)  |
 
 ## Contributing
 
 We welcome contributions! If you have any updates or improvements to the package, please open an issue or submit a pull request. We're happy to review and incorporate your changes.
 
 ## Authors
```

### Comparing `radprompter-1.1.3/logo.png` & `radprompter-1.1.5/logo.png`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.3/pyproject.toml` & `radprompter-1.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.3/radprompter/clients/clients.py` & `radprompter-1.1.5/radprompter/clients/clients.py`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.3/radprompter/clients/huggingface/clients.py` & `radprompter-1.1.5/radprompter/clients/huggingface/clients.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,45 +23,59 @@
         for stop_id in self.stop_ids:
             if stop_id not in input_ids[0, -len(self.stop_ids):]:
                 return torch.zeros(input_ids.shape[0], dtype=torch.bool, device=input_ids.device)
         
         return torch.ones(input_ids.shape[0], dtype=torch.bool, device=input_ids.device)
 
 class HuggingFaceClient(Client):
-    def __init__(self, model_name, hf_model, hf_tokenizer, **kwargs):
+    def __init__(self, hf_model, hf_tokenizer, **kwargs):
         if os.environ['HAS_TRANSFORMERS'] != "True":
             raise ImportError("HuggingFaceClient requires the `transformers` package to be installed.")
-        
+
+        model_name = hf_model.__class__.__name__
         super().__init__(model_name)
-        self.tokenizer = hf_tokenizer
-        self.model = hf_model
+        self.hf_tokenizer = hf_tokenizer
+        self.hf_model = hf_model
         self.temperature = kwargs.pop("temperature", 0.7)
         self.top_p = kwargs.pop("top_p", 0.9)
         self.frequency_penalty = kwargs.pop("frequency_penalty", 0.0)
         self.max_tokens = kwargs.pop("max_tokens", 200)
 
     def chat_complete(self, messages, stop=None, max_tokens=None):
         if max_tokens is None:
             max_tokens = self.max_tokens
 
-        tokenized_chat = self.tokenizer.apply_chat_template(
+        if messages[-1]['role'] == "assistant":
+            last_message = messages[-1]['content']
+            messages = messages[:-1]
+        else:
+            last_message = None
+            
+        tokenized_chat = self.hf_tokenizer.apply_chat_template(
             messages, 
             tokenize=True, 
             add_generation_prompt=True, 
             return_tensors="pt"
         )
+        
+        if last_message:
+            tokenized_last_message = self.hf_tokenizer.encode(last_message, return_tensors="pt", add_special_tokens=False)
+            tokenized_chat = torch.cat([tokenized_chat, tokenized_last_message], dim=-1)
 
         stopping_criteria_list = StoppingCriteriaList()
         if stop:
-            stopping_criteria_list.append(StopStringCriteria(stop, self.tokenizer))
+            stopping_criteria_list.append(StopStringCriteria(stop, self.hf_tokenizer))
 
-        outputs = self.model.generate(
-            tokenized_chat['input_ids'], 
+        outputs = self.hf_model.generate(
+            tokenized_chat, 
             max_new_tokens=max_tokens, 
             temperature=self.temperature, 
             top_p=self.top_p, 
             num_return_sequences=1,
             stopping_criteria=stopping_criteria_list
         )
 
-        response = self.tokenizer.decode(outputs[0], skip_special_tokens=True)
-        return response
+        prompt_size = tokenized_chat.size(-1)
+        answer_tokens = outputs[0, prompt_size:]
+        answer_text = self.hf_tokenizer.decode(answer_tokens, skip_special_tokens=True)
+
+        return answer_text
```

### Comparing `radprompter-1.1.3/radprompter/clients/openai/clients.py` & `radprompter-1.1.5/radprompter/clients/openai/clients.py`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.3/radprompter/prompts/prompts.py` & `radprompter-1.1.5/radprompter/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.3/radprompter/radprompter.py` & `radprompter-1.1.5/radprompter/radprompter.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pandas as pd
 import re
 from copy import deepcopy
 from tqdm import tqdm
 from datetime import datetime
 from concurrent.futures import ThreadPoolExecutor, as_completed
 import csv
-from .clients import OpenAIClient
+from .clients import OpenAIClient, HuggingFaceClient
 from .__version__ import __version__
 
 class RadPrompter():
     def __init__(self, client, prompt, output_file, hide_blocks=False, concurrency=1):
         self.client = client
         self.prompt = prompt
         self.hide_blocks = hide_blocks
@@ -21,14 +21,18 @@
         
         if file_exists:
             print(f"WARNING: Output file {self.output_file} already exists. Appending to it. If you want to create a new file, please delete the existing file first or pass a new file name.")
         
         if isinstance(self.client, OpenAIClient) and self.prompt.response_templates.count("") != prompt.num_turns:
             print("WARNING: OpenAI client does not accept response templates and will be ignored.")
             self.prompt.response_templates = [""]*prompt.num_turns
+            
+        if isinstance(self.client, HuggingFaceClient) and self.concurrency > 1:
+            print("WARNING: HuggingFace client does not support concurrency > 1 and will be set to 1.")
+            self.concurrency = 1
         
         self.log = {
             "RadPrompter Version": __version__,
             "Model": self.client.model,
             "Prompt TOML": self.prompt.prompt_file,
             "Prompt Version": self.prompt.version,
             "Prompt Hash": self.prompt.md5_hash,
```

### Comparing `radprompter-1.1.3/sample_reports/sample_report_1.txt` & `radprompter-1.1.5/sample_reports/sample_report_1.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.3/sample_reports/sample_report_2.txt` & `radprompter-1.1.5/sample_reports/sample_report_2.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.3/sample_reports/sample_report_3.txt` & `radprompter-1.1.5/sample_reports/sample_report_3.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.3/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb` & `radprompter-1.1.5/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8644198468168917%*

 * *Differences: {"'cells'": '{14: {\'outputs\': {0: {\'data\': {\'text/plain\': ["{\'report\': \'Clinical '*

 * *            'Information:\\\\n67-year-old male with shortness of breath and pleuritic chest pain. '*

 * *            'Rule out pulmonary embolism.\\\\n\\\\nTechnique:\\\\nCT pulmonary angiography with IV '*

 * *            'contrast was performed.\\\\n\\\\nFindings:\\\\nThere are filling defects within the '*

 * *            'right and left main pulmonary arteries extending into the lobar branches, compatible '*

 * *            'with bi […]*

```diff
@@ -212,16 +212,16 @@
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "{'report': 'Clinical Information:\\n72-year-old female with sudden onset shortness of breath and hypoxia. Evaluate for pulmonary embolism.\\nTechnique:\\nCT pulmonary angiography with IV contrast was performed.\\nFindings:\\nThere is a large saddle embolus extending from the main pulmonary artery into the right and left main pulmonary arteries. Multiple filling defects are also seen within the segmental and subsegmental branches bilaterally, indicating additional pulmonary emboli.\\nThe right ventricle appears dilated at 4.6 cm, greater than the left ventricle. There is flattening of the interventricular septum, suggesting right heart strain.\\nMosaic perfusion is present within the lungs bilaterally, likely representing pulmonary infarcts.\\nSmall bilateral pleural effusions are noted.\\nImpression:\\n\\nSaddle pulmonary embolism involving the main pulmonary artery, right and left main branches, and multiple segmental/subsegmental branches.\\nFindings of right heart strain with right ventricular dilation and interventricular septal flattening.\\nBilateral pleural effusions, likely due to pulmonary infarcts.\\n\\nRecommendation:\\nEmergent anticoagulation therapy is recommended given the large burden of pulmonary arterial clot and evidence of right heart strain. Surgical or catheter-based embolectomy may need to be considered. Echocardiography can further evaluate right heart function and pulmonary pressures.',\n",
-                            " 'file_name': '../../sample_reports/sample_report_2.txt'}"
+                            "{'report': 'Clinical Information:\\n67-year-old male with shortness of breath and pleuritic chest pain. Rule out pulmonary embolism.\\n\\nTechnique:\\nCT pulmonary angiography with IV contrast was performed.\\n\\nFindings:\\nThere are filling defects within the right and left main pulmonary arteries extending into the lobar branches, compatible with bilateral pulmonary emboli. No evidence of right heart strain.\\n\\nGround glass opacities are present within the peripheral lungs bilaterally, suggesting a component of hemorrhage.\\n\\nThe main pulmonary arteries are dilated, with a diameter of 3.4 cm on the right and 3.1 cm on the left (upper limits of normal).\\n\\nNo pleural effusion is identified.\\n\\nImpression:\\n1. Bilateral pulmonary emboli involving the right and left main pulmonary arteries and lobar branches.\\n2. Findings suggestive of pulmonary hemorrhage.\\n3. Pulmonary artery dilation suggesting chronic pulmonary hypertension.\\n\\nRecommendation:\\nClinical correlation is recommended. Anticoagulation therapy should be initiated if not already started. Consider echocardiography to evaluate for right heart strain.',\n",
+                            " 'file_name': '../../sample_reports/sample_report_1.txt'}"
                         ]
                     },
                     "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -252,15 +252,15 @@
             "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "Processing items: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 3/3 [00:00<00:00, 11.64it/s]\n"
+                        "Processing items: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 3/3 [00:00<00:00, 15.28it/s]\n"
                     ]
                 }
             ],
             "source": [
                 "engine(reports)"
             ]
         },
@@ -308,45 +308,45 @@
                             "      <th></th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>Abnormal</td>\n",
-                            "      <td>Here is an example radiology report describing...</td>\n",
-                            "      <td>../../sample_reports/sample_report_3.txt</td>\n",
+                            "      <td>Clinical Information:\\n72-year-old female with...</td>\n",
+                            "      <td>../../sample_reports/sample_report_2.txt</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>Abnormal</td>\n",
-                            "      <td>Clinical Information:\\n72-year-old female with...</td>\n",
-                            "      <td>../../sample_reports/sample_report_2.txt</td>\n",
+                            "      <td>Clinical Information:\\n67-year-old male with s...</td>\n",
+                            "      <td>../../sample_reports/sample_report_1.txt</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>Abnormal</td>\n",
-                            "      <td>Clinical Information:\\n67-year-old male with s...</td>\n",
-                            "      <td>../../sample_reports/sample_report_1.txt</td>\n",
+                            "      <td>Here is an example radiology report describing...</td>\n",
+                            "      <td>../../sample_reports/sample_report_3.txt</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "      default_response                                             report  \\\n",
                             "index                                                                       \n",
-                            "1             Abnormal  Here is an example radiology report describing...   \n",
-                            "0             Abnormal  Clinical Information:\\n72-year-old female with...   \n",
-                            "2             Abnormal  Clinical Information:\\n67-year-old male with s...   \n",
+                            "1             Abnormal  Clinical Information:\\n72-year-old female with...   \n",
+                            "0             Abnormal  Clinical Information:\\n67-year-old male with s...   \n",
+                            "2             Abnormal  Here is an example radiology report describing...   \n",
                             "\n",
                             "                                      file_name  \n",
                             "index                                            \n",
-                            "1      ../../sample_reports/sample_report_3.txt  \n",
-                            "0      ../../sample_reports/sample_report_2.txt  \n",
-                            "2      ../../sample_reports/sample_report_1.txt  "
+                            "1      ../../sample_reports/sample_report_2.txt  \n",
+                            "0      ../../sample_reports/sample_report_1.txt  \n",
+                            "2      ../../sample_reports/sample_report_3.txt  "
                         ]
                     },
                     "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -376,22 +376,22 @@
             "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "RadPrompter Version: 1.1.2\n",
+                        "RadPrompter Version: 1.1.3\n",
                         "Model: meta-llama/Meta-Llama-3-8B-Instruct\n",
-                        "Prompt TOML: /Users/bardiakhosravi/Desktop/GitHub/RadPrompter/tutorials/01_Basic-Usecase/01_Basic-Usecase.toml\n",
+                        "Prompt TOML: /mnt/NAS3/homes/bkhosra/RadPrompter/tutorials/01_Basic-Usecase/01_Basic-Usecase.toml\n",
                         "Prompt Version: 0.1\n",
                         "Prompt Hash: ce8b273997755ad7279e9c7a13337c70\n",
                         "Concurrency Factor: 2\n",
-                        "Start Time: 2024-05-19 22:42:59\n",
-                        "End Time: 2024-05-19 22:42:59\n",
+                        "Start Time: 2024-05-20 09:35:59\n",
+                        "End Time: 2024-05-20 09:35:59\n",
                         "Duration: 0.0\n",
                         "Number of Items: 3\n",
                         "Average Processing Time: 0.0\n",
                         "\n",
                         "\n",
                         "-------------------- *** - Prompt Content - *** --------------------\n",
                         "[METADATA]\n",
@@ -425,17 +425,17 @@
                 "\n",
                 "And that's it for the basics of using RadPrompter! In the next tutorials we'll cover more advanced features."
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "RadPrompter",
             "language": "python",
-            "name": "python3"
+            "name": "rp"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
@@ -443,9 +443,9 @@
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.11.9"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 4
 }
```

### Comparing `radprompter-1.1.3/tutorials/02_RDP-Templating/02_RDP-Templating.ipynb` & `radprompter-1.1.5/tutorials/02_RDP-Templating/02_RDP-Templating.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.3/tutorials/02_RDP-Templating/02_RDP-Templating.toml` & `radprompter-1.1.5/tutorials/02_RDP-Templating/02_RDP-Templating.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.3/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.ipynb` & `radprompter-1.1.5/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.3/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.toml` & `radprompter-1.1.5/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.3/tutorials/04_Using-Schemas/04_Using-Schemas.ipynb` & `radprompter-1.1.5/tutorials/04_Using-Schemas/04_Using-Schemas.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.3/tutorials/04_Using-Schemas/04_Using-Schemas.toml` & `radprompter-1.1.5/tutorials/04_Using-Schemas/04_Using-Schemas.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.3/tutorials/05_Assistant-Prefill/05_Assistant-Prefill.ipynb` & `radprompter-1.1.5/tutorials/05_JSON-Prefill/05_JSON-Prefill.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993364197530864%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, '**Note:** Assistant prefills are not currently "*

 * *            'supported with the `OpenAIClient`. However, they are supported by other clients such '*

 * *            "as `HuggingFaceClient`, `vLLMClient` and `OllamaClient`.')], delete: [4]}}, 2: "*

 * *            '{\'source\': {insert: [(2, "prompt = Prompt(\'05_JSON-Prefill.toml\')\\n")], delete: '*

 * *            '[2]}}}'}*

```diff
@@ -4,15 +4,15 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Tutorial 5: Assistant Prefill in RadPrompter\n",
                 "\n",
                 "In this tutorial, we'll explore how to use assistant prefills in RadPrompter. Assistant prefills are pre-filled responses that guide the model to generate outputs in a specific format.\n",
                 "\n",
-                "**Note:** Assistant prefills are not currently supported with the `OpenAIClient`. However, they are supported by other clients such as `vLLMClient` and `OllamaClient`."
+                "**Note:** Assistant prefills are not currently supported with the `OpenAIClient`. However, they are supported by other clients such as `HuggingFaceClient`, `vLLMClient` and `OllamaClient`."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Prompt\n",
@@ -45,15 +45,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from radprompter import Prompt\n",
                 "\n",
-                "prompt = Prompt('05_Assistant-Prefill.toml')\n",
+                "prompt = Prompt('05_JSON-Prefill.toml')\n",
                 "prompt"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `radprompter-1.1.3/tutorials/05_Assistant-Prefill/05_Assistant-Prefill.toml` & `radprompter-1.1.5/tutorials/05_JSON-Prefill/05_JSON-Prefill.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.3/PKG-INFO` & `radprompter-1.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radprompter
-Version: 1.1.3
+Version: 1.1.5
 Summary: A package for simplified and reproducible LLM prompting.
 Author-email: Bardia Khosravi <bardiakhosravi95@gmail.com>, Theo Dapamede <theo.dapamede@emory.edu>
 Maintainer-email: Bardia Khosravi <bardiakhosravi95@gmail.com>, Theo Dapamede <theo.dapamede@emory.edu>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: pandas
@@ -73,15 +73,16 @@
 
 | Tutorial                    | Description                                         | Notebook                                                                         |
 |-----------------------------|-----------------------------------------------------|----------------------------------------------------------------------------------|
 | 01_Basic-Usecase            | Covers the basic usage of RadPrompter               | [📓](./tutorials/01_Basic-Usecase)     |
 | 02_RDP-Templating           | Introduces the `[PROMPTS]` section and `rdp` operator | [📓](./tutorials/02_RDP-Templating)    |
 | 03_Multiturn-Prompting      | Demonstrates multi-turn prompting                   | [📓](./tutorials/03_Multiturn-Prompting) |
 | 04_Using-Schemas            | Shows how to use schemas for structured output      | [📓](./tutorials/04_Using-Schemas)     |
-| 05_Assistant-Prefill        | Covers using assistant prefills                     | [📓](./tutorials/05_Assistant-Prefill)  |
+| 05_JSON-Prefill        | Covers using assistant prefills                     | [📓](./tutorials/05_JSON-Prefill)  |
+| 06_HuggingFace-Client        | Covers using the new `HuggingFaceClient`                     | [📓](./tutorials/06_HuggingFace-Client)  |
 
 ## Contributing
 
 We welcome contributions! If you have any updates or improvements to the package, please open an issue or submit a pull request. We're happy to review and incorporate your changes.
 
 ## Authors
```

