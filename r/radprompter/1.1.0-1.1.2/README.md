# Comparing `tmp/radprompter-1.1.0.tar.gz` & `tmp/radprompter-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radprompter-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "radprompter-1.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `radprompter-1.1.0.tar` & `radprompter-1.1.2.tar`

### file list

```diff
@@ -1,33 +1,31 @@
--rw-r--r--   0        0        0     6148 2024-05-15 00:50:49.718415 radprompter-1.1.0/.DS_Store
--rw-r--r--   0        0        0     3169 2024-05-19 17:32:04.647315 radprompter-1.1.0/.gitignore
--rw-r--r--   0        0        0    11357 2024-05-14 18:23:37.432618 radprompter-1.1.0/LICENSE
--rw-r--r--   0        0        0      133 2024-05-15 19:08:43.183784 radprompter-1.1.0/Plan.md
--rw-r--r--   0        0        0       13 2024-05-14 18:23:37.432717 radprompter-1.1.0/README.md
--rw-r--r--   0        0        0    12401 2024-05-14 18:23:37.432957 radprompter-1.1.0/demo.ipynb
--rw-r--r--   0        0        0    23670 2024-05-15 19:39:22.162953 radprompter-1.1.0/demo_no_CoT.ipynb
--rw-r--r--   0        0        0     4382 2024-05-14 19:04:54.672733 radprompter-1.1.0/demo_prompt_no_CoT.toml
--rw-r--r--   0        0        0      669 2024-05-19 17:56:30.082674 radprompter-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      225 2024-05-19 18:13:05.689042 radprompter-1.1.0/radprompter/__init__.py
--rw-r--r--   0        0        0       21 2024-05-19 20:38:38.191128 radprompter-1.1.0/radprompter/__version__.py
--rw-r--r--   0        0        0       59 2024-05-14 18:54:49.737505 radprompter-1.1.0/radprompter/clients/__init__.py
--rw-r--r--   0        0        0     3596 2024-05-19 17:51:15.981258 radprompter-1.1.0/radprompter/clients/clients.py
--rw-r--r--   0        0        0       27 2024-05-14 22:18:09.544596 radprompter-1.1.0/radprompter/prompts/__init__.py
--rw-r--r--   0        0        0     9907 2024-05-19 18:00:58.295860 radprompter-1.1.0/radprompter/prompts/prompts.py
--rw-r--r--   0        0        0     7054 2024-05-19 20:37:23.343879 radprompter-1.1.0/radprompter/radprompter.py
--rw-r--r--   0        0        0     4350 2024-05-15 19:04:16.915270 radprompter-1.1.0/sample_prompt.toml
--rw-r--r--   0        0        0     1089 2024-05-14 18:23:37.434577 radprompter-1.1.0/sample_reports/sample_report_1.txt
--rw-r--r--   0        0        0     1388 2024-05-14 18:23:37.434671 radprompter-1.1.0/sample_reports/sample_report_2.txt
--rw-r--r--   0        0        0     1374 2024-05-14 18:23:37.434764 radprompter-1.1.0/sample_reports/sample_report_3.txt
--rw-r--r--   0        0        0     6148 2024-05-19 19:37:48.126029 radprompter-1.1.0/tutorials/.DS_Store
--rw-r--r--   0        0        0    16762 2024-05-19 18:51:21.283638 radprompter-1.1.0/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb
--rw-r--r--   0        0        0      386 2024-05-19 18:49:48.028574 radprompter-1.1.0/tutorials/01_Basic-Usecase/01_Basic-Usecase.toml
--rw-r--r--   0        0        0    17583 2024-05-19 19:52:03.804859 radprompter-1.1.0/tutorials/02_RDP-Templating/02_RDP-Templating.ipynb
--rw-r--r--   0        0        0     1716 2024-05-19 18:34:44.363741 radprompter-1.1.0/tutorials/02_RDP-Templating/02_RDP-Templating.toml
--rw-r--r--   0        0        0    19012 2024-05-19 19:51:58.516551 radprompter-1.1.0/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.ipynb
--rw-r--r--   0        0        0     1884 2024-05-19 19:04:34.358936 radprompter-1.1.0/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.toml
--rw-r--r--   0        0        0    26892 2024-05-19 19:51:53.847964 radprompter-1.1.0/tutorials/04_Using-Schemas/04_Using-Schemas.ipynb
--rw-r--r--   0        0        0     4478 2024-05-19 19:55:16.714928 radprompter-1.1.0/tutorials/04_Using-Schemas/04_Using-Schemas.toml
--rw-r--r--   0        0        0    28952 2024-05-19 20:38:21.626249 radprompter-1.1.0/tutorials/05_Assistant-Prefill/05_Assistant-Prefill.ipynb
--rw-r--r--   0        0        0     3275 2024-05-19 20:37:55.612863 radprompter-1.1.0/tutorials/05_Assistant-Prefill/05_Assistant-Prefill.toml
--rw-r--r--   0        0        0        0 2024-05-15 18:54:34.909069 radprompter-1.1.0/tutorials/README.md
--rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 radprompter-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2024-05-15 00:50:49.718415 radprompter-1.1.2/.DS_Store
+-rw-r--r--   0        0        0     3169 2024-05-19 17:32:04.647315 radprompter-1.1.2/.gitignore
+-rw-r--r--   0        0        0    11357 2024-05-14 18:23:37.432618 radprompter-1.1.2/LICENSE
+-rw-r--r--   0        0        0     2689 2024-05-19 21:37:15.946367 radprompter-1.1.2/README.md
+-rw-r--r--   0        0        0    91362 2024-05-19 21:36:28.548393 radprompter-1.1.2/logo.png
+-rw-r--r--   0        0        0      669 2024-05-19 17:56:30.082674 radprompter-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      225 2024-05-19 18:13:05.689042 radprompter-1.1.2/radprompter/__init__.py
+-rw-r--r--   0        0        0       21 2024-05-20 02:31:09.498737 radprompter-1.1.2/radprompter/__version__.py
+-rw-r--r--   0        0        0      146 2024-05-20 02:33:21.208331 radprompter-1.1.2/radprompter/clients/__init__.py
+-rw-r--r--   0        0        0      586 2024-05-19 22:16:28.933183 radprompter-1.1.2/radprompter/clients/clients.py
+-rw-r--r--   0        0        0     2651 2024-05-20 02:37:42.872389 radprompter-1.1.2/radprompter/clients/huggingface/clients.py
+-rw-r--r--   0        0        0     3022 2024-05-19 22:09:18.270492 radprompter-1.1.2/radprompter/clients/openai/clients.py
+-rw-r--r--   0        0        0       27 2024-05-14 22:18:09.544596 radprompter-1.1.2/radprompter/prompts/__init__.py
+-rw-r--r--   0        0        0     9907 2024-05-19 18:00:58.295860 radprompter-1.1.2/radprompter/prompts/prompts.py
+-rw-r--r--   0        0        0     7054 2024-05-19 21:54:55.853203 radprompter-1.1.2/radprompter/radprompter.py
+-rw-r--r--   0        0        0     1089 2024-05-14 18:23:37.434577 radprompter-1.1.2/sample_reports/sample_report_1.txt
+-rw-r--r--   0        0        0     1388 2024-05-14 18:23:37.434671 radprompter-1.1.2/sample_reports/sample_report_2.txt
+-rw-r--r--   0        0        0     1374 2024-05-14 18:23:37.434764 radprompter-1.1.2/sample_reports/sample_report_3.txt
+-rw-r--r--   0        0        0     6148 2024-05-19 19:37:48.126029 radprompter-1.1.2/tutorials/.DS_Store
+-rw-r--r--   0        0        0    16856 2024-05-20 02:44:22.407044 radprompter-1.1.2/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb
+-rw-r--r--   0        0        0      386 2024-05-19 18:49:48.028574 radprompter-1.1.2/tutorials/01_Basic-Usecase/01_Basic-Usecase.toml
+-rw-r--r--   0        0        0    17598 2024-05-19 20:43:40.346642 radprompter-1.1.2/tutorials/02_RDP-Templating/02_RDP-Templating.ipynb
+-rw-r--r--   0        0        0     1716 2024-05-19 18:34:44.363741 radprompter-1.1.2/tutorials/02_RDP-Templating/02_RDP-Templating.toml
+-rw-r--r--   0        0        0    19012 2024-05-19 20:43:59.917234 radprompter-1.1.2/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.ipynb
+-rw-r--r--   0        0        0     1884 2024-05-19 19:04:34.358936 radprompter-1.1.2/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.toml
+-rw-r--r--   0        0        0    26880 2024-05-19 20:44:10.453045 radprompter-1.1.2/tutorials/04_Using-Schemas/04_Using-Schemas.ipynb
+-rw-r--r--   0        0        0     4478 2024-05-19 19:55:16.714928 radprompter-1.1.2/tutorials/04_Using-Schemas/04_Using-Schemas.toml
+-rw-r--r--   0        0        0    23827 2024-05-19 20:45:24.923958 radprompter-1.1.2/tutorials/05_Assistant-Prefill/05_Assistant-Prefill.ipynb
+-rw-r--r--   0        0        0     3277 2024-05-19 20:44:47.851630 radprompter-1.1.2/tutorials/05_Assistant-Prefill/05_Assistant-Prefill.toml
+-rw-r--r--   0        0        0        0 2024-05-15 18:54:34.909069 radprompter-1.1.2/tutorials/README.md
+-rw-r--r--   0        0        0     3224 1970-01-01 00:00:00.000000 radprompter-1.1.2/PKG-INFO
```

### Comparing `radprompter-1.1.0/.DS_Store` & `radprompter-1.1.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.0/.gitignore` & `radprompter-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.0/LICENSE` & `radprompter-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.0/demo_no_CoT.ipynb` & `radprompter-1.1.2/tutorials/05_Assistant-Prefill/05_Assistant-Prefill.ipynb`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9360436934351944%*

 * *Differences: {"'cells'": "{0: {'cell_type': 'markdown', 'source': ['# Tutorial 5: Assistant Prefill in "*

 * *            'RadPrompter\\n\', \'\\n\', "In this tutorial, we\'ll explore how to use assistant '*

 * *            'prefills in RadPrompter. Assistant prefills are pre-filled responses that guide the '*

 * *            'model to generate outputs in a specific format.\\n", \'\\n\', \'**Note:** Assistant '*

 * *            'prefills are not currently supported with the `OpenAIClient`. However, they are '*

 * *            "supported by othe […]*

```diff
@@ -1,228 +1,326 @@
 {
     "cells": [
         {
-            "cell_type": "code",
-            "execution_count": 1,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "%load_ext autoreload\n",
-                "%autoreload 2"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 90,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "import os\n",
-                "import pandas as pd\n",
-                "import glob\n",
-                "from radprompter import RadPrompter, Prompt, vLLMClient, OllamaClient"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 91,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "report_files = glob.glob(\"sample_reports/*.txt\")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 92,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "reports = []\n",
-                "report_ids = []\n",
-                "for report_file in report_files:\n",
-                "    report_ids.append(os.path.basename(report_file))\n",
-                "    with open(report_file, 'r') as f:\n",
-                "        reports.append(f.read())"
+                "# Tutorial 5: Assistant Prefill in RadPrompter\n",
+                "\n",
+                "In this tutorial, we'll explore how to use assistant prefills in RadPrompter. Assistant prefills are pre-filled responses that guide the model to generate outputs in a specific format.\n",
+                "\n",
+                "**Note:** Assistant prefills are not currently supported with the `OpenAIClient`. However, they are supported by other clients such as `vLLMClient` and `OllamaClient`."
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 95,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "# prompt = Prompt('demo_prompt_no_CoT.toml')\n",
-                "prompt = Prompt('sample_prompt.toml')"
+                "## Prompt\n",
+                "\n",
+                "As always, we start by importing the `Prompt` class and creating a prompt object from a TOML file:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 96,
+            "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style='padding: 0; border-radius: 5px; font-family: Arial; line-height: 1.2rem; border: 1px solid currentColor'><div style='display: flex; align-items: top; padding: 0; border-right-width: 1px'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px; '>System:</h4><p style='margin: 0; padding: 8px; border-left: 1px solid currentColor;'>You are a helpful assistant that has 20 years of experience in reading radiology reports and extracting data elements.</p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>User:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'>Carefully review the provided chest CT report (in the &lt;report&gt; tag). Ensure that each data element is accurately captured.<br><br>Here is the report:<br>&lt;report&gt;<br><span style='background-color: rgb(255, 224, 178, 0.3);'>{{report}}</span><br>&lt;/report&gt;<br><br>Please pay attention to the following details:<br>- Your attention to detail is crucial for maintaining the integrity of the medical records. <br>- You should not confabulate information, and if something is not mentioned, you should assume that it is `Absent` unless otherwise stated.<br>- The report may contain additional information that is not relevant to the requested data elements. Please ignore that information.<br>- We are interested at findings at the time of scan, not the previous ones, so only consider the impression and findings sections of the report.<br>- Do not print anything else other than the provided output format.<br>I want you to extract the following data element from the report:<br><span style='background-color: rgb(255, 224, 178, 0.3);'>{{hint}}</span><br><br>After you provide the data element, I will ask you to provide an explanation and then the final answer.<br><br>Now give your initial answer. Then provide a step-by-step explanation based on the information in the report, using no more than three short sentences. You can use less sentences if needed.Try to critically appraise your initial answer, which MIGHT be wrong. Then give me your final answer. Format your answers with this format as:<br><br>&lt;answer&gt;<br>&lt;initial_answer&gt;<br>initial answer goes here<br>&lt;/initial_answer&gt;<br>&lt;explanation&gt;<br>1. your first explanation goes here<br>2. your second explanation goes here (if needed)<br>3. your third explanation goes here (if needed)<br>&lt;/explanation&gt;<br>&lt;final_answer&gt;<br>final answer goes here<br>&lt;/final_answer&gt;<br>&lt;/answer&gt;<br></p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>Assistant:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'>&lt;answer&gt;<br>&lt;initial_answer&gt;<span style='background-color: rgb(178, 219, 255, 0.3);'>[... response ...]</span>&lt;/answer&gt;</p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>User:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'>Now, based on your expalanation, provide your final answer elements in a valid JSON format and is between &lt;json&gt; and &lt;/json&gt; tags:<br><br>&lt;json&gt;<br>{<br>  &quot;<span style='background-color: rgb(255, 224, 178, 0.3);'>{{variable_name}}</span>&quot;: &quot;answer&quot; <br>}<br>&lt;/json&gt;<br></p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>Assistant:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'>&lt;json&gt;<br>{<br>  &quot;<span style='background-color: rgb(255, 224, 178, 0.3);'>{{variable_name}}</span>&quot; : &quot;<span style='background-color: rgb(178, 219, 255, 0.3);'>[... response ...]</span>&lt;/json&gt;</p></div></div>"
+                            "<div style='padding: 0; border-radius: 5px; font-family: Arial; line-height: 1.2rem; border: 1px solid currentColor'><div style='display: flex; align-items: top; padding: 0; border-right-width: 1px'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px; '>System:</h4><p style='margin: 0; padding: 8px; border-left: 1px solid currentColor;'>You are a helpful assistant that has 20 years of experience in reading radiology reports and extracting data elements.</p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>User:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'><span style='background-color: rgb(255, 224, 178, 0.3);'>{{intro_prompt}}</span><br>I want you to extract the following data element from the report: <br><span style='background-color: rgb(255, 224, 178, 0.3);'>{{hint}}</span><br><br>Your final answer elements in a valid JSON format and is between &lt;json&gt; and &lt;/json&gt; tags:<br><br>&lt;json&gt;<br>{<br>  &quot;<span style='background-color: rgb(255, 224, 178, 0.3);'>{{variable_name}}</span>&quot;: &quot;answer&quot;<br>}<br>&lt;/json&gt;<br></p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>Assistant:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'>&lt;json&gt;<br>{<br>  &quot;<span style='background-color: rgb(255, 224, 178, 0.3);'>{{variable_name}}</span>&quot; : &quot;<span style='background-color: rgb(178, 219, 255, 0.3);'>[... response ...]</span>&lt;/json&gt;</p></div></div>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "text/plain": []
                     },
-                    "execution_count": 96,
+                    "execution_count": 1,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
+                "from radprompter import Prompt\n",
+                "\n",
+                "prompt = Prompt('05_Assistant-Prefill.toml')\n",
                 "prompt"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "The key feature of this TOML file is the `assistant_response_template`:\n",
+                "\n",
+                "```toml\n",
+                "assistant_response_template = \"\"\"\n",
+                "<json>\n",
+                "{\n",
+                "  \"{{variable_name}}\" : \\\"\"\"\"\n",
+                "```\n",
+                "\n",
+                "This prefill requires the model to generate the output in JSON format. We also included the `{{variable_name}}` to replace this placeholder with each schema's `variable_name` attribute.\n",
+                "\n",
+                "We also add a `stop_tags` field in the `[CONSTRUCTOR]` section:\n",
+                "\n",
+                "```toml\n",
+                "[CONSTRUCTOR]\n",
+                "system = \"rdp(system_prompt)\"\n",
+                "user = \"rdp(user_prompt_intro + user_prompt_cot)\"\n",
+                "response_templates = \"rdp(assistant_response_template)\"\n",
+                "stop_tags = \"</json>\"\n",
+                "```\n",
+                "\n",
+                "This tells the model to stop generating when it reaches the `</json>` tag, ensuring that it doesn't generate any extra text after the JSON object.\n",
+                "\n",
+                "Let's look at the first schema:\n"
+            ]
+        },
+        {
             "cell_type": "code",
-            "execution_count": 97,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style='padding: 0; border-radius: 5px; font-family: Arial; line-height: 1.2rem; border: 1px solid currentColor'><div style='display: flex; align-items: top; padding: 0; border-right-width: 1px'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px; '>System:</h4><p style='margin: 0; padding: 8px; border-left: 1px solid currentColor;'>You are a helpful assistant that has 20 years of experience in reading radiology reports and extracting data elements.</p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>User:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'>Carefully review the provided chest CT report (in the &lt;report&gt; tag). Ensure that each data element is accurately captured.<br><br>Here is the report:<br>&lt;report&gt;<br><span style='background-color: rgb(255, 224, 178, 0.3);'>{{report}}</span><br>&lt;/report&gt;<br><br>Please pay attention to the following details:<br>- Your attention to detail is crucial for maintaining the integrity of the medical records. <br>- You should not confabulate information, and if something is not mentioned, you should assume that it is `Absent` unless otherwise stated.<br>- The report may contain additional information that is not relevant to the requested data elements. Please ignore that information.<br>- We are interested at findings at the time of scan, not the previous ones, so only consider the impression and findings sections of the report.<br>- Do not print anything else other than the provided output format.<br>I want you to extract the following data element from the report:<br>&#x27;Pulmonary Embolism&#x27;<br>Here are your options and you can explicitly use one of these:<br>  - `Present`<br>  - `Absent`<br><br>Hint: &quot;Indicate `Present` if the report explicitly mentions the patient has pulmonary embolism in their CT scan. <br>Indicate `Absent` if pulmonary embolism is not seen or if a previously observed pulmonary embolism is mentioned as resolved.<br><br>After you provide the data element, I will ask you to provide an explanation and then the final answer.<br><br>Now give your initial answer. Then provide a step-by-step explanation based on the information in the report, using no more than three short sentences. You can use less sentences if needed.Try to critically appraise your initial answer, which MIGHT be wrong. Then give me your final answer. Format your answers with this format as:<br><br>&lt;answer&gt;<br>&lt;initial_answer&gt;<br>initial answer goes here<br>&lt;/initial_answer&gt;<br>&lt;explanation&gt;<br>1. your first explanation goes here<br>2. your second explanation goes here (if needed)<br>3. your third explanation goes here (if needed)<br>&lt;/explanation&gt;<br>&lt;final_answer&gt;<br>final answer goes here<br>&lt;/final_answer&gt;<br>&lt;/answer&gt;<br></p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>Assistant:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'>&lt;answer&gt;<br>&lt;initial_answer&gt;<span style='background-color: rgb(178, 219, 255, 0.3);'>[... response ...]</span>&lt;/answer&gt;</p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>User:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'>Now, based on your expalanation, provide your final answer elements in a valid JSON format and is between &lt;json&gt; and &lt;/json&gt; tags:<br><br>&lt;json&gt;<br>{<br>  &quot;Pulmonary Embolism&quot;: &quot;answer&quot; <br>}<br>&lt;/json&gt;<br></p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>Assistant:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'>&lt;json&gt;<br>{<br>  &quot;Pulmonary Embolism&quot; : &quot;<span style='background-color: rgb(178, 219, 255, 0.3);'>[... response ...]</span>&lt;/json&gt;</p></div></div>"
+                            "<div style='padding: 0; border-radius: 5px; font-family: Arial; line-height: 1.2rem; border: 1px solid currentColor'><div style='display: flex; align-items: top; padding: 0; border-right-width: 1px'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px; '>System:</h4><p style='margin: 0; padding: 8px; border-left: 1px solid currentColor;'>You are a helpful assistant that has 20 years of experience in reading radiology reports and extracting data elements.</p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>User:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'><br>I want you to extract the following data element from the report: <br>&#x27;Laterality&#x27;<br>Here are your options and you can explicitly use one of these:<br>  - `Left`<br>  - `Right`<br>  - `Bilateral`<br>  - `Not Mentioned`<br><br>Hint: Indicate `Left` if the report explicitly mentions the patient has a left-sided pulmonary embolism in their CT scan. <br>Indicate `Right` if the report explicitly mentions the patient has a right-sided pulmonary embolism in their CT scan. <br>Indicate `Bilateral` if the report explicitly mentions the patient has a bilateral pulmonary embolism in their CT scan or if patient has both left and right sided pulmonary embolism.<br>Indicate `Not Mentioned` if side of pulmonary embolism is not mentioned.<br><br><br>Your final answer elements in a valid JSON format and is between &lt;json&gt; and &lt;/json&gt; tags:<br><br>&lt;json&gt;<br>{<br>  &quot;Laterality&quot;: &quot;answer&quot;<br>}<br>&lt;/json&gt;<br></p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>Assistant:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'>&lt;json&gt;<br>{<br>  &quot;Laterality&quot; : &quot;<span style='background-color: rgb(178, 219, 255, 0.3);'>[... response ...]</span>&lt;/json&gt;</p></div></div>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "text/plain": []
                     },
-                    "execution_count": 97,
+                    "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "prompt.schemas[0]"
+                "prompt.schemas[1]"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "You can see the prefilled assistant response, preceding model's `[... response ...]`."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Client and Engine\n",
+                "\n",
+                "We'll use the `vLLMClient` and `RadPrompter` engine:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 98,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [],
             "source": [
+                "from radprompter import RadPrompter, vLLMClient\n",
+                "\n",
                 "client = vLLMClient(\n",
                 "    model = \"meta-llama/Meta-Llama-3-8B-Instruct\",\n",
-                "    base_url = \"http://localhost:8000/v1\",\n",
+                "    base_url = \"http://localhost:9999/v1\",\n",
                 "    temperature = 0.0,\n",
                 "    seed=42\n",
+                ")\n",
+                "\n",
+                "engine = RadPrompter(\n",
+                "    client=client,\n",
+                "    prompt=prompt, \n",
+                "    output_file=\"output_tutorial_5.csv\",\n",
+                "    concurrency=2,\n",
+                "    hide_blocks=False,\n",
                 ")"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 99,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "# client = OllamaClient(\n",
-                "#     model = \"phi3\",\n",
-                "#     base_url = \"http://localhost:11434/v1\",\n",
-                "#     temperature = 0.0,\n",
-                "#     seed=42\n",
-                "# )"
+                "And we run it on our sample reports:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 108,
+            "execution_count": 4,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "Processing items: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 3/3 [00:02<00:00,  1.08it/s]\n"
+                    ]
+                }
+            ],
             "source": [
-                "engine = RadPrompter(\n",
-                "    client=client,\n",
-                "    prompt=prompt,\n",
-                "    concurrency=12,\n",
-                "    hide_blocks=False,\n",
-                "    output_file=\"output3.csv\",\n",
-                ")"
+                "import glob\n",
+                "\n",
+                "report_files = glob.glob(\"../../sample_reports/*.txt\")\n",
+                "\n",
+                "reports = []\n",
+                "for file in report_files:\n",
+                "    with open(file, \"r\") as f:\n",
+                "        reports.append({\"report\": f.read(), \"file_name\": file})\n",
+                "\n",
+                "engine(reports)"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 109,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "sample = [{'report': sample_report, 'report_id': report_id} for sample_report, report_id in zip(reports, report_ids)]"
+                "The engine will process each report using **ALL** the schemas in the prompt and save the results to `output_tutorial_5.csv`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 110,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
+                        "text/html": [
+                            "<div>\n",
+                            "<style scoped>\n",
+                            "    .dataframe tbody tr th:only-of-type {\n",
+                            "        vertical-align: middle;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe tbody tr th {\n",
+                            "        vertical-align: top;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe thead th {\n",
+                            "        text-align: right;\n",
+                            "    }\n",
+                            "</style>\n",
+                            "<table border=\"1\" class=\"dataframe\">\n",
+                            "  <thead>\n",
+                            "    <tr style=\"text-align: right;\">\n",
+                            "      <th></th>\n",
+                            "      <th>Pulmonary Embolism_response</th>\n",
+                            "      <th>Laterality_response</th>\n",
+                            "      <th>Acuity_response</th>\n",
+                            "      <th>report</th>\n",
+                            "      <th>file_name</th>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>index</th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "      <th></th>\n",
+                            "    </tr>\n",
+                            "  </thead>\n",
+                            "  <tbody>\n",
+                            "    <tr>\n",
+                            "      <th>0</th>\n",
+                            "      <td>\"Present\"\\n</td>\n",
+                            "      <td>&lt;json&gt;\\n{\\n  \"Laterality\" : \"Bilateral\"\\n}\\n</td>\n",
+                            "      <td>&lt;json&gt;\\n{\\n  \"Acuity\" : \"Acute\"\\n}\\n</td>\n",
+                            "      <td>Clinical Information:\\n72-year-old female with...</td>\n",
+                            "      <td>../../sample_reports/sample_report_2.txt</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>1</th>\n",
+                            "      <td>Present</td>\n",
+                            "      <td>&lt;json&gt;\\n{\\n  \"Laterality\" : \"Bilateral\"\\n}\\n</td>\n",
+                            "      <td>&lt;json&gt;\\n{\\n  \"Acuity\" : \"Not Mentioned\"\\n}\\n</td>\n",
+                            "      <td>Here is an example radiology report describing...</td>\n",
+                            "      <td>../../sample_reports/sample_report_3.txt</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2</th>\n",
+                            "      <td>\"Present\"\\n</td>\n",
+                            "      <td>&lt;json&gt;\\n{\\n  \"Laterality\" : \"Bilateral\"\\n}\\n</td>\n",
+                            "      <td>&lt;json&gt;\\n{\\n  \"Acuity\" : \"Not Mentioned\"\\n}\\n</td>\n",
+                            "      <td>Clinical Information:\\n67-year-old male with s...</td>\n",
+                            "      <td>../../sample_reports/sample_report_1.txt</td>\n",
+                            "    </tr>\n",
+                            "  </tbody>\n",
+                            "</table>\n",
+                            "</div>"
+                        ],
                         "text/plain": [
-                            "[{'report': 'Clinical Information:\\n72-year-old female with sudden onset shortness of breath and hypoxia. Evaluate for pulmonary embolism.\\nTechnique:\\nCT pulmonary angiography with IV contrast was performed.\\nFindings:\\nThere is a large saddle embolus extending from the main pulmonary artery into the right and left main pulmonary arteries. Multiple filling defects are also seen within the segmental and subsegmental branches bilaterally, indicating additional pulmonary emboli.\\nThe right ventricle appears dilated at 4.6 cm, greater than the left ventricle. There is flattening of the interventricular septum, suggesting right heart strain.\\nMosaic perfusion is present within the lungs bilaterally, likely representing pulmonary infarcts.\\nSmall bilateral pleural effusions are noted.\\nImpression:\\n\\nSaddle pulmonary embolism involving the main pulmonary artery, right and left main branches, and multiple segmental/subsegmental branches.\\nFindings of right heart strain with right ventricular dilation and interventricular septal flattening.\\nBilateral pleural effusions, likely due to pulmonary infarcts.\\n\\nRecommendation:\\nEmergent anticoagulation therapy is recommended given the large burden of pulmonary arterial clot and evidence of right heart strain. Surgical or catheter-based embolectomy may need to be considered. Echocardiography can further evaluate right heart function and pulmonary pressures.',\n",
-                            "  'report_id': 'sample_report_2.txt'},\n",
-                            " {'report': 'Here is an example radiology report describing subsegmental pulmonary emboli:\\n\\nClinical Information:\\n65-year-old male with history of recent surgery presenting with pleuritic chest pain. Rule out pulmonary embolism.\\n\\nTechnique:\\nCT pulmonary angiogram with IV contrast was performed.\\n\\nFindings: \\nThe main pulmonary arteries are patent and normal in caliber. No evidence of central pulmonary embolism.\\n\\nThere are few subsegmental pulmonary arterial filling defects identified within the right lower lobe and left upper lobe, compatible with subsegmental pulmonary emboli.\\n\\nNo large pulmonary infarcts are seen. Minimal bibasilar atelectasis is present.\\n\\nThe heart size and pulmonary vascularity are within normal limits. No pleural effusions.\\n\\nImpression:\\n1. Subsegmental pulmonary emboli within the right lower lobe and left upper lobe.\\n2. No central pulmonary emboli or evidence of right heart strain.\\n3. Minimal bibasilar atelectasis.\\n\\nRecommendation:\\nClinical correlation is recommended regarding need for anticoagulation given the subsegmental nature of the emboli. Follow-up imaging can be considered if symptoms persist or worsen to evaluate for interval development of more proximal clot propagation.\\n\\nPatient should be clinically risk stratified for bleeding risk versus benefit of anticoagulation for subsegmental pulmonary emboli based on symptoms and risk factors.',\n",
-                            "  'report_id': 'sample_report_3.txt'},\n",
-                            " {'report': 'Clinical Information:\\n67-year-old male with shortness of breath and pleuritic chest pain. Rule out pulmonary embolism.\\n\\nTechnique:\\nCT pulmonary angiography with IV contrast was performed.\\n\\nFindings:\\nThere are filling defects within the right and left main pulmonary arteries extending into the lobar branches, compatible with bilateral pulmonary emboli. No evidence of right heart strain.\\n\\nGround glass opacities are present within the peripheral lungs bilaterally, suggesting a component of hemorrhage.\\n\\nThe main pulmonary arteries are dilated, with a diameter of 3.4 cm on the right and 3.1 cm on the left (upper limits of normal).\\n\\nNo pleural effusion is identified.\\n\\nImpression:\\n1. Bilateral pulmonary emboli involving the right and left main pulmonary arteries and lobar branches.\\n2. Findings suggestive of pulmonary hemorrhage.\\n3. Pulmonary artery dilation suggesting chronic pulmonary hypertension.\\n\\nRecommendation:\\nClinical correlation is recommended. Anticoagulation therapy should be initiated if not already started. Consider echocardiography to evaluate for right heart strain.',\n",
-                            "  'report_id': 'sample_report_1.txt'}]"
+                            "      Pulmonary Embolism_response  \\\n",
+                            "index                               \n",
+                            "0                     \"Present\"\\n   \n",
+                            "1                         Present   \n",
+                            "2                     \"Present\"\\n   \n",
+                            "\n",
+                            "                                Laterality_response  \\\n",
+                            "index                                                 \n",
+                            "0      <json>\\n{\\n  \"Laterality\" : \"Bilateral\"\\n}\\n   \n",
+                            "1      <json>\\n{\\n  \"Laterality\" : \"Bilateral\"\\n}\\n   \n",
+                            "2      <json>\\n{\\n  \"Laterality\" : \"Bilateral\"\\n}\\n   \n",
+                            "\n",
+                            "                                    Acuity_response  \\\n",
+                            "index                                                 \n",
+                            "0              <json>\\n{\\n  \"Acuity\" : \"Acute\"\\n}\\n   \n",
+                            "1      <json>\\n{\\n  \"Acuity\" : \"Not Mentioned\"\\n}\\n   \n",
+                            "2      <json>\\n{\\n  \"Acuity\" : \"Not Mentioned\"\\n}\\n   \n",
+                            "\n",
+                            "                                                  report  \\\n",
+                            "index                                                      \n",
+                            "0      Clinical Information:\\n72-year-old female with...   \n",
+                            "1      Here is an example radiology report describing...   \n",
+                            "2      Clinical Information:\\n67-year-old male with s...   \n",
+                            "\n",
+                            "                                      file_name  \n",
+                            "index                                            \n",
+                            "0      ../../sample_reports/sample_report_2.txt  \n",
+                            "1      ../../sample_reports/sample_report_3.txt  \n",
+                            "2      ../../sample_reports/sample_report_1.txt  "
                         ]
                     },
-                    "execution_count": 110,
+                    "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "sample"
+                "import pandas as pd\n",
+                "\n",
+                "df = pd.read_csv(\"output_tutorial_5.csv\", index_col='index')\n",
+                "df"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 111,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "Processing items:   0%|          | 0/3 [00:00<?, ?it/s]"
-                    ]
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "Processing items: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 3/3 [00:10<00:00,  3.40s/it]\n"
-                    ]
-                }
-            ],
             "source": [
-                "engine(sample)"
+                "As you can see, the model does not always stick to the template and might deviate from that. But, we've got you covered. You can use this simple utility function to sanitize JSON outputs."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 112,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -238,142 +336,234 @@
                             "        text-align: right;\n",
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
-                            "      <th>Pulmonary Embolism_response_0</th>\n",
-                            "      <th>Pulmonary Embolism_response_1</th>\n",
-                            "      <th>Laterality_response_0</th>\n",
-                            "      <th>Laterality_response_1</th>\n",
-                            "      <th>Acuity_response_0</th>\n",
-                            "      <th>Acuity_response_1</th>\n",
+                            "      <th>Pulmonary Embolism_response</th>\n",
+                            "      <th>Laterality_response</th>\n",
+                            "      <th>Acuity_response</th>\n",
                             "      <th>report</th>\n",
-                            "      <th>report_id</th>\n",
+                            "      <th>file_name</th>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>index</th>\n",
                             "      <th></th>\n",
                             "      <th></th>\n",
                             "      <th></th>\n",
                             "      <th></th>\n",
                             "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
+                            "      <th>0</th>\n",
+                            "      <td>Present</td>\n",
+                            "      <td>Bilateral</td>\n",
+                            "      <td>Acute</td>\n",
+                            "      <td>Clinical Information:\\n72-year-old female with...</td>\n",
+                            "      <td>../../sample_reports/sample_report_2.txt</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>Present\\n&lt;/initial_answer&gt;\\n&lt;explanation&gt;\\n1. ...</td>\n",
-                            "      <td>\"Present\"\\n</td>\n",
-                            "      <td>I'm going to take a guess that the initial ans...</td>\n",
-                            "      <td>&lt;json&gt;\\n{\\n  \"Laterality\" : \"Present\"\\n</td>\n",
-                            "      <td>I'm going to take a guess that the initial ans...</td>\n",
-                            "      <td>&lt;json&gt;\\n{\\n  \"Acuity\" : \"Not Mentioned\"\\n}\\n</td>\n",
+                            "      <td>Present</td>\n",
+                            "      <td>Bilateral</td>\n",
+                            "      <td>Not Mentioned</td>\n",
                             "      <td>Here is an example radiology report describing...</td>\n",
-                            "      <td>sample_report_3.txt</td>\n",
+                            "      <td>../../sample_reports/sample_report_3.txt</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
-                            "      <td>Present\\n&lt;/initial_answer&gt;\\n&lt;explanation&gt;\\n1. ...</td>\n",
-                            "      <td>\"Present\"\\n</td>\n",
-                            "      <td>Bilateral\\n&lt;/initial_answer&gt;\\n&lt;explanation&gt;\\n1...</td>\n",
-                            "      <td>&lt;json&gt;\\n{\\n  \"Laterality\" : \"Bilateral\"\\n</td>\n",
-                            "      <td>I apologize for the mistake. Here is the corre...</td>\n",
-                            "      <td>&lt;json&gt;\\n{\\n  \"Acuity\" : \"Chronic\"\\n}\\n</td>\n",
+                            "      <td>Present</td>\n",
+                            "      <td>Bilateral</td>\n",
+                            "      <td>Not Mentioned</td>\n",
                             "      <td>Clinical Information:\\n67-year-old male with s...</td>\n",
-                            "      <td>sample_report_1.txt</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>0</th>\n",
-                            "      <td>Present\\n&lt;/initial_answer&gt;\\n&lt;explanation&gt;\\n1. ...</td>\n",
-                            "      <td>\"Present\"\\n</td>\n",
-                            "      <td>Bilateral\\n&lt;/initial_answer&gt;\\n&lt;explanation&gt;\\n1...</td>\n",
-                            "      <td>&lt;json&gt;\\n{\\n  \"Laterality\" : \"Bilateral\"\\n</td>\n",
-                            "      <td>&lt;answer&gt;\\n&lt;initial_answer&gt;Acute\\n&lt;/initial_ans...</td>\n",
-                            "      <td>&lt;json&gt;\\n{\\n  \"Acuity\" : \"Acute\"\\n}\\n</td>\n",
-                            "      <td>Clinical Information:\\n72-year-old female with...</td>\n",
-                            "      <td>sample_report_2.txt</td>\n",
+                            "      <td>../../sample_reports/sample_report_1.txt</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "                           Pulmonary Embolism_response_0  \\\n",
-                            "index                                                      \n",
-                            "1      Present\\n</initial_answer>\\n<explanation>\\n1. ...   \n",
-                            "2      Present\\n</initial_answer>\\n<explanation>\\n1. ...   \n",
-                            "0      Present\\n</initial_answer>\\n<explanation>\\n1. ...   \n",
-                            "\n",
-                            "      Pulmonary Embolism_response_1  \\\n",
-                            "index                                 \n",
-                            "1                       \"Present\"\\n   \n",
-                            "2                       \"Present\"\\n   \n",
-                            "0                       \"Present\"\\n   \n",
+                            "      Pulmonary Embolism_response Laterality_response Acuity_response  \\\n",
+                            "index                                                                   \n",
+                            "0                         Present           Bilateral           Acute   \n",
+                            "1                         Present           Bilateral   Not Mentioned   \n",
+                            "2                         Present           Bilateral   Not Mentioned   \n",
                             "\n",
-                            "                                   Laterality_response_0  \\\n",
+                            "                                                  report  \\\n",
                             "index                                                      \n",
-                            "1      I'm going to take a guess that the initial ans...   \n",
-                            "2      Bilateral\\n</initial_answer>\\n<explanation>\\n1...   \n",
-                            "0      Bilateral\\n</initial_answer>\\n<explanation>\\n1...   \n",
+                            "0      Clinical Information:\\n72-year-old female with...   \n",
+                            "1      Here is an example radiology report describing...   \n",
+                            "2      Clinical Information:\\n67-year-old male with s...   \n",
                             "\n",
-                            "                           Laterality_response_1  \\\n",
-                            "index                                              \n",
-                            "1        <json>\\n{\\n  \"Laterality\" : \"Present\"\\n   \n",
-                            "2      <json>\\n{\\n  \"Laterality\" : \"Bilateral\"\\n   \n",
-                            "0      <json>\\n{\\n  \"Laterality\" : \"Bilateral\"\\n   \n",
-                            "\n",
-                            "                                       Acuity_response_0  \\\n",
-                            "index                                                      \n",
-                            "1      I'm going to take a guess that the initial ans...   \n",
-                            "2      I apologize for the mistake. Here is the corre...   \n",
-                            "0      <answer>\\n<initial_answer>Acute\\n</initial_ans...   \n",
-                            "\n",
-                            "                                  Acuity_response_1  \\\n",
-                            "index                                                 \n",
-                            "1      <json>\\n{\\n  \"Acuity\" : \"Not Mentioned\"\\n}\\n   \n",
-                            "2            <json>\\n{\\n  \"Acuity\" : \"Chronic\"\\n}\\n   \n",
-                            "0              <json>\\n{\\n  \"Acuity\" : \"Acute\"\\n}\\n   \n",
-                            "\n",
-                            "                                                  report            report_id  \n",
-                            "index                                                                          \n",
-                            "1      Here is an example radiology report describing...  sample_report_3.txt  \n",
-                            "2      Clinical Information:\\n67-year-old male with s...  sample_report_1.txt  \n",
-                            "0      Clinical Information:\\n72-year-old female with...  sample_report_2.txt  "
+                            "                                      file_name  \n",
+                            "index                                            \n",
+                            "0      ../../sample_reports/sample_report_2.txt  \n",
+                            "1      ../../sample_reports/sample_report_3.txt  \n",
+                            "2      ../../sample_reports/sample_report_1.txt  "
                         ]
                     },
-                    "execution_count": 112,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "results = pd.read_csv(\"output3.csv\", index_col=0)\n",
-                "results"
+                "sanitized_df = engine.sanitize_json(\"all\")\n",
+                "sanitized_df"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 52,
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Now, you can see that the outputs are sanitized. If there is no appropriate match found, the response will be flagged with  `**RECHECK**` (look at the second row).\n",
+                "\n",
+                "**Note**: `engine.sanitize_json` will not modify the model output dataframe and will <u>return a sanitized copy of that</u>."
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "engine.save_log(\"demo_no_CoT.log\")"
+                "Finally, we save the log:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 7,
             "metadata": {},
-            "outputs": [],
-            "source": []
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "RadPrompter Version: 1.1.0\n",
+                        "Model: meta-llama/Meta-Llama-3-8B-Instruct\n",
+                        "Prompt TOML: /Users/bardiakhosravi/Desktop/GitHub/RadPrompter/tutorials/05_Assistant-Prefill/05_Assistant-Prefill.toml\n",
+                        "Prompt Version: 0.1\n",
+                        "Prompt Hash: 306178fe893a26b4d198bc9031761f2e\n",
+                        "Concurrency Factor: 2\n",
+                        "Start Time: 2024-05-19 16:45:08\n",
+                        "End Time: 2024-05-19 16:45:10\n",
+                        "Duration: 2.0\n",
+                        "Number of Items: 3\n",
+                        "Average Processing Time: 0.6666666666666666\n",
+                        "\n",
+                        "\n",
+                        "-------------------- *** - Prompt Content - *** --------------------\n",
+                        "[METADATA]\n",
+                        "\n",
+                        "version = 0.1\n",
+                        "description = \"A sample prompt for RadPrompter\"\n",
+                        "\n",
+                        "[PROMPTS]\n",
+                        "\n",
+                        "system_prompt = \"You are a helpful assistant that has 20 years of experience in reading radiology reports and extracting data elements.\"\n",
+                        "\n",
+                        "user_prompt_intro = \"\"\"\n",
+                        "{{intro_prompt}}\n",
+                        "\"\"\"\n",
+                        "\n",
+                        "user_prompt_no_cot = \"\"\"\n",
+                        "I want you to extract the following data element from the report: \n",
+                        "{{hint}}\n",
+                        "\n",
+                        "Your final answer elements in a valid JSON format and is between <json> and </json> tags:\n",
+                        "\n",
+                        "<json>\n",
+                        "{\n",
+                        "  \"{{variable_name}}\": \"answer\"\n",
+                        "}\n",
+                        "</json>\n",
+                        "\"\"\"\n",
+                        "\n",
+                        "assistant_response_template = \"\"\"\n",
+                        "<json>\n",
+                        "{\n",
+                        "  \"{{variable_name}}\" : \\\"\"\"\"\n",
+                        "\n",
+                        "[CONSTRUCTOR]\n",
+                        "system = \"rdp(system_prompt)\"\n",
+                        "user = \"rdp(user_prompt_intro + user_prompt_no_cot)\"\n",
+                        "response_templates = \"rdp(assistant_response_template)\"\n",
+                        "stop_tags = \"</json>\"\n",
+                        "\n",
+                        "[SCHEMAS]\n",
+                        "\n",
+                        "[SCHEMAS.PulmonaryEmbolism]\n",
+                        "variable_name = \"Pulmonary Embolism\"\n",
+                        "intro_prompt = \"\"\"\n",
+                        "Carefully review the provided chest CT report (in the <report> tag). Ensure that each data element is accurately captured.\n",
+                        "\n",
+                        "Here is the report:\n",
+                        "<report>\n",
+                        "{{report}}\n",
+                        "</report>\n",
+                        "\n",
+                        "Please pay attention to the following details:\n",
+                        "- Your attention to detail is crucial for maintaining the integrity of the medical records. \n",
+                        "- You should not confabulate information, and if something is not mentioned, you should assume that it is `Absent` unless otherwise stated.\n",
+                        "- The report may contain additional information that is not relevant to the requested data elements. Please ignore that information.\n",
+                        "- We are interested at findings at the time of scan, not the previous ones, so only consider the impression and findings sections of the report.\n",
+                        "- Do not print anything else other than the provided output format.\n",
+                        "\"\"\"\n",
+                        "type = \"select\"\n",
+                        "options = [\"Present\", \"Absent\"]\n",
+                        "hint = \"\"\"\"Indicate `Present` if the report explicitly mentions the patient has pulmonary embolism in their CT scan. \n",
+                        "Indicate `Absent` if pulmonary embolism is not seen or if a previously observed pulmonary embolism is mentioned as resolved.\"\"\"\n",
+                        "show_options_in_hint = true\n",
+                        "\n",
+                        "[SCHEMAS.Laterality]\n",
+                        "variable_name = \"Laterality\"\n",
+                        "intro_prompt = \"\"\n",
+                        "type = \"select\"\n",
+                        "options = [\"Left\", \"Right\", \"Bilateral\", \"Not Mentioned\"]\n",
+                        "hint = \"\"\"\n",
+                        "Indicate `Left` if the report explicitly mentions the patient has a left-sided pulmonary embolism in their CT scan. \n",
+                        "Indicate `Right` if the report explicitly mentions the patient has a right-sided pulmonary embolism in their CT scan. \n",
+                        "Indicate `Bilateral` if the report explicitly mentions the patient has a bilateral pulmonary embolism in their CT scan or if patient has both left and right sided pulmonary embolism.\n",
+                        "Indicate `Not Mentioned` if side of pulmonary embolism is not mentioned.\n",
+                        "\"\"\"\n",
+                        "show_options_in_hint = true\n",
+                        "\n",
+                        "\n",
+                        "[SCHEMAS.Acuity]\n",
+                        "variable_name = \"Acuity\"\n",
+                        "intro_prompt = \"\"\n",
+                        "type = \"select\"\n",
+                        "options = [\"Acute\", \"Chronic\", \"Mixed\", \"Not Mentioned\"]\n",
+                        "hint = \"\"\"\n",
+                        "Indicate `Acute` if the report explicitly mentions the patient has an acute pulmonary embolism in their CT scan. \n",
+                        "Indicate `Chronic` if the report explicitly mentions the patient has a chronic pulmonary embolism in their CT scan. \n",
+                        "Indicate `Mixed` if the report explicitly mentions the patient has a acute on chronic pulmonary embolism in their CT scan. \n",
+                        "Indicate `Not Mentioned` if acuity of pulmonary embolism is not mentioned.\n",
+                        "\"\"\"\n",
+                        "show_options_in_hint = true\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "engine.save_log(\"log_tutorial_5.log\")\n",
+                "\n",
+                "with open(\"log_tutorial_5.log\", \"r\") as f:\n",
+                "    print(f.read())"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Assistant prefills are a powerful feature that allow us to guide the model's output into a specific format. By providing a template in the `assistant_templates` field, we can ensure that the model's responses are structured in a way that's easy to parse and process downstream.\n",
+                "\n",
+                "In this tutorial, we used assistant prefills to have the model generate its outputs as JSON objects. This can greatly simplify the task of extracting the relevant information from the model's responses."
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
```

### Comparing `radprompter-1.1.0/demo_prompt_no_CoT.toml` & `radprompter-1.1.2/tutorials/04_Using-Schemas/04_Using-Schemas.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,18 @@
 
 [METADATA]
 
 version = 0.1
-description = "A sample prompt for RadPrompter with no CoT"
+description = "A sample prompt for RadPrompter"
 
 [PROMPTS]
 
 system_prompt = "You are a helpful assistant that has 20 years of experience in reading radiology reports and extracting data elements."
 
-user_prompt_intro = """
-Carefully review the provided chest CT report (in the <report> tag). Ensure that each data element is accurately captured.
-
-Here is the report:
-<report>
-{{report}}
-</report>
-
-Please pay attention to the following details:
-- Your attention to detail is crucial for maintaining the integrity of the medical records. 
-- You should not confabulate information, and if something is not mentioned, you should assume that it is `Absent` unless otherwise stated.
-- The report may contain additional information that is not relevant to the requested data elements. Please ignore that information.
-- We are interested at findings at the time of scan, not the previous ones, so only consider the impression and findings sections of the report.
-- Do not print anything else other than the provided output format.
-"""
+user_prompt_intro = "{{intro_prompt}}\n"
 
 user_prompt_no_cot = """
 I want you to extract the following data element from the report: 
 {{hint}}
 
 Provide a single answer:
 
@@ -34,87 +20,105 @@
 
 [CONSTRUCTOR]
 system = "rdp(system_prompt)"
 user = [
 "rdp(user_prompt_intro + user_prompt_no_cot)"
 ]
 stop_tags = [
-"</answer>"
-]
-response_templates = [
-""
+" "
 ]
 
 
 [SCHEMAS]
 [SCHEMAS.PulmonaryEmbolism]
 variable_name = "Pulmonary Embolism"
+intro_prompt = """
+Carefully review the provided chest CT report (in the <report> tag). Ensure that each data element is accurately captured.
+
+Here is the report:
+<report>
+{{report}}
+</report>
+
+Please pay attention to the following details:
+- Your attention to detail is crucial for maintaining the integrity of the medical records. 
+- You should not confabulate information, and if something is not mentioned, you should assume that it is `Absent` unless otherwise stated.
+- The report may contain additional information that is not relevant to the requested data elements. Please ignore that information.
+- We are interested at findings at the time of scan, not the previous ones, so only consider the impression and findings sections of the report.
+- Do not print anything else other than the provided output format.
+"""
 type = "select"
 options = ["Present", "Absent"]
 show_options_in_hint = true
 hint = """
 Indicate `Present` if the report explicitly mentions the patient has pulmonary embolism in their CT scan. 
 Indicate `Absent` if pulmonary embolism is not seen or if a previously observed pulmonary embolism is mentioned as resolved.
 """
 
 [SCHEMAS.Left]
 variable_name = "Left"
+intro_prompt = ""
 type = "select"
 options = ["Yes", "No"]
 show_options_in_hint = true
 hint = """
 Indicate `Yes` if the report explicitly mentions the patient has a left-sided pulmonary embolism in their CT scan. 
 Indicate `Yes` if the report explicitly mentions the patient has a bilateral pulmonary embolism in their CT scan or if patient has both left and right sided pulmonary embolism.
 Indicate `No` if the report doesn't explicitly mentions the patient has a left-sided or bilateral pulmonary embolism in their CT scan. 
 """
 
 [SCHEMAS.Right]
 variable_name = "Right"
 type = "select"
+intro_prompt = ""
 options = ["Yes", "No"]
 show_options_in_hint = true
 hint = """
 Indicate `Yes` if the report explicitly mentions the patient has a right-sided pulmonary embolism in their CT scan. 
 Indicate `Yes` if the report explicitly mentions the patient has a bilateral pulmonary embolism in their CT scan or if patient has both left and right sided pulmonary embolism.
 Indicate `No` if the report doesn't explicitly mentions the patient has a right-sided or bilateral pulmonary embolism in their CT scan. 
 """
 
 [SCHEMAS.Acute]
 variable_name = "Acute"
 type = "select"
+intro_prompt = ""
 options = ["Yes", "No"]
 show_options_in_hint = true
 hint = """
 Indicate `Yes` if the report explicitly mentions the patient has an acute pulmonary embolism in their CT scan. 
 Indicate `No` if the report doesn't explicitly mentions the patient has an acute pulmonary embolism in their CT scan. 
 """
 
 [SCHEMAS.Chronic]
 variable_name = "Chronic"
 type = "select"
+intro_prompt = ""
 options = ["Yes", "No"]
 show_options_in_hint = true
 hint = """
 Indicate `Yes` if the report explicitly mentions the patient has an chronic pulmonary embolism in their CT scan. 
 Indicate `No` if the report doesn't explicitly mentions the patient has an chronic pulmonary embolism in their CT scan. 
 """
 
 
 [SCHEMAS.RightHeartStrain]
 variable_name = "RightHeartStrain"
 type = "select"
+intro_prompt = ""
 options = ["Yes", "No"]
 show_options_in_hint = true
 hint = """
 Indicate `Yes` if the report does explicitly mentions that the patient has a right heart strain in their CT scan. 
 Indicate `No` if the report doesn't explicitly mentions that the patient has a right heart strain in their CT scan. 
 """
 
 [SCHEMAS.PulmonaryArteryHypertension]
 variable_name = "PulmonaryArteryHypertension"
 type = "select"
+intro_prompt = ""
 options = ["Yes", "No"]
 show_options_in_hint = true
 hint = """
 Indicate `Yes` if the report does explicitly mentions that the patient has a pulmonary artery hypertension in their CT scan. 
 Indicate `No` if the report doesn't explicitly mentions that the patient has a pulmonary artery hypertension in their CT scan. 
 """
```

### Comparing `radprompter-1.1.0/pyproject.toml` & `radprompter-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.0/radprompter/clients/clients.py` & `radprompter-1.1.2/radprompter/clients/openai/clients.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,10 @@
 from openai import OpenAI
+from .. import Client
 
-class Client():
-    def __init__(self, model):
-        self.model = model
-        
-    def chat_complete(self, messages, stop, **kwargs):
-        raise NotImplementedError()
-    
-    def ask_model(self, messages, stop, max_tokens=200):
-        response = self.chat_complete(messages, stop, max_tokens)
-        messages = self.update_last_message(messages, response, suffix=stop)
-        return response, messages
-        
-    def update_last_message(self, messages, response, suffix=None):
-        messages[-1]['content'] += response + (suffix if suffix else "")
-        return messages
-        
 class OpenAIClient(Client):
     def __init__(self, model, **kwargs):
         Client.__init__(self, model)
         self.seed = kwargs.pop("seed", 42)
         self.temperature = kwargs.pop("temperature", 0.0)
         self.frequency_penalty = kwargs.pop("frequency_penalty", 1)
         self.top_p = kwargs.pop("top_p", 1)
```

### Comparing `radprompter-1.1.0/radprompter/prompts/prompts.py` & `radprompter-1.1.2/radprompter/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.0/radprompter/radprompter.py` & `radprompter-1.1.2/radprompter/radprompter.py`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.0/sample_reports/sample_report_1.txt` & `radprompter-1.1.2/sample_reports/sample_report_1.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.0/sample_reports/sample_report_2.txt` & `radprompter-1.1.2/sample_reports/sample_report_2.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.0/sample_reports/sample_report_3.txt` & `radprompter-1.1.2/sample_reports/sample_report_3.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.0/tutorials/.DS_Store` & `radprompter-1.1.2/tutorials/.DS_Store`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.0/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb` & `radprompter-1.1.2/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997977283795004%*

 * *Differences: {"'cells'": '{4: {\'outputs\': {0: {\'text\': {insert: [(8, \'user = """Does the following report '*

 * *            "indicate a normal or abnormal finding?\\n')], delete: [8]}}}}, 6: {'outputs': {0: "*

 * *            '{\'data\': {\'text/html\': ["<div style=\'padding: 0; border-radius: 5px; '*

 * *            "font-family: Arial; line-height: 1.2rem; border: 1px solid currentColor'><div "*

 * *            "style='display: flex; align-items: top; padding: 0; border-right-width: 1px'><h4 "*

 * *            "style='margin: 0; paddin […]*

```diff
@@ -53,15 +53,15 @@
                         "\n",
                         "version = 0.1\n",
                         "description = \"A sample prompt for RadPrompter\"\n",
                         "\n",
                         "\n",
                         "[CONSTRUCTOR]\n",
                         "system = \"You are an experienced radiologist that help users extract infromation from radiology reports.\"\n",
-                        "user = \"\"\"\"Does the following report indicate a normal or abnormal finding?\n",
+                        "user = \"\"\"Does the following report indicate a normal or abnormal finding?\n",
                         "{{report}}\n",
                         "\n",
                         "Just reply with \"normal\" or \"abnormal\" to indicate your answer, without any additional information.\n",
                         "\"\"\"\n"
                     ]
                 }
             ],
@@ -86,15 +86,15 @@
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style='padding: 0; border-radius: 5px; font-family: Arial; line-height: 1.2rem; border: 1px solid currentColor'><div style='display: flex; align-items: top; padding: 0; border-right-width: 1px'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px; '>System:</h4><p style='margin: 0; padding: 8px; border-left: 1px solid currentColor;'>You are an experienced radiologist that help users extract infromation from radiology reports.</p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>User:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'>&quot;Does the following report indicate a normal or abnormal finding?<br><span style='background-color: rgb(255, 224, 178, 0.3);'>{{report}}</span><br><br>Just reply with &quot;normal&quot; or &quot;abnormal&quot; to indicate your answer, without any additional information.<br></p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>Assistant:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'><span style='background-color: rgb(178, 219, 255, 0.3);'>[... response ...]</span></p></div></div>"
+                            "<div style='padding: 0; border-radius: 5px; font-family: Arial; line-height: 1.2rem; border: 1px solid currentColor'><div style='display: flex; align-items: top; padding: 0; border-right-width: 1px'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px; '>System:</h4><p style='margin: 0; padding: 8px; border-left: 1px solid currentColor;'>You are an experienced radiologist that help users extract infromation from radiology reports.</p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>User:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'>Does the following report indicate a normal or abnormal finding?<br><span style='background-color: rgb(255, 224, 178, 0.3);'>{{report}}</span><br><br>Just reply with &quot;normal&quot; or &quot;abnormal&quot; to indicate your answer, without any additional information.<br></p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>Assistant:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'><span style='background-color: rgb(178, 219, 255, 0.3);'>[... response ...]</span></p></div></div>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -127,14 +127,15 @@
                 "## Client\n",
                 "\n",
                 "RadPrompter supports several LLM clients out of the box, including:\n",
                 "\n",
                 "- `OpenAIClient`: For accessing OpenAI's models\n",
                 "- `vLLMClient`: For accessing open-source LLMs like Llama hosted using the [vLLM package](https://vllm.ai/).\n",
                 "- `OllamaClient`: For accesing [Ollama](https://ollama.com/) open source models.\n",
+                "- `HuggingFaceClient`: For accesing [HuggingFace](https://huggingface.co/) open source models.\n",
                 "\n",
                 "To instantiate a client, you need to provide the following:\n",
                 "\n",
                 "1. `model` [Required]: The name of the model to use (e.g., \"gpt-3.5-turbo\" for OpenAI,  \"meta-llama/Meta-Llama-3-8B-Instruct\" for vLLM and \"phi3\" for Ollama).\n",
                 "2. `base_url` [Optional]: The URL of the REST API endpoint.\n",
                 "3. `api_key` [Optional]: Your API key for the service. If not provided, the client will attempt to read it from an environment variable (in case of `OpenAIClient`) or set that to \"EMPTY\" (`vLLMClient` and `OllamaClient`).\n",
                 "4. `temperature` [Optional]: Sampling temperature for the LLM (Default: `0.0`).\n",
@@ -251,15 +252,15 @@
             "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "Processing items: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 3/3 [00:00<00:00, 11.13it/s]\n"
+                        "Processing items: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 3/3 [00:00<00:00, 11.64it/s]\n"
                     ]
                 }
             ],
             "source": [
                 "engine(reports)"
             ]
         },
@@ -305,46 +306,46 @@
                             "      <th></th>\n",
                             "      <th></th>\n",
                             "      <th></th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th>0</th>\n",
-                            "      <td>Abnormal</td>\n",
-                            "      <td>Clinical Information:\\n72-year-old female with...</td>\n",
-                            "      <td>../../sample_reports/sample_report_2.txt</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>Abnormal</td>\n",
                             "      <td>Here is an example radiology report describing...</td>\n",
                             "      <td>../../sample_reports/sample_report_3.txt</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
+                            "      <th>0</th>\n",
+                            "      <td>Abnormal</td>\n",
+                            "      <td>Clinical Information:\\n72-year-old female with...</td>\n",
+                            "      <td>../../sample_reports/sample_report_2.txt</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>Abnormal</td>\n",
                             "      <td>Clinical Information:\\n67-year-old male with s...</td>\n",
                             "      <td>../../sample_reports/sample_report_1.txt</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "      default_response                                             report  \\\n",
                             "index                                                                       \n",
-                            "0             Abnormal  Clinical Information:\\n72-year-old female with...   \n",
                             "1             Abnormal  Here is an example radiology report describing...   \n",
+                            "0             Abnormal  Clinical Information:\\n72-year-old female with...   \n",
                             "2             Abnormal  Clinical Information:\\n67-year-old male with s...   \n",
                             "\n",
                             "                                      file_name  \n",
                             "index                                            \n",
-                            "0      ../../sample_reports/sample_report_2.txt  \n",
                             "1      ../../sample_reports/sample_report_3.txt  \n",
+                            "0      ../../sample_reports/sample_report_2.txt  \n",
                             "2      ../../sample_reports/sample_report_1.txt  "
                         ]
                     },
                     "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -375,37 +376,37 @@
             "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "RadPrompter Version: 1.0.8\n",
+                        "RadPrompter Version: 1.1.2\n",
                         "Model: meta-llama/Meta-Llama-3-8B-Instruct\n",
                         "Prompt TOML: /Users/bardiakhosravi/Desktop/GitHub/RadPrompter/tutorials/01_Basic-Usecase/01_Basic-Usecase.toml\n",
                         "Prompt Version: 0.1\n",
-                        "Prompt Hash: 369eb088846feaa3e6ea0fdc3a1a40b2\n",
+                        "Prompt Hash: ce8b273997755ad7279e9c7a13337c70\n",
                         "Concurrency Factor: 2\n",
-                        "Start Time: 2024-05-19 14:14:28\n",
-                        "End Time: 2024-05-19 14:14:28\n",
+                        "Start Time: 2024-05-19 22:42:59\n",
+                        "End Time: 2024-05-19 22:42:59\n",
                         "Duration: 0.0\n",
                         "Number of Items: 3\n",
                         "Average Processing Time: 0.0\n",
                         "\n",
                         "\n",
                         "-------------------- *** - Prompt Content - *** --------------------\n",
                         "[METADATA]\n",
                         "\n",
                         "version = 0.1\n",
                         "description = \"A sample prompt for RadPrompter\"\n",
                         "\n",
                         "\n",
                         "[CONSTRUCTOR]\n",
                         "system = \"You are an experienced radiologist that help users extract infromation from radiology reports.\"\n",
-                        "user = \"\"\"\"Does the following report indicate a normal or abnormal finding?\n",
+                        "user = \"\"\"Does the following report indicate a normal or abnormal finding?\n",
                         "{{report}}\n",
                         "\n",
                         "Just reply with \"normal\" or \"abnormal\" to indicate your answer, without any additional information.\n",
                         "\"\"\"\n"
                     ]
                 }
             ],
```

### Comparing `radprompter-1.1.0/tutorials/02_RDP-Templating/02_RDP-Templating.ipynb` & `radprompter-1.1.2/tutorials/02_RDP-Templating/02_RDP-Templating.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998509208937199%*

 * *Differences: {"'cells'": "{9: {'outputs': {0: {'text': ['Processing items: 100%|██████████| 3/3 [00:06<00:00,  "*

 * *            "2.20s/it]\\n']}}}, 14: {'outputs': {0: {'text': {insert: [(0, 'RadPrompter Version: "*

 * *            "1.1.0\\n'), (6, 'Start Time: 2024-05-19 16:43:32\\n'), (7, 'End Time: 2024-05-19 "*

 * *            "16:43:39\\n'), (8, 'Duration: 7.0\\n'), (10, 'Average Processing Time: "*

 * *            "2.3333333333333335\\n')], delete: [10, 8, 7, 6, 0]}}}}}"}*

```diff
@@ -198,15 +198,15 @@
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "Processing items: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 3/3 [00:06<00:00,  2.11s/it]\n"
+                        "Processing items: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 3/3 [00:06<00:00,  2.20s/it]\n"
                     ]
                 }
             ],
             "source": [
                 "import glob\n",
                 "\n",
                 "report_files = glob.glob(\"../../sample_reports/*.txt\")\n",
@@ -344,25 +344,25 @@
             "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "RadPrompter Version: 1.0.8\n",
+                        "RadPrompter Version: 1.1.0\n",
                         "Model: meta-llama/Meta-Llama-3-8B-Instruct\n",
                         "Prompt TOML: /Users/bardiakhosravi/Desktop/GitHub/RadPrompter/tutorials/02_RDP-Templating/02_RDP-Templating.toml\n",
                         "Prompt Version: 0.1\n",
                         "Prompt Hash: b5b6e7cc73163ad0c3024020aa06a0a7\n",
                         "Concurrency Factor: 2\n",
-                        "Start Time: 2024-05-19 14:36:49\n",
-                        "End Time: 2024-05-19 14:36:55\n",
-                        "Duration: 6.0\n",
+                        "Start Time: 2024-05-19 16:43:32\n",
+                        "End Time: 2024-05-19 16:43:39\n",
+                        "Duration: 7.0\n",
                         "Number of Items: 3\n",
-                        "Average Processing Time: 2.0\n",
+                        "Average Processing Time: 2.3333333333333335\n",
                         "\n",
                         "\n",
                         "-------------------- *** - Prompt Content - *** --------------------\n",
                         "[METADATA]\n",
                         "\n",
                         "version = 0.1\n",
                         "description = \"A sample prompt for RadPrompter\"\n",
```

### Comparing `radprompter-1.1.0/tutorials/02_RDP-Templating/02_RDP-Templating.toml` & `radprompter-1.1.2/tutorials/02_RDP-Templating/02_RDP-Templating.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.0/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.ipynb` & `radprompter-1.1.2/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999795751633986%*

 * *Differences: {"'cells'": "{13: {'outputs': {0: {'text': {insert: [(0, 'RadPrompter Version: 1.1.0\\n'), (6, "*

 * *            "'Start Time: 2024-05-19 16:43:44\\n'), (7, 'End Time: 2024-05-19 16:43:58\\n'), (8, "*

 * *            "'Duration: 14.0\\n'), (10, 'Average Processing Time: 4.666666666666667\\n')], delete: "*

 * *            '[10, 8, 7, 6, 0]}}}}}'}*

```diff
@@ -332,25 +332,25 @@
             "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "RadPrompter Version: 1.0.8\n",
+                        "RadPrompter Version: 1.1.0\n",
                         "Model: meta-llama/Meta-Llama-3-8B-Instruct\n",
                         "Prompt TOML: /Users/bardiakhosravi/Desktop/GitHub/RadPrompter/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.toml\n",
                         "Prompt Version: 0.1\n",
                         "Prompt Hash: 06f66066098813d66e786cbc2d86e6fa\n",
                         "Concurrency Factor: 2\n",
-                        "Start Time: 2024-05-19 15:10:58\n",
-                        "End Time: 2024-05-19 15:11:11\n",
-                        "Duration: 13.0\n",
+                        "Start Time: 2024-05-19 16:43:44\n",
+                        "End Time: 2024-05-19 16:43:58\n",
+                        "Duration: 14.0\n",
                         "Number of Items: 3\n",
-                        "Average Processing Time: 4.333333333333333\n",
+                        "Average Processing Time: 4.666666666666667\n",
                         "\n",
                         "\n",
                         "-------------------- *** - Prompt Content - *** --------------------\n",
                         "[METADATA]\n",
                         "version = 0.1\n",
                         "description = \"A sample prompt for RadPrompter\"\n",
                         "\n",
```

### Comparing `radprompter-1.1.0/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.toml` & `radprompter-1.1.2/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.0/tutorials/04_Using-Schemas/04_Using-Schemas.ipynb` & `radprompter-1.1.2/tutorials/04_Using-Schemas/04_Using-Schemas.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999876221707819%*

 * *Differences: {"'cells'": "{11: {'outputs': {0: {'text': ['Processing items: 100%|██████████| 3/3 [00:02<00:00,  "*

 * *            "1.22it/s]\\n']}}}, 16: {'outputs': {0: {'text': {insert: [(0, 'RadPrompter Version: "*

 * *            "1.1.0\\n'), (4, 'Prompt Hash: 3a708a9b57a333d6fa94b8f25cafd593\\n'), (6, 'Start Time: "*

 * *            "2024-05-19 16:44:04\\n'), (7, 'End Time: 2024-05-19 16:44:07\\n'), (18, 'description "*

 * *            '= "A sample prompt for RadPrompter"\\n\')], delete: [18, 7, 6, 4, 0]}}}}}'}*

```diff
@@ -220,15 +220,15 @@
             "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "Processing items: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 3/3 [00:02<00:00,  1.20it/s]\n"
+                        "Processing items: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 3/3 [00:02<00:00,  1.22it/s]\n"
                     ]
                 }
             ],
             "source": [
                 "import glob\n",
                 "\n",
                 "report_files = glob.glob(\"../../sample_reports/*.txt\")\n",
@@ -401,33 +401,33 @@
             "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "RadPrompter Version: 1.0.8\n",
+                        "RadPrompter Version: 1.1.0\n",
                         "Model: meta-llama/Meta-Llama-3-8B-Instruct\n",
                         "Prompt TOML: /Users/bardiakhosravi/Desktop/GitHub/RadPrompter/tutorials/04_Using-Schemas/04_Using-Schemas.toml\n",
                         "Prompt Version: 0.1\n",
-                        "Prompt Hash: 2254abf376cfa05a5026fdcc6cf6e428\n",
+                        "Prompt Hash: 3a708a9b57a333d6fa94b8f25cafd593\n",
                         "Concurrency Factor: 2\n",
-                        "Start Time: 2024-05-19 15:37:06\n",
-                        "End Time: 2024-05-19 15:37:09\n",
+                        "Start Time: 2024-05-19 16:44:04\n",
+                        "End Time: 2024-05-19 16:44:07\n",
                         "Duration: 3.0\n",
                         "Number of Items: 3\n",
                         "Average Processing Time: 1.0\n",
                         "\n",
                         "\n",
                         "-------------------- *** - Prompt Content - *** --------------------\n",
                         "\n",
                         "[METADATA]\n",
                         "\n",
                         "version = 0.1\n",
-                        "description = \"A sample prompt for RadPrompter with no CoT\"\n",
+                        "description = \"A sample prompt for RadPrompter\"\n",
                         "\n",
                         "[PROMPTS]\n",
                         "\n",
                         "system_prompt = \"You are a helpful assistant that has 20 years of experience in reading radiology reports and extracting data elements.\"\n",
                         "\n",
                         "user_prompt_intro = \"{{intro_prompt}}\\n\"\n",
                         "\n",
```

### Comparing `radprompter-1.1.0/tutorials/04_Using-Schemas/04_Using-Schemas.toml` & `radprompter-1.1.2/tutorials/05_Assistant-Prefill/05_Assistant-Prefill.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,46 @@
-
 [METADATA]
 
 version = 0.1
 description = "A sample prompt for RadPrompter"
 
 [PROMPTS]
 
 system_prompt = "You are a helpful assistant that has 20 years of experience in reading radiology reports and extracting data elements."
 
-user_prompt_intro = "{{intro_prompt}}\n"
+user_prompt_intro = """
+{{intro_prompt}}
+"""
 
 user_prompt_no_cot = """
 I want you to extract the following data element from the report: 
 {{hint}}
 
-Provide a single answer:
+Your final answer elements in a valid JSON format and is between <json> and </json> tags:
 
+<json>
+{
+  "{{variable_name}}": "answer"
+}
+</json>
 """
 
+assistant_response_template = """
+<json>
+{
+  "{{variable_name}}" : \""""
+
 [CONSTRUCTOR]
 system = "rdp(system_prompt)"
-user = [
-"rdp(user_prompt_intro + user_prompt_no_cot)"
-]
-stop_tags = [
-" "
-]
-
+user = "rdp(user_prompt_intro + user_prompt_no_cot)"
+response_templates = "rdp(assistant_response_template)"
+stop_tags = "</json>"
 
 [SCHEMAS]
+
 [SCHEMAS.PulmonaryEmbolism]
 variable_name = "Pulmonary Embolism"
 intro_prompt = """
 Carefully review the provided chest CT report (in the <report> tag). Ensure that each data element is accurately captured.
 
 Here is the report:
 <report>
@@ -44,81 +52,37 @@
 - You should not confabulate information, and if something is not mentioned, you should assume that it is `Absent` unless otherwise stated.
 - The report may contain additional information that is not relevant to the requested data elements. Please ignore that information.
 - We are interested at findings at the time of scan, not the previous ones, so only consider the impression and findings sections of the report.
 - Do not print anything else other than the provided output format.
 """
 type = "select"
 options = ["Present", "Absent"]
+hint = """"Indicate `Present` if the report explicitly mentions the patient has pulmonary embolism in their CT scan. 
+Indicate `Absent` if pulmonary embolism is not seen or if a previously observed pulmonary embolism is mentioned as resolved."""
 show_options_in_hint = true
-hint = """
-Indicate `Present` if the report explicitly mentions the patient has pulmonary embolism in their CT scan. 
-Indicate `Absent` if pulmonary embolism is not seen or if a previously observed pulmonary embolism is mentioned as resolved.
-"""
 
-[SCHEMAS.Left]
-variable_name = "Left"
+[SCHEMAS.Laterality]
+variable_name = "Laterality"
 intro_prompt = ""
 type = "select"
-options = ["Yes", "No"]
-show_options_in_hint = true
+options = ["Left", "Right", "Bilateral", "Not Mentioned"]
 hint = """
-Indicate `Yes` if the report explicitly mentions the patient has a left-sided pulmonary embolism in their CT scan. 
-Indicate `Yes` if the report explicitly mentions the patient has a bilateral pulmonary embolism in their CT scan or if patient has both left and right sided pulmonary embolism.
-Indicate `No` if the report doesn't explicitly mentions the patient has a left-sided or bilateral pulmonary embolism in their CT scan. 
+Indicate `Left` if the report explicitly mentions the patient has a left-sided pulmonary embolism in their CT scan. 
+Indicate `Right` if the report explicitly mentions the patient has a right-sided pulmonary embolism in their CT scan. 
+Indicate `Bilateral` if the report explicitly mentions the patient has a bilateral pulmonary embolism in their CT scan or if patient has both left and right sided pulmonary embolism.
+Indicate `Not Mentioned` if side of pulmonary embolism is not mentioned.
 """
-
-[SCHEMAS.Right]
-variable_name = "Right"
-type = "select"
-intro_prompt = ""
-options = ["Yes", "No"]
 show_options_in_hint = true
-hint = """
-Indicate `Yes` if the report explicitly mentions the patient has a right-sided pulmonary embolism in their CT scan. 
-Indicate `Yes` if the report explicitly mentions the patient has a bilateral pulmonary embolism in their CT scan or if patient has both left and right sided pulmonary embolism.
-Indicate `No` if the report doesn't explicitly mentions the patient has a right-sided or bilateral pulmonary embolism in their CT scan. 
-"""
 
-[SCHEMAS.Acute]
-variable_name = "Acute"
-type = "select"
-intro_prompt = ""
-options = ["Yes", "No"]
-show_options_in_hint = true
-hint = """
-Indicate `Yes` if the report explicitly mentions the patient has an acute pulmonary embolism in their CT scan. 
-Indicate `No` if the report doesn't explicitly mentions the patient has an acute pulmonary embolism in their CT scan. 
-"""
 
-[SCHEMAS.Chronic]
-variable_name = "Chronic"
-type = "select"
+[SCHEMAS.Acuity]
+variable_name = "Acuity"
 intro_prompt = ""
-options = ["Yes", "No"]
-show_options_in_hint = true
-hint = """
-Indicate `Yes` if the report explicitly mentions the patient has an chronic pulmonary embolism in their CT scan. 
-Indicate `No` if the report doesn't explicitly mentions the patient has an chronic pulmonary embolism in their CT scan. 
-"""
-
-
-[SCHEMAS.RightHeartStrain]
-variable_name = "RightHeartStrain"
 type = "select"
-intro_prompt = ""
-options = ["Yes", "No"]
-show_options_in_hint = true
+options = ["Acute", "Chronic", "Mixed", "Not Mentioned"]
 hint = """
-Indicate `Yes` if the report does explicitly mentions that the patient has a right heart strain in their CT scan. 
-Indicate `No` if the report doesn't explicitly mentions that the patient has a right heart strain in their CT scan. 
+Indicate `Acute` if the report explicitly mentions the patient has an acute pulmonary embolism in their CT scan. 
+Indicate `Chronic` if the report explicitly mentions the patient has a chronic pulmonary embolism in their CT scan. 
+Indicate `Mixed` if the report explicitly mentions the patient has a acute on chronic pulmonary embolism in their CT scan. 
+Indicate `Not Mentioned` if acuity of pulmonary embolism is not mentioned.
 """
-
-[SCHEMAS.PulmonaryArteryHypertension]
-variable_name = "PulmonaryArteryHypertension"
-type = "select"
-intro_prompt = ""
-options = ["Yes", "No"]
 show_options_in_hint = true
-hint = """
-Indicate `Yes` if the report does explicitly mentions that the patient has a pulmonary artery hypertension in their CT scan. 
-Indicate `No` if the report doesn't explicitly mentions that the patient has a pulmonary artery hypertension in their CT scan. 
-"""
```

