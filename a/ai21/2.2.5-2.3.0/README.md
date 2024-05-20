# Comparing `tmp/ai21-2.2.5.tar.gz` & `tmp/ai21-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai21-2.2.5.tar", max compression
+gzip compressed data, was "ai21-2.3.0.tar", max compression
```

## Comparing `ai21-2.2.5.tar` & `ai21-2.3.0.tar`

### file list

```diff
@@ -1,103 +1,105 @@
--rw-r--r--   0        0        0    11357 2024-05-14 18:42:02.363846 ai21-2.2.5/LICENSE
--rw-r--r--   0        0        0    11868 2024-05-14 18:42:02.363846 ai21-2.2.5/README.md
--rw-r--r--   0        0        0     1575 2024-05-14 18:42:02.363846 ai21-2.2.5/ai21/__init__.py
--rw-r--r--   0        0        0     1014 2024-05-14 18:42:02.363846 ai21-2.2.5/ai21/ai21_env_config.py
--rw-r--r--   0        0        0     2626 2024-05-14 18:42:02.363846 ai21-2.2.5/ai21/ai21_http_client.py
--rw-r--r--   0        0        0        0 2024-05-14 18:42:02.363846 ai21-2.2.5/ai21/clients/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 18:42:02.363846 ai21-2.2.5/ai21/clients/bedrock/__init__.py
--rw-r--r--   0        0        0      844 2024-05-14 18:42:02.363846 ai21-2.2.5/ai21/clients/bedrock/ai21_bedrock_client.py
--rw-r--r--   0        0        0       92 2024-05-14 18:42:02.363846 ai21-2.2.5/ai21/clients/bedrock/bedrock_model_id.py
--rw-r--r--   0        0        0     2414 2024-05-14 18:42:02.363846 ai21-2.2.5/ai21/clients/bedrock/bedrock_session.py
--rw-r--r--   0        0        0        0 2024-05-14 18:42:02.363846 ai21-2.2.5/ai21/clients/bedrock/resources/__init__.py
--rw-r--r--   0        0        0     1996 2024-05-14 18:42:02.363846 ai21-2.2.5/ai21/clients/bedrock/resources/bedrock_completion.py
--rw-r--r--   0        0        0      522 2024-05-14 18:42:02.363846 ai21-2.2.5/ai21/clients/bedrock/resources/bedrock_resource.py
--rw-r--r--   0        0        0        0 2024-05-14 18:42:02.363846 ai21-2.2.5/ai21/clients/common/__init__.py
--rw-r--r--   0        0        0      857 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/common/answer_base.py
--rw-r--r--   0        0        0     3710 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/common/chat_base.py
--rw-r--r--   0        0        0     4216 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/common/completion_base.py
--rw-r--r--   0        0        0     1634 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/common/custom_model_base.py
--rw-r--r--   0        0        0     1886 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/common/dataset_base.py
--rw-r--r--   0        0        0      888 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/common/embed_base.py
--rw-r--r--   0        0        0      577 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/common/gec_base.py
--rw-r--r--   0        0        0      771 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/common/improvements_base.py
--rw-r--r--   0        0        0     1478 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/common/paraphrase_base.py
--rw-r--r--   0        0        0      806 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/common/segmentation_base.py
--rw-r--r--   0        0        0     1217 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/common/summarize_base.py
--rw-r--r--   0        0        0     1143 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/common/summarize_by_segment_base.py
--rw-r--r--   0        0        0        0 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/sagemaker/__init__.py
--rw-r--r--   0        0        0     1545 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/sagemaker/ai21_sagemaker_client.py
--rw-r--r--   0        0        0      154 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/sagemaker/constants.py
--rw-r--r--   0        0        0        0 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/sagemaker/resources/__init__.py
--rw-r--r--   0        0        0      498 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/sagemaker/resources/sagemaker_answer.py
--rw-r--r--   0        0        0     3194 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/sagemaker/resources/sagemaker_completion.py
--rw-r--r--   0        0        0      399 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/sagemaker/resources/sagemaker_gec.py
--rw-r--r--   0        0        0      789 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/sagemaker/resources/sagemaker_paraphrase.py
--rw-r--r--   0        0        0      484 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/sagemaker/resources/sagemaker_resource.py
--rw-r--r--   0        0        0      810 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/sagemaker/resources/sagemaker_summarize.py
--rw-r--r--   0        0        0     2522 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/sagemaker/sagemaker_session.py
--rw-r--r--   0        0        0        0 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/__init__.py
--rw-r--r--   0        0        0     3496 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/ai21_client.py
--rw-r--r--   0        0        0        0 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/__init__.py
--rw-r--r--   0        0        0      101 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/chat/__init__.py
--rw-r--r--   0        0        0     2435 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/chat/chat_completions.py
--rw-r--r--   0        0        0      574 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_answer.py
--rw-r--r--   0        0        0     2061 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_chat.py
--rw-r--r--   0        0        0     1996 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_completion.py
--rw-r--r--   0        0        0     1290 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_custom_model.py
--rw-r--r--   0        0        0     1507 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_dataset.py
--rw-r--r--   0        0        0      584 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_embed.py
--rw-r--r--   0        0        0      472 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_gec.py
--rw-r--r--   0        0        0      739 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_improvements.py
--rw-r--r--   0        0        0     3670 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_library.py
--rw-r--r--   0        0        0      873 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_paraphrase.py
--rw-r--r--   0        0        0     1096 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_resource.py
--rw-r--r--   0        0        0      612 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_segmentation.py
--rw-r--r--   0        0        0      891 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_summarize.py
--rw-r--r--   0        0        0      782 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_summarize_by_segment.py
--rw-r--r--   0        0        0       64 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/constants.py
--rw-r--r--   0        0        0     2615 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/errors.py
--rw-r--r--   0        0        0     4868 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/http_client.py
--rw-r--r--   0        0        0      484 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/logger.py
--rw-r--r--   0        0        0     2633 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/__init__.py
--rw-r--r--   0        0        0      262 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/ai21_base_model_mixin.py
--rw-r--r--   0        0        0      343 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/chat/__init__.py
--rw-r--r--   0        0        0      592 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/chat/chat_completion_response.py
--rw-r--r--   0        0        0      219 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/chat/chat_message.py
--rw-r--r--   0        0        0       97 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/chat/role_type.py
--rw-r--r--   0        0        0      233 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/chat_message.py
--rw-r--r--   0        0        0       89 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/document_type.py
--rw-r--r--   0        0        0       96 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/embed_type.py
--rw-r--r--   0        0        0      286 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/improvement_type.py
--rw-r--r--   0        0        0      410 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/logprobs.py
--rw-r--r--   0        0        0      168 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/paraphrase_style_type.py
--rw-r--r--   0        0        0      503 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/penalty.py
--rw-r--r--   0        0        0        0 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/__init__.py
--rw-r--r--   0        0        0      273 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/answer_response.py
--rw-r--r--   0        0        0      518 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/chat_response.py
--rw-r--r--   0        0        0      786 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/completion_response.py
--rw-r--r--   0        0        0      713 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/custom_model_response.py
--rw-r--r--   0        0        0      376 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/dataset_response.py
--rw-r--r--   0        0        0      300 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/embed_response.py
--rw-r--r--   0        0        0      550 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/file_response.py
--rw-r--r--   0        0        0      635 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/gec_response.py
--rw-r--r--   0        0        0      401 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/improvement_response.py
--rw-r--r--   0        0        0      469 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/library_answer_response.py
--rw-r--r--   0        0        0      450 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/library_search_response.py
--rw-r--r--   0        0        0      294 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/paraphrase_response.py
--rw-r--r--   0        0        0      317 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/segmentation_response.py
--rw-r--r--   0        0        0      564 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/summarize_by_segment_response.py
--rw-r--r--   0        0        0      187 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/summarize_response.py
--rw-r--r--   0        0        0      139 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/summary_method.py
--rw-r--r--   0        0        0      222 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/usage_info.py
--rw-r--r--   0        0        0        0 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/py.typed
--rw-r--r--   0        0        0        0 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/services/__init__.py
--rw-r--r--   0        0        0     2296 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/services/sagemaker.py
--rw-r--r--   0        0        0      123 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/tokenizers/__init__.py
--rw-r--r--   0        0        0      608 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/tokenizers/ai21_tokenizer.py
--rw-r--r--   0        0        0      628 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/tokenizers/factory.py
--rw-r--r--   0        0        0      722 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/types.py
--rw-r--r--   0        0        0        0 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/utils/__init__.py
--rw-r--r--   0        0        0      668 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/utils/typing.py
--rw-r--r--   0        0        0       18 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/version.py
--rw-r--r--   0        0        0     2269 2024-05-14 18:42:02.371846 ai21-2.2.5/pyproject.toml
--rw-r--r--   0        0        0    12580 1970-01-01 00:00:00.000000 ai21-2.2.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-20 11:35:42.419077 ai21-2.3.0/LICENSE
+-rw-r--r--   0        0        0    12340 2024-05-20 11:35:42.419077 ai21-2.3.0/README.md
+-rw-r--r--   0        0        0     1575 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/__init__.py
+-rw-r--r--   0        0        0     1014 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/ai21_env_config.py
+-rw-r--r--   0        0        0     2703 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/ai21_http_client.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/bedrock/__init__.py
+-rw-r--r--   0        0        0      844 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/bedrock/ai21_bedrock_client.py
+-rw-r--r--   0        0        0       92 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/bedrock/bedrock_model_id.py
+-rw-r--r--   0        0        0     2414 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/bedrock/bedrock_session.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/bedrock/resources/__init__.py
+-rw-r--r--   0        0        0     1996 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/bedrock/resources/bedrock_completion.py
+-rw-r--r--   0        0        0      522 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/bedrock/resources/bedrock_resource.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/common/__init__.py
+-rw-r--r--   0        0        0      857 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/common/answer_base.py
+-rw-r--r--   0        0        0     3594 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/common/chat_base.py
+-rw-r--r--   0        0        0     4081 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/common/completion_base.py
+-rw-r--r--   0        0        0     1496 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/common/custom_model_base.py
+-rw-r--r--   0        0        0     1723 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/common/dataset_base.py
+-rw-r--r--   0        0        0      770 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/common/embed_base.py
+-rw-r--r--   0        0        0      577 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/common/gec_base.py
+-rw-r--r--   0        0        0      639 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/common/improvements_base.py
+-rw-r--r--   0        0        0     1478 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/common/paraphrase_base.py
+-rw-r--r--   0        0        0      674 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/common/segmentation_base.py
+-rw-r--r--   0        0        0     1217 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/common/summarize_base.py
+-rw-r--r--   0        0        0      999 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/common/summarize_by_segment_base.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/sagemaker/__init__.py
+-rw-r--r--   0        0        0     1545 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/sagemaker/ai21_sagemaker_client.py
+-rw-r--r--   0        0        0      154 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/sagemaker/constants.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/sagemaker/resources/__init__.py
+-rw-r--r--   0        0        0      498 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/sagemaker/resources/sagemaker_answer.py
+-rw-r--r--   0        0        0     3194 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/sagemaker/resources/sagemaker_completion.py
+-rw-r--r--   0        0        0      399 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/sagemaker/resources/sagemaker_gec.py
+-rw-r--r--   0        0        0      789 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/sagemaker/resources/sagemaker_paraphrase.py
+-rw-r--r--   0        0        0      484 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/sagemaker/resources/sagemaker_resource.py
+-rw-r--r--   0        0        0      810 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/sagemaker/resources/sagemaker_summarize.py
+-rw-r--r--   0        0        0     2522 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/sagemaker/sagemaker_session.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/studio/__init__.py
+-rw-r--r--   0        0        0     3496 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/studio/ai21_client.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/studio/resources/__init__.py
+-rw-r--r--   0        0        0      101 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/studio/resources/chat/__init__.py
+-rw-r--r--   0        0        0     3647 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/studio/resources/chat/chat_completions.py
+-rw-r--r--   0        0        0      550 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/studio/resources/studio_answer.py
+-rw-r--r--   0        0        0     2036 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/studio/resources/studio_chat.py
+-rw-r--r--   0        0        0     2006 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/studio/resources/studio_completion.py
+-rw-r--r--   0        0        0     1301 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/clients/studio/resources/studio_custom_model.py
+-rw-r--r--   0        0        0     1455 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/clients/studio/resources/studio_dataset.py
+-rw-r--r--   0        0        0      560 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/clients/studio/resources/studio_embed.py
+-rw-r--r--   0        0        0      446 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/clients/studio/resources/studio_gec.py
+-rw-r--r--   0        0        0      722 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/clients/studio/resources/studio_improvements.py
+-rw-r--r--   0        0        0     4100 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/clients/studio/resources/studio_library.py
+-rw-r--r--   0        0        0      854 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/clients/studio/resources/studio_paraphrase.py
+-rw-r--r--   0        0        0     2808 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/clients/studio/resources/studio_resource.py
+-rw-r--r--   0        0        0      587 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/clients/studio/resources/studio_segmentation.py
+-rw-r--r--   0        0        0      871 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/clients/studio/resources/studio_summarize.py
+-rw-r--r--   0        0        0      772 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/clients/studio/resources/studio_summarize_by_segment.py
+-rw-r--r--   0        0        0       64 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/constants.py
+-rw-r--r--   0        0        0     2821 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/errors.py
+-rw-r--r--   0        0        0     5373 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/http_client.py
+-rw-r--r--   0        0        0      484 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/logger.py
+-rw-r--r--   0        0        0     2633 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/__init__.py
+-rw-r--r--   0        0        0      262 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/ai21_base_model_mixin.py
+-rw-r--r--   0        0        0      510 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/chat/__init__.py
+-rw-r--r--   0        0        0      651 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/chat/chat_completion_chunk.py
+-rw-r--r--   0        0        0      592 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/chat/chat_completion_response.py
+-rw-r--r--   0        0        0      219 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/chat/chat_message.py
+-rw-r--r--   0        0        0       97 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/chat/role_type.py
+-rw-r--r--   0        0        0      233 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/chat_message.py
+-rw-r--r--   0        0        0       89 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/document_type.py
+-rw-r--r--   0        0        0       96 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/embed_type.py
+-rw-r--r--   0        0        0      286 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/improvement_type.py
+-rw-r--r--   0        0        0      410 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/logprobs.py
+-rw-r--r--   0        0        0      168 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/paraphrase_style_type.py
+-rw-r--r--   0        0        0      503 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/penalty.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/__init__.py
+-rw-r--r--   0        0        0      273 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/answer_response.py
+-rw-r--r--   0        0        0      518 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/chat_response.py
+-rw-r--r--   0        0        0      786 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/completion_response.py
+-rw-r--r--   0        0        0      713 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/custom_model_response.py
+-rw-r--r--   0        0        0      376 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/dataset_response.py
+-rw-r--r--   0        0        0      300 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/embed_response.py
+-rw-r--r--   0        0        0      550 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/file_response.py
+-rw-r--r--   0        0        0      635 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/gec_response.py
+-rw-r--r--   0        0        0      401 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/improvement_response.py
+-rw-r--r--   0        0        0      469 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/library_answer_response.py
+-rw-r--r--   0        0        0      450 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/library_search_response.py
+-rw-r--r--   0        0        0      294 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/paraphrase_response.py
+-rw-r--r--   0        0        0      317 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/segmentation_response.py
+-rw-r--r--   0        0        0      564 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/summarize_by_segment_response.py
+-rw-r--r--   0        0        0      187 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/summarize_response.py
+-rw-r--r--   0        0        0      139 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/summary_method.py
+-rw-r--r--   0        0        0      222 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/usage_info.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/py.typed
+-rw-r--r--   0        0        0        0 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/services/__init__.py
+-rw-r--r--   0        0        0     2310 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/services/sagemaker.py
+-rw-r--r--   0        0        0     2105 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/stream.py
+-rw-r--r--   0        0        0      123 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/tokenizers/__init__.py
+-rw-r--r--   0        0        0      608 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/tokenizers/ai21_tokenizer.py
+-rw-r--r--   0        0        0      628 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/tokenizers/factory.py
+-rw-r--r--   0        0        0     1074 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/types.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/utils/__init__.py
+-rw-r--r--   0        0        0      989 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/utils/typing.py
+-rw-r--r--   0        0        0       18 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/version.py
+-rw-r--r--   0        0        0     2286 2024-05-20 11:35:42.427077 ai21-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0    13091 1970-01-01 00:00:00.000000 ai21-2.3.0/PKG-INFO
```

### Comparing `ai21-2.2.5/LICENSE` & `ai21-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ai21-2.2.5/README.md` & `ai21-2.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -208,14 +208,38 @@
 
 </details>
 
 For a more detailed example, see the completion [examples](examples/studio/completion.py).
 
 ---
 
+## Streaming
+
+We currently support streaming for the Chat Completions API in Jamba.
+
+```python
+from ai21 import AI21Client
+from ai21.models.chat import ChatMessage
+
+messages = [ChatMessage(content="What is the meaning of life?", role="user")]
+
+client = AI21Client()
+
+response = client.chat.completions.create(
+    messages=messages,
+    model="jamba-instruct-preview",
+    stream=True,
+)
+for chunk in response:
+    print(chunk.choices[0].delta.content, end="")
+
+```
+
+---
+
 ## TSMs
 
 AI21 Studio's Task-Specific Models offer a range of powerful tools. These models have been specifically designed for their respective tasks and provide high-quality results while optimizing efficiency.
 The full documentation and guides can be found [here](https://docs.ai21.com/docs/task-specific).
 
 ### Contextual Answers
```

#### html2text {}

```diff
@@ -61,41 +61,47 @@
 having trouble signing up for your product with my Google account.",
 role=RoleType.USER), ] client = AI21Client() chat_response = client.chat.create
 ( system=system, messages=messages, model="j2-ultra", ) ``` For a more detailed
 example, see the chat [examples](examples/studio/chat.py). ### Completion
 ```python from ai21 import AI21Client client = AI21Client() completion_response
 = client.completion.create( prompt="This is a test prompt", model="j2-mid", )
 ``` For a more detailed example, see the completion [examples](examples/studio/
-completion.py). --- ## TSMs AI21 Studio's Task-Specific Models offer a range of
-powerful tools. These models have been specifically designed for their
-respective tasks and provide high-quality results while optimizing efficiency.
-The full documentation and guides can be found [here](https://docs.ai21.com/
-docs/task-specific). ### Contextual Answers The `answer` API allows you to
-access our high-quality question answering model. ```python from ai21 import
-AI21Client client = AI21Client() response = client.answer.create( context="This
-is a text is for testing purposes", question="Question about context", ) ``` A
-detailed explanation on Contextual Answers, can be found [here](https://
-docs.ai21.com/docs/contextual-answers-api) ### Token Counting --- By using the
-`count_tokens` method, you can estimate the billing for a given request.
-```python from ai21.tokenizers import get_tokenizer tokenizer = get_tokenizer
-(name="jamba-instruct-tokenizer") total_tokens = tokenizer.count_tokens
-(text="some text") # returns int print(total_tokens) ``` Available tokenizers
-are: - `jamba-instruct-tokenizer` - `j2-tokenizer` For more information on AI21
-Tokenizers, see the [documentation](https://github.com/AI21Labs/ai21-
-tokenizer). ### File Upload --- ```python from ai21 import AI21Client client =
-AI21Client() file_id = client.library.files.create( file_path="path/to/file",
-path="path/to/file/in/library", labels=["label1", "label2"],
-public_url="www.example.com", ) uploaded_file = client.library.files.get
-(file_id) ``` ## Environment Variables --- You can set several environment
-variables to configure the client. ### Logging We use the standard library
-[`logging`](https://docs.python.org/3/library/logging.html) module. To enable
-logging, set the `AI21_LOG_LEVEL` environment variable. ```bash $ export
-AI21_LOG_LEVEL=debug ``` ### Other Important Environment Variables -
-`AI21_API_KEY` - Your API key. If not set, you must pass it to the client
-constructor. - `AI21_API_VERSION` - The API version. Defaults to `v1`. -
+completion.py). --- ## Streaming We currently support streaming for the Chat
+Completions API in Jamba. ```python from ai21 import AI21Client from
+ai21.models.chat import ChatMessage messages = [ChatMessage(content="What is
+the meaning of life?", role="user")] client = AI21Client() response =
+client.chat.completions.create( messages=messages, model="jamba-instruct-
+preview", stream=True, ) for chunk in response: print(chunk.choices
+[0].delta.content, end="") ``` --- ## TSMs AI21 Studio's Task-Specific Models
+offer a range of powerful tools. These models have been specifically designed
+for their respective tasks and provide high-quality results while optimizing
+efficiency. The full documentation and guides can be found [here](https://
+docs.ai21.com/docs/task-specific). ### Contextual Answers The `answer` API
+allows you to access our high-quality question answering model. ```python from
+ai21 import AI21Client client = AI21Client() response = client.answer.create
+( context="This is a text is for testing purposes", question="Question about
+context", ) ``` A detailed explanation on Contextual Answers, can be found
+[here](https://docs.ai21.com/docs/contextual-answers-api) ### Token Counting --
+- By using the `count_tokens` method, you can estimate the billing for a given
+request. ```python from ai21.tokenizers import get_tokenizer tokenizer =
+get_tokenizer(name="jamba-instruct-tokenizer") total_tokens =
+tokenizer.count_tokens(text="some text") # returns int print(total_tokens) ```
+Available tokenizers are: - `jamba-instruct-tokenizer` - `j2-tokenizer` For
+more information on AI21 Tokenizers, see the [documentation](https://
+github.com/AI21Labs/ai21-tokenizer). ### File Upload --- ```python from ai21
+import AI21Client client = AI21Client() file_id = client.library.files.create
+( file_path="path/to/file", path="path/to/file/in/library", labels=["label1",
+"label2"], public_url="www.example.com", ) uploaded_file =
+client.library.files.get(file_id) ``` ## Environment Variables --- You can set
+several environment variables to configure the client. ### Logging We use the
+standard library [`logging`](https://docs.python.org/3/library/logging.html)
+module. To enable logging, set the `AI21_LOG_LEVEL` environment variable.
+```bash $ export AI21_LOG_LEVEL=debug ``` ### Other Important Environment
+Variables - `AI21_API_KEY` - Your API key. If not set, you must pass it to the
+client constructor. - `AI21_API_VERSION` - The API version. Defaults to `v1`. -
 `AI21_API_HOST` - The API host. Defaults to `https://api.ai21.com/v1/`. -
 `AI21_TIMEOUT_SEC` - The timeout for API requests. - `AI21_NUM_RETRIES` - The
 maximum number of retries for API requests. Defaults to `3` retries. -
 `AI21_AWS_REGION` - The AWS region to use for AWS clients. Defaults to `us-
 east-1`. ## Error Handling --- ```python from ai21 import errors as ai21_errors
 from ai21 import AI21Client, AI21APIError from ai21.models import ChatMessage
 client = AI21Client() system = "You're a support engineer in a SaaS company"
```

### Comparing `ai21-2.2.5/ai21/__init__.py` & `ai21-2.3.0/ai21/__init__.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.5/ai21/ai21_env_config.py` & `ai21-2.3.0/ai21/ai21_env_config.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.5/ai21/ai21_http_client.py` & `ai21-2.3.0/ai21/ai21_http_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import platform
 from typing import Optional, Dict, Any, BinaryIO
 
+import httpx
+
 from ai21.errors import MissingApiKeyError
 from ai21.http_client import HttpClient
 from ai21.version import VERSION
 
 
 class AI21HTTPClient:
     def __init__(
@@ -72,13 +74,14 @@
         return user_agent
 
     def execute_http_request(
         self,
         method: str,
         url: str,
         params: Optional[Dict] = None,
+        stream: bool = False,
         files: Optional[Dict[str, BinaryIO]] = None,
-    ):
-        return self._http_client.execute_http_request(method=method, url=url, params=params, files=files)
+    ) -> httpx.Response:
+        return self._http_client.execute_http_request(method=method, url=url, params=params, files=files, stream=stream)
 
     def get_base_url(self) -> str:
         return f"{self._api_host}/studio/{self._api_version}"
```

### Comparing `ai21-2.2.5/ai21/clients/bedrock/ai21_bedrock_client.py` & `ai21-2.3.0/ai21/clients/bedrock/ai21_bedrock_client.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.5/ai21/clients/bedrock/bedrock_session.py` & `ai21-2.3.0/ai21/clients/bedrock/bedrock_session.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.5/ai21/clients/bedrock/resources/bedrock_completion.py` & `ai21-2.3.0/ai21/clients/bedrock/resources/bedrock_completion.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.5/ai21/clients/bedrock/resources/bedrock_resource.py` & `ai21-2.3.0/ai21/clients/bedrock/resources/bedrock_resource.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.5/ai21/clients/common/answer_base.py` & `ai21-2.3.0/ai21/clients/common/answer_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.5/ai21/clients/common/chat_base.py` & `ai21-2.3.0/ai21/clients/common/chat_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,17 +49,14 @@
         pass
 
     @property
     @abstractmethod
     def completions(self) -> ChatCompletions:
         pass
 
-    def _json_to_response(self, json: Dict[str, Any]) -> ChatResponse:
-        return ChatResponse.from_dict(json)
-
     def _create_body(
         self,
         model: str,
         messages: List[ChatMessage],
         system: str,
         num_results: Optional[int] = 1,
         temperature: Optional[float] = 0.7,
```

### Comparing `ai21-2.2.5/ai21/clients/common/completion_base.py` & `ai21-2.3.0/ai21/clients/common/completion_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import List, Dict, Any
+from typing import List, Dict
 
 from ai21.models import Penalty, CompletionsResponse
 from ai21.types import NOT_GIVEN, NotGiven
 from ai21.utils.typing import remove_not_given
 
 
 class Completion(ABC):
@@ -51,17 +51,14 @@
         representations of the tokens and the floats are the biases themselves. A positive bias increases generation
         probability for a given token and a negative bias decreases it.
         :param kwargs:
         :return:
         """
         pass
 
-    def _json_to_response(self, json: Dict[str, Any]) -> CompletionsResponse:
-        return CompletionsResponse.from_dict(json)
-
     def _create_body(
         self,
         model: str,
         prompt: str,
         max_tokens: int | NotGiven,
         num_results: int | NotGiven,
         min_tokens: int | NotGiven,
```

### Comparing `ai21-2.2.5/ai21/clients/common/custom_model_base.py` & `ai21-2.3.0/ai21/clients/common/custom_model_base.py`

 * *Files 19% similar despite different names*

```diff
@@ -34,17 +34,14 @@
     def list(self) -> List[CustomBaseModelResponse]:
         pass
 
     @abstractmethod
     def get(self, resource_id: str) -> CustomBaseModelResponse:
         pass
 
-    def _json_to_response(self, json: Dict[str, Any]) -> CustomBaseModelResponse:
-        return CustomBaseModelResponse.from_dict(json)
-
     def _create_body(
         self,
         dataset_id: str,
         model_name: str,
         model_type: str,
         learning_rate: Optional[float],
         num_epochs: Optional[int],
```

### Comparing `ai21-2.2.5/ai21/clients/common/dataset_base.py` & `ai21-2.3.0/ai21/clients/common/dataset_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from abc import ABC, abstractmethod
 from typing import Optional, Any, Dict
 
-from ai21.models import DatasetResponse
-
 
 class Dataset(ABC):
     _module_name = "dataset"
 
     @abstractmethod
     def create(
         self,
@@ -36,17 +34,14 @@
     def list(self):
         pass
 
     @abstractmethod
     def get(self, dataset_pid: str):
         pass
 
-    def _json_to_response(self, json: Dict[str, Any]) -> DatasetResponse:
-        return DatasetResponse.from_dict(json)
-
     def _create_body(
         self,
         dataset_name: str,
         selected_columns: Optional[str],
         approve_whitespace_correction: Optional[bool],
         delete_long_rows: Optional[bool],
         split_ratio: Optional[float],
```

### Comparing `ai21-2.2.5/ai21/clients/common/embed_base.py` & `ai21-2.3.0/ai21/clients/common/embed_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,12 +15,9 @@
         :param type: For retrieval/search use cases, indicates whether the texts that were
          sent are segments or the query.
         :param kwargs:
         :return:
         """
         pass
 
-    def _json_to_response(self, json: Dict[str, Any]) -> EmbedResponse:
-        return EmbedResponse.from_dict(json)
-
     def _create_body(self, texts: List[str], type: Optional[str], **kwargs) -> Dict[str, Any]:
         return {"texts": texts, "type": type, **kwargs}
```

### Comparing `ai21-2.2.5/ai21/clients/common/gec_base.py` & `ai21-2.3.0/ai21/clients/common/gec_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.5/ai21/clients/common/improvements_base.py` & `ai21-2.3.0/ai21/clients/common/improvements_base.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,12 +14,9 @@
         :param text: The input text to be improved.
         :param types: Types of improvements to apply.
         :param kwargs:
         :return:
         """
         pass
 
-    def _json_to_response(self, json: Dict[str, Any]) -> ImprovementsResponse:
-        return ImprovementsResponse.from_dict(json)
-
     def _create_body(self, text: str, types: List[str], **kwargs) -> Dict[str, Any]:
         return {"text": text, "types": types, **kwargs}
```

### Comparing `ai21-2.2.5/ai21/clients/common/paraphrase_base.py` & `ai21-2.3.0/ai21/clients/common/paraphrase_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.5/ai21/clients/common/segmentation_base.py` & `ai21-2.3.0/ai21/clients/common/segmentation_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,12 +14,9 @@
         :param source: Raw input text, or URL of a web page.
         :param source_type: The type of the source - either TEXT or URL.
         :param kwargs:
         :return:
         """
         pass
 
-    def _json_to_response(self, json: Dict[str, Any]) -> SegmentationResponse:
-        return SegmentationResponse.from_dict(json)
-
     def _create_body(self, source: str, source_type: str, **kwargs) -> Dict[str, Any]:
         return {"source": source, "sourceType": source_type, **kwargs}
```

### Comparing `ai21-2.2.5/ai21/clients/common/summarize_base.py` & `ai21-2.3.0/ai21/clients/common/summarize_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.5/ai21/clients/common/summarize_by_segment_base.py` & `ai21-2.3.0/ai21/clients/common/summarize_by_segment_base.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,17 +22,14 @@
         :param source_type: Either TEXT or URL
         :param focus: Summaries focused on a topic of your choice.
         :param kwargs:
         :return:
         """
         pass
 
-    def _json_to_response(self, json: Dict[str, Any]) -> SummarizeBySegmentResponse:
-        return SummarizeBySegmentResponse.from_dict(json)
-
     def _create_body(
         self,
         source: str,
         source_type: str,
         focus: Optional[str],
         **kwargs,
     ) -> Dict[str, Any]:
```

### Comparing `ai21-2.2.5/ai21/clients/sagemaker/ai21_sagemaker_client.py` & `ai21-2.3.0/ai21/clients/sagemaker/ai21_sagemaker_client.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.5/ai21/clients/sagemaker/resources/sagemaker_completion.py` & `ai21-2.3.0/ai21/clients/sagemaker/resources/sagemaker_completion.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.5/ai21/clients/sagemaker/resources/sagemaker_paraphrase.py` & `ai21-2.3.0/ai21/clients/sagemaker/resources/sagemaker_paraphrase.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.5/ai21/clients/sagemaker/resources/sagemaker_summarize.py` & `ai21-2.3.0/ai21/clients/sagemaker/resources/sagemaker_summarize.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.5/ai21/clients/sagemaker/sagemaker_session.py` & `ai21-2.3.0/ai21/clients/sagemaker/sagemaker_session.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.5/ai21/clients/studio/ai21_client.py` & `ai21-2.3.0/ai21/clients/studio/ai21_client.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.5/ai21/clients/studio/resources/chat/chat_completions.py` & `ai21-2.3.0/ai21/clients/studio/resources/studio_chat.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,74 +1,56 @@
-from __future__ import annotations
-
-from typing import List, Optional, Union, Any, Dict
+from typing import List, Optional
 
+from ai21.clients.common.chat_base import Chat
+from ai21.clients.studio.resources.chat import ChatCompletions
+from ai21.models.chat import ChatMessage as JambaChatMessage
 from ai21.clients.studio.resources.studio_resource import StudioResource
-from ai21.models.chat import ChatMessage, ChatCompletionResponse
-from ai21.models import ChatMessage as J2ChatMessage
-from ai21.types import NotGiven, NOT_GIVEN
-from ai21.utils.typing import remove_not_given
-
-__all__ = ["ChatCompletions"]
-
+from ai21.models import ChatMessage, Penalty, ChatResponse
 
-class ChatCompletions(StudioResource):
-    _module_name = "chat/completions"
 
+class StudioChat(StudioResource, Chat):
     def create(
         self,
         model: str,
         messages: List[ChatMessage],
-        max_tokens: int | NotGiven = NOT_GIVEN,
-        temperature: float | NotGiven = NOT_GIVEN,
-        top_p: float | NotGiven = NOT_GIVEN,
-        stop: str | List[str] | NotGiven = NOT_GIVEN,
-        n: int | NotGiven = NOT_GIVEN,
-        **kwargs: Any,
-    ) -> ChatCompletionResponse:
-        if any(isinstance(item, J2ChatMessage) for item in messages):
+        system: str,
+        *,
+        num_results: Optional[int] = 1,
+        temperature: Optional[float] = 0.7,
+        max_tokens: Optional[int] = 300,
+        min_tokens: Optional[int] = 0,
+        top_p: Optional[float] = 1.0,
+        top_k_return: Optional[int] = 0,
+        stop_sequences: Optional[List[str]] = None,
+        frequency_penalty: Optional[Penalty] = None,
+        presence_penalty: Optional[Penalty] = None,
+        count_penalty: Optional[Penalty] = None,
+        **kwargs,
+    ) -> ChatResponse:
+        if any(isinstance(item, JambaChatMessage) for item in messages):
             raise ValueError(
-                "Please use the ChatMessage class from ai21.models.chat"
-                " instead of ai21.models when working with chat completions."
+                "Please use the ChatMessage class from ai21.models"
+                " instead of ai21.models.chat when working with chat"
             )
 
         body = self._create_body(
             model=model,
             messages=messages,
-            stop=stop,
+            system=system,
+            num_results=num_results,
             temperature=temperature,
             max_tokens=max_tokens,
+            min_tokens=min_tokens,
             top_p=top_p,
-            n=n,
+            top_k_return=top_k_return,
+            stop_sequences=stop_sequences,
+            frequency_penalty=frequency_penalty,
+            presence_penalty=presence_penalty,
+            count_penalty=count_penalty,
             **kwargs,
         )
+        url = f"{self._client.get_base_url()}/{model}/{self._module_name}"
+        return self._post(url=url, body=body, response_cls=ChatResponse)
 
-        url = f"{self._client.get_base_url()}/{self._module_name}"
-        response = self._post(url=url, body=body)
-        return self._json_to_response(response)
-
-    def _create_body(
-        self,
-        model: str,
-        messages: List[ChatMessage],
-        max_tokens: Optional[int] | NotGiven,
-        temperature: Optional[float] | NotGiven,
-        top_p: Optional[float] | NotGiven,
-        stop: Optional[Union[str, List[str]]] | NotGiven,
-        n: Optional[int] | NotGiven,
-        **kwargs: Any,
-    ) -> Dict[str, Any]:
-        return remove_not_given(
-            {
-                "model": model,
-                "messages": [message.to_dict() for message in messages],
-                "temperature": temperature,
-                "maxTokens": max_tokens,
-                "topP": top_p,
-                "stop": stop,
-                "n": n,
-                **kwargs,
-            }
-        )
-
-    def _json_to_response(self, json: Dict[str, Any]) -> ChatCompletionResponse:
-        return ChatCompletionResponse.from_dict(json)
+    @property
+    def completions(self) -> ChatCompletions:
+        return ChatCompletions(self._client)
```

### Comparing `ai21-2.2.5/ai21/clients/studio/resources/studio_answer.py` & `ai21-2.3.0/ai21/clients/studio/resources/studio_improvements.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-from ai21.clients.common.answer_base import Answer
-from ai21.clients.studio.resources.studio_resource import StudioResource
-from ai21.models import AnswerResponse
+from typing import List
 
+from ai21.clients.common.improvements_base import Improvements
+from ai21.clients.studio.resources.studio_resource import StudioResource
+from ai21.errors import EmptyMandatoryListError
+from ai21.models import ImprovementType, ImprovementsResponse
 
-class StudioAnswer(StudioResource, Answer):
-    def create(
-        self,
-        context: str,
-        question: str,
-        **kwargs,
-    ) -> AnswerResponse:
-        url = f"{self._client.get_base_url()}/{self._module_name}"
 
-        body = self._create_body(context=context, question=question, **kwargs)
+class StudioImprovements(StudioResource, Improvements):
+    def create(self, text: str, types: List[ImprovementType], **kwargs) -> ImprovementsResponse:
+        if len(types) == 0:
+            raise EmptyMandatoryListError("types")
 
-        response = self._post(url=url, body=body)
+        url = f"{self._client.get_base_url()}/{self._module_name}"
+        body = self._create_body(text=text, types=types, **kwargs)
 
-        return self._json_to_response(response)
+        return self._post(url=url, body=body, response_cls=ImprovementsResponse)
```

### Comparing `ai21-2.2.5/ai21/clients/studio/resources/studio_completion.py` & `ai21-2.3.0/ai21/clients/studio/resources/studio_completion.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,8 +49,8 @@
             frequency_penalty=frequency_penalty,
             presence_penalty=presence_penalty,
             count_penalty=count_penalty,
             epoch=epoch,
             logit_bias=logit_bias,
             **kwargs,
         )
-        return self._json_to_response(self._post(url=url, body=body))
+        return self._post(url=url, body=body, response_cls=CompletionsResponse)
```

### Comparing `ai21-2.2.5/ai21/clients/studio/resources/studio_custom_model.py` & `ai21-2.3.0/ai21/clients/studio/resources/studio_custom_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,18 +21,16 @@
             dataset_id=dataset_id,
             model_name=model_name,
             model_type=model_type,
             learning_rate=learning_rate,
             num_epochs=num_epochs,
             **kwargs,
         )
-        self._post(url=url, body=body)
+        self._post(url=url, body=body, response_cls=None)
 
     def list(self) -> List[CustomBaseModelResponse]:
         url = f"{self._client.get_base_url()}/{self._module_name}"
-        response = self._get(url=url)
-
-        return [self._json_to_response(r) for r in response]
+        return self._get(url=url, response_cls=List[CustomBaseModelResponse])
 
     def get(self, resource_id: str) -> CustomBaseModelResponse:
         url = f"{self._client.get_base_url()}/{self._module_name}/{resource_id}"
-        return self._json_to_response(self._get(url=url))
+        return self._get(url=url, response_cls=CustomBaseModelResponse)
```

### Comparing `ai21-2.2.5/ai21/clients/studio/resources/studio_dataset.py` & `ai21-2.3.0/ai21/clients/studio/resources/studio_dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,18 +29,15 @@
         return self._post(
             url=self._base_url(),
             body=body,
             files=files,
         )
 
     def list(self) -> List[DatasetResponse]:
-        response = self._get(url=self._base_url())
-        return [self._json_to_response(r) for r in response]
+        return self._get(url=self._base_url(), response_cls=List[DatasetResponse])
 
     def get(self, dataset_pid: str) -> DatasetResponse:
         url = f"{self._base_url()}/{dataset_pid}"
-        response = self._get(url=url)
-
-        return self._json_to_response(response)
+        return self._get(url=url, response_cls=DatasetResponse)
 
     def _base_url(self) -> str:
         return f"{self._client.get_base_url()}/{self._module_name}"
```

### Comparing `ai21-2.2.5/ai21/clients/studio/resources/studio_embed.py` & `ai21-2.3.0/ai21/clients/studio/resources/studio_embed.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,10 +5,9 @@
 from ai21.models import EmbedType, EmbedResponse
 
 
 class StudioEmbed(StudioResource, Embed):
     def create(self, texts: List[str], type: Optional[EmbedType] = None, **kwargs) -> EmbedResponse:
         url = f"{self._client.get_base_url()}/{self._module_name}"
         body = self._create_body(texts=texts, type=type, **kwargs)
-        response = self._post(url=url, body=body)
 
-        return self._json_to_response(response)
+        return self._post(url=url, body=body, response_cls=EmbedResponse)
```

### Comparing `ai21-2.2.5/ai21/clients/studio/resources/studio_library.py` & `ai21-2.3.0/ai21/clients/studio/resources/studio_library.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+from __future__ import annotations
 from typing import Optional, List
 
+
 from ai21.ai21_http_client import AI21HTTPClient
 from ai21.clients.studio.resources.studio_resource import StudioResource
 from ai21.models import FileResponse, LibraryAnswerResponse, LibrarySearchResponse
+from ai21.types import NotGiven, NOT_GIVEN
+from ai21.utils.typing import remove_not_given
 
 
 class StudioLibrary(StudioResource):
     _module_name = "library/files"
 
     def __init__(self, client: AI21HTTPClient):
         super().__init__(client)
@@ -18,106 +22,110 @@
 class LibraryFiles(StudioResource):
     _module_name = "library/files"
 
     def create(
         self,
         file_path: str,
         *,
-        path: Optional[str] = None,
-        labels: Optional[List[str]] = None,
-        public_url: Optional[str] = None,
+        path: Optional[str] | NotGiven = NOT_GIVEN,
+        labels: Optional[List[str]] | NotGiven = NOT_GIVEN,
+        public_url: Optional[str] | NotGiven = NOT_GIVEN,
         **kwargs,
     ) -> str:
         url = f"{self._client.get_base_url()}/{self._module_name}"
         files = {"file": open(file_path, "rb")}
-        body = {"path": path, "labels": labels, "publicUrl": public_url, **kwargs}
+        body = remove_not_given({"path": path, "labels": labels, "publicUrl": public_url, **kwargs})
 
-        raw_response = self._post(url=url, files=files, body=body)
+        raw_response = self._post(url=url, files=files, body=body, response_cls=dict)
 
         return raw_response["fileId"]
 
     def get(self, file_id: str) -> FileResponse:
         url = f"{self._client.get_base_url()}/{self._module_name}/{file_id}"
-        raw_response = self._get(url=url)
 
-        return FileResponse.from_dict(raw_response)
+        return self._get(url=url, response_cls=FileResponse)
 
     def list(
         self,
         *,
-        offset: Optional[int] = None,
-        limit: Optional[int] = None,
+        offset: Optional[int] | NotGiven = NOT_GIVEN,
+        limit: Optional[int] | NotGiven = NOT_GIVEN,
         **kwargs,
     ) -> List[FileResponse]:
         url = f"{self._client.get_base_url()}/{self._module_name}"
-        params = {"offset": offset, "limit": limit}
-        raw_response = self._get(url=url, params=params)
+        params = remove_not_given({"offset": offset, "limit": limit})
 
-        return [FileResponse.from_dict(file) for file in raw_response]
+        return self._get(url=url, params=params, response_cls=List[FileResponse])
 
     def update(
         self,
         file_id: str,
         *,
-        public_url: Optional[str] = None,
-        labels: Optional[List[str]] = None,
+        public_url: Optional[str] | NotGiven = NOT_GIVEN,
+        labels: Optional[List[str]] | NotGiven = NOT_GIVEN,
         **kwargs,
     ) -> None:
         url = f"{self._client.get_base_url()}/{self._module_name}/{file_id}"
-        body = {
-            "publicUrl": public_url,
-            "labels": labels,
-            **kwargs,
-        }
+        body = remove_not_given(
+            {
+                "publicUrl": public_url,
+                "labels": labels,
+                **kwargs,
+            }
+        )
         self._put(url=url, body=body)
 
     def delete(self, file_id: str) -> None:
         url = f"{self._client.get_base_url()}/{self._module_name}/{file_id}"
         self._delete(url=url)
 
 
 class LibrarySearch(StudioResource):
     _module_name = "library/search"
 
     def create(
         self,
         query: str,
         *,
-        path: Optional[str] = None,
-        field_ids: Optional[List[str]] = None,
-        max_segments: Optional[int] = None,
+        path: Optional[str] | NotGiven = NOT_GIVEN,
+        field_ids: Optional[List[str]] | NotGiven = NOT_GIVEN,
+        max_segments: Optional[int] | NotGiven = NOT_GIVEN,
         **kwargs,
     ) -> LibrarySearchResponse:
         url = f"{self._client.get_base_url()}/{self._module_name}"
-        body = {
-            "query": query,
-            "path": path,
-            "fieldIds": field_ids,
-            "maxSegments": max_segments,
-            **kwargs,
-        }
-        raw_response = self._post(url=url, body=body)
-        return LibrarySearchResponse.from_dict(raw_response)
+        body = remove_not_given(
+            {
+                "query": query,
+                "path": path,
+                "fieldIds": field_ids,
+                "maxSegments": max_segments,
+                **kwargs,
+            }
+        )
+
+        return self._post(url=url, body=body, response_cls=LibrarySearchResponse)
 
 
 class LibraryAnswer(StudioResource):
     _module_name = "library/answer"
 
     def create(
         self,
         question: str,
         *,
-        path: Optional[str] = None,
-        field_ids: Optional[List[str]] = None,
-        labels: Optional[List[str]] = None,
+        path: Optional[str] | NotGiven = NOT_GIVEN,
+        field_ids: Optional[List[str]] | NotGiven = NOT_GIVEN,
+        labels: Optional[List[str]] | NotGiven = NOT_GIVEN,
         **kwargs,
     ) -> LibraryAnswerResponse:
         url = f"{self._client.get_base_url()}/{self._module_name}"
-        body = {
-            "question": question,
-            "path": path,
-            "fieldIds": field_ids,
-            "labels": labels,
-            **kwargs,
-        }
-        raw_response = self._post(url=url, body=body)
-        return LibraryAnswerResponse.from_dict(raw_response)
+        body = remove_not_given(
+            {
+                "question": question,
+                "path": path,
+                "fieldIds": field_ids,
+                "labels": labels,
+                **kwargs,
+            }
+        )
+
+        return self._post(url=url, body=body, response_cls=LibraryAnswerResponse)
```

### Comparing `ai21-2.2.5/ai21/clients/studio/resources/studio_paraphrase.py` & `ai21-2.3.0/ai21/clients/studio/resources/studio_paraphrase.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,10 +19,9 @@
             text=text,
             style=style,
             start_index=start_index,
             end_index=end_index,
             **kwargs,
         )
         url = f"{self._client.get_base_url()}/{self._module_name}"
-        response = self._post(url=url, body=body)
 
-        return self._json_to_response(response)
+        return self._post(url=url, body=body, response_cls=ParaphraseResponse)
```

### Comparing `ai21-2.2.5/ai21/clients/studio/resources/studio_segmentation.py` & `ai21-2.3.0/ai21/clients/studio/resources/studio_segmentation.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,10 +3,9 @@
 from ai21.models import DocumentType, SegmentationResponse
 
 
 class StudioSegmentation(StudioResource, Segmentation):
     def create(self, source: str, source_type: DocumentType, **kwargs) -> SegmentationResponse:
         body = self._create_body(source=source, source_type=source_type.value, **kwargs)
         url = f"{self._client.get_base_url()}/{self._module_name}"
-        raw_response = self._post(url=url, body=body)
 
-        return self._json_to_response(raw_response)
+        return self._post(url=url, body=body, response_cls=SegmentationResponse)
```

### Comparing `ai21-2.2.5/ai21/clients/studio/resources/studio_summarize.py` & `ai21-2.3.0/ai21/clients/studio/resources/studio_summarize.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,10 +21,9 @@
             source=source,
             source_type=source_type,
             focus=focus,
             summary_method=summary_method,
             **kwargs,
         )
         url = f"{self._client.get_base_url()}/{self._module_name}"
-        response = self._post(url=url, body=body)
 
-        return self._json_to_response(response)
+        return self._post(url=url, body=body, response_cls=SummarizeResponse)
```

### Comparing `ai21-2.2.5/ai21/errors.py` & `ai21-2.3.0/ai21/errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -83,7 +83,13 @@
         self.message = message
 
 
 class EmptyMandatoryListError(AI21Error):
     def __init__(self, key: str):
         message = f"Supplied {key} is empty. At least one element should be present in the list"
         super().__init__(message)
+
+
+class StreamingDecodeError(AI21Error):
+    def __init__(self, chunk: str):
+        message = f"Failed to decode chunk: {chunk} in stream. Please check the stream format"
+        super().__init__(message)
```

### Comparing `ai21-2.2.5/ai21/http_client.py` & `ai21-2.3.0/ai21/http_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 from typing import Optional, Dict, Any, BinaryIO
 
-import requests
-from requests.adapters import HTTPAdapter, Retry, RetryError
+import httpx
+from httpx import ConnectError
+from tenacity import retry, retry_if_result, stop_after_attempt, wait_exponential, RetryError
 
 from ai21.errors import (
     BadRequest,
     Unauthorized,
     UnprocessableEntity,
     TooManyRequestsError,
     AI21ServerError,
@@ -14,15 +15,15 @@
     AI21APIError,
 )
 from ai21.logger import logger
 
 DEFAULT_TIMEOUT_SEC = 300
 DEFAULT_NUM_RETRIES = 0
 RETRY_BACK_OFF_FACTOR = 0.5
-TIME_BETWEEN_RETRIES = 1000
+TIME_BETWEEN_RETRIES = 1
 RETRY_ERROR_CODES = (408, 429, 500, 503)
 RETRY_METHOD_WHITELIST = ["GET", "POST", "PUT"]
 
 
 def handle_non_success_response(status_code: int, response_text: str):
     if status_code == 400:
         raise BadRequest(details=response_text)
@@ -35,106 +36,120 @@
     if status_code == 500:
         raise AI21ServerError(details=response_text)
     if status_code == 503:
         raise ServiceUnavailable(details=response_text)
     raise AI21APIError(status_code, details=response_text)
 
 
-def requests_retry_session(session, retries=0):
-    retry = Retry(
-        total=retries,
-        read=retries,
-        connect=retries,
-        backoff_factor=RETRY_BACK_OFF_FACTOR,
-        status_forcelist=RETRY_ERROR_CODES,
-        allowed_methods=frozenset(RETRY_METHOD_WHITELIST),
+def _requests_retry_session(retries: int) -> httpx.HTTPTransport:
+    return httpx.HTTPTransport(
+        retries=retries,
     )
-    adapter = HTTPAdapter(max_retries=retry)
-    session.mount("https://", adapter)
-    session.mount("http://", adapter)
-    return session
 
 
 class HttpClient:
     def __init__(
         self,
-        session: Optional[requests.Session] = None,
+        client: Optional[httpx.Client] = None,
         timeout_sec: int = None,
         num_retries: int = None,
         headers: Dict = None,
     ):
         self._timeout_sec = timeout_sec or DEFAULT_TIMEOUT_SEC
         self._num_retries = num_retries or DEFAULT_NUM_RETRIES
         self._headers = headers or {}
         self._apply_retry_policy = self._num_retries > 0
-        self._session = self._init_session(session)
+        self._client = self._init_client(client)
+
+        # Since we can't use the retry decorator on a method of a class as we can't access class attributes,
+        # we have to wrap the method in a function
+        self._request = retry(
+            wait=wait_exponential(multiplier=RETRY_BACK_OFF_FACTOR, min=TIME_BETWEEN_RETRIES),
+            retry=retry_if_result(self._should_retry),
+            stop=stop_after_attempt(self._num_retries),
+        )(self._request)
+
+    def _should_retry(self, response: httpx.Response) -> bool:
+        return response.status_code in RETRY_ERROR_CODES and response.request.method in RETRY_METHOD_WHITELIST
 
     def execute_http_request(
         self,
         method: str,
         url: str,
         params: Optional[Dict] = None,
+        stream: bool = False,
         files: Optional[Dict[str, BinaryIO]] = None,
-    ):
-        timeout = self._timeout_sec
-        headers = self._headers
-        data = json.dumps(params).encode()
-        logger.debug(f"Calling {method} {url} {headers} {data}")
-
+    ) -> httpx.Response:
         try:
-            if method == "GET":
-                response = self._session.request(
-                    method=method,
-                    url=url,
-                    headers=headers,
-                    timeout=timeout,
-                    params=params,
-                )
-            elif files is not None:
-                if method != "POST":
-                    raise ValueError(
-                        f"execute_http_request supports only POST for files upload, but {method} was supplied instead"
-                    )
-                if "Content-Type" in headers:
-                    headers.pop(
-                        "Content-Type"
-                    )  # multipart/form-data 'Content-Type' is being added when passing rb files and payload
-                response = self._session.request(
-                    method=method,
-                    url=url,
-                    headers=headers,
-                    data=params,
-                    files=files,
-                    timeout=timeout,
-                )
+            response = self._request(files=files, method=method, params=params, url=url, stream=stream)
+        except RetryError as retry_error:
+            last_attempt = retry_error.last_attempt
+
+            if last_attempt.failed:
+                raise last_attempt.exception()
             else:
-                response = self._session.request(method=method, url=url, headers=headers, data=data, timeout=timeout)
-        except ConnectionError as connection_error:
+                response = last_attempt.result()
+
+        except ConnectError as connection_error:
             logger.error(f"Calling {method} {url} failed with ConnectionError: {connection_error}")
             raise connection_error
-        except RetryError as retry_error:
-            logger.error(
-                f"Calling {method} {url} failed with RetryError after {self._num_retries} attempts: {retry_error}"
-            )
-            raise retry_error
         except Exception as exception:
             logger.error(f"Calling {method} {url} failed with Exception: {exception}")
             raise exception
 
-        if response.status_code != 200:
+        if response.status_code != httpx.codes.OK:
             logger.error(f"Calling {method} {url} failed with a non-200 response code: {response.status_code}")
             handle_non_success_response(response.status_code, response.text)
 
-        return response.json()
+        return response
 
-    def _init_session(self, session: Optional[requests.Session]) -> requests.Session:
-        if session is not None:
-            return session
-
-        return (
-            requests_retry_session(requests.Session(), retries=self._num_retries)
-            if self._apply_retry_policy
-            else requests.Session()
+    def _request(
+        self,
+        files: Optional[Dict[str, BinaryIO]],
+        method: str,
+        params: Optional[Dict],
+        url: str,
+        stream: bool,
+    ) -> httpx.Response:
+        timeout = self._timeout_sec
+        headers = self._headers
+        logger.debug(f"Calling {method} {url} {headers} {params}")
+
+        if method == "GET":
+            request = self._client.build_request(
+                method=method, url=url, headers=headers, timeout=timeout, params=params
+            )
+
+            return self._client.send(request=request, stream=stream)
+
+        if files is not None:
+            if method != "POST":
+                raise ValueError(
+                    f"execute_http_request supports only POST for files upload, but {method} was supplied instead"
+                )
+            if "Content-Type" in headers:
+                headers.pop(
+                    "Content-Type"
+                )  # multipart/form-data 'Content-Type' is being added when passing rb files and payload
+            data = params
+        else:
+            data = json.dumps(params).encode() if params else None
+
+        request = self._client.build_request(
+            method=method,
+            url=url,
+            headers=headers,
+            data=data,
+            timeout=timeout,
+            files=files,
         )
 
+        return self._client.send(request=request, stream=stream)
+
+    def _init_client(self, client: Optional[httpx.Client]) -> httpx.Client:
+        if client is not None:
+            return client
+
+        return _requests_retry_session(retries=self._num_retries) if self._apply_retry_policy else httpx.Client()
+
     def add_headers(self, headers: Dict[str, Any]) -> None:
         self._headers.update(headers)
```

### Comparing `ai21-2.2.5/ai21/models/__init__.py` & `ai21-2.3.0/ai21/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.5/ai21/models/chat/chat_completion_response.py` & `ai21-2.3.0/ai21/models/chat/chat_completion_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.5/ai21/models/responses/chat_response.py` & `ai21-2.3.0/ai21/models/responses/chat_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.5/ai21/models/responses/completion_response.py` & `ai21-2.3.0/ai21/models/responses/completion_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.5/ai21/models/responses/custom_model_response.py` & `ai21-2.3.0/ai21/models/responses/custom_model_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.5/ai21/models/responses/file_response.py` & `ai21-2.3.0/ai21/models/responses/file_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.5/ai21/models/responses/gec_response.py` & `ai21-2.3.0/ai21/models/responses/gec_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.5/ai21/models/responses/summarize_by_segment_response.py` & `ai21-2.3.0/ai21/models/responses/summarize_by_segment_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.5/ai21/services/sagemaker.py` & `ai21-2.3.0/ai21/services/sagemaker.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             params={
                 "modelName": model_name,
                 "region": region,
                 "version": version,
             },
         )
 
-        arn = response["arn"]
+        arn = response.json()["arn"]
 
         if not arn:
             raise ModelPackageDoesntExistError(model_name=model_name, region=region, version=version)
 
         return arn
 
     @classmethod
@@ -49,15 +49,15 @@
             url=f"{client.get_base_url()}/{_LIST_VERSIONS_ENDPOINT}",
             params={
                 "modelName": model_name,
                 "region": region,
             },
         )
 
-        return response["versions"]
+        return response.json()["versions"]
 
     @classmethod
     def _create_ai21_http_client(cls) -> AI21HTTPClient:
         return AI21HTTPClient(
             api_key=AI21EnvConfig.api_key,
             api_host=AI21EnvConfig.api_host,
             requires_api_key=False,
```

### Comparing `ai21-2.2.5/ai21/tokenizers/ai21_tokenizer.py` & `ai21-2.3.0/ai21/tokenizers/ai21_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.5/ai21/tokenizers/factory.py` & `ai21-2.3.0/ai21/tokenizers/factory.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.5/pyproject.toml` & `ai21-2.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -42,29 +42,30 @@
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
   "if typing.TYPE_CHECKING:"
 ]
 
 [tool.poetry]
 name = "ai21"
-version = "2.2.5"
+version = "2.3.0"
 description = ""
 authors = ["AI21 Labs"]
 readme = "README.md"
 packages = [
     { include = "ai21" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-requests = "^2.31.0"
 ai21-tokenizer = ">=0.9.1,<1.0.0"
 boto3 = { version = "^1.28.82", optional = true }
 dataclasses-json = "^0.6.3"
 typing-extensions = "^4.9.0"
+httpx = "^0.27.0"
+tenacity = "^8.3.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 invoke = "*"
 isort = "*"
 mypy = "*"
```

### Comparing `ai21-2.2.5/PKG-INFO` & `ai21-2.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: ai21
-Version: 2.2.5
+Version: 2.3.0
 Summary: 
 Author: AI21 Labs
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: aws
 Requires-Dist: ai21-tokenizer (>=0.9.1,<1.0.0)
 Requires-Dist: boto3 (>=1.28.82,<2.0.0) ; extra == "aws"
 Requires-Dist: dataclasses-json (>=0.6.3,<0.7.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
+Requires-Dist: tenacity (>=8.3.0,<9.0.0)
 Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 <h1 align="center">
     <a href="https://github.com/AI21Labs/ai21-python">AI21 Labs Python SDK</a>
 </h1>
 
@@ -228,14 +229,38 @@
 
 </details>
 
 For a more detailed example, see the completion [examples](examples/studio/completion.py).
 
 ---
 
+## Streaming
+
+We currently support streaming for the Chat Completions API in Jamba.
+
+```python
+from ai21 import AI21Client
+from ai21.models.chat import ChatMessage
+
+messages = [ChatMessage(content="What is the meaning of life?", role="user")]
+
+client = AI21Client()
+
+response = client.chat.completions.create(
+    messages=messages,
+    model="jamba-instruct-preview",
+    stream=True,
+)
+for chunk in response:
+    print(chunk.choices[0].delta.content, end="")
+
+```
+
+---
+
 ## TSMs
 
 AI21 Studio's Task-Specific Models offer a range of powerful tools. These models have been specifically designed for their respective tasks and provide high-quality results while optimizing efficiency.
 The full documentation and guides can be found [here](https://docs.ai21.com/docs/task-specific).
 
 ### Contextual Answers
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: ai21 Version: 2.2.5 Summary: Author: AI21 Labs
+Metadata-Version: 2.1 Name: ai21 Version: 2.3.0 Summary: Author: AI21 Labs
 Requires-Python: >=3.8,<4.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Provides-Extra: aws Requires-Dist: ai21-tokenizer
 (>=0.9.1,<1.0.0) Requires-Dist: boto3 (>=1.28.82,<2.0.0) ; extra == "aws"
-Requires-Dist: dataclasses-json (>=0.6.3,<0.7.0) Requires-Dist: requests
-(>=2.31.0,<3.0.0) Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
-Description-Content-Type: text/markdown
+Requires-Dist: dataclasses-json (>=0.6.3,<0.7.0) Requires-Dist: httpx
+(>=0.27.0,<0.28.0) Requires-Dist: tenacity (>=8.3.0,<9.0.0) Requires-Dist:
+typing-extensions (>=4.9.0,<5.0.0) Description-Content-Type: text/markdown
                       ************ _AA_II_22_11_ _LL_aa_bb_ss_ _PP_yy_tt_hh_oo_nn_ _SS_DD_KK ************
 [//]: # "Add when public" [//]: # '_[_T_e_s_t_]' [//]: # '_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n
 _v_e_r_s_i_o_n_s_]'
  _[_T_e_s_t_]_[_I_n_t_e_g_r_a_t_i_o_n_ _T_e_s_t_s_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_o_e_t_r_y_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
                       _[_S_e_m_a_n_t_i_c_ _R_e_l_e_a_s_e_ _S_u_p_p_o_r_t_]_[_L_i_c_e_n_s_e_]
 --- ## Migration from v1.3.4 and below In `v2.0.0` we introduced a new SDK that
 is not backwards compatible with the previous version. This version allows for
@@ -71,41 +71,47 @@
 having trouble signing up for your product with my Google account.",
 role=RoleType.USER), ] client = AI21Client() chat_response = client.chat.create
 ( system=system, messages=messages, model="j2-ultra", ) ``` For a more detailed
 example, see the chat [examples](examples/studio/chat.py). ### Completion
 ```python from ai21 import AI21Client client = AI21Client() completion_response
 = client.completion.create( prompt="This is a test prompt", model="j2-mid", )
 ``` For a more detailed example, see the completion [examples](examples/studio/
-completion.py). --- ## TSMs AI21 Studio's Task-Specific Models offer a range of
-powerful tools. These models have been specifically designed for their
-respective tasks and provide high-quality results while optimizing efficiency.
-The full documentation and guides can be found [here](https://docs.ai21.com/
-docs/task-specific). ### Contextual Answers The `answer` API allows you to
-access our high-quality question answering model. ```python from ai21 import
-AI21Client client = AI21Client() response = client.answer.create( context="This
-is a text is for testing purposes", question="Question about context", ) ``` A
-detailed explanation on Contextual Answers, can be found [here](https://
-docs.ai21.com/docs/contextual-answers-api) ### Token Counting --- By using the
-`count_tokens` method, you can estimate the billing for a given request.
-```python from ai21.tokenizers import get_tokenizer tokenizer = get_tokenizer
-(name="jamba-instruct-tokenizer") total_tokens = tokenizer.count_tokens
-(text="some text") # returns int print(total_tokens) ``` Available tokenizers
-are: - `jamba-instruct-tokenizer` - `j2-tokenizer` For more information on AI21
-Tokenizers, see the [documentation](https://github.com/AI21Labs/ai21-
-tokenizer). ### File Upload --- ```python from ai21 import AI21Client client =
-AI21Client() file_id = client.library.files.create( file_path="path/to/file",
-path="path/to/file/in/library", labels=["label1", "label2"],
-public_url="www.example.com", ) uploaded_file = client.library.files.get
-(file_id) ``` ## Environment Variables --- You can set several environment
-variables to configure the client. ### Logging We use the standard library
-[`logging`](https://docs.python.org/3/library/logging.html) module. To enable
-logging, set the `AI21_LOG_LEVEL` environment variable. ```bash $ export
-AI21_LOG_LEVEL=debug ``` ### Other Important Environment Variables -
-`AI21_API_KEY` - Your API key. If not set, you must pass it to the client
-constructor. - `AI21_API_VERSION` - The API version. Defaults to `v1`. -
+completion.py). --- ## Streaming We currently support streaming for the Chat
+Completions API in Jamba. ```python from ai21 import AI21Client from
+ai21.models.chat import ChatMessage messages = [ChatMessage(content="What is
+the meaning of life?", role="user")] client = AI21Client() response =
+client.chat.completions.create( messages=messages, model="jamba-instruct-
+preview", stream=True, ) for chunk in response: print(chunk.choices
+[0].delta.content, end="") ``` --- ## TSMs AI21 Studio's Task-Specific Models
+offer a range of powerful tools. These models have been specifically designed
+for their respective tasks and provide high-quality results while optimizing
+efficiency. The full documentation and guides can be found [here](https://
+docs.ai21.com/docs/task-specific). ### Contextual Answers The `answer` API
+allows you to access our high-quality question answering model. ```python from
+ai21 import AI21Client client = AI21Client() response = client.answer.create
+( context="This is a text is for testing purposes", question="Question about
+context", ) ``` A detailed explanation on Contextual Answers, can be found
+[here](https://docs.ai21.com/docs/contextual-answers-api) ### Token Counting --
+- By using the `count_tokens` method, you can estimate the billing for a given
+request. ```python from ai21.tokenizers import get_tokenizer tokenizer =
+get_tokenizer(name="jamba-instruct-tokenizer") total_tokens =
+tokenizer.count_tokens(text="some text") # returns int print(total_tokens) ```
+Available tokenizers are: - `jamba-instruct-tokenizer` - `j2-tokenizer` For
+more information on AI21 Tokenizers, see the [documentation](https://
+github.com/AI21Labs/ai21-tokenizer). ### File Upload --- ```python from ai21
+import AI21Client client = AI21Client() file_id = client.library.files.create
+( file_path="path/to/file", path="path/to/file/in/library", labels=["label1",
+"label2"], public_url="www.example.com", ) uploaded_file =
+client.library.files.get(file_id) ``` ## Environment Variables --- You can set
+several environment variables to configure the client. ### Logging We use the
+standard library [`logging`](https://docs.python.org/3/library/logging.html)
+module. To enable logging, set the `AI21_LOG_LEVEL` environment variable.
+```bash $ export AI21_LOG_LEVEL=debug ``` ### Other Important Environment
+Variables - `AI21_API_KEY` - Your API key. If not set, you must pass it to the
+client constructor. - `AI21_API_VERSION` - The API version. Defaults to `v1`. -
 `AI21_API_HOST` - The API host. Defaults to `https://api.ai21.com/v1/`. -
 `AI21_TIMEOUT_SEC` - The timeout for API requests. - `AI21_NUM_RETRIES` - The
 maximum number of retries for API requests. Defaults to `3` retries. -
 `AI21_AWS_REGION` - The AWS region to use for AWS clients. Defaults to `us-
 east-1`. ## Error Handling --- ```python from ai21 import errors as ai21_errors
 from ai21 import AI21Client, AI21APIError from ai21.models import ChatMessage
 client = AI21Client() system = "You're a support engineer in a SaaS company"
```

