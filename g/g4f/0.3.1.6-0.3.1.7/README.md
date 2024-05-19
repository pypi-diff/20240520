# Comparing `tmp/g4f-0.3.1.6.tar.gz` & `tmp/g4f-0.3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g4f-0.3.1.6.tar", last modified: Sun May 19 04:02:11 2024, max compression
+gzip compressed data, was "g4f-0.3.1.7.tar", last modified: Sun May 19 08:14:12 2024, max compression
```

## Comparing `g4f-0.3.1.6.tar` & `g4f-0.3.1.7.tar`

### file list

```diff
@@ -1,250 +1,250 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.377868 g4f-0.3.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-19 04:02:00.000000 g4f-0.3.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-19 04:02:00.000000 g4f-0.3.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    56222 2024-05-19 04:02:11.377868 g4f-0.3.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    53026 2024-05-19 04:02:00.000000 g4f-0.3.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.337868 g4f-0.3.1.6/g4f/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.345868 g4f-0.3.1.6/g4f/Provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Aichatos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Aura.py
--rw-r--r--   0 runner    (1001) docker     (127)    21427 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Bing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/BingCreateImages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Blackbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/ChatForAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Chatgpt4Online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/ChatgptAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/ChatgptFree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/ChatgptNext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/ChatgptX.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Cnote.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/DeepInfra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/DeepInfraImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/DuckDuckGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Ecosia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Feedough.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/FlowGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/FreeChatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/FreeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/GeminiPro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/GeminiProChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/GigaChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/GptTalkRu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/HuggingChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/HuggingFace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Koala.py
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Liaobots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Llama.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Local.py
--rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/MetaAI.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/MetaAIAccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/PerplexityLabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Pi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Reka.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Replicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/ReplicateImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/WhiteRabbitNeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/You.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/base_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.345868 g4f-0.3.1.6/g4f/Provider/bing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/bing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/bing/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/bing/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/bing/upload_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.353868 g4f-0.3.1.6/g4f/Provider/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Acytoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/AiAsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/AiChatOnline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/AiService.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Aibn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Aichat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Ails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Aivvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Berlin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/ChatAnywhere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/ChatgptDuo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/CodeLinkAva.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Cromicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/DfeHub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/EasyChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Equing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/FakeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/FastGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Forefront.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/GPTalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/GeekGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/GetGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/H2o.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Hashnode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Lockchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Myshell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/NoowAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Opchatgpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/OpenAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/V50.py
--rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Vitalentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/VoiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Wewordle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Wuguokai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Ylokh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/Yqcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/deprecated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.353868 g4f-0.3.1.6/g4f/Provider/gigachat_crt/
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.353868 g4f-0.3.1.6/g4f/Provider/needs_auth/
--rw-r--r--   0 runner    (1001) docker     (127)    10986 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/needs_auth/Gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/needs_auth/Groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/needs_auth/OpenRouter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/needs_auth/Openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/needs_auth/OpenaiAccount.py
--rw-r--r--   0 runner    (1001) docker     (127)    33277 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/needs_auth/OpenaiChat.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/needs_auth/PerplexityApi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/needs_auth/Poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/needs_auth/Raycast.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/needs_auth/Theb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/needs_auth/ThebApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/needs_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.357868 g4f-0.3.1.6/g4f/Provider/not_working/
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/AItianhu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/Bestim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/ChatBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/ChatgptDemo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/ChatgptDemoAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/ChatgptLogin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/Chatxyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/Gpt6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/GptChatly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/GptForLove.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/GptGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/GptGod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/OnlineGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/not_working/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.357868 g4f-0.3.1.6/g4f/Provider/npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.357868 g4f-0.3.1.6/g4f/Provider/npm/node_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/npm/node_modules/.package-lock.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.357868 g4f-0.3.1.6/g4f/Provider/npm/node_modules/crypto-js/
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/npm/node_modules/crypto-js/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/npm/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/npm/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.357868 g4f-0.3.1.6/g4f/Provider/openai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/openai/crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/openai/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/openai/proofofwork.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.361868 g4f-0.3.1.6/g4f/Provider/selenium/
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/selenium/AItianhuSpace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/selenium/Bard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/selenium/MyShell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/selenium/PerplexityAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/selenium/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/selenium/TalkAi.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/selenium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.361868 g4f-0.3.1.6/g4f/Provider/unfinished/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/unfinished/AiChatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/unfinished/ChatAiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/unfinished/Komo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/unfinished/MikuChat.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/unfinished/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.361868 g4f-0.3.1.6/g4f/Provider/you/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/you/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/Provider/you/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.361868 g4f-0.3.1.6/g4f/api/
--rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/api/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/api/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/api/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.361868 g4f-0.3.1.6/g4f/client/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/client/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/client/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/client/image_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/client/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/client/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.365868 g4f-0.3.1.6/g4f/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.365868 g4f-0.3.1.6/g4f/gui/client/
--rw-r--r--   0 runner    (1001) docker     (127)    13390 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.333868 g4f-0.3.1.6/g4f/gui/client/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.365868 g4f-0.3.1.6/g4f/gui/client/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/css/dracula.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    20937 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.365868 g4f-0.3.1.6/g4f/gui/client/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/img/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/img/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/img/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/img/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/img/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/img/gpt.png
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/img/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/img/user.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.365868 g4f-0.3.1.6/g4f/gui/client/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    50252 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/js/chat.v1.js
--rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/js/highlightjs-copy.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/js/icons.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.369868 g4f-0.3.1.6/g4f/gui/client/static/js/text_to_speech/
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/js/text_to_speech/630.index.js
--rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/js/text_to_speech/900.index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/client/static/js/text_to_speech/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/gui_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.369868 g4f-0.3.1.6/g4f/gui/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/server/android_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/server/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/server/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/server/internet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/server/js_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/server/website.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/gui/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.369868 g4f-0.3.1.6/g4f/local/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.369868 g4f-0.3.1.6/g4f/locals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/locals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/locals/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/locals/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.373868 g4f-0.3.1.6/g4f/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/providers/base_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/providers/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/providers/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/providers/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    12147 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/providers/retry_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/providers/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.373868 g4f-0.3.1.6/g4f/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/requests/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/requests/curl_cffi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/requests/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/requests/raise_for_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-19 04:02:00.000000 g4f-0.3.1.6/g4f/webdriver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:11.373868 g4f-0.3.1.6/g4f.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    56222 2024-05-19 04:02:11.000000 g4f-0.3.1.6/g4f.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-05-19 04:02:11.000000 g4f-0.3.1.6/g4f.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 04:02:11.000000 g4f-0.3.1.6/g4f.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-19 04:02:11.000000 g4f-0.3.1.6/g4f.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-19 04:02:11.000000 g4f-0.3.1.6/g4f.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 04:02:11.000000 g4f-0.3.1.6/g4f.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 04:02:11.377868 g4f-0.3.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-19 04:02:00.000000 g4f-0.3.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:12.031974 g4f-0.3.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-19 08:14:01.000000 g4f-0.3.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-19 08:14:01.000000 g4f-0.3.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    55910 2024-05-19 08:14:12.027974 g4f-0.3.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    52714 2024-05-19 08:14:01.000000 g4f-0.3.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:11.991974 g4f-0.3.1.7/g4f/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:11.999974 g4f-0.3.1.7/g4f/Provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/Aichatos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/Aura.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21427 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/Bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/BingCreateImages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/Blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/ChatForAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/Chatgpt4Online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/ChatgptAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/ChatgptFree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/ChatgptNext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/ChatgptX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/Cnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/Cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/DeepInfra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/DeepInfraImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/DuckDuckGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/Ecosia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/Feedough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/FlowGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/FreeChatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/FreeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/GeminiPro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/GeminiProChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/GigaChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/GptTalkRu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/HuggingChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/HuggingFace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/Koala.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/Liaobots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/Llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/Local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/MetaAI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/MetaAIAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/Ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/PerplexityLabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/Pi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/Reka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/Replicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/ReplicateImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/WhiteRabbitNeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/You.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/base_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:11.999974 g4f-0.3.1.7/g4f/Provider/bing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/bing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/bing/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/bing/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/bing/upload_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:12.007974 g4f-0.3.1.7/g4f/Provider/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/Acytoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/AiAsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/AiChatOnline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/AiService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/Aibn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/Aichat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/Ails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/Aivvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/Berlin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/ChatAnywhere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/ChatgptDuo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/CodeLinkAva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/Cromicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/DfeHub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/EasyChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/Equing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/FakeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/FastGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/Forefront.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/GPTalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/GeekGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/GetGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/H2o.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/Hashnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/Lockchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/Myshell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/NoowAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/Opchatgpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/OpenAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/V50.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/Vitalentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/VoiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/Wewordle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/Wuguokai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/Ylokh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/Yqcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/deprecated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:12.007974 g4f-0.3.1.7/g4f/Provider/gigachat_crt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:12.007974 g4f-0.3.1.7/g4f/Provider/needs_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)    10986 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/needs_auth/Gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/needs_auth/Groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/needs_auth/OpenRouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/needs_auth/Openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/needs_auth/OpenaiAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33277 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/needs_auth/OpenaiChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/needs_auth/PerplexityApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/needs_auth/Poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/needs_auth/Raycast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/needs_auth/Theb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/needs_auth/ThebApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/needs_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:12.011974 g4f-0.3.1.7/g4f/Provider/not_working/
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/not_working/AItianhu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/not_working/Bestim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/not_working/ChatBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/not_working/ChatgptDemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/not_working/ChatgptDemoAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/not_working/ChatgptLogin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/not_working/Chatxyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/not_working/Gpt6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/not_working/GptChatly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/not_working/GptForLove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/not_working/GptGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/not_working/GptGod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/not_working/OnlineGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/not_working/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:12.011974 g4f-0.3.1.7/g4f/Provider/npm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:12.011974 g4f-0.3.1.7/g4f/Provider/npm/node_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/npm/node_modules/.package-lock.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:12.011974 g4f-0.3.1.7/g4f/Provider/npm/node_modules/crypto-js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/npm/node_modules/crypto-js/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/npm/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/npm/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:12.011974 g4f-0.3.1.7/g4f/Provider/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/openai/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/openai/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/openai/proofofwork.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:12.011974 g4f-0.3.1.7/g4f/Provider/selenium/
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/selenium/AItianhuSpace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/selenium/Bard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/selenium/MyShell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/selenium/PerplexityAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/selenium/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/selenium/TalkAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/selenium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:12.015974 g4f-0.3.1.7/g4f/Provider/unfinished/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/unfinished/AiChatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/unfinished/ChatAiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/unfinished/Komo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/unfinished/MikuChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/unfinished/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:12.015974 g4f-0.3.1.7/g4f/Provider/you/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/you/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/Provider/you/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:12.015974 g4f-0.3.1.7/g4f/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/api/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/api/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/api/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:12.015974 g4f-0.3.1.7/g4f/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/client/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/client/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/client/image_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/client/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/client/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:12.015974 g4f-0.3.1.7/g4f/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:12.015974 g4f-0.3.1.7/g4f/gui/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    13390 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/client/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:11.987974 g4f-0.3.1.7/g4f/gui/client/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:12.015974 g4f-0.3.1.7/g4f/gui/client/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/client/static/css/dracula.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    21124 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/client/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:12.019974 g4f-0.3.1.7/g4f/gui/client/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/client/static/img/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/client/static/img/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/client/static/img/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/client/static/img/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/client/static/img/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/client/static/img/gpt.png
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/client/static/img/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/client/static/img/user.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:12.019974 g4f-0.3.1.7/g4f/gui/client/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    50252 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/client/static/js/chat.v1.js
+-rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/client/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/client/static/js/highlightjs-copy.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/client/static/js/icons.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:12.019974 g4f-0.3.1.7/g4f/gui/client/static/js/text_to_speech/
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/client/static/js/text_to_speech/630.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/client/static/js/text_to_speech/900.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/client/static/js/text_to_speech/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/gui_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:12.023974 g4f-0.3.1.7/g4f/gui/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/server/android_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/server/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/server/internet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/server/js_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/server/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/gui/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:12.023974 g4f-0.3.1.7/g4f/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:12.023974 g4f-0.3.1.7/g4f/locals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/locals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/locals/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/locals/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:12.023974 g4f-0.3.1.7/g4f/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/providers/base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/providers/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/providers/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/providers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12147 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/providers/retry_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/providers/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:12.023974 g4f-0.3.1.7/g4f/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/requests/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/requests/curl_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/requests/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/requests/raise_for_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-19 08:14:01.000000 g4f-0.3.1.7/g4f/webdriver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:14:12.023974 g4f-0.3.1.7/g4f.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    55910 2024-05-19 08:14:11.000000 g4f-0.3.1.7/g4f.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-05-19 08:14:11.000000 g4f-0.3.1.7/g4f.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 08:14:11.000000 g4f-0.3.1.7/g4f.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-19 08:14:11.000000 g4f-0.3.1.7/g4f.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-19 08:14:11.000000 g4f-0.3.1.7/g4f.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 08:14:11.000000 g4f-0.3.1.7/g4f.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 08:14:12.031974 g4f-0.3.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-19 08:14:01.000000 g4f-0.3.1.7/setup.py
```

### Comparing `g4f-0.3.1.6/LICENSE` & `g4f-0.3.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/PKG-INFO` & `g4f-0.3.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.3.1.6
+Version: 0.3.1.7
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
@@ -178,20 +178,18 @@
    - Or set the API base for your client to: [http://localhost:1337/v1](http://localhost:1337/v1)
 
 4. **(Optional) Provider Login:**
    If required, you can access the container's desktop here: http://localhost:7900/?autoconnect=1&resize=scale&password=secret for provider login purposes.
 
 #### Installation Guide for Windows (.exe)
 To ensure the seamless operation of our application, please follow the instructions below. These steps are designed to guide you through the installation process on Windows operating systems.
-##### Prerequisites
-1. **WebView2 Runtime**: Our application requires the *WebView2 Runtime* to be installed on your system. If you do not have it installed, please download and install it from the [Microsoft Developer Website](https://developer.microsoft.com/en-us/microsoft-edge/webview2/). If you already have *WebView2 Runtime* installed but are encountering issues, navigate to *Installed Windows Apps*, select *WebView2*, and opt for the repair option.
-##### Installation Steps
-2. **Download the Application**: Visit our [latest releases page](https://github.com/xtekky/gpt4free/releases/latest) and download the most recent version of the application, named `g4f.webview.*.exe`.
-3. **File Placement**: Once downloaded, transfer the `.exe` file from your downloads folder to a directory of your choice on your system, and then execute it to run the app.
-##### Post-Installation Adjustment
+### Installation Steps
+1. **Download the Application**: Visit our [latest releases page](https://github.com/xtekky/gpt4free/releases/latest) and download the most recent version of the application, named `g4f.exe.zip`.
+2. **File Placement**: After downloading, locate the `.zip` file in your Downloads folder. Unpack it to a directory of your choice on your system, then execute the `g4f.exe` file to run the app.
+3. **Open GUI**: The app starts a web server with the GUI. Open your favorite browser and navigate to `http://localhost:8080/chat/` to access the application interface.
 4. **Firewall Configuration (Hotfix)**: Upon installation, it may be necessary to adjust your Windows Firewall settings to allow the application to operate correctly. To do this, access your Windows Firewall settings and allow the application.
 
 By following these steps, you should be able to successfully install and run the application on your Windows system. If you encounter any issues during the installation process, please refer to our Issue Tracker or try to get contact over Discord for assistance.
 
 Run the **Webview UI** on other Platfroms:
 - [/docs/guides/webview](https://github.com/xtekky/gpt4free/blob/main/docs/webview.md)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.3.1.6 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.1.7 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
@@ -106,54 +106,49 @@
 the included client, navigate to: [http://localhost:8080/chat/](http://
 localhost:8080/chat/) - Or set the API base for your client to: [http://
 localhost:1337/v1](http://localhost:1337/v1) 4. **(Optional) Provider Login:**
 If required, you can access the container's desktop here: http://localhost:
 7900/?autoconnect=1&resize=scale&password=secret for provider login purposes.
 #### Installation Guide for Windows (.exe) To ensure the seamless operation of
 our application, please follow the instructions below. These steps are designed
-to guide you through the installation process on Windows operating systems.
-##### Prerequisites 1. **WebView2 Runtime**: Our application requires the
-*WebView2 Runtime* to be installed on your system. If you do not have it
-installed, please download and install it from the [Microsoft Developer
-Website](https://developer.microsoft.com/en-us/microsoft-edge/webview2/). If
-you already have *WebView2 Runtime* installed but are encountering issues,
-navigate to *Installed Windows Apps*, select *WebView2*, and opt for the repair
-option. ##### Installation Steps 2. **Download the Application**: Visit our
-[latest releases page](https://github.com/xtekky/gpt4free/releases/latest) and
-download the most recent version of the application, named `g4f.webview.*.exe`.
-3. **File Placement**: Once downloaded, transfer the `.exe` file from your
-downloads folder to a directory of your choice on your system, and then execute
-it to run the app. ##### Post-Installation Adjustment 4. **Firewall
-Configuration (Hotfix)**: Upon installation, it may be necessary to adjust your
-Windows Firewall settings to allow the application to operate correctly. To do
-this, access your Windows Firewall settings and allow the application. By
-following these steps, you should be able to successfully install and run the
-application on your Windows system. If you encounter any issues during the
-installation process, please refer to our Issue Tracker or try to get contact
-over Discord for assistance. Run the **Webview UI** on other Platfroms: - [/
-docs/guides/webview](https://github.com/xtekky/gpt4free/blob/main/docs/
-webview.md) ##### Use your smartphone: Run the Web UI on Your Smartphone: - [/
-docs/guides/phone](https://github.com/xtekky/gpt4free/blob/main/docs/guides/
-phone.md) #### Use python ##### Prerequisites: 1. [Download and install Python]
-(https://www.python.org/downloads/) (Version 3.10+ is recommended). 2. [Install
-Google Chrome](https://www.google.com/chrome/) for providers with webdriver
-##### Install using PyPI package: ``` pip install -U g4f[all] ``` How do I
-install only parts or do disable parts? Use partial requirements: [/docs/
-requirements](https://github.com/xtekky/gpt4free/blob/main/docs/
-requirements.md) ##### Install from source: How do I load the project using git
-and installing the project requirements? Read this tutorial and follow it step
-by step: [/docs/git](https://github.com/xtekky/gpt4free/blob/main/docs/git.md)
-##### Install using Docker: How do I build and run composer image from source?
-Use docker-compose: [/docs/docker](https://github.com/xtekky/gpt4free/blob/
-main/docs/docker.md) ## ð¡ Usage #### Text Generation ```python from
-g4f.client import Client client = Client() response =
-client.chat.completions.create( model="gpt-3.5-turbo", messages=[{"role":
-"user", "content": "Hello"}], ... ) print(response.choices[0].message.content)
-``` ``` Hello! How can I assist you today? ``` #### Image Generation ```python
-from g4f.client import Client client = Client() response =
+to guide you through the installation process on Windows operating systems. ###
+Installation Steps 1. **Download the Application**: Visit our [latest releases
+page](https://github.com/xtekky/gpt4free/releases/latest) and download the most
+recent version of the application, named `g4f.exe.zip`. 2. **File Placement**:
+After downloading, locate the `.zip` file in your Downloads folder. Unpack it
+to a directory of your choice on your system, then execute the `g4f.exe` file
+to run the app. 3. **Open GUI**: The app starts a web server with the GUI. Open
+your favorite browser and navigate to `http://localhost:8080/chat/` to access
+the application interface. 4. **Firewall Configuration (Hotfix)**: Upon
+installation, it may be necessary to adjust your Windows Firewall settings to
+allow the application to operate correctly. To do this, access your Windows
+Firewall settings and allow the application. By following these steps, you
+should be able to successfully install and run the application on your Windows
+system. If you encounter any issues during the installation process, please
+refer to our Issue Tracker or try to get contact over Discord for assistance.
+Run the **Webview UI** on other Platfroms: - [/docs/guides/webview](https://
+github.com/xtekky/gpt4free/blob/main/docs/webview.md) ##### Use your
+smartphone: Run the Web UI on Your Smartphone: - [/docs/guides/phone](https://
+github.com/xtekky/gpt4free/blob/main/docs/guides/phone.md) #### Use python
+##### Prerequisites: 1. [Download and install Python](https://www.python.org/
+downloads/) (Version 3.10+ is recommended). 2. [Install Google Chrome](https://
+www.google.com/chrome/) for providers with webdriver ##### Install using PyPI
+package: ``` pip install -U g4f[all] ``` How do I install only parts or do
+disable parts? Use partial requirements: [/docs/requirements](https://
+github.com/xtekky/gpt4free/blob/main/docs/requirements.md) ##### Install from
+source: How do I load the project using git and installing the project
+requirements? Read this tutorial and follow it step by step: [/docs/git](https:
+//github.com/xtekky/gpt4free/blob/main/docs/git.md) ##### Install using Docker:
+How do I build and run composer image from source? Use docker-compose: [/docs/
+docker](https://github.com/xtekky/gpt4free/blob/main/docs/docker.md) ## ð¡
+Usage #### Text Generation ```python from g4f.client import Client client =
+Client() response = client.chat.completions.create( model="gpt-3.5-turbo",
+messages=[{"role": "user", "content": "Hello"}], ... ) print(response.choices
+[0].message.content) ``` ``` Hello! How can I assist you today? ``` #### Image
+Generation ```python from g4f.client import Client client = Client() response =
 client.images.generate( model="gemini", prompt="a white siamese cat", ... )
 image_url = response.data[0].url ``` [![Image with cat](/docs/cat.jpeg)](https:
 //github.com/xtekky/gpt4free/blob/main/docs/client.md) **Full Documentation for
 Python API** - New AsyncClient API from G4F: [/docs/async_client](https://
 github.com/xtekky/gpt4free/blob/main/docs/async_client.md) - Client API like
 the OpenAI Python library: [/docs/client](https://github.com/xtekky/gpt4free/
 blob/main/docs/client.md) - Legacy API with python modules: [/docs/legacy]
```

### Comparing `g4f-0.3.1.6/README.md` & `g4f-0.3.1.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -100,20 +100,18 @@
    - Or set the API base for your client to: [http://localhost:1337/v1](http://localhost:1337/v1)
 
 4. **(Optional) Provider Login:**
    If required, you can access the container's desktop here: http://localhost:7900/?autoconnect=1&resize=scale&password=secret for provider login purposes.
 
 #### Installation Guide for Windows (.exe)
 To ensure the seamless operation of our application, please follow the instructions below. These steps are designed to guide you through the installation process on Windows operating systems.
-##### Prerequisites
-1. **WebView2 Runtime**: Our application requires the *WebView2 Runtime* to be installed on your system. If you do not have it installed, please download and install it from the [Microsoft Developer Website](https://developer.microsoft.com/en-us/microsoft-edge/webview2/). If you already have *WebView2 Runtime* installed but are encountering issues, navigate to *Installed Windows Apps*, select *WebView2*, and opt for the repair option.
-##### Installation Steps
-2. **Download the Application**: Visit our [latest releases page](https://github.com/xtekky/gpt4free/releases/latest) and download the most recent version of the application, named `g4f.webview.*.exe`.
-3. **File Placement**: Once downloaded, transfer the `.exe` file from your downloads folder to a directory of your choice on your system, and then execute it to run the app.
-##### Post-Installation Adjustment
+### Installation Steps
+1. **Download the Application**: Visit our [latest releases page](https://github.com/xtekky/gpt4free/releases/latest) and download the most recent version of the application, named `g4f.exe.zip`.
+2. **File Placement**: After downloading, locate the `.zip` file in your Downloads folder. Unpack it to a directory of your choice on your system, then execute the `g4f.exe` file to run the app.
+3. **Open GUI**: The app starts a web server with the GUI. Open your favorite browser and navigate to `http://localhost:8080/chat/` to access the application interface.
 4. **Firewall Configuration (Hotfix)**: Upon installation, it may be necessary to adjust your Windows Firewall settings to allow the application to operate correctly. To do this, access your Windows Firewall settings and allow the application.
 
 By following these steps, you should be able to successfully install and run the application on your Windows system. If you encounter any issues during the installation process, please refer to our Issue Tracker or try to get contact over Discord for assistance.
 
 Run the **Webview UI** on other Platfroms:
 - [/docs/guides/webview](https://github.com/xtekky/gpt4free/blob/main/docs/webview.md)
```

#### html2text {}

```diff
@@ -64,54 +64,49 @@
 the included client, navigate to: [http://localhost:8080/chat/](http://
 localhost:8080/chat/) - Or set the API base for your client to: [http://
 localhost:1337/v1](http://localhost:1337/v1) 4. **(Optional) Provider Login:**
 If required, you can access the container's desktop here: http://localhost:
 7900/?autoconnect=1&resize=scale&password=secret for provider login purposes.
 #### Installation Guide for Windows (.exe) To ensure the seamless operation of
 our application, please follow the instructions below. These steps are designed
-to guide you through the installation process on Windows operating systems.
-##### Prerequisites 1. **WebView2 Runtime**: Our application requires the
-*WebView2 Runtime* to be installed on your system. If you do not have it
-installed, please download and install it from the [Microsoft Developer
-Website](https://developer.microsoft.com/en-us/microsoft-edge/webview2/). If
-you already have *WebView2 Runtime* installed but are encountering issues,
-navigate to *Installed Windows Apps*, select *WebView2*, and opt for the repair
-option. ##### Installation Steps 2. **Download the Application**: Visit our
-[latest releases page](https://github.com/xtekky/gpt4free/releases/latest) and
-download the most recent version of the application, named `g4f.webview.*.exe`.
-3. **File Placement**: Once downloaded, transfer the `.exe` file from your
-downloads folder to a directory of your choice on your system, and then execute
-it to run the app. ##### Post-Installation Adjustment 4. **Firewall
-Configuration (Hotfix)**: Upon installation, it may be necessary to adjust your
-Windows Firewall settings to allow the application to operate correctly. To do
-this, access your Windows Firewall settings and allow the application. By
-following these steps, you should be able to successfully install and run the
-application on your Windows system. If you encounter any issues during the
-installation process, please refer to our Issue Tracker or try to get contact
-over Discord for assistance. Run the **Webview UI** on other Platfroms: - [/
-docs/guides/webview](https://github.com/xtekky/gpt4free/blob/main/docs/
-webview.md) ##### Use your smartphone: Run the Web UI on Your Smartphone: - [/
-docs/guides/phone](https://github.com/xtekky/gpt4free/blob/main/docs/guides/
-phone.md) #### Use python ##### Prerequisites: 1. [Download and install Python]
-(https://www.python.org/downloads/) (Version 3.10+ is recommended). 2. [Install
-Google Chrome](https://www.google.com/chrome/) for providers with webdriver
-##### Install using PyPI package: ``` pip install -U g4f[all] ``` How do I
-install only parts or do disable parts? Use partial requirements: [/docs/
-requirements](https://github.com/xtekky/gpt4free/blob/main/docs/
-requirements.md) ##### Install from source: How do I load the project using git
-and installing the project requirements? Read this tutorial and follow it step
-by step: [/docs/git](https://github.com/xtekky/gpt4free/blob/main/docs/git.md)
-##### Install using Docker: How do I build and run composer image from source?
-Use docker-compose: [/docs/docker](https://github.com/xtekky/gpt4free/blob/
-main/docs/docker.md) ## ð¡ Usage #### Text Generation ```python from
-g4f.client import Client client = Client() response =
-client.chat.completions.create( model="gpt-3.5-turbo", messages=[{"role":
-"user", "content": "Hello"}], ... ) print(response.choices[0].message.content)
-``` ``` Hello! How can I assist you today? ``` #### Image Generation ```python
-from g4f.client import Client client = Client() response =
+to guide you through the installation process on Windows operating systems. ###
+Installation Steps 1. **Download the Application**: Visit our [latest releases
+page](https://github.com/xtekky/gpt4free/releases/latest) and download the most
+recent version of the application, named `g4f.exe.zip`. 2. **File Placement**:
+After downloading, locate the `.zip` file in your Downloads folder. Unpack it
+to a directory of your choice on your system, then execute the `g4f.exe` file
+to run the app. 3. **Open GUI**: The app starts a web server with the GUI. Open
+your favorite browser and navigate to `http://localhost:8080/chat/` to access
+the application interface. 4. **Firewall Configuration (Hotfix)**: Upon
+installation, it may be necessary to adjust your Windows Firewall settings to
+allow the application to operate correctly. To do this, access your Windows
+Firewall settings and allow the application. By following these steps, you
+should be able to successfully install and run the application on your Windows
+system. If you encounter any issues during the installation process, please
+refer to our Issue Tracker or try to get contact over Discord for assistance.
+Run the **Webview UI** on other Platfroms: - [/docs/guides/webview](https://
+github.com/xtekky/gpt4free/blob/main/docs/webview.md) ##### Use your
+smartphone: Run the Web UI on Your Smartphone: - [/docs/guides/phone](https://
+github.com/xtekky/gpt4free/blob/main/docs/guides/phone.md) #### Use python
+##### Prerequisites: 1. [Download and install Python](https://www.python.org/
+downloads/) (Version 3.10+ is recommended). 2. [Install Google Chrome](https://
+www.google.com/chrome/) for providers with webdriver ##### Install using PyPI
+package: ``` pip install -U g4f[all] ``` How do I install only parts or do
+disable parts? Use partial requirements: [/docs/requirements](https://
+github.com/xtekky/gpt4free/blob/main/docs/requirements.md) ##### Install from
+source: How do I load the project using git and installing the project
+requirements? Read this tutorial and follow it step by step: [/docs/git](https:
+//github.com/xtekky/gpt4free/blob/main/docs/git.md) ##### Install using Docker:
+How do I build and run composer image from source? Use docker-compose: [/docs/
+docker](https://github.com/xtekky/gpt4free/blob/main/docs/docker.md) ## ð¡
+Usage #### Text Generation ```python from g4f.client import Client client =
+Client() response = client.chat.completions.create( model="gpt-3.5-turbo",
+messages=[{"role": "user", "content": "Hello"}], ... ) print(response.choices
+[0].message.content) ``` ``` Hello! How can I assist you today? ``` #### Image
+Generation ```python from g4f.client import Client client = Client() response =
 client.images.generate( model="gemini", prompt="a white siamese cat", ... )
 image_url = response.data[0].url ``` [![Image with cat](/docs/cat.jpeg)](https:
 //github.com/xtekky/gpt4free/blob/main/docs/client.md) **Full Documentation for
 Python API** - New AsyncClient API from G4F: [/docs/async_client](https://
 github.com/xtekky/gpt4free/blob/main/docs/async_client.md) - Client API like
 the OpenAI Python library: [/docs/client](https://github.com/xtekky/gpt4free/
 blob/main/docs/client.md) - Legacy API with python modules: [/docs/legacy]
```

### Comparing `g4f-0.3.1.6/g4f/Provider/Aichatos.py` & `g4f-0.3.1.7/g4f/Provider/Aichatos.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/Aura.py` & `g4f-0.3.1.7/g4f/Provider/Aura.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/Bing.py` & `g4f-0.3.1.7/g4f/Provider/Bing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/BingCreateImages.py` & `g4f-0.3.1.7/g4f/Provider/BingCreateImages.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/Blackbox.py` & `g4f-0.3.1.7/g4f/Provider/Blackbox.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/ChatForAi.py` & `g4f-0.3.1.7/g4f/Provider/ChatForAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/Chatgpt4Online.py` & `g4f-0.3.1.7/g4f/Provider/Chatgpt4Online.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/ChatgptAi.py` & `g4f-0.3.1.7/g4f/Provider/ChatgptAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/ChatgptFree.py` & `g4f-0.3.1.7/g4f/Provider/ChatgptFree.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/ChatgptNext.py` & `g4f-0.3.1.7/g4f/Provider/ChatgptNext.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/ChatgptX.py` & `g4f-0.3.1.7/g4f/Provider/ChatgptX.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/Cnote.py` & `g4f-0.3.1.7/g4f/Provider/Cnote.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/Cohere.py` & `g4f-0.3.1.7/g4f/Provider/Cohere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/DeepInfra.py` & `g4f-0.3.1.7/g4f/Provider/DeepInfra.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/DeepInfraImage.py` & `g4f-0.3.1.7/g4f/Provider/DeepInfraImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/DuckDuckGo.py` & `g4f-0.3.1.7/g4f/Provider/DuckDuckGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/Ecosia.py` & `g4f-0.3.1.7/g4f/Provider/Ecosia.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/Feedough.py` & `g4f-0.3.1.7/g4f/Provider/Feedough.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/FlowGpt.py` & `g4f-0.3.1.7/g4f/Provider/FlowGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/FreeChatgpt.py` & `g4f-0.3.1.7/g4f/Provider/FreeChatgpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/FreeGpt.py` & `g4f-0.3.1.7/g4f/Provider/FreeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/GeminiPro.py` & `g4f-0.3.1.7/g4f/Provider/GeminiPro.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/GeminiProChat.py` & `g4f-0.3.1.7/g4f/Provider/GeminiProChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/GigaChat.py` & `g4f-0.3.1.7/g4f/Provider/GigaChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/GptTalkRu.py` & `g4f-0.3.1.7/g4f/Provider/GptTalkRu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/HuggingChat.py` & `g4f-0.3.1.7/g4f/Provider/HuggingChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/HuggingFace.py` & `g4f-0.3.1.7/g4f/Provider/HuggingFace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/Koala.py` & `g4f-0.3.1.7/g4f/Provider/Koala.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/Liaobots.py` & `g4f-0.3.1.7/g4f/Provider/Liaobots.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/Llama.py` & `g4f-0.3.1.7/g4f/Provider/Llama.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/Local.py` & `g4f-0.3.1.7/g4f/Provider/Local.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/MetaAI.py` & `g4f-0.3.1.7/g4f/Provider/MetaAI.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/MetaAIAccount.py` & `g4f-0.3.1.7/g4f/Provider/MetaAIAccount.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/Ollama.py` & `g4f-0.3.1.7/g4f/Provider/Ollama.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/PerplexityLabs.py` & `g4f-0.3.1.7/g4f/Provider/PerplexityLabs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/Pi.py` & `g4f-0.3.1.7/g4f/Provider/Pi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/Reka.py` & `g4f-0.3.1.7/g4f/Provider/Reka.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/Replicate.py` & `g4f-0.3.1.7/g4f/Provider/Replicate.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/ReplicateImage.py` & `g4f-0.3.1.7/g4f/Provider/ReplicateImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/Vercel.py` & `g4f-0.3.1.7/g4f/Provider/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/WhiteRabbitNeo.py` & `g4f-0.3.1.7/g4f/Provider/WhiteRabbitNeo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/You.py` & `g4f-0.3.1.7/g4f/Provider/You.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/__init__.py` & `g4f-0.3.1.7/g4f/Provider/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/bing/conversation.py` & `g4f-0.3.1.7/g4f/Provider/bing/conversation.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/bing/create_images.py` & `g4f-0.3.1.7/g4f/Provider/bing/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/bing/upload_image.py` & `g4f-0.3.1.7/g4f/Provider/bing/upload_image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/Acytoo.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/Acytoo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/AiAsk.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/AiAsk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/AiChatOnline.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/AiChatOnline.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/AiService.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/AiService.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/Aibn.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/Aibn.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/Aichat.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/Aichat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/Ails.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/Ails.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/Aivvm.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/Aivvm.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/Berlin.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/Berlin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/ChatAnywhere.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/ChatAnywhere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/ChatgptDuo.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/ChatgptDuo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/CodeLinkAva.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/CodeLinkAva.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/Cromicle.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/Cromicle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/DfeHub.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/DfeHub.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/EasyChat.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/EasyChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/Equing.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/Equing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/FakeGpt.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/FakeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/FastGpt.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/FastGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/Forefront.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/Forefront.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/GPTalk.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/GPTalk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/GeekGpt.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/GeekGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/GetGpt.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/GetGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/H2o.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/H2o.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/Hashnode.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/Hashnode.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/Lockchat.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/Lockchat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/Myshell.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/Myshell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/NoowAi.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/NoowAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/Opchatgpts.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/Opchatgpts.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/OpenAssistant.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/OpenAssistant.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/Phind.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/V50.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/V50.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/Vercel.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/Vitalentum.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/Vitalentum.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/VoiGpt.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/VoiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/Wewordle.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/Wewordle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/Wuguokai.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/Wuguokai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/Ylokh.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/Ylokh.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/Yqcloud.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/Yqcloud.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/deprecated/__init__.py` & `g4f-0.3.1.7/g4f/Provider/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt` & `g4f-0.3.1.7/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/needs_auth/Gemini.py` & `g4f-0.3.1.7/g4f/Provider/needs_auth/Gemini.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/needs_auth/Groq.py` & `g4f-0.3.1.7/g4f/Provider/needs_auth/Groq.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/needs_auth/OpenRouter.py` & `g4f-0.3.1.7/g4f/Provider/needs_auth/OpenRouter.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/needs_auth/Openai.py` & `g4f-0.3.1.7/g4f/Provider/needs_auth/Openai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/needs_auth/OpenaiChat.py` & `g4f-0.3.1.7/g4f/Provider/needs_auth/OpenaiChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/needs_auth/PerplexityApi.py` & `g4f-0.3.1.7/g4f/Provider/needs_auth/PerplexityApi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/needs_auth/Poe.py` & `g4f-0.3.1.7/g4f/Provider/needs_auth/Poe.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/needs_auth/Raycast.py` & `g4f-0.3.1.7/g4f/Provider/needs_auth/Raycast.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/needs_auth/Theb.py` & `g4f-0.3.1.7/g4f/Provider/needs_auth/Theb.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/needs_auth/ThebApi.py` & `g4f-0.3.1.7/g4f/Provider/needs_auth/ThebApi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/not_working/AItianhu.py` & `g4f-0.3.1.7/g4f/Provider/not_working/AItianhu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/not_working/Bestim.py` & `g4f-0.3.1.7/g4f/Provider/not_working/Bestim.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/not_working/ChatBase.py` & `g4f-0.3.1.7/g4f/Provider/not_working/ChatBase.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/not_working/ChatgptDemo.py` & `g4f-0.3.1.7/g4f/Provider/not_working/ChatgptDemo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/not_working/ChatgptDemoAi.py` & `g4f-0.3.1.7/g4f/Provider/not_working/ChatgptDemoAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/not_working/ChatgptLogin.py` & `g4f-0.3.1.7/g4f/Provider/not_working/ChatgptLogin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/not_working/Chatxyz.py` & `g4f-0.3.1.7/g4f/Provider/not_working/Chatxyz.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/not_working/Gpt6.py` & `g4f-0.3.1.7/g4f/Provider/not_working/Gpt6.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/not_working/GptChatly.py` & `g4f-0.3.1.7/g4f/Provider/not_working/GptChatly.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/not_working/GptForLove.py` & `g4f-0.3.1.7/g4f/Provider/not_working/GptForLove.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/not_working/GptGo.py` & `g4f-0.3.1.7/g4f/Provider/not_working/GptGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/not_working/GptGod.py` & `g4f-0.3.1.7/g4f/Provider/not_working/GptGod.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/not_working/OnlineGpt.py` & `g4f-0.3.1.7/g4f/Provider/not_working/OnlineGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/npm/node_modules/crypto-js/README.md` & `g4f-0.3.1.7/g4f/Provider/npm/node_modules/crypto-js/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js` & `g4f-0.3.1.7/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/npm/package-lock.json` & `g4f-0.3.1.7/g4f/Provider/npm/package-lock.json`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/openai/crypt.py` & `g4f-0.3.1.7/g4f/Provider/openai/crypt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/openai/har_file.py` & `g4f-0.3.1.7/g4f/Provider/openai/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/openai/proofofwork.py` & `g4f-0.3.1.7/g4f/Provider/openai/proofofwork.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/selenium/AItianhuSpace.py` & `g4f-0.3.1.7/g4f/Provider/selenium/AItianhuSpace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/selenium/Bard.py` & `g4f-0.3.1.7/g4f/Provider/selenium/Bard.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/selenium/MyShell.py` & `g4f-0.3.1.7/g4f/Provider/selenium/MyShell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/selenium/PerplexityAi.py` & `g4f-0.3.1.7/g4f/Provider/selenium/PerplexityAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/selenium/Phind.py` & `g4f-0.3.1.7/g4f/Provider/selenium/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/selenium/TalkAi.py` & `g4f-0.3.1.7/g4f/Provider/selenium/TalkAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/unfinished/AiChatting.py` & `g4f-0.3.1.7/g4f/Provider/unfinished/AiChatting.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/unfinished/ChatAiGpt.py` & `g4f-0.3.1.7/g4f/Provider/unfinished/ChatAiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/unfinished/Komo.py` & `g4f-0.3.1.7/g4f/Provider/unfinished/Komo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/unfinished/MikuChat.py` & `g4f-0.3.1.7/g4f/Provider/unfinished/MikuChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/Provider/you/har_file.py` & `g4f-0.3.1.7/g4f/Provider/you/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/__init__.py` & `g4f-0.3.1.7/g4f/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/api/__init__.py` & `g4f-0.3.1.7/g4f/api/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/api/_logging.py` & `g4f-0.3.1.7/g4f/api/_logging.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/cli.py` & `g4f-0.3.1.7/g4f/cli.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/client/async_client.py` & `g4f-0.3.1.7/g4f/client/async_client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/client/client.py` & `g4f-0.3.1.7/g4f/client/client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/client/helper.py` & `g4f-0.3.1.7/g4f/client/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/client/image_models.py` & `g4f-0.3.1.7/g4f/client/image_models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/client/service.py` & `g4f-0.3.1.7/g4f/client/service.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/client/stubs.py` & `g4f-0.3.1.7/g4f/client/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/client/types.py` & `g4f-0.3.1.7/g4f/client/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/cookies.py` & `g4f-0.3.1.7/g4f/cookies.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/errors.py` & `g4f-0.3.1.7/g4f/errors.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/gui/__init__.py` & `g4f-0.3.1.7/g4f/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/gui/client/index.html` & `g4f-0.3.1.7/g4f/gui/client/index.html`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/gui/client/static/css/dracula.min.css` & `g4f-0.3.1.7/g4f/gui/client/static/css/dracula.min.css`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/gui/client/static/css/style.css` & `g4f-0.3.1.7/g4f/gui/client/static/css/style.css`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,16 @@
     --accent: #8b3dff;
     --gradient: var(--accent);
     --blur-bg: #16101b66;
     --blur-border: #84719040;
     --user-input: #ac87bb;
     --conversations: #c7a2ff;
     --conversations-hover: #c7a2ff4d;
+    --scrollbar: var(--colour-3);
+    --scrollbar-thumb: var(--blur-bg);
 }
 
 :root {
     --font-1: "Inter", sans-serif;
     --section-gap: 25px;
     --inner-gap: 15px;
     --border-radius-1: 8px;
@@ -375,28 +377,27 @@
 .message .user .fa-xmark {
     position: absolute;
     top: -2px;
     left: 0px;
     z-index: 1000;
     display: none;
     cursor: pointer;
-    filter: grayscale(1) invert(1);
+}
+
+.message .user .fa-xmark {
+    color: var(--colour-1);
 }
 
 .message .count .fa-clipboard,
 .message .count .fa-volume-high,
 .message .count .fa-rotate {
     z-index: 1000;
     cursor: pointer;
 }
 
-.message .user .fa-xmark {
-    color: var(--colour-1);
-}
-
 .message .count .fa-clipboard {
     color: var(--colour-3);
 }
 
 .message .count .fa-clipboard.clicked {
     color: var(--accent);
 }
@@ -693,14 +694,15 @@
     position: absolute;
     top: 0;
     padding: var(--inner-gap) 10px;
     border: none;
     background: transparent;
     cursor: pointer;
     height: 49px;
+    color: var(--colour-3);
 }
 
 @media only screen and (min-width: 40em) {
     select {
         width: 200px;
     }
     .field {
@@ -999,14 +1001,24 @@
 .white {
     --blur-bg: transparent;
     --accent: #007bff;
     --gradient: #ccc;
     --conversations: #0062cc;
     --colour-1: #ffffff;
     --colour-3: #212529;
+    --scrollbar: var(--colour-1);
+    --scrollbar-thumb: var(--gradient);
+}
+
+.white .message .assistant .fa-xmark {
+    color: var(--colour-1);
+}
+
+.white .message .user .fa-xmark {
+    color: var(--colour-3);
 }
 
 #send-button {
     border: 1px dashed #e4d4ffa6;
     border-radius: 4px;
     cursor: pointer;
     padding-left: 8px;
@@ -1068,23 +1080,20 @@
 
 .settings .label {
     font-size: 15px;
     margin-left: var(--inner-gap);
     white-space:nowrap;
 }
 
-::-webkit-scrollbar {
-    width: 10px;
-}
 ::-webkit-scrollbar-track {
-    background: var(--colour-3);
+    background: var(--scrollbar);
 }
 ::-webkit-scrollbar-thumb {
-    background: var(--blur-bg);
-    border-radius: 5px;
+    background: var(--scrollbar-thumb);
+    border-radius: 2px;
 }
 ::-webkit-scrollbar-thumb:hover {
     background: var(--accent);
 }
 
 .hljs {
     color: #e9e9f4;
@@ -1096,18 +1105,14 @@
 
 #message-input {
     height: 90px;
     margin-left: 20px;
     max-height: 200px;
 }
 
-#message-input::-webkit-scrollbar {
-    width: 5px;
-}
-
 .hidden {
     display: none;
 }
 
 .blink {
     animation: blinker 1s step-start infinite;
 }
```

### Comparing `g4f-0.3.1.6/g4f/gui/client/static/img/android-chrome-192x192.png` & `g4f-0.3.1.7/g4f/gui/client/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/gui/client/static/img/android-chrome-512x512.png` & `g4f-0.3.1.7/g4f/gui/client/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/gui/client/static/img/apple-touch-icon.png` & `g4f-0.3.1.7/g4f/gui/client/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/gui/client/static/img/favicon-32x32.png` & `g4f-0.3.1.7/g4f/gui/client/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/gui/client/static/img/gpt.png` & `g4f-0.3.1.7/g4f/gui/client/static/img/gpt.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/gui/client/static/img/user.png` & `g4f-0.3.1.7/g4f/gui/client/static/img/user.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/gui/client/static/js/chat.v1.js` & `g4f-0.3.1.7/g4f/gui/client/static/js/chat.v1.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/gui/client/static/js/highlight.min.js` & `g4f-0.3.1.7/g4f/gui/client/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/gui/client/static/js/highlightjs-copy.min.js` & `g4f-0.3.1.7/g4f/gui/client/static/js/highlightjs-copy.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/gui/client/static/js/icons.js` & `g4f-0.3.1.7/g4f/gui/client/static/js/icons.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/gui/client/static/js/text_to_speech/630.index.js` & `g4f-0.3.1.7/g4f/gui/client/static/js/text_to_speech/630.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/gui/client/static/js/text_to_speech/900.index.js` & `g4f-0.3.1.7/g4f/gui/client/static/js/text_to_speech/900.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/gui/client/static/js/text_to_speech/index.js` & `g4f-0.3.1.7/g4f/gui/client/static/js/text_to_speech/index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/gui/server/android_gallery.py` & `g4f-0.3.1.7/g4f/gui/server/android_gallery.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/gui/server/api.py` & `g4f-0.3.1.7/g4f/gui/server/api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/gui/server/backend.py` & `g4f-0.3.1.7/g4f/gui/server/backend.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/gui/server/config.py` & `g4f-0.3.1.7/g4f/gui/server/config.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/gui/server/internet.py` & `g4f-0.3.1.7/g4f/gui/server/internet.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/gui/server/js_api.py` & `g4f-0.3.1.7/g4f/gui/server/js_api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/gui/server/website.py` & `g4f-0.3.1.7/g4f/gui/server/website.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/gui/webview.py` & `g4f-0.3.1.7/g4f/gui/webview.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/image.py` & `g4f-0.3.1.7/g4f/image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/local/__init__.py` & `g4f-0.3.1.7/g4f/local/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/locals/models.py` & `g4f-0.3.1.7/g4f/locals/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/locals/provider.py` & `g4f-0.3.1.7/g4f/locals/provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/models.py` & `g4f-0.3.1.7/g4f/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/providers/base_provider.py` & `g4f-0.3.1.7/g4f/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/providers/create_images.py` & `g4f-0.3.1.7/g4f/providers/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/providers/helper.py` & `g4f-0.3.1.7/g4f/providers/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/providers/retry_provider.py` & `g4f-0.3.1.7/g4f/providers/retry_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/providers/types.py` & `g4f-0.3.1.7/g4f/providers/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/requests/__init__.py` & `g4f-0.3.1.7/g4f/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/requests/aiohttp.py` & `g4f-0.3.1.7/g4f/requests/aiohttp.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/requests/curl_cffi.py` & `g4f-0.3.1.7/g4f/requests/curl_cffi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/requests/defaults.py` & `g4f-0.3.1.7/g4f/requests/defaults.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/requests/raise_for_status.py` & `g4f-0.3.1.7/g4f/requests/raise_for_status.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/stubs.py` & `g4f-0.3.1.7/g4f/stubs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/typing.py` & `g4f-0.3.1.7/g4f/typing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/version.py` & `g4f-0.3.1.7/g4f/version.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f/webdriver.py` & `g4f-0.3.1.7/g4f/webdriver.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f.egg-info/PKG-INFO` & `g4f-0.3.1.7/g4f.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.3.1.6
+Version: 0.3.1.7
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
@@ -178,20 +178,18 @@
    - Or set the API base for your client to: [http://localhost:1337/v1](http://localhost:1337/v1)
 
 4. **(Optional) Provider Login:**
    If required, you can access the container's desktop here: http://localhost:7900/?autoconnect=1&resize=scale&password=secret for provider login purposes.
 
 #### Installation Guide for Windows (.exe)
 To ensure the seamless operation of our application, please follow the instructions below. These steps are designed to guide you through the installation process on Windows operating systems.
-##### Prerequisites
-1. **WebView2 Runtime**: Our application requires the *WebView2 Runtime* to be installed on your system. If you do not have it installed, please download and install it from the [Microsoft Developer Website](https://developer.microsoft.com/en-us/microsoft-edge/webview2/). If you already have *WebView2 Runtime* installed but are encountering issues, navigate to *Installed Windows Apps*, select *WebView2*, and opt for the repair option.
-##### Installation Steps
-2. **Download the Application**: Visit our [latest releases page](https://github.com/xtekky/gpt4free/releases/latest) and download the most recent version of the application, named `g4f.webview.*.exe`.
-3. **File Placement**: Once downloaded, transfer the `.exe` file from your downloads folder to a directory of your choice on your system, and then execute it to run the app.
-##### Post-Installation Adjustment
+### Installation Steps
+1. **Download the Application**: Visit our [latest releases page](https://github.com/xtekky/gpt4free/releases/latest) and download the most recent version of the application, named `g4f.exe.zip`.
+2. **File Placement**: After downloading, locate the `.zip` file in your Downloads folder. Unpack it to a directory of your choice on your system, then execute the `g4f.exe` file to run the app.
+3. **Open GUI**: The app starts a web server with the GUI. Open your favorite browser and navigate to `http://localhost:8080/chat/` to access the application interface.
 4. **Firewall Configuration (Hotfix)**: Upon installation, it may be necessary to adjust your Windows Firewall settings to allow the application to operate correctly. To do this, access your Windows Firewall settings and allow the application.
 
 By following these steps, you should be able to successfully install and run the application on your Windows system. If you encounter any issues during the installation process, please refer to our Issue Tracker or try to get contact over Discord for assistance.
 
 Run the **Webview UI** on other Platfroms:
 - [/docs/guides/webview](https://github.com/xtekky/gpt4free/blob/main/docs/webview.md)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.3.1.6 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.1.7 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
@@ -106,54 +106,49 @@
 the included client, navigate to: [http://localhost:8080/chat/](http://
 localhost:8080/chat/) - Or set the API base for your client to: [http://
 localhost:1337/v1](http://localhost:1337/v1) 4. **(Optional) Provider Login:**
 If required, you can access the container's desktop here: http://localhost:
 7900/?autoconnect=1&resize=scale&password=secret for provider login purposes.
 #### Installation Guide for Windows (.exe) To ensure the seamless operation of
 our application, please follow the instructions below. These steps are designed
-to guide you through the installation process on Windows operating systems.
-##### Prerequisites 1. **WebView2 Runtime**: Our application requires the
-*WebView2 Runtime* to be installed on your system. If you do not have it
-installed, please download and install it from the [Microsoft Developer
-Website](https://developer.microsoft.com/en-us/microsoft-edge/webview2/). If
-you already have *WebView2 Runtime* installed but are encountering issues,
-navigate to *Installed Windows Apps*, select *WebView2*, and opt for the repair
-option. ##### Installation Steps 2. **Download the Application**: Visit our
-[latest releases page](https://github.com/xtekky/gpt4free/releases/latest) and
-download the most recent version of the application, named `g4f.webview.*.exe`.
-3. **File Placement**: Once downloaded, transfer the `.exe` file from your
-downloads folder to a directory of your choice on your system, and then execute
-it to run the app. ##### Post-Installation Adjustment 4. **Firewall
-Configuration (Hotfix)**: Upon installation, it may be necessary to adjust your
-Windows Firewall settings to allow the application to operate correctly. To do
-this, access your Windows Firewall settings and allow the application. By
-following these steps, you should be able to successfully install and run the
-application on your Windows system. If you encounter any issues during the
-installation process, please refer to our Issue Tracker or try to get contact
-over Discord for assistance. Run the **Webview UI** on other Platfroms: - [/
-docs/guides/webview](https://github.com/xtekky/gpt4free/blob/main/docs/
-webview.md) ##### Use your smartphone: Run the Web UI on Your Smartphone: - [/
-docs/guides/phone](https://github.com/xtekky/gpt4free/blob/main/docs/guides/
-phone.md) #### Use python ##### Prerequisites: 1. [Download and install Python]
-(https://www.python.org/downloads/) (Version 3.10+ is recommended). 2. [Install
-Google Chrome](https://www.google.com/chrome/) for providers with webdriver
-##### Install using PyPI package: ``` pip install -U g4f[all] ``` How do I
-install only parts or do disable parts? Use partial requirements: [/docs/
-requirements](https://github.com/xtekky/gpt4free/blob/main/docs/
-requirements.md) ##### Install from source: How do I load the project using git
-and installing the project requirements? Read this tutorial and follow it step
-by step: [/docs/git](https://github.com/xtekky/gpt4free/blob/main/docs/git.md)
-##### Install using Docker: How do I build and run composer image from source?
-Use docker-compose: [/docs/docker](https://github.com/xtekky/gpt4free/blob/
-main/docs/docker.md) ## ð¡ Usage #### Text Generation ```python from
-g4f.client import Client client = Client() response =
-client.chat.completions.create( model="gpt-3.5-turbo", messages=[{"role":
-"user", "content": "Hello"}], ... ) print(response.choices[0].message.content)
-``` ``` Hello! How can I assist you today? ``` #### Image Generation ```python
-from g4f.client import Client client = Client() response =
+to guide you through the installation process on Windows operating systems. ###
+Installation Steps 1. **Download the Application**: Visit our [latest releases
+page](https://github.com/xtekky/gpt4free/releases/latest) and download the most
+recent version of the application, named `g4f.exe.zip`. 2. **File Placement**:
+After downloading, locate the `.zip` file in your Downloads folder. Unpack it
+to a directory of your choice on your system, then execute the `g4f.exe` file
+to run the app. 3. **Open GUI**: The app starts a web server with the GUI. Open
+your favorite browser and navigate to `http://localhost:8080/chat/` to access
+the application interface. 4. **Firewall Configuration (Hotfix)**: Upon
+installation, it may be necessary to adjust your Windows Firewall settings to
+allow the application to operate correctly. To do this, access your Windows
+Firewall settings and allow the application. By following these steps, you
+should be able to successfully install and run the application on your Windows
+system. If you encounter any issues during the installation process, please
+refer to our Issue Tracker or try to get contact over Discord for assistance.
+Run the **Webview UI** on other Platfroms: - [/docs/guides/webview](https://
+github.com/xtekky/gpt4free/blob/main/docs/webview.md) ##### Use your
+smartphone: Run the Web UI on Your Smartphone: - [/docs/guides/phone](https://
+github.com/xtekky/gpt4free/blob/main/docs/guides/phone.md) #### Use python
+##### Prerequisites: 1. [Download and install Python](https://www.python.org/
+downloads/) (Version 3.10+ is recommended). 2. [Install Google Chrome](https://
+www.google.com/chrome/) for providers with webdriver ##### Install using PyPI
+package: ``` pip install -U g4f[all] ``` How do I install only parts or do
+disable parts? Use partial requirements: [/docs/requirements](https://
+github.com/xtekky/gpt4free/blob/main/docs/requirements.md) ##### Install from
+source: How do I load the project using git and installing the project
+requirements? Read this tutorial and follow it step by step: [/docs/git](https:
+//github.com/xtekky/gpt4free/blob/main/docs/git.md) ##### Install using Docker:
+How do I build and run composer image from source? Use docker-compose: [/docs/
+docker](https://github.com/xtekky/gpt4free/blob/main/docs/docker.md) ## ð¡
+Usage #### Text Generation ```python from g4f.client import Client client =
+Client() response = client.chat.completions.create( model="gpt-3.5-turbo",
+messages=[{"role": "user", "content": "Hello"}], ... ) print(response.choices
+[0].message.content) ``` ``` Hello! How can I assist you today? ``` #### Image
+Generation ```python from g4f.client import Client client = Client() response =
 client.images.generate( model="gemini", prompt="a white siamese cat", ... )
 image_url = response.data[0].url ``` [![Image with cat](/docs/cat.jpeg)](https:
 //github.com/xtekky/gpt4free/blob/main/docs/client.md) **Full Documentation for
 Python API** - New AsyncClient API from G4F: [/docs/async_client](https://
 github.com/xtekky/gpt4free/blob/main/docs/async_client.md) - Client API like
 the OpenAI Python library: [/docs/client](https://github.com/xtekky/gpt4free/
 blob/main/docs/client.md) - Legacy API with python modules: [/docs/legacy]
```

### Comparing `g4f-0.3.1.6/g4f.egg-info/SOURCES.txt` & `g4f-0.3.1.7/g4f.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/g4f.egg-info/requires.txt` & `g4f-0.3.1.7/g4f.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.6/setup.py` & `g4f-0.3.1.7/setup.py`

 * *Files identical despite different names*

