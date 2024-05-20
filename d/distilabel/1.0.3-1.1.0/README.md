# Comparing `tmp/distilabel-1.0.3.tar.gz` & `tmp/distilabel-1.1.0.tar.gz`

## Comparing `distilabel-1.0.3.tar` & `distilabel-1.1.0.tar`

### file list

```diff
@@ -1,256 +1,307 @@
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 distilabel-1.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 distilabel-1.0.3/Makefile
--rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 distilabel-1.0.3/mkdocs.yml
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 distilabel-1.0.3/.github/ISSUE_TEMPLATE/blank-issue-template.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 distilabel-1.0.3/.github/ISSUE_TEMPLATE/🆕-feature-request.md
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 distilabel-1.0.3/.github/ISSUE_TEMPLATE/🐛-bug-report.md
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 distilabel-1.0.3/.github/ISSUE_TEMPLATE/📚-documentation-update.md
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 distilabel-1.0.3/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 distilabel-1.0.3/.github/workflows/release.yml
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 distilabel-1.0.3/.github/workflows/test.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/CNAME
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/index.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/overview.md
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/cli.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/llms/anthropic.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/llms/anyscale.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/llms/azure.md
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/llms/huggingface.md
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/llms/index.md
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/llms/litellm.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/llms/llamacpp.md
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/llms/mistral.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/llms/ollama.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/llms/openai.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/llms/together.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/llms/vertexai.md
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/llms/vllm.md
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/pipeline/pipeline.md
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/steps/argilla.md
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/steps/decorator.md
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/steps/extra.md
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/steps/index.md
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/steps/generator_steps/generator_steps.md
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/steps/global_steps/global_steps.md
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/steps/tasks/embeddings.md
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/steps/tasks/preference_tasks.md
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/api/steps/tasks/text_generation.md
--rw-r--r--   0        0        0    16279 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/distilabel-badge-dark.png
--rw-r--r--   0        0        0    15551 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/distilabel-badge-light.png
--rw-r--r--   0        0        0    11187 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/distilabel-black.png
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/distilabel-icon.svg
--rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/distilabel-white.png
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/logo.svg
--rw-r--r--   0        0        0    47284 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/images/distilabel-diagram-dark.svg
--rw-r--r--   0        0        0    47244 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/images/distilabel-diagram.svg
--rw-r--r--   0        0        0   301103 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/images/sections/caching/caching_pipe_1.png
--rw-r--r--   0        0        0   329256 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/images/sections/caching/caching_pipe_2.png
--rw-r--r--   0        0        0   129190 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/images/sections/caching/caching_pipe_3.png
--rw-r--r--   0        0        0    24695 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/images/sections/caching/caching_pipe_4.png
--rw-r--r--   0        0        0   368245 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/images/sections/cli/cli_pipe.png
--rw-r--r--   0        0        0  1290074 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/images/sections/learn/steps/argilla/preference.png
--rw-r--r--   0        0        0  1014081 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/images/sections/learn/steps/argilla/text_generation.png
--rw-r--r--   0        0        0   173971 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/tutorials-assets/instrucion_dataset_notus_ui.png
--rw-r--r--   0        0        0   356586 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/tutorials-assets/preference_dataset_notus_ui.png
--rw-r--r--   0        0        0    19151 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/tutorials-assets/deita/datasets.png
--rw-r--r--   0        0        0    96338 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/tutorials-assets/deita/diversity.png
--rw-r--r--   0        0        0   191403 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/tutorials-assets/deita/overview.png
--rw-r--r--   0        0        0    94813 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/assets/tutorials-assets/deita/results.png
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/scripts/gen_ref_pages.py
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/caching.md
--rw-r--r--   0        0        0     7963 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/cli.md
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/distiset.md
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/index.md
--rw-r--r--   0        0        0     7708 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/llms/index.md
--rw-r--r--   0        0        0    14701 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/pipelines/index.md
--rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/steps/argilla.md
--rw-r--r--   0        0        0     8669 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/steps/general_steps.md
--rw-r--r--   0        0        0     6941 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/steps/generator_steps.md
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/steps/global_steps.md
--rw-r--r--   0        0        0     8491 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/steps/index.md
--rw-r--r--   0        0        0     7803 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/tasks/feedback_tasks.md
--rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/tasks/index.md
--rw-r--r--   0        0        0     5887 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/tasks/special_tasks.md
--rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/learn/tasks/text_generation.md
--rw-r--r--   0        0        0    21822 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/papers/deita.md
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/papers/index.md
--rw-r--r--   0        0        0     5921 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/papers/instruction_backtranslation.md
--rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/sections/papers/ultrafeedback.md
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 distilabel-1.0.3/docs/stylesheets/extra.css
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/__init__.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/__main__.py
--rw-r--r--   0        0        0     9461 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/distiset.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/cli/__init__.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/cli/app.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/cli/pipeline/__init__.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/cli/pipeline/app.py
--rw-r--r--   0        0        0     8197 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/cli/pipeline/utils.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/__init__.py
--rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/anthropic.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/anyscale.py
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/azure.py
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/base.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/chat_templates.py
--rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/cohere.py
--rw-r--r--   0        0        0     8176 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/litellm.py
--rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/llamacpp.py
--rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/mistral.py
--rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/mixins.py
--rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/ollama.py
--rw-r--r--   0        0        0     6861 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/openai.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/together.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/typing.py
--rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/vertexai.py
--rw-r--r--   0        0        0     7201 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/vllm.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/huggingface/__init__.py
--rw-r--r--   0        0        0    16868 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/huggingface/inference_endpoints.py
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/llms/huggingface/transformers.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/mixins/__init__.py
--rw-r--r--   0        0        0     7026 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/mixins/runtime_parameters.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/pipeline/__init__.py
--rw-r--r--   0        0        0    18795 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/pipeline/_dag.py
--rw-r--r--   0        0        0    37076 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/pipeline/base.py
--rw-r--r--   0        0        0    32476 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/pipeline/local.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/pipeline/utils.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/__init__.py
--rw-r--r--   0        0        0    19355 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/base.py
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/combine.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/conversation.py
--rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/decorator.py
--rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/deita.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/expand.py
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/keep.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/typing.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/argilla/__init__.py
--rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/argilla/base.py
--rw-r--r--   0        0        0    10934 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/argilla/preference.py
--rw-r--r--   0        0        0     6705 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/argilla/text_generation.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/generators/__init__.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/generators/data.py
--rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/generators/huggingface.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/globals/__init__.py
--rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/globals/huggingface.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/__init__.py
--rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/base.py
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/complexity_scorer.py
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/generate_embeddings.py
--rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/instruction_backtranslation.py
--rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/pair_rm.py
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/quality_scorer.py
--rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/self_instruct.py
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/text_generation.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/typing.py
--rw-r--r--   0        0        0     9452 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/ultrafeedback.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/__init__.py
--rw-r--r--   0        0        0    12081 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/base.py
--rw-r--r--   0        0        0    10714 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/english_nouns.txt
--rw-r--r--   0        0        0    12857 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/generator.py
--rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/evol_complexity/__init__.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/evol_complexity/base.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/evol_complexity/generator.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/evol_complexity/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/evol_quality/__init__.py
--rw-r--r--   0        0        0     9098 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/evol_quality/base.py
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/evol_quality/utils.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/templates/instruction-backtranslation.jinja2
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/templates/self-instruct.jinja2
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/templates/ultrafeedback/helpfulness.jinja2
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/templates/ultrafeedback/honesty.jinja2
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/templates/ultrafeedback/instruction-following.jinja2
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/templates/ultrafeedback/overall-rating.jinja2
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/steps/tasks/templates/ultrafeedback/truthfulness.jinja2
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/__init__.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/chat.py
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/dicts.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/docstring.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/files.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/itertools.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/lists.py
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/logging.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/notebook.py
--rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/serialization.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/typing_.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/card/__init__.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/card/dataset_card.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 distilabel-1.0.3/src/distilabel/utils/card/distilabel_template.md
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/__init__.py
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/integration/test_pipe_llms.py
--rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/integration/test_pipe_simple.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/__init__.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/test_distiset.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/test_imports.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/cli/__init__.py
--rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/cli/test_pipeline.yaml
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/cli/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/cli/pipeline/__init__.py
--rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/cli/pipeline/test_app.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/cli/pipeline/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/__init__.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/test_anthropic.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/test_anyscale.py
--rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/test_azure.py
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/test_cohere.py
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/test_litellm.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/test_llamacpp.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/test_mistral.py
--rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/test_mixins.py
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/test_ollama.py
--rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/test_openai.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/test_together.py
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/test_vertexai.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/huggingface/__init__.py
--rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/huggingface/test_inference_endpoints.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/llms/huggingface/test_transformers.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/mixins/__init__.py
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/mixins/test_runtime_parameters.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/pipeline/__init__.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/pipeline/conftest.py
--rw-r--r--   0        0        0    44539 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/pipeline/test_base.py
--rw-r--r--   0        0        0    18140 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/pipeline/test_dag.py
--rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/pipeline/test_local.py
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/pipeline/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/__init__.py
--rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/test_base.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/test_combine.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/test_conversation.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/test_decorator.py
--rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/test_deita.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/test_expand.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/test_keep.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/argilla/__init__.py
--rw-r--r--   0        0        0     5814 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/argilla/test_base.py
--rw-r--r--   0        0        0     5725 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/argilla/test_preference.py
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/argilla/test_text_generation.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/generators/test_data.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/__init__.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/conftest.py
--rw-r--r--   0        0        0     8172 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/test_base.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/test_complexity_scorer.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/test_generate_embeddings.py
--rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/test_instruction_backtranslation.py
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/test_pair_rm.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/test_quality_scorer.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/test_self_instruct.py
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/test_text_generation.py
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/test_ultrafeedback.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/utils.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/evol_instruct/__init__.py
--rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/evol_instruct/test_base.py
--rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/evol_instruct/test_generator.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/__init__.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_base.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_generator.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/evol_quality/__init__.py
--rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/steps/tasks/evol_quality/test_base.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/utils/__init__.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/utils/test_chat.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/utils/test_docstring.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/utils/test_lists.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 distilabel-1.0.3/tests/unit/utils/test_typing.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 distilabel-1.0.3/.gitignore
--rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 distilabel-1.0.3/LICENSE
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 distilabel-1.0.3/LICENSE_HEADER
--rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 distilabel-1.0.3/README.md
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 distilabel-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    12184 2020-02-02 00:00:00.000000 distilabel-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 distilabel-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 distilabel-1.1.0/Makefile
+-rw-r--r--   0        0        0     6588 2020-02-02 00:00:00.000000 distilabel-1.1.0/mkdocs.yml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 distilabel-1.1.0/.github/ISSUE_TEMPLATE/blank-issue-template.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 distilabel-1.1.0/.github/ISSUE_TEMPLATE/🆕-feature-request.md
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 distilabel-1.1.0/.github/ISSUE_TEMPLATE/🐛-bug-report.md
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 distilabel-1.1.0/.github/ISSUE_TEMPLATE/📚-documentation-update.md
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 distilabel-1.1.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 distilabel-1.1.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 distilabel-1.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/CNAME
+-rw-r--r--   0        0        0     9308 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/index.md
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/cli.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/anthropic.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/anyscale.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/azure.md
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/groq.md
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/huggingface.md
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/index.md
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/litellm.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/llamacpp.md
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/mistral.md
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/ollama.md
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/openai.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/together.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/vertexai.md
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/llm/vllm.md
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/pipeline/index.md
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/pipeline/routing_batch_function.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/pipeline/typing.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/pipeline/utils.md
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/step/decorator.md
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/step/generator_step.md
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/step/global_step.md
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/step/index.md
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/step_gallery/argilla.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/step_gallery/columns.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/step_gallery/extra.md
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/task/generator_task.md
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/task/index.md
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/api/task_gallery/index.md
+-rw-r--r--   0        0        0    16279 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/distilabel-badge-dark.png
+-rw-r--r--   0        0        0    15551 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/distilabel-badge-light.png
+-rw-r--r--   0        0        0    11187 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/distilabel-black.png
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/distilabel-icon.svg
+-rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/distilabel-white.png
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/logo.svg
+-rw-r--r--   0        0        0    47284 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/images/distilabel-diagram-dark.svg
+-rw-r--r--   0        0        0    47244 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/images/distilabel-diagram.svg
+-rw-r--r--   0        0        0   301103 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/images/sections/caching/caching_pipe_1.png
+-rw-r--r--   0        0        0   329256 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/images/sections/caching/caching_pipe_2.png
+-rw-r--r--   0        0        0   129190 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/images/sections/caching/caching_pipe_3.png
+-rw-r--r--   0        0        0    24695 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/images/sections/caching/caching_pipe_4.png
+-rw-r--r--   0        0        0   368245 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/images/sections/cli/cli_pipe.png
+-rw-r--r--   0        0        0  1290074 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/images/sections/learn/steps/argilla/preference.png
+-rw-r--r--   0        0        0  1014081 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/images/sections/learn/steps/argilla/text_generation.png
+-rw-r--r--   0        0        0   336223 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/images/sections/pipeline/pipeline-ctrlc.png
+-rw-r--r--   0        0        0   173971 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/tutorials-assets/instrucion_dataset_notus_ui.png
+-rw-r--r--   0        0        0   356586 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/tutorials-assets/preference_dataset_notus_ui.png
+-rw-r--r--   0        0        0    19151 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/tutorials-assets/deita/datasets.png
+-rw-r--r--   0        0        0    96338 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/tutorials-assets/deita/diversity.png
+-rw-r--r--   0        0        0   191403 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/tutorials-assets/deita/overview.png
+-rw-r--r--   0        0        0    94813 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/assets/tutorials-assets/deita/results.png
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/scripts/gen_ref_pages.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/faq.md
+-rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/how_to_guide.md
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/installation.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/index.md
+-rw-r--r--   0        0        0     8671 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/advanced/argilla.md
+-rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/advanced/caching.md
+-rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/advanced/distiset.md
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/advanced/index.md
+-rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/advanced/structured_generation.md
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/tutorial/index.md
+-rw-r--r--   0        0        0     8272 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/tutorial/cli/index.md
+-rw-r--r--   0        0        0     7983 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/tutorial/llm/index.md
+-rw-r--r--   0        0        0    21776 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/tutorial/pipeline/index.md
+-rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/tutorial/step/generator_step.md
+-rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/tutorial/step/global_step.md
+-rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/tutorial/step/index.md
+-rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/tutorial/task/generator_task.md
+-rw-r--r--   0        0        0     4833 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/learn/tutorial/task/index.md
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/pipeline_samples/index.md
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/pipeline_samples/examples/index.md
+-rw-r--r--   0        0        0    21843 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/pipeline_samples/papers/deita.md
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/pipeline_samples/papers/index.md
+-rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/pipeline_samples/papers/instruction_backtranslation.md
+-rw-r--r--   0        0        0    10707 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/sections/pipeline_samples/papers/ultrafeedback.md
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 distilabel-1.1.0/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 distilabel-1.1.0/examples/structured_generation_with_outlines.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/__init__.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/__main__.py
+-rw-r--r--   0        0        0    10989 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/distiset.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/cli/__init__.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/cli/app.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/cli/pipeline/__init__.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/cli/pipeline/app.py
+-rw-r--r--   0        0        0     9741 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/cli/pipeline/utils.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/__init__.py
+-rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/anthropic.py
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/anyscale.py
+-rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/azure.py
+-rw-r--r--   0        0        0    11651 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/base.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/chat_templates.py
+-rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/cohere.py
+-rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/groq.py
+-rw-r--r--   0        0        0     8188 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/litellm.py
+-rw-r--r--   0        0        0     9518 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/llamacpp.py
+-rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/mistral.py
+-rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/mixins.py
+-rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/ollama.py
+-rw-r--r--   0        0        0     7817 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/openai.py
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/together.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/typing.py
+-rw-r--r--   0        0        0     6948 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/vertexai.py
+-rw-r--r--   0        0        0    10496 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/vllm.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/huggingface/__init__.py
+-rw-r--r--   0        0        0    18361 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/huggingface/inference_endpoints.py
+-rw-r--r--   0        0        0    10334 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/llms/huggingface/transformers.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/mixins/__init__.py
+-rw-r--r--   0        0        0     7822 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/mixins/runtime_parameters.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/pipeline/__init__.py
+-rw-r--r--   0        0        0    26498 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/pipeline/_dag.py
+-rw-r--r--   0        0        0    57088 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/pipeline/base.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/pipeline/constants.py
+-rw-r--r--   0        0        0    39256 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/pipeline/local.py
+-rw-r--r--   0        0        0    13786 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/pipeline/routing_batch_function.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/pipeline/typing.py
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/pipeline/utils.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/__init__.py
+-rw-r--r--   0        0        0    24715 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/base.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/combine.py
+-rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/decorator.py
+-rw-r--r--   0        0        0     9246 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/deita.py
+-rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/expand.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/keep.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/typing.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/argilla/__init__.py
+-rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/argilla/base.py
+-rw-r--r--   0        0        0    10978 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/argilla/preference.py
+-rw-r--r--   0        0        0     6839 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/argilla/text_generation.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/formatting/__init__.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/formatting/conversation.py
+-rw-r--r--   0        0        0    12377 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/formatting/dpo.py
+-rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/formatting/sft.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/generators/__init__.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/generators/data.py
+-rw-r--r--   0        0        0     8694 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/generators/huggingface.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/globals/__init__.py
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/globals/huggingface.py
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/__init__.py
+-rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/base.py
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/complexity_scorer.py
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/generate_embeddings.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/genstruct.py
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/instruction_backtranslation.py
+-rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/pair_rm.py
+-rw-r--r--   0        0        0    15783 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/prometheus_eval.py
+-rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/quality_scorer.py
+-rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/self_instruct.py
+-rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/text_generation.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/typing.py
+-rw-r--r--   0        0        0     9539 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/ultrafeedback.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/__init__.py
+-rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/base.py
+-rw-r--r--   0        0        0    10714 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/english_nouns.txt
+-rw-r--r--   0        0        0    12983 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/generator.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/__init__.py
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/base.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/generator.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/evol_quality/__init__.py
+-rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/evol_quality/base.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/evol_quality/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/structured_outputs/__init__.py
+-rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/structured_outputs/outlines.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/complexity-scorer.jinja2
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/genstruct.jinja2
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/instruction-backtranslation.jinja2
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/quality-scorer.jinja2
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/self-instruct.jinja2
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/prometheus/absolute_with_reference.jinja2
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/prometheus/absolute_without_reference.jinja2
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/prometheus/relative_with_reference.jinja2
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/prometheus/relative_without_reference.jinja2
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/ultrafeedback/helpfulness.jinja2
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/ultrafeedback/honesty.jinja2
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/ultrafeedback/instruction-following.jinja2
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/ultrafeedback/overall-rating.jinja2
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/steps/tasks/templates/ultrafeedback/truthfulness.jinja2
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/__init__.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/chat.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/dicts.py
+-rw-r--r--   0        0        0     6853 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/docstring.py
+-rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/export_components_info.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/files.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/itertools.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/lists.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/logging.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/notebook.py
+-rw-r--r--   0        0        0    10685 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/serialization.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/typing_.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/card/__init__.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/card/dataset_card.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/card/distilabel_template.md
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/mkdocs/__init__.py
+-rw-r--r--   0        0        0    14542 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/mkdocs/components_gallery.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/mkdocs/templates/components-gallery/components-list.jinja2
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/mkdocs/templates/components-gallery/index.md
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/mkdocs/templates/components-gallery/llm-detail.jinja2
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 distilabel-1.1.0/src/distilabel/utils/mkdocs/templates/components-gallery/step-detail.jinja2
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/integration/test_branching_missaligmnent.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/integration/test_dry_run.py
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/integration/test_pipe_llms.py
+-rw-r--r--   0        0        0     6481 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/integration/test_pipe_simple.py
+-rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/integration/test_routing_batch_function.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/helpers.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/test_distiset.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/test_imports.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/cli/__init__.py
+-rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/cli/test_pipeline.yaml
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/cli/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/cli/pipeline/__init__.py
+-rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/cli/pipeline/test_app.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/cli/pipeline/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/__init__.py
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/test_anthropic.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/test_anyscale.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/test_azure.py
+-rw-r--r--   0        0        0     3750 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/test_cohere.py
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/test_groq.py
+-rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/test_litellm.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/test_llamacpp.py
+-rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/test_mistral.py
+-rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/test_mixins.py
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/test_ollama.py
+-rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/test_openai.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/test_together.py
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/test_vertexai.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/huggingface/__init__.py
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/huggingface/test_inference_endpoints.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/llms/huggingface/test_transformers.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/mixins/__init__.py
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/mixins/test_runtime_parameters.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/pipeline/__init__.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/pipeline/conftest.py
+-rw-r--r--   0        0        0    82348 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/pipeline/test_base.py
+-rw-r--r--   0        0        0    23637 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/pipeline/test_dag.py
+-rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/pipeline/test_local.py
+-rw-r--r--   0        0        0     5578 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/pipeline/test_routing_batch_function.py
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/pipeline/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/__init__.py
+-rw-r--r--   0        0        0    11237 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/test_base.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/test_combine.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/test_decorator.py
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/test_deita.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/test_expand.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/test_keep.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/argilla/__init__.py
+-rw-r--r--   0        0        0     5777 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/argilla/test_base.py
+-rw-r--r--   0        0        0     5655 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/argilla/test_preference.py
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/argilla/test_text_generation.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/formatting/__init__.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/formatting/test_conversation.py
+-rw-r--r--   0        0        0     5313 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/formatting/test_dpo.py
+-rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/formatting/test_sft.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/generators/test_data.py
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/generators/test_huggingface.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/__init__.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/conftest.py
+-rw-r--r--   0        0        0     8550 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/test_base.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/test_complexity_scorer.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/test_generate_embeddings.py
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/test_genstruct.py
+-rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/test_instruction_backtranslation.py
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/test_pair_rm.py
+-rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/test_prometheus_eval.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/test_quality_scorer.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/test_self_instruct.py
+-rw-r--r--   0        0        0     5348 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/test_text_generation.py
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/test_ultrafeedback.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/evol_instruct/__init__.py
+-rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/evol_instruct/test_base.py
+-rw-r--r--   0        0        0    11637 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/evol_instruct/test_generator.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/__init__.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_base.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_generator.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/evol_quality/__init__.py
+-rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/evol_quality/test_base.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/structured_outputs/__init__.py
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/steps/tasks/structured_outputs/test_outlines.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/utils/__init__.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/utils/test_chat.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/utils/test_docstring.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/utils/test_files.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/utils/test_lists.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 distilabel-1.1.0/tests/unit/utils/test_typing.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 distilabel-1.1.0/.gitignore
+-rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 distilabel-1.1.0/LICENSE
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 distilabel-1.1.0/LICENSE_HEADER
+-rw-r--r--   0        0        0     9115 2020-02-02 00:00:00.000000 distilabel-1.1.0/README.md
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 distilabel-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    12566 2020-02-02 00:00:00.000000 distilabel-1.1.0/PKG-INFO
```

### Comparing `distilabel-1.0.3/.pre-commit-config.yaml` & `distilabel-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/mkdocs.yml` & `distilabel-1.1.0/mkdocs.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Project information
 site_name: distilabel
 site_url: https://argilla-io.github.io/distilabel
 site_author: Argilla, Inc.
-site_description: AI Feedback framework
+site_description: Distilabel is an AI Feedback (AIF) framework for building datasets with and for LLMs.
 
 # Repository
 repo_name: argilla-io/distilabel
 repo_url: https://github.com/argilla-io/distilabel
 
 extra:
   version:
@@ -20,20 +20,23 @@
   - https://polyfill.io/v3/polyfill.min.js?features=es6
   - https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js
 
 theme:
   name: material
   logo: assets/logo.svg
   favicon: assets/logo.svg
+  icon:
+    repo: fontawesome/brands/github-alt
   features:
     - navigation.sections # Sections are included in the navigation on the left.
     # - toc.integrate # # Table of contents is integrated on the left; does not appear separately on the right.
     - header.autohide # header disappears as you scroll
     - content.code.copy
     - content.code.annotate
+    - content.tabs.link
   palette:
     - media: "(prefers-color-scheme)"
       primary: white
       toggle:
         icon: material/brightness-auto
         name: Switch to light mode
     - media: "(prefers-color-scheme: light)"
@@ -55,26 +58,36 @@
   - src/distilabel
 
 # Extensions
 markdown_extensions:
   - attr_list
   - md_in_html
   - admonition
+  - pymdownx.superfences
   - pymdownx.arithmatex:
       generic: true
   - pymdownx.highlight:
       anchor_linenums: true
       line_spans: __span
       pygments_lang_class: true
   - pymdownx.inlinehilite
-  - pymdownx.snippets
-  - pymdownx.superfences
+  - pymdownx.superfences:
+      custom_fences:
+        - name: mermaid
+          class: mermaid
+          format: !!python/name:pymdownx.superfences.fence_code_format
+  - pymdownx.snippets:
+      check_paths: true
+      base_path: [examples/, docs/, "."]
   - pymdownx.details
   - pymdownx.tabbed:
       alternate_style: true
+  - pymdownx.emoji:
+      emoji_index: !!python/name:material.extensions.emoji.twemoji
+      emoji_generator: !!python/name:material.extensions.emoji.to_svg
   - footnotes
   - toc:
       permalink: true
 
 plugins:
   - search
   - autorefs # Cross-links to headings
@@ -85,77 +98,93 @@
       nav_file: SUMMARY.md
   - section-index
   - mkdocstrings:
       handlers:
         python:
           selection:
             inherited_members: true # Allow looking up inherited methods
+          options:
+            show_protected_members: true
+            show_private_members: true
           rendering:
             show_root_heading: true # actually display anything at all...
             # show_root_full_path: true  # display "diffrax.asdf" not just "asdf"
             show_if_no_docstring: true
             show_signature_annotations: true
             show_source: false # don't include source code
             members_order: source # order methods according to their order of definition in the source code, not alphabetical order
             heading_level: 4
   - social
+  - distilabel/components-gallery:
+      add_after_page: Learn
 
 nav:
-  - Getting started: index.md
+  - Introduction: "index.md"
+  - Getting started:
+      - Installation: "sections/installation.md"
+      - How-to-Guide: "sections/how_to_guide.md"
   - Learn:
       - "sections/learn/index.md"
       - Tutorial:
-          - Steps:
-              - "sections/learn/steps/index.md"
-              - "sections/learn/steps/generator_steps.md"
-              - "sections/learn/steps/global_steps.md"
-              - "sections/learn/steps/general_steps.md"
-              - "sections/learn/steps/argilla.md"
-          - Tasks:
-              - "sections/learn/tasks/index.md"
-              - "sections/learn/tasks/text_generation.md"
-              - "sections/learn/tasks/feedback_tasks.md"
-              - "sections/learn/tasks/special_tasks.md"
-          - LLMs:
-              - "sections/learn/llms/index.md"
-          - Pipeline:
-              - "sections/learn/pipelines/index.md"
-          - Command Line Interface:
-              - "sections/learn/cli.md"
+          - "sections/learn/tutorial/index.md"
+          - Step:
+              - "sections/learn/tutorial/step/index.md"
+              - GeneratorStep: "sections/learn/tutorial/step/generator_step.md"
+              - GlobalStep: "sections/learn/tutorial/step/global_step.md"
+          - Task:
+              - "sections/learn/tutorial/task/index.md"
+              - GeneratorTask: "sections/learn/tutorial/task/generator_task.md"
+          - LLM: "sections/learn/tutorial/llm/index.md"
+          - Pipeline: "sections/learn/tutorial/pipeline/index.md"
+          - CLI: "sections/learn/tutorial/cli/index.md"
       - Advanced:
-          - Distiset:
-              - "sections/learn/distiset.md"
-          - Caching:
-              - "sections/learn/caching.md"
-  - Paper reproductions:
-      - "sections/papers/index.md"
+          - "sections/learn/advanced/index.md"
+          - Argilla: "sections/learn/advanced/argilla.md"
+          - Caching: "sections/learn/advanced/caching.md"
+          - Distiset: "sections/learn/advanced/distiset.md"
+          - Structured Generation: "sections/learn/advanced/structured_generation.md"
+  - Pipeline Samples:
+      - "sections/pipeline_samples/index.md"
+      - Examples: "sections/pipeline_samples/examples/index.md"
       - Papers:
-          - "What Makes Good Data for Alignment? A Comprehensive Study of Automatic Data Selection in Instruction Tuning": "sections/papers/deita.md"
-          - "Self-Alignment with Instruction Backtranslation": "sections/papers/instruction_backtranslation.md"
-          - "UltraFeedback: Boosting Language Models with High-quality Feedback": "sections/papers/ultrafeedback.md"
+          - "sections/pipeline_samples/papers/index.md"
+          - DEITA: "sections/pipeline_samples/papers/deita.md"
+          - Instruction Backtranslation: "sections/pipeline_samples/papers/instruction_backtranslation.md"
+          # - Prometheus: "sections/examples/papers/prometheus.md"
+          - UltraFeedback: "sections/pipeline_samples/papers/ultrafeedback.md"
+  - FAQ: "sections/faq.md"
   - API Reference:
       - Pipeline:
-          - "api/pipeline/pipeline.md"
-      - Steps:
-          - "api/steps/index.md"
-          - Generator Steps: "api/steps/generator_steps/generator_steps.md"
-          - Global Steps: "api/steps/global_steps/global_steps.md"
-          - Tasks:
-              - "api/steps/tasks/text_generation.md"
-              - "api/steps/tasks/preference_tasks.md"
-              - "api/steps/tasks/embeddings.md"
-          - "api/steps/decorator.md"
-      - LLMs:
-          - "api/llms/index.md"
-          - "api/llms/anthropic.md"
-          - "api/llms/anyscale.md"
-          - "api/llms/huggingface.md"
-          - "api/llms/litellm.md"
-          - "api/llms/llamacpp.md"
-          - "api/llms/mistral.md"
-          - "api/llms/ollama.md"
-          - "api/llms/openai.md"
-          - "api/llms/together.md"
-          - "api/llms/vertexai.md"
-          - "api/llms/vllm.md"
-      - Command Line Interface:
-          - "api/cli.md"
+          - "api/pipeline/index.md"
+          - Routing Batch Function: "api/pipeline/routing_batch_function.md"
+          - Typing: "api/pipeline/typing.md"
+          - Utils: "api/pipeline/utils.md"
+      - Step:
+          - "api/step/index.md"
+          - GeneratorStep: "api/step/generator_step.md"
+          - GlobalStep: "api/step/global_step.md"
+          - "@step": "api/step/decorator.md"
+          - Step Gallery:
+            - Argilla: "api/step_gallery/argilla.md"
+            - Columns: "api/step_gallery/columns.md"
+            - Extra: "api/step_gallery/extra.md"
+      - Task:
+          - "api/task/index.md"
+          - GeneratorTask: "api/task/generator_task.md"
+          - Task Gallery: "api/task_gallery/index.md"
+      - LLM:
+          - "api/llm/index.md"
+          - LLM Gallery:
+              - Anthropic: "api/llm/anthropic.md"
+              - Anyscale: "api/llm/anyscale.md"
+              - Azure (via OpenAI): "api/llm/azure.md"
+              - Groq: "api/llm/groq.md"
+              - Hugging Face: "api/llm/huggingface.md"
+              - LiteLLM: "api/llm/litellm.md"
+              - llama.cpp: "api/llm/llamacpp.md"
+              - Mistral: "api/llm/mistral.md"
+              - Ollama: "api/llm/ollama.md"
+              - OpenAI: "api/llm/openai.md"
+              - Together AI: "api/llm/together.md"
+              - Google Vertex AI: "api/llm/vertexai.md"
+              - vLLM: "api/llm/vllm.md"
+      - CLI: "api/cli.md"
```

### Comparing `distilabel-1.0.3/.github/ISSUE_TEMPLATE/🆕-feature-request.md` & `distilabel-1.1.0/.github/ISSUE_TEMPLATE/🆕-feature-request.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/.github/ISSUE_TEMPLATE/🐛-bug-report.md` & `distilabel-1.1.0/.github/ISSUE_TEMPLATE/🐛-bug-report.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/.github/ISSUE_TEMPLATE/📚-documentation-update.md` & `distilabel-1.1.0/.github/ISSUE_TEMPLATE/📚-documentation-update.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/.github/workflows/docs.yml` & `distilabel-1.1.0/.github/workflows/docs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: Publish documentation
 
 on:
   push:
     branches:
-      - main
+      - develop
       - gh-pages
     tags:
       - "**"
 
 jobs:
   publish:
     runs-on: ubuntu-latest
@@ -40,11 +40,11 @@
 
       - name: Set git credentials
         run: |
           git config --global user.name "${{ github.actor }}"
           git config --global user.email "${{ github.actor }}@users.noreply.github.com"
 
       - run: mike deploy dev --push
-        if: github.ref == 'refs/heads/main'
+        if: github.ref == 'refs/heads/develop'
 
       - run: mike deploy ${{ github.ref_name }} latest --update-aliases --push
         if: startsWith(github.ref, 'refs/tags/')
```

### Comparing `distilabel-1.0.3/.github/workflows/release.yml` & `distilabel-1.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/.github/workflows/test.yml` & `distilabel-1.1.0/.github/workflows/test.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 name: Test
 
 on:
   push:
     branches:
       - main
+      - develop
   pull_request:
     types:
       - opened
       - synchronize
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.event.pull_request.number || github.ref }}
@@ -18,44 +19,44 @@
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.8", "3.9", "3.10", "3.11"]
       fail-fast: false
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
           # Looks like it's not working very well for other people:
           # https://github.com/actions/setup-python/issues/436
           # cache: "pip"
           # cache-dependency-path: pyproject.toml
 
-      - uses: actions/cache@v3
+      - uses: actions/cache@v4
         id: cache
         with:
           path: ${{ env.pythonLocation }}
-          key: ${{ runner.os }}-python-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-test
+          key: ${{ runner.os }}-python-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-test-v00
 
       - name: Install dependencies
         if: steps.cache.outputs.cache-hit != 'true'
         run: |
           python_version=$(python -c "import sys; print(sys.version_info[:2])")
 
+          pip install -e .[dev,tests,anthropic,argilla,cohere,groq,hf-inference-endpoints,hf-transformers,litellm,llama-cpp,ollama,openai,outlines,vertexai,vllm]
           if [ "${python_version}" != "(3, 8)" ]; then
-            pip install -e .[dev,tests,cohere,hf-transformers,hf-inference-endpoints,vertexai,ollama,openai,together,argilla,mistralai,llama-cpp,anthropic,litellm]
-          else
-            pip install -e .[dev,tests,cohere,hf-transformers,hf-inference-endpoints,vertexai,ollama,openai,together,argilla,llama-cpp,anthropic,litellm]
-          fi
+            pip install -e .[mistralai]
+          fi;
           pip install git+https://github.com/argilla-io/LLM-Blender.git
 
       - name: Lint
         run: make lint
 
       - name: Unit Tests
         run: make unit-tests
 
       - name: Integration Tests
         run: make integration-tests
+        timeout-minutes: 5
```

### Comparing `distilabel-1.0.3/docs/assets/distilabel-badge-dark.png` & `distilabel-1.1.0/docs/assets/distilabel-badge-dark.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/docs/assets/distilabel-badge-light.png` & `distilabel-1.1.0/docs/assets/distilabel-badge-light.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/docs/assets/distilabel-black.png` & `distilabel-1.1.0/docs/assets/distilabel-black.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/docs/assets/distilabel-icon.svg` & `distilabel-1.1.0/docs/assets/distilabel-icon.svg`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/docs/assets/distilabel-white.png` & `distilabel-1.1.0/docs/assets/distilabel-white.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/docs/assets/logo.svg` & `distilabel-1.1.0/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/docs/assets/images/distilabel-diagram-dark.svg` & `distilabel-1.1.0/docs/assets/images/distilabel-diagram-dark.svg`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/docs/assets/images/distilabel-diagram.svg` & `distilabel-1.1.0/docs/assets/images/distilabel-diagram.svg`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/docs/assets/images/sections/caching/caching_pipe_1.png` & `distilabel-1.1.0/docs/assets/images/sections/caching/caching_pipe_1.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/docs/assets/images/sections/caching/caching_pipe_2.png` & `distilabel-1.1.0/docs/assets/images/sections/caching/caching_pipe_2.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/docs/assets/images/sections/caching/caching_pipe_3.png` & `distilabel-1.1.0/docs/assets/images/sections/caching/caching_pipe_3.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/docs/assets/images/sections/caching/caching_pipe_4.png` & `distilabel-1.1.0/docs/assets/images/sections/caching/caching_pipe_4.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/docs/assets/images/sections/cli/cli_pipe.png` & `distilabel-1.1.0/docs/assets/images/sections/cli/cli_pipe.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/docs/assets/images/sections/learn/steps/argilla/preference.png` & `distilabel-1.1.0/docs/assets/images/sections/learn/steps/argilla/preference.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/docs/assets/images/sections/learn/steps/argilla/text_generation.png` & `distilabel-1.1.0/docs/assets/images/sections/learn/steps/argilla/text_generation.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/docs/assets/tutorials-assets/instrucion_dataset_notus_ui.png` & `distilabel-1.1.0/docs/assets/tutorials-assets/instrucion_dataset_notus_ui.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/docs/assets/tutorials-assets/preference_dataset_notus_ui.png` & `distilabel-1.1.0/docs/assets/tutorials-assets/preference_dataset_notus_ui.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/docs/assets/tutorials-assets/deita/datasets.png` & `distilabel-1.1.0/docs/assets/tutorials-assets/deita/datasets.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/docs/assets/tutorials-assets/deita/diversity.png` & `distilabel-1.1.0/docs/assets/tutorials-assets/deita/diversity.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/docs/assets/tutorials-assets/deita/overview.png` & `distilabel-1.1.0/docs/assets/tutorials-assets/deita/overview.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/docs/assets/tutorials-assets/deita/results.png` & `distilabel-1.1.0/docs/assets/tutorials-assets/deita/results.png`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/docs/scripts/gen_ref_pages.py` & `distilabel-1.1.0/docs/scripts/gen_ref_pages.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pathlib import Path
 
 import mkdocs_gen_files
 
 nav = mkdocs_gen_files.Nav()
 
 src = Path(__file__).parent.parent.parent / "src"
-excluded = ["distilabel/utils", "distilabel/logger.py", "distilabel/progress_bar.py"]
+excluded = ["distilabel/utils"]
 
 for path in sorted(src.rglob("*.py")):
     if any(path.name.__contains__(exclude) for exclude in excluded):
         continue
     module_path = path.relative_to(src).with_suffix("")
     doc_path = path.relative_to(src).with_suffix(".md")
     full_doc_path = Path("reference", doc_path)
```

### Comparing `distilabel-1.0.3/docs/sections/learn/cli.md` & `distilabel-1.1.0/docs/sections/learn/tutorial/cli/index.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# Command Line Interface
+# Command Line Interface (CLI)
 
-`Distilabel` offers a [`CLI`][distilabel.cli.pipeline.utils] to initially *explore* and *rerun* `Pipelines`, let's take a look.
+`Distilabel` offers a [`CLI`][distilabel.cli.pipeline.utils] to _explore_ and _re-run_ existing [`Pipeline`][distilabel.pipeline.Pipeline] dumps, meaning that an existing dump can be explored to see the steps, how those are connected, the runtime parameters used, and also re-run it with the same or different runtime parameters, respectively.
 
 ## Available commands
 
-We have two commands under the `CLI` app, `distilabel pipeline`:
+The only available command as of the current version of `distilabel` is `distilabel pipeline`.
 
 ```bash
 $ distilabel pipeline --help
 
  Usage: distilabel pipeline [OPTIONS] COMMAND [ARGS]...
 
  Commands to run and inspect Distilabel pipelines.
@@ -18,19 +18,17 @@
 ╰─────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ──────────────────────────────────────────────────────────────────────────────╮
 │ info      Get information about a Distilabel pipeline.                                  │
 │ run       Run a Distilabel pipeline.                                                    │
 ╰─────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
-Will run them using as an example the following [dataset](https://huggingface.co/datasets/distilabel-internal-testing/ultrafeedback-mini) for testing purposes:
+So on, `distilabel pipeline` has two subcommands: `info` and `run`, as described below. Note that for testing purposes we will be using the following [dataset](https://huggingface.co/datasets/distilabel-internal-testing/ultrafeedback-mini).
 
-### Pipeline info
-
-The first command is `distilabel pipeline info`:
+### `distilabel pipeline info`
 
 ```bash
 $ distilabel pipeline info --help
 
  Usage: distilabel pipeline info [OPTIONS]
 
  Get information about a Distilabel pipeline.
@@ -47,19 +45,19 @@
 
 ```bash
 distilabel pipeline info --config "https://huggingface.co/datasets/distilabel-internal-testing/instruction-dataset-mini-with-generations/raw/main/pipeline.yaml"
 ```
 
 If we take a look:
 
-![CLI 1](../../assets/images/sections/cli/cli_pipe.png)
+![CLI 1](../../../../assets/images/sections/cli/cli_pipe.png)
 
 The pipeline information includes the steps used in the `Pipeline` along with the `Runtime Parameter` that was used, as well as a description of each of them, and also the connections between these steps. These can be helpful to explore the Pipeline locally.
 
-### Running a Pipeline
+### `distilabel pipeline run`
 
 We can also run a `Pipeline` from the CLI just pointing to the same `pipeline.yaml` file or an URL pointing to it and calling `distilabel pipeline run`:
 
 ```bash
 $ distilabel pipeline run --help
 
  Usage: distilabel pipeline run [OPTIONS]
```

### Comparing `distilabel-1.0.3/docs/sections/learn/llms/index.md` & `distilabel-1.1.0/docs/sections/learn/tutorial/llm/index.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# LLMs
+# LLM
 
 The LLMs are implemented as subclasses of either [`LLM`][distilabel.llms.LLM] or [`AsyncLLM`][distilabel.llms.AsyncLLM], and are only in charge of running the text generation for a given prompt or conversation. The LLMs are intended to be used together with the [`Task`][distilabel.steps.tasks.Task] and any of its subclasses, via the `llm` argument, this means that any of the implemented LLMs can be easily plugged seamlessly into any task.
 
 ## Working with LLMs
 
 The subclasses of both [`LLM`][distilabel.llms.LLM] or [`AsyncLLM`][distilabel.llms.AsyncLLM] are intended to be used within the scope of a [`Task`][distilabel.steps.tasks.Task], since those are seamlessly integrated within the different tasks; but nonetheless, they can be used standalone if needed.
 
@@ -23,15 +23,15 @@
 ```
 
 !!! NOTE
     The `load` method needs to be called ALWAYS if using the LLMs as standalone or as part of a task, otherwise, if the `Pipeline` context manager is used, there's no need to call that method, since it will be automatically called on `Pipeline.run`; but in any other case the method `load` needs to be called from the parent class e.g. a `Task` with an `LLM` will need to call `Task.load` to load both the task and the LLM.
 
 ### Within a Task
 
-Now, in order to use the LLM within a [Task][distilabel.steps.tasks.Task], we need to pass it as an argument to the task, and the task will take care of the rest.
+Now, in order to use the LLM within a [`Task`][distilabel.steps.tasks.Task], we need to pass it as an argument to the task, and the task will take care of the rest.
 
 ```python
 from distilabel.llms import OpenAILLM
 from distilabel.steps.tasks import TextGeneration
 
 
 llm = OpenAILLM(model="gpt-4")
@@ -41,15 +41,15 @@
 
 next(task.process(inputs=[{"instruction": "What's the capital of Spain?"}]))
 # [{'instruction': "What's the capital of Spain?", "generation": "The capital of Spain is Madrid."}]
 ```
 
 ### Runtime Parameters
 
-Additionally, besides the runtime parameters that can / need to be provided to the [Task][distilabel.steps.tasks], the LLMs can also define their own runtime parameters such as the `generation_kwargs`, and those need to be provided within the `Pipeline.run` method via the variable `params`.
+Additionally, besides the runtime parameters that can / need to be provided to the [`Task`][distilabel.steps.tasks], the LLMs can also define their own runtime parameters such as the `generation_kwargs`, and those need to be provided within the `Pipeline.run` method via the argument `params`.
 
 !!! NOTE
     Each LLM subclass may have its own runtime parameters and those can differ between the different implementations, as those are not aligned, since the LLM engines offer different functionalities.
 
 ```python
 from distilabel.pipeline import Pipeline
 from distilabel.llms import OpenAILLM
@@ -67,47 +67,53 @@
         ],
     )
 
     text_generation = TextGeneration(
         name="text_generation",
         llm=OpenAILLM(model="gpt-4"),
     )
-    load_dataset.connect(text_generation)
+
+    load_dataset >> text_generation
 
 if __name__ == "__main__":
-    pipeline.run(params={"text_generation": {"llm": {"generation_kwargs": {"temperature": 0.3}}}})
+    pipeline.run(
+        parameters={
+            text_generation.name: {"llm": {"generation_kwargs": {"temperature": 0.3}}},
+        },
+    )
 ```
 
 ## Defining custom LLMs
 
 In order to define custom LLMs, one must subclass either [`LLM`][distilabel.llms.LLM] or [`AsyncLLM`][distilabel.llms.AsyncLLM], to define a synchronous or asynchronous LLM, respectively.
 
 One can either extend any of the existing LLMs to override the default behaviour if needed, but also to define a new one from scratch, that could be potentially contributed to the `distilabel` codebase.
 
 In order to define a new LLM, one must define the following methods:
 
-* `model_name`: is a property that contains the name of the model to be used, which means that it needs to be retrieved from the LLM using the LLM-specific approach i.e. for `TransformersLLM` the `model_name` will be the `model_name_or_path` provided as an argument, or in `OpenAILLM` the `model_name` will be the `model` provided as an argument.
+* `model_name`: is a property that contains the name of the model to be used, which means that it needs to be retrieved from the LLM using the LLM-specific approach i.e. for [`TransformersLLM`][distilabel.llms.TransformersLLM] the `model_name` will be the `model_name_or_path` provided as an argument, or in [`OpenAILLM`][distilabel.llms.OpenAILLM] the `model_name` will be the `model` provided as an argument.
 
-* `generate`: is a method that will take a list of prompts and return a list of generated texts. This method will be called by the `Task` to generate the texts, so it's the most important method to define. This method will be implemented in the subclass of the [LLM][distilabel.llms.LLM] i.e. the synchronous LLM.
+* `generate`: is a method that will take a list of prompts and return a list of generated texts. This method will be called by the [`Task`][distilabel.steps.tasks.Task] to generate the texts, so it's the most important method to define. This method will be implemented in the subclass of the [`LLM`][distilabel.llms.LLM] i.e. the synchronous LLM.
 
-* `agenerate`: is a method that will take a single prompt and return a list of generated texts, since the rest of the behaviour will be controlled by the `generate` method that cannot be overwritten when subclassing [AsyncLLM][distilabel.llms.AsyncLLM]. This method will be called by the `Task` to generate the texts, so it's the most important method to define. This method will be implemented in the subclass of the [AsyncLLM][distilabel.llms.AsyncLLM] i.e. the asynchronous LLM.
+* `agenerate`: is a method that will take a single prompt and return a list of generated texts, since the rest of the behaviour will be controlled by the `generate` method that cannot be overwritten when subclassing [`AsyncLLM`][distilabel.llms.AsyncLLM]. This method will be called by the [`Task`][distilabel.steps.tasks.Task] to generate the texts, so it's the most important method to define. This method will be implemented in the subclass of the [`AsyncLLM`][distilabel.llms.AsyncLLM] i.e. the asynchronous LLM.
 
-* (optional) `get_last_hidden_state`: is a method that will take a list of prompts and return a list of hidden states. This method is optional and will be used by some tasks such as the [GenerateEmbeddings][distilabel.steps.tasks] task.
+* (optional) `get_last_hidden_state`: is a method that will take a list of prompts and return a list of hidden states. This method is optional and will be used by some tasks such as the [`GenerateEmbeddings`][distilabel.steps.tasks.GenerateEmbeddings] task.
 
 Once those methods have been implemented, then the custom LLM will be ready to be integrated within either any of the existing or a new task.
 
 ```python
 from typing import Any
 
 from pydantic import validate_call
 
 from distilabel.llms import AsyncLLM, LLM
 from distilabel.llms.typing import GenerateOutput, HiddenState
 from distilabel.steps.tasks.typing import ChatType
 
+
 class CustomLLM(LLM):
     @property
     def model_name(self) -> str:
         return "my-model"
 
     @validate_call
     def generate(self, inputs: List[ChatType], num_generations: int = 1, **kwargs: Any) -> List[GenerateOutput]:
@@ -137,21 +143,22 @@
 !!! NOTE
     To have the arguments of the `generate` and `agenerate` coerced to the expected types, the `validate_call` decorator is used, which will automatically coerce the arguments to the expected types, and raise an error if the types are not correct. This is specially useful when providing a value for an argument of `generate` or `agenerate` from the CLI, since the CLI will always provide the arguments as strings.
 
 ## Available LLMs
 
 Here's a list with the available LLMs that can be used within the `distilabel` library:
 
-* [AnthropicLLM][distilabel.llms.anthropic]
-* [AnyscaleLLM][distilabel.llms.anyscale]
-* [AzureOpenAILLM][distilabel.llms.azure]
-* [CohereLLM][distilabel.llms.cohere]
-* [InferenceEndpointsLLM][distilabel.llms.huggingface.inference_endpoints]
-* [LiteLLM][distilabel.llms.litellm]
-* [LlamaCppLLM][distilabel.llms.llamacpp]
-* [MistralLLM][distilabel.llms.mistral]
-* [OllamaLLM][distilabel.llms.ollama]
-* [OpenAILLM][distilabel.llms.openai]
-* [TogetherLLM][distilabel.llms.together]
-* [TransformersLLM][distilabel.llms.huggingface.transformers]
-* [VertexAILLM][distilabel.llms.vertexai]
-* [vLLM][distilabel.llms.vllm]
+* [AnthropicLLM][distilabel.llms.AnthropicLLM]
+* [AnyscaleLLM][distilabel.llms.AnyscaleLLM]
+* [AzureOpenAILLM][distilabel.llms.AzureOpenAILLM]
+* [CohereLLM][distilabel.llms.CohereLLM]
+* [GroqLLM][distilabel.llms.GroqLLM]
+* [InferenceEndpointsLLM][distilabel.llms.huggingface.InferenceEndpointsLLM]
+* [LiteLLM][distilabel.llms.LiteLLM]
+* [LlamaCppLLM][distilabel.llms.LlamaCppLLM]
+* [MistralLLM][distilabel.llms.MistralLLM]
+* [OllamaLLM][distilabel.llms.OllamaLLM]
+* [OpenAILLM][distilabel.llms.OpenAILLM]
+* [TogetherLLM][distilabel.llms.TogetherLLM]
+* [TransformersLLM][distilabel.llms.huggingface.TransformersLLM]
+* [VertexAILLM][distilabel.llms.VertexAILLM]
+* [vLLM][distilabel.llms.vLLM]
```

### Comparing `distilabel-1.0.3/docs/sections/learn/pipelines/index.md` & `distilabel-1.1.0/docs/sections/learn/tutorial/pipeline/index.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 # Pipeline
 
-The [`Pipeline`][distilabel.pipeline.local.Pipeline] is the central point in `distilabel`, the way to organize the steps to create your datasets. Up to this point we've seen how we can define different [`Steps`](../steps/index.md) and [`Tasks`](../tasks/index.md), that together with an [`LLM`](.) are the building blocks of our datasets, in this section we will take a look at how all these blocks are organized inside a `Pipeline`.
+The [`Pipeline`][distilabel.pipeline.Pipeline] is the central point in `distilabel`, the way to organize the steps to create your datasets. Up to this point we've seen how we can define different [`Step`][distilabel.steps.Step] and [`Task`][distilabel.steps.tasks.Task] subclasses in [Tutorial - Step](../step/index.md) and [Tutorial - Task](../task/index.md), respectively; which together with an [`LLM`][distilabel.llms.LLM] are the building blocks of our datasets, in this section we will take a look at how all these blocks are organized inside a [`Pipeline`][distilabel.pipeline.Pipeline].
 
 !!! Note
-    Currently `distilabel` implements a *local* version of a `Pipeline`, and will assume that's the only definition, but this can be extended in the future to include remote execution of the `Pipeline`.
+    Currently `distilabel` implements a *local* version of a [`Pipeline`][distilabel.pipeline.Pipeline], and will assume that's the only definition, but this can be extended in the future to include remote execution of the [`Pipeline`][distilabel.pipeline.Pipeline].
 
 ## How to create a pipeline
 
-The most common way a `Pipeline` should be created is by making use of the context manager, we just need to give our `Pipeline` a **name**, and optionally a **description**, and that's it[^1]:
+The most common way a [`Pipeline`][distilabel.pipeline.Pipeline] should be created is by making use of the context manager, we just need to give our [`Pipeline`][distilabel.pipeline.Pipeline] a **name**, and optionally a **description**, and that's it[^1]:
 
 ```python
 from distilabel.pipeline import Pipeline
 
 with Pipeline("pipe-name", description="My first pipe") as pipeline:  # (1)
     ...
 
 ```
 
-1. Use the context manager to create a `Pipeline` with a name and an optional description.
+1. Use the context manager to create a [`Pipeline`][distilabel.pipeline.Pipeline] with a name and an optional description.
 
-This way, we ensure all the steps we define there are connected with each other under the same `Pipeline`. The next step is to define the steps of our `Pipeline`. It's mandatory that the root steps of the pipeline i.e. the ones that doesn't have any predecessors, are `GeneratorStep`s such as [`LoadDataFromDicts`](/distilabel/api/steps/generator_steps/generator_steps/#distilabel.steps.generators.data.LoadDataFromDicts) or [`LoadHubDataset`](/distilabel/api/steps/generator_steps/generator_steps/#distilabel.steps.generators.huggingface.LoadHubDataset).
+This way, we ensure all the steps we define there are connected with each other under the same [`Pipeline`][distilabel.pipeline.Pipeline]. The next step is to define the steps of our [`Pipeline`][distilabel.pipeline.Pipeline]. It's mandatory that the root steps of the pipeline i.e. the ones that doesn't have any predecessors, are [`GeneratorStep`][distilabel.steps.GeneratorStep]s such as [`LoadDataFromDicts`][distilabel.steps.LoadDataFromDicts] or [`LoadHubDataset`][distilabel.steps.LoadHubDataset].
 
 ```python
 from distilabel.pipeline import Pipeline
 from distilabel.steps import LoadHubDataset
 
 with Pipeline("pipe-name", description="My first pipe") as pipeline:
     load_dataset = LoadHubDataset(name="load_dataset")  # (1)
     ...
 
 ```
 
 1. Define the first step of the pipeline, in this case `LoadHubDataset`, a `GeneratorStep` used to load a dataset from the Hugging Face Hub.
 
-Once we have a source of data, we can create another `Step`s that will consume and process the data generated by the `GeneratorStep`s. Let's assume that the dataset we're going to load from the Hub contains a `prompt` column and that we want to generate texts based on this prompt. We also want to use several `LLM`s for this task. To do so, we will create several `TextGeneration` tasks, each with a different `LLM`.  
+Once we have a source of data, we can create another [`Step`][distilabel.steps.Step]s that will consume and process the data generated by the `GeneratorStep`s. Let's assume that the dataset we're going to load from the Hub contains a `prompt` column and that we want to generate texts based on this prompt. We also want to use several `LLM`s for this task. To do so, we will create several `TextGeneration` tasks, each with a different `LLM`.
 
 ```python
 from distilabel.llms import MistralLLM, OpenAILLM, VertexAILLM
 from distilabel.pipeline import Pipeline
 from distilabel.steps import LoadHubDataset
 from distilabel.steps.tasks import TextGeneration
 
@@ -57,15 +57,15 @@
 
 1. Create a `TextGeneration` task for each `LLM` we want to use.
 2. Connect the `TextGeneration` task with the `LoadHubDataset` step, so the output data from the dataset is passed to the task.
 
 !!! NOTE
     The order of the execution of the steps will be determined by the connections of the steps. In this case, the `TextGeneration` tasks will be executed after the `LoadHubDataset` step.
 
-For each row of the dataset, the `TextGeneration` task will generate a text based on the `instruction` column and the `LLM` model, and store the result (a single string) in a new column called `generation`. As we would like to have all the `response`s in the same column, we will add an extra step to combine them all in the same column, so the value of this column is a list of strings or responses. 
+For each row of the dataset, the `TextGeneration` task will generate a text based on the `instruction` column and the `LLM` model, and store the result (a single string) in a new column called `generation`. As we would like to have all the `response`s in the same column, we will add an extra step to combine them all in the same column, so the value of this column is a list of strings or responses.
 
 ```python
 from distilabel.llms import MistralLLM, OpenAILLM, VertexAILLM
 from distilabel.pipeline import Pipeline
 from distilabel.steps import CombineColumns, LoadHubDataset
 from distilabel.steps.tasks import TextGeneration
 
@@ -87,21 +87,155 @@
         load_dataset.connect(task)
         task.connect(combine_generations)  # (2)
 ```
 
 1. Create a `CombineColumns` step to combine all the `generation` columns into a single column called `generations` and the `model_name` columns into a single column called `model_names`.
 2. Connect the `TextGeneration` task with the `CombineColumns` step, so the output data from the task is passed to the step that will combine all the `generation` columns.
 
-As the `CombineColumns` is the last step or it's a leaf step of the pipeline because it doesn't have any successors, that means that the outputs of this step will be included in the returned [`Distiset`](/distilabel/sections/learn/distiset) by the pipeline.
+As the [`CombineColumns`][distilabel.steps.CombineColumns] is the last step or it's a leaf step of the pipeline because it doesn't have any successors, that means that the outputs of this step will be included in the returned [`Distiset`][distilabel.distiset.Distiset] (more information about it in [Advanced - Distiset](../../advanced/distiset.md)).
 
 !!! NOTE
     One pipeline can have several leaf steps, which means that the outputs of all the leaf steps will be included in the returned `Distiset`, which will contain several subsets, one for each leaf step.
 
+### Connecting steps
+
+In the previous example we saw how to create a `Pipeline` and connect different steps using the `Step.connect` method: `step1.connect(step2)`, but there's an alternative way by making use of the `>>` operator, let's see how using the previous `Pipeline` as an example:
+
+=== "Step per step"
+
+    Each call to `step1.connect(step2)` has been exchanged by `step1 >> step2`:
+
+    ```python
+    from distilabel.llms import MistralLLM, OpenAILLM, VertexAILLM
+    from distilabel.pipeline import Pipeline
+    from distilabel.steps import CombineColumns, LoadHubDataset
+    from distilabel.steps.tasks import TextGeneration
+
+    with Pipeline("pipe-name", description="My first pipe") as pipeline:
+        load_dataset = LoadHubDataset(name="load_dataset")
+
+        combine_generations = CombineColumns(
+            name="combine_generations",
+            columns=["generation", "model_name"],
+            output_columns=["generations", "model_names"],
+        )
+
+        for llm in (
+            OpenAILLM(model="gpt-4-0125-preview"),
+            MistralLLM(model="mistral-large-2402"),
+            VertexAILLM(model="gemini-1.5-pro"),
+        ):
+            task = TextGeneration(name=f"text_generation_with_{llm.model_name}", llm=llm)
+            load_dataset >> task >> combine_generations  # (1)
+    ```
+
+    1. Here `load_dataset >> task >> combine_generations` was exchanged with `load_dataset.connect(task).connect(combine_generations)`.
+
+
+=== "Multiple steps at once"
+
+    All the calls to connections from the `load_dataset` step to the different `task` objects are done in a single call:
+
+    ```python
+    from distilabel.llms import MistralLLM, OpenAILLM, VertexAILLM
+    from distilabel.pipeline import Pipeline
+    from distilabel.steps import CombineColumns, LoadHubDataset
+    from distilabel.steps.tasks import TextGeneration
+
+    with Pipeline("pipe-name", description="My first pipe") as pipeline:
+        load_dataset = LoadHubDataset(name="load_dataset")
+
+        combine_generations = CombineColumns(
+            name="combine_generations",
+            columns=["generation", "model_name"],
+            output_columns=["generations", "model_names"],
+        )
+
+        tasks = []
+        for llm in (
+            OpenAILLM(model="gpt-4-0125-preview"),
+            MistralLLM(model="mistral-large-2402"),
+            VertexAILLM(model="gemini-1.5-pro"),
+        ):
+            tasks.append(
+                TextGeneration(name=f"text_generation_with_{llm.model_name}", llm=llm)
+            )
+
+        load_dataset >> tasks >> combine_generations  # (1)
+    ```
+
+    1. Notice how `tasks` is a list of different `Tasks`. In a single call to the operator we are connecting `load_dataset` with all the `tasks`, and all of those again to `combine_generations`.
+
+
+### Routing batches to specific downstream steps
+
+In some pipelines, it's likely that you will need to have a list of downstream steps receiving batches from the same upstream step, but you would like to route the batches to specific downstream steps based on some condition. To do so, you can use a `routing_batch_function`, which is a simple function that receives a list of the downstream steps to which a batch can be routed, and returns a list containing the names of steps to which the batch should be routed. Let's update the example above to route the batches loaded by the `LoadHubDataset` step to just 2 of the `TextGeneration` tasks. First, we will create our custom [`routing_batch_function`][distilabel.pipeline.routing_batch_function.routing_batch_function], and then we will update the pipeline to use it:
+
+```python
+import random
+from distilabel.llms import MistralLLM, OpenAILLM, VertexAILLM
+from distilabel.pipeline import Pipeline, routing_batch_function
+from distilabel.steps import CombineColumns, LoadHubDataset
+from distilabel.steps.tasks import TextGeneration
+
+@routing_batch_function
+def sample_two_steps(steps: list[str]) -> list[str]:
+    return random.sample(steps, 2)
+
+with Pipeline("pipe-name", description="My first pipe") as pipeline:
+    load_dataset = LoadHubDataset(
+        name="load_dataset",
+        output_mappings={"prompt": "instruction"},
+    )
+
+    tasks = []
+    for llm in (
+        OpenAILLM(model="gpt-4-0125-preview"),
+        MistralLLM(model="mistral-large-2402"),
+        VertexAILLM(model="gemini-1.0-pro"),
+    ):
+        tasks.append(
+            TextGeneration(name=f"text_generation_with_{llm.model_name}", llm=llm)
+        )
+
+    combine_generations = CombineColumns(
+        name="combine_generations",
+        columns=["generation", "model_name"],
+        output_columns=["generations", "model_names"],
+    )
+
+    load_dataset >> sample_two_steps >> tasks >> combine_generations
+```
+
+As it can be seen, the `routing_batch_function` can be used with the `>>` operator to route the batches to specific downstream steps. In this case, each batch yielded by the `load_dataset` step will be routed to just 2 of the `TextGeneration` tasks, and then all the outputs of the tasks will be combined in the `CombineColumns` step so each row of the final dataset will contain generations of 2 `LLM`s at most. The `routing_batch_function` that we just built is a common one, so `distilabel` comes with an auxiliary function that can be used to achieve the same behavior:
+
+```python
+from distilable.pipeline import sample_n_steps
+
+sample_two_steps = sample_n_steps(2)
+```
+
 ## Running the pipeline
 
+### Pipeline.dry_run
+
+Before running the `Pipeline` we may want to check all the components behave as expected. We can do a `dry_run` for this case:
+
+```python
+with Pipeline("pipe-name", description="My first pipe") as pipeline:
+    ...
+
+if __name__ == "__main__":
+    distiset = pipeline.dry_run(parameters=..., batch_size=1)
+```
+
+It takes the same parameters as the `run` method we will see in the following section, plus the `batch_size` we want the dry run to use (by default set to 1). In this case, the `Pipeline` would select a single example from our generator steps and pass through all the steps. Assuming the `dry_run` runs successfully, we are ready to run our pipeline.
+
+### Pipeline.run
+
 Once we have created the pipeline, we can run it. To do so, we need to call the `run` method of the `Pipeline`, and specify the runtime parameters for each step:
 
 ```python
 with Pipeline("pipe-name", description="My first pipe") as pipeline:
     ...
 
 if __name__ == "__main__":
@@ -138,16 +272,16 @@
         },
     )
 ```
 
 But if we run it, we will see that the `run` method will fail:
 
 ```
-ValueError: Step 'text_generation_with_gpt-4-0125-preview' requires inputs ['instruction'] which are not available when the step gets to be executed in the pipeline. Please make sure previous steps to 'text_generation_with_gpt-4-0125-preview' are 
-generating the required inputs. Available inputs are: ['prompt', 'completion', 'meta']
+ValueError: Step 'text_generation_with_gpt-4-0125-preview' requires inputs ['instruction'], but only the inputs=['prompt', 'completion', 'meta'] are available, which means that the inputs=['instruction'] are missing or not available
+when the step gets to be executed in the pipeline. Please make sure previous steps to 'text_generation_with_gpt-4-0125-preview' are generating the required inputs.
 ```
 
 This is because, before actually running the pipeline, the pipeline is validated to verify that everything is correct and all the steps in the pipeline are chainable i.e. each step has the necessary inputs to be executed. In this case, the `TextGeneration` task requires the `instruction` column, but the `LoadHubDataset` step generates the `prompt` column. To solve this, we can use the `output_mappings` argument that every `Step` has, to map or rename the output columns of a step to the required input columns of another step:
 
 ```python
 with Pipeline("pipe-name", description="My first pipe") as pipeline:
     load_dataset = LoadHubDataset(
@@ -164,14 +298,24 @@
 
 ```python
 if __name__ == "__main__":
     distiset = pipeline.run(...)
     distiset.push_to_hub("distilabel-internal-testing/instruction-dataset-mini-with-generations")
 ```
 
+### Stopping the pipeline
+
+In case you want to stop the pipeline while it's running using the `Ctrl+c` (`Cmd+c` in macos), we automatically catch the signal and try to finish whatever steps are currently running. If it got hang by some reason, repeating the command 2 times it will force the pipeline close.
+
+!!! Note
+
+    When pushing sending the signal to kill the process, you can expect to see the following log messages:
+
+    ![Pipeline ctrl+c](../../../../assets/images/sections/pipeline/pipeline-ctrlc.png)
+
 ## Cache
 
 If we try to execute the pipeline again, the pipeline won't execute as it will load the dataset from the cache, and the outputs of the pipeline will be the same as the previous run. If for some reason, we decide to stop the pipeline execution in the middle of the process pressing CTRL + C, the pipeline will stop and the state of the pipeline and the outputs will be stored in the cache, so we can resume the pipeline execution from the point where it was stopped.
 
 If we want to force the pipeline to run again, then we can use the `use_cache` argument of the `run` method and set it to `False`:
 
 ```python
@@ -194,15 +338,15 @@
 
     for llm in (
         OpenAILLM(model="gpt-4-0125-preview"),
         MistralLLM(model="mistral-large-2402"),
         VertexAILLM(model="gemini-1.5-pro"),
     ):
         task = TextGeneration(
-            name=f"text_generation_with_{llm.model_name}", 
+            name=f"text_generation_with_{llm.model_name}",
             llm=llm,
             input_batch_size=5,  # (1)
         )
 
     ...
 ```
 
@@ -236,15 +380,15 @@
 
 To load the pipeline, we can use the `from_yaml` or `from_json` methods:
 
 ```python
 pipeline = Pipeline.from_yaml("pipeline.yaml")
 ```
 
-Serializing the pipeline is very useful when we want to share the pipeline with others, or when we want to store the pipeline for future use. It can even be hosted online, so the pipeline can be executed directly using the [CLI](/distilabel/sections/learn/cli) knowing the URL of the pipeline.
+Serializing the pipeline is very useful when we want to share the pipeline with others, or when we want to store the pipeline for future use. It can even be hosted online, so the pipeline can be executed directly using the [CLI](../cli/index.md) knowing the URL of the pipeline.
 
 ## Fully working example
 
 To sump up, here is the full code of the pipeline we have created in this section. Note that you will need to change the name of the Hugging Face repository where the resulting will be pushed, set `OPENAI_API_KEY` environment variable, set `MISTRAL_API_KEY` and have `gcloud` installed and configured:
 
 ??? Code
     ```python
@@ -308,8 +452,8 @@
             },
         )
         distiset.push_to_hub(
             "distilabel-internal-testing/instruction-dataset-mini-with-generations"
         )
     ```
 
-[^1]: We also have the *cache_dir* argument to pass, for more information on this parameter, we refer the reader to the [caching](../caching.md) section.
+[^1]: We also have the *cache_dir* argument to pass, for more information on this parameter, we refer the reader to the [caching](../../advanced/caching.md) section.
```

### Comparing `distilabel-1.0.3/docs/sections/learn/steps/index.md` & `distilabel-1.1.0/src/distilabel/steps/tasks/ultrafeedback.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,167 +1,235 @@
-# Steps
-
-The [`Step`][distilabel.steps.base.Step] is the base class in `distilabel`, every unit of work in a `Pipeline` will inherit from it.
-
-## What's a Step in distilabel?
-
-It's a base class is in charge of processing data, which in the end will be lists of dictionaries. In order to process, it defines two properties: `inputs` and `outputs`, which are a list of strings that represent the names of the columns that the step needs as input or output respectively i.e. the keys that have to be present in the list of dictionaries received by the step and the keys that will be added to these dictionaries after running it.
-
-Every `Step` is connected to a `Pipeline`, which in practice means that we will build them in the context of a `Pipeline`.
-
-Lastly, these steps inherit from `pydantic.BaseModel`, so all the attributes of a step will be validated upon definition.
-
-## An example: ConversationTemplate
+# Copyright 2023-present, Argilla, Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import re
+import sys
+
+if sys.version_info < (3, 9):
+    import importlib_resources
+else:
+    import importlib.resources as importlib_resources
+
+from typing import Any, Dict, List, Literal, Optional, Union
+
+from jinja2 import Template
+from pydantic import PrivateAttr
+
+from distilabel.steps.tasks.base import Task
+from distilabel.steps.tasks.typing import ChatType
+from distilabel.utils.dicts import combine_dicts
+
+
+class UltraFeedback(Task):
+    """Rank generations focusing on different aspects using an `LLM`.
+
+    UltraFeedback: Boosting Language Models with High-quality Feedback.
+
+    Attributes:
+        aspect: The aspect to perform with the `UltraFeedback` model. The available aspects are:
+            - `helpfulness`: Evaluate text outputs based on helpfulness.
+            - `honesty`: Evaluate text outputs based on honesty.
+            - `instruction-following`: Evaluate text outputs based on given instructions.
+            - `truthfulness`: Evaluate text outputs based on truthfulness.
+            Additionally, a custom aspect has been defined by Argilla, so as to evaluate the overall
+            assessment of the text outputs within a single prompt. The custom aspect is:
+            - `overall-rating`: Evaluate text outputs based on an overall assessment.
+
+    Input columns:
+        - instruction (`str`): The reference instruction to evaluate the text outputs.
+        - generations (`List[str]`): The text outputs to evaluate for the given instruction.
+
+    Output columns:
+        - ratings (`List[float]`): The ratings for each of the provided text outputs.
+        - rationales (`List[str]`): The rationales for each of the provided text outputs.
+        - model_name (`str`): The name of the model used to generate the ratings and rationales.
+
+    Categories:
+        - preference
+
+    References:
+        - [`UltraFeedback: Boosting Language Models with High-quality Feedback`](https://arxiv.org/abs/2310.01377)
+        - [`UltraFeedback - GitHub Repository`](https://github.com/OpenBMB/UltraFeedback)
+    """
+
+    aspect: Literal[
+        "helpfulness",
+        "honesty",
+        "instruction-following",
+        "truthfulness",
+        # Custom aspects
+        "overall-rating",
+    ]
+
+    _system_prompt: str = PrivateAttr(
+        default=(
+            "Your role is to evaluate text quality based on given criteria.\n"
+            'You\'ll receive an instructional description ("Instruction") and {no_texts} text outputs ("Text").\n'
+            "Understand and interpret instructions to evaluate effectively.\n"
+            "Provide annotations for each text with a rating and rationale.\n"
+            "The {no_texts} texts given are independent, and should be evaluated separately.\n"
+        )
+    )
+    _template: Optional["Template"] = PrivateAttr(default=...)
 
-Let's see one simple type of step as an example, the [`ConversationTemplate`][distilabel.steps.conversation.ConversationTemplate]. Let's take a look at it's definition (the docstrings are removed for clarity, but it can be reviewd in the API reference):
+    def load(self) -> None:
+        """Loads the Jinja2 template for the given `aspect`."""
+        super().load()
+
+        _path = str(
+            importlib_resources.files("distilabel")
+            / "steps"
+            / "tasks"
+            / "templates"
+            / "ultrafeedback"
+            / f"{self.aspect}.jinja2"
+        )
 
-```python
-class ConversationTemplate(Step):
+        self._template = Template(open(_path).read())
 
     @property
     def inputs(self) -> List[str]:
-        return ["instruction", "response"]
-
-    @property
-    def outputs(self) -> List[str]:
-        return ["conversation"]
-
-    def process(self, inputs: StepInput) -> "StepOutput":
-        for input in inputs:
-            input["conversation"] = [
-                {"role": "user", "content": input["instruction"]},
-                {"role": "assistant", "content": input["response"]},
-            ]
-        yield inputs
-```
-
-At the very minimal, we need to define the `inputs` and `outputs` properties with the column names required as input, and returned as output respectively, and the processing logic of the step in the `process` method.
-
-In this example, we see that it takes `inputs` as argument, annotated as `StepInput`, which is a list of dictionaries with the data, and *yields* a `StepOutput`.
-
-### Working with the step
-
-Let's see how to instantiate this `Step` outside of a `Pipeline`:
-
-```python
-from distilabel.pipeline.local import Pipeline
-from distilabel.steps.conversation import ConversationTemplate
-
-conversation_template = ConversationTemplate(
-    name="my-conversation-template",
-    pipeline=Pipeline(name="my-pipeline"),
-)
-```
-
-As we mentioned, every `Step` must be defined in the context of a `Pipeline`, which means we need to pass it as an argument if we decide to create a standalone step. If we take a look at the `conversation_template` step, we see the following fields:
-
-```python
-conversation_template
-# ConversationTemplate(name='my-conversation-template', input_mappings={}, output_mappings={}, input_batch_size=50)
-```
-
-- The `name` of the `Step`, a mandatory field to identify the `Step` within the `Pipeline`. 
-- `input_mappings`, which is a dictionary that can be useful to map keys from the input dictionaries to the keys expected by the step. For example, if `input_mappings={"instruction": "prompt"}`, that means that the key `prompt` from the input dictionaries will be used as the key `instruction` for the step.
-- `output_mappings`, which is a dictionary that can be used to map the `outputs` of the step to other names. For example, if `output_mappings={"conversation": "prompt"}`, that means that the key `conversation` generated by the step will be renamed to `prompt` and the output dictionaries of this step will contain a key called `prompt` instead of `conversation`.
-- `input_batch_size` (by default set to 50), which is independent for every step and will determine how many input dictionaries will process at once. If won't matter that much in this step, but as we will see later, other types of steps will come with an `LLM`, so having this flexibility will be really useful.
-
-### Processing data
-
-Internally, the `Pipeline` will call the `process` method when appropriate, but we can see it in action with some dummy data:
-
-```python
-next(conversation_template.process([{"instruction": "Hello", "response": "Hi"}]))
-# [
-#   {
-#     "instruction": "Hello",
-#     "response": "Hi",
-#     "conversation": [
-#       {
-#         "role": "user",
-#         "content": "Hello"
-#       },
-#       {
-#         "role": "assistant",
-#         "content": "Hi"
-#       }
-#     ]
-#   }
-# ]
-```
-
-It takes the dictionary with data, adds another `conversation` with the data formatted as a conversation template, and passes this data to the following step.
-
-This is a small type step that shows what to expect when we are creating our `Step` objects, which can start from something as simple as generating a conversation template from some columns on a dataset.
-
-
-## Runtime Parameters
-
-Let's take a look at a special argument implementation that we will find when dealing with the `Steps`, the [Runtime parameters][distilabel.mixins.runtime_parameters.RuntimeParameter]. Let's inspect them using the previous example class:
-
-```python
-print(conversation_template.runtime_parameters_names)
-# {'input_batch_size': True}
-```
-
-The `ConversationTemplate` only has one `runtime_parameter`, which comes defined from the `Step` class, and can be defined as such:
-
-```python
-from distilabel.mixins.runtime_parameters import RuntimeParameter
-
-class Step(...):
-    ...
-    input_batch_size: RuntimeParameter[PositiveInt] = Field(
-        default=DEFAULT_INPUT_BATCH_SIZE,
-        description="The number of rows that will contain the batches processed by the"
-        " step.",
-    )
-```
-
-When we define the `input_batch_size` as a `RuntimeParameter`, the most direct effect we can see is we have some access to some extra information, thanks to the [RuntimeParamatersMixin][distilabel.mixins.runtime_parameters.RuntimeParametersMixin]:
-
-```python
-print(conversation_template.get_runtime_parameters_info())
-# [{'name': 'input_batch_size', 'optional': True, 'description': 'The number of rows that will contain the batches processed by the step.'}]
-```
+        """The input for the task is the `instruction`, and the `generations` for it."""
+        return ["instruction", "generations"]
 
-But other than accessing some extra information internally, we can directly interact with these parameters when we interacting or modifying the arguments of our `Steps` while running them in the context of a `Pipeline`. We will see them in action once we interact with the `Steps` inside of a `Pipeline`.
-
-## step decorator
-
-If all that we want to apply in a step is some simple processing, it can be easier to just create a plain function, and decorate it. We can find more examples in the [API reference][distilabel.steps.decorator], but let's see how we could define the previous step as a function and use the decorator:
-
-```python
-from distilabel.steps import StepInput, StepOutput, step 
-
-# Normal step
-@step(inputs=["instruction", "response"], outputs=["conversation"])
-def ConversationTemplate(inputs: StepInput) -> StepOutput:
-    for input in inputs:
-        input["conversation"] = [
-            {"role": "user", "content": input["instruction"]},
-            {"role": "assistant", "content": input["response"]},
+    def format_input(self, input: Dict[str, Any]) -> ChatType:
+        """The input is formatted as a `ChatType` assuming that the instruction
+        is the first interaction from the user within a conversation."""
+        return [
+            {
+                "role": "system",
+                "content": self._system_prompt.format(
+                    no_texts=len(input["generations"])
+                ),
+            },
+            {
+                "role": "user",
+                "content": self._template.render(  # type: ignore
+                    instruction=input["instruction"], generations=input["generations"]
+                ),
+            },
         ]
-    yield inputs
-```
-
-Which can be instantiated exactly the same as the `ConversationTemplate` class:
-
-```python
-conversation_template = ConversationTemplate(
-    name="my-conversation-template",
-    pipeline=Pipeline(name="my-pipeline"),
-)
-```
-
-This `@step` decorator has a special type depending `step_type` which will be better understood once we see the different types of steps.
 
-## Types of steps
-
-Other than the general or normal steps we have seen, there are special types of steps that have a restricted behaviour compared to the general `Step`.
-
-### Generator steps
-
-These are steps that are able to generate data, and don't need to receive any input from previous step, as it's implied in the normal steps. The typical use for these steps will be loading data for example, as can be seen in [`LoadDataFromDicts`][distilabel.steps.generators.data]. For this type of steps we will only need to define the `process` method, and we can optionally pass a `batch_size` argument, that will determine the batch size of the generated batches.
-
-### Global steps
-
-Other special type of step are the global steps. These steps don't have any `inputs` or `outputs`, and their `process` method receives all the data at once instead of using batches. This kind of behavior is necessary for example to push a dataset to a specific place, or doing some filtering on the whole data before continuing with the pipeline.
+    @property
+    def outputs(self) -> List[str]:
+        """The output for the task is the `generation` and the `model_name`."""
+        columns = []
+        if self.aspect in ["honesty", "instruction-following", "overall-rating"]:
+            columns = ["ratings", "rationales"]
+        elif self.aspect in ["helpfulness", "truthfulness"]:
+            columns = ["types", "rationales", "ratings", "rationales-for-ratings"]
+        return columns + ["model_name"]
+
+    def format_output(
+        self, output: Union[str, None], input: Dict[str, Any]
+    ) -> Dict[str, Any]:
+        """The output is formatted as a dictionary with the `ratings` and `rationales` for
+        each of the provided `generations` for the given `instruction`. The `model_name`
+        will be automatically included within the `process` method of `Task`.
+
+        Args:
+            output: a string representing the output of the LLM via the `process` method.
+            input: the input to the task, as required by some tasks to format the output.
+
+        Returns:
+            A dictionary containing either the `ratings` and `rationales` for each of the provided
+            `generations` for the given `instruction` if the provided aspect is either `honesty`,
+            `instruction-following`, or `overall-rating`; or the `types`, `rationales`,
+            `ratings`, and `rationales-for-ratings` for each of the provided `generations` for the
+            given `instruction` if the provided aspect is either `helpfulness` or `truthfulness`.
+        """
+        if self.aspect in [
+            "honesty",
+            "instruction-following",
+            "overall-rating",
+        ]:
+            return self._format_ratings_rationales_output(output, input)
+        return self._format_types_ratings_rationales_output(output, input)
+
+    def _format_ratings_rationales_output(
+        self, output: Union[str, None], input: Dict[str, Any]
+    ) -> Dict[str, List[Any]]:
+        """Formats the output when the aspect is either `honesty`, `instruction-following`, or `overall-rating`."""
+        if output is None:
+            return {
+                "ratings": [None] * len(input["generations"]),
+                "rationales": [None] * len(input["generations"]),
+            }
+
+        pattern = r"Rating: (.+?)\nRationale: (.+)"
+        sections = output.split("\n\n")
+
+        formatted_outputs = []
+        for section in sections:
+            matches = None
+            if section is not None and section != "":
+                matches = re.search(pattern, section, re.DOTALL)
+            if not matches:
+                formatted_outputs.append({"ratings": None, "rationales": None})
+                continue
+
+            formatted_outputs.append(
+                {
+                    "ratings": int(re.findall(r"\b\d+\b", matches.group(1))[0])
+                    if matches.group(1) not in ["None", "N/A"]
+                    else None,
+                    "rationales": matches.group(2),
+                }
+            )
+        return combine_dicts(*formatted_outputs)
+
+    def _format_types_ratings_rationales_output(
+        self, output: Union[str, None], input: Dict[str, Any]
+    ) -> Dict[str, List[Any]]:
+        """Formats the output when the aspect is either `helpfulness` or `truthfulness`."""
+        if output is None:
+            return {
+                "types": [None] * len(input["generations"]),
+                "rationales": [None] * len(input["generations"]),
+                "ratings": [None] * len(input["generations"]),
+                "rationales-for-ratings": [None] * len(input["generations"]),
+            }
+
+        pattern = r"Type: (.+?)\nRationale: (.+?)\nRating: (.+?)\nRationale: (.+)"
+
+        sections = output.split("\n\n")
+
+        formatted_outputs = []
+        for section in sections:
+            matches = None
+            if section is not None and section != "":
+                matches = re.search(pattern, section, re.DOTALL)
+            if not matches:
+                formatted_outputs.append(
+                    {
+                        "types": None,
+                        "rationales": None,
+                        "ratings": None,
+                        "rationales-for-ratings": None,
+                    }
+                )
+                continue
+
+            formatted_outputs.append(
+                {
+                    "types": int(re.findall(r"\b\d+\b", matches.group(1))[0])
+                    if matches.group(1) not in ["None", "N/A"]
+                    else None,
+                    "rationales": matches.group(2),
+                    "ratings": int(re.findall(r"\b\d+\b", matches.group(3))[0])
+                    if matches.group(3) not in ["None", "N/A"]
+                    else None,
+                    "rationales-for-ratings": matches.group(4),
+                }
+            )
+        return combine_dicts(*formatted_outputs)
```

### Comparing `distilabel-1.0.3/docs/sections/learn/tasks/special_tasks.md` & `distilabel-1.1.0/docs/sections/pipeline_samples/papers/instruction_backtranslation.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,164 +1,125 @@
-# Special Tasks
+# Instruction Backtranslation
 
-This section covers some tasks that don't implement the [`Task`][distilabel.steps.tasks.base.Task] API, but can be thought of as tasks, instead they inherit from [`Step`][distilabel.steps.base.Step].
+["Self Alignment with Instruction Backtranslation"](https://arxiv.org/abs/2308.06259) presents a scalable method to build a high quality instruction following language model by automatically labelling human-written text with corresponding instructions. Their approach, named instruction backtranslation, starts with a language model finetuned on a small amount of seed data, and a given web corpus. The seed model is used to construct training examples by generating instruction prompts for web documents (self-augmentation), and then selecting high quality examples from among these candidates (self-curation). This data is then used to finetune a stronger model.
 
-## Embedding Generation
+Their self-training approach assumes access to a base language model, a small amount of seed data, and a collection of unlabelled examples, e.g. a web corpus. The unlabelled data is a large, diverse set of human-written documents which includes writing about all manner of topics humans are interested in – but crucially is not paired with instructions.
 
-The [`DEITA`](../../papers/deita.md) paper needs to tackle the challenge of ensuring diversity in the final dataset, and they propose an embedding-based method to filter the dataset. For this end, the [`GenerateEmbeddings`][distilabel.steps.tasks.generate_embeddings] step is in charge of generating embeddings for the datasets' text.
+A first key assumption is that there exists some subset of this very large human-written text that would be suitable as gold generations for some user instructions. A second key assumption is that they can predict instructions for these candidate gold answers that can be used as high quality example pairs to train an instruction following model.
 
-```python
-from distilabel.llms.huggingface.transformers import TransformersLLM
-from distilabel.pipeline.local import Pipeline
-from distilabel.steps.tasks.generate_embeddings import GenerateEmbeddings
-
-llm = TransformersLLM(
-    model="TaylorAI/bge-micro-v2",
-    model_kwargs={"is_decoder": True},
-)
-llm.load()
+Their overall process, called instruction backtranslation performs two core steps:
 
-task = GenerateEmbeddings(
-    name="task",
-    llm=llm,
-    pipeline=Pipeline(name="unit-test-pipeline"),
-)
-```
+1. Self-augment: Generate instructions for unlabelled data, i.e. the web corpus, to produce candidate training data of (instruction, output) pairs for instruction tuning.
 
-This step needs an `LLM` to generate the embeddings, we have chosen to use a `TransformersLLM` with `TaylorAI/bge-micro-v2` in this case. Upon call, this step will compute the embedding for the input text and add it to the row:
+2. Self-curate: Self-select high quality demonstration examples as training data to finetune the base model to follow instructions. This approach is done iteratively where a better intermediate instruction-following model can improve on selecting data for finetuning in the next iteration.
 
-```python
-result = next(task.process([{"text": "Hello, how are you?"}]))
-print(result[0]["embedding"])
-# [-8.12729941, -5.24642847, -6.34003029, ...]
-```
+This replication covers the self-curation step i.e. the second / latter step as mentioned above, so as to be able to use the proposed prompting approach to rate the quality of the generated text, which can either be synthetically generated or real human-written text.
 
-## Ranking LLM Responses
+### Replication
 
-Jian et al. present in their paper [`LLM-Blender: Ensembling Large Language Models with Pairwise Ranking and Generative Fusion`](https://arxiv.org/abs/2306.02561) a "small" model that is able to take a instruction and a **pair** output candidates, and output a score for each candidate to measure their **relative** quality, hence **ranking** the responses. You can use [`PairRM`][distilabel.steps.tasks.pair_rm] in distilabel to accomplish this task, let's see how it works:
+To replicate the paper we will be using `distilabel` and a smaller dataset created by the Hugging Face H4 team named [`HuggingFaceH4/instruction-dataset`](https://huggingface.co/datasets/HuggingFaceH4/instruction-dataset) for testing purposes.
 
-```python
-from distilabel.pipeline.local import Pipeline
-from distilabel.steps.tasks.pair_rm import PairRM
+#### Installation
 
-ranker = PairRM(
-    name="pair_rm_ranker", pipeline=Pipeline(name="ranking-pipeline")
-)
-# NOTE: Keep in mind this call will automatically try to load an LLM internally
-ranker.load()
+To replicate Self Alignment with Instruction Backtranslation one will need to install `distilabel` as it follows:
+
+```bash
+pip install "distilabel[hf-inference-endpoints,openai]>=1.0.0"
 ```
 
-For this step the model is fixed by default contrary to other steps, as the implementation relies completely on [`LLM-Blender`](https://github.com/yuchenlin/LLM-Blender) for it to work.
+And since we will be using [`InferenceEndpointsLLM`][distilabel.llms.InferenceEndpointsLLM] (installed via the extra `hf-inference-endpoints`) we will need deploy those in advance either locally or in the Hugging Face Hub (alternatively also the serverless endpoints can be used, but most of the times the inference times are slower, and there's a limited quota to use those as those are free) and set both the `HF_TOKEN` (to use the [`InferenceEndpointsLLM`][distilabel.llms.InferenceEndpointsLLM]) and the `OPENAI_API_KEY` environment variable value (to use the [`OpenAILLM`][distilabel.llms.OpenAILLM]).
 
-To ingest data for this task you would need an input, which corresponds to the instruction, and a list of candidates to compare, that the model will rank working on pairs:
+#### Building blocks
 
-```python
-result = next(
-    ranker.process(
-        [
-            {"input": "Hello, how are you?", "candidates": ["fine", "good", "bad"]},
-        ]
-    )
-)
-```
+- [`LoadHubDataset`][distilabel.steps.LoadHubDataset]: Generator Step to load a dataset from the Hugging Face Hub.
+- [`TextGeneration`][distilabel.steps.tasks.TextGeneration]: Task to generate responses for a given instruction using an LLM.
+    - [`InferenceEndpointsLLM`][distilabel.llms.InferenceEndpointsLLM]: LLM that runs a model from an Inference Endpoint in the Hugging Face Hub.
+- [`InstructionBacktranslation`][distilabel.steps.tasks.InstructionBacktranslation]: Task that generates a score and a reason for a response for a given instruction using the Self Alignment with Instruction Backtranslation prompt.
+    - [`OpenAILLM`][distilabel.llms.OpenAILLM]: LLM that loads a model from OpenAI.
 
-Let's see what the result looks like:
+#### Code
+
+As mentioned before, we will put the previously mentioned building blocks together to replicate Self Alignment with Instruction Backtranslation.
 
 ```python
-import json
-print(json.dumps(result, indent=2))
-# [
-#   {
-#     "input": "Hello, how are you?",
-#     "candidates": [
-#       "fine",
-#       "good",
-#       "bad"
-#     ],
-#     "ranks": [
-#       2,
-#       1,
-#       3
-#     ],
-#     "ranked_candidates": [
-#       "good",
-#       "fine",
-#       "bad"
-#     ]
-#   }
-# ]
-```
+from distilabel.llms import InferenceEndpointsLLM, OpenAILLM
+from distilabel.pipeline import Pipeline
+from distilabel.steps import LoadHubDataset
+from distilabel.steps.tasks import InstructionBacktranslation, TextGeneration
 
-We see we have both the `ranks`, that determine the position that would order the `candidates` field, and the `ranked_candidates` in case these want to be used directly.
 
-## Filtering data to ensure diversity
+with Pipeline(name="self-alignment-with-instruction-backtranslation") as pipeline:
+    load_hub_dataset = LoadHubDataset(
+        name="load_dataset",
+        output_mappings={"prompt": "instruction"},
+    )
 
-We have already mentioned a global step that appeared in the `Global Steps` section, but it was quite specific to be introduced at that time. This `Task` is the [`DeitaFiltering`][distilabel.steps.deita.DeitaFiltering] step.
+    text_generation = TextGeneration(
+        name="text_generation",
+        llm=InferenceEndpointsLLM(
+            base_url="<INFERENCE_ENDPOINT_URL>",
+            tokenizer_id="argilla/notus-7b-v1",
+            model_display_name="argilla/notus-7b-v1",
+        ),
+        input_batch_size=10,
+        output_mappings={"model_name": "generation_model"},
+    )
 
-It's a special type of step developed to reproduce the [`DEITA`](../../papers/deita.md) paper, in charge of filtering responses according to a predefined score. Let's see how it is defined:
+    instruction_backtranslation = InstructionBacktranslation(
+        name="instruction_backtranslation",
+        llm=OpenAILLM(model="gpt-4"),
+        input_batch_size=10,
+        output_mappings={"model_name": "scoring_model"},
+    )
 
-```python
-from distilabel.pipeline.local import Pipeline
-from distilabel.steps.deita import DeitaFiltering
+    keep_columns = KeepColumns(
+        name="keep_columns",
+        columns=[
+            "instruction",
+            "generation",
+            "generation_model",
+            "score",
+            "reason",
+            "scoring_model",
+        ],
+    )
 
-deita_filtering = DeitaFiltering(
-    name="deita_filtering",
-    data_budget=1,
-    pipeline=Pipeline(name="deita-filtering-pipeline"),
-)
-# Remember to call the load method if working outside of a Pipeline context
-deita_filtering.load()
+    load_hub_dataset >> text_generation >> instruction_backtranslation >> keep_columns
 ```
 
-This step is prepared to work on `DEITA` outputs:
-It expects instructions evolved following the `Evol Instruct` procedure, with a score assigned to the complexity of the instruction and the quality of the response ([`ComplexityScorer`][distilabel.steps.tasks.complexity_scorer] and [`QualityScorer`][distilabel.steps.tasks.quality_scorer] respectively), and embeddings computed on the responses. The following is a random example following the structure of the input needed from the process method:
+Then we need to call `pipeline.run` with the runtime parameters so that the pipeline can be launched.
 
 ```python
-result = next(
-    deita_filtering.process(
-        [
-            {
-                "evol_instruction_score": 0.5,
-                "evol_response_score": 0.5,
-                "embedding": [-8.12729941, -5.24642847, -6.34003029],
-            },
-            {
-                "evol_instruction_score": 0.6,
-                "evol_response_score": 0.6,
-                "embedding": [2.99329242, 0.7800932, 0.7799726],
+distiset = pipeline.run(
+    parameters={
+        load_hub_dataset.name: {
+            "repo_id": "HuggingFaceH4/instruction-dataset",
+            "split": "test",
+        },
+        text_generation.name: {
+            "llm": {
+                "generation_kwargs": {
+                    "max_new_tokens": 1024,
+                    "temperature": 0.7,
+                },
             },
-            {
-                "evol_instruction_score": 0.7,
-                "evol_response_score": 0.7,
-                "embedding": [10.29041806, 14.33088073, 13.00557506],
+        },
+        instruction_backtranslation.name: {
+            "llm": {
+                "generation_kwargs": {
+                    "max_new_tokens": 1024,
+                    "temperature": 0.7,
+                },
             },
-        ]
-    )
+        },
+    },
 )
 ```
 
-And this is what we could expect from the output:
+Finally, we can optionally push the generated dataset, named [`Distiset`][distilabel.distiset.Distiset], to the Hugging Face Hub via the `push_to_hub` method, so that each subset generated in the leaf steps is pushed to the Hub.
 
 ```python
-import json
-
-print(json.dumps(result, indent=2))
-# [
-#   {
-#     "evol_instruction_score": 0.5,
-#     "evol_response_score": 0.5,
-#     "embedding": [
-#       -8.12729941,
-#       -5.24642847,
-#       -6.34003029
-#     ],
-#     "deita_score": 0.25,
-#     "deita_score_computed_with": [
-#       "evol_instruction_score",
-#       "evol_response_score"
-#     ],
-#     "nearest_neighbor_distance": 1.9042812683723933
-#   }
-# ]
+distiset.push_to_hub(
+    "instruction-backtranslation-instruction-dataset",
+    private=True,
+)
 ```
-
-We would obtain the dataset size expected for our `data_budget` and `diversity_threshold` set. For more information on how this `Task` works take a look at the `API Reference`.
```

### Comparing `distilabel-1.0.3/docs/sections/learn/tasks/text_generation.md` & `distilabel-1.1.0/docs/sections/pipeline_samples/papers/deita.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,383 +1,369 @@
-# Text Generation
+# DEITA
 
-This section will walk you through the tasks designed to generate text, from the most basic case to more involved ones like [`SelfInstruct`][distilabel.steps.tasks.self_instruct.SelfInstruct], which allows to generate instructions starting from a number of seed terms.
+DEITA (Data-Efficient Instruction Tuning for Alignment) studies an automatic data selection process by first quantifying the data quality based on complexity, quality and diversity. And second, selecting across the best potential combination from an open-source dataset that would fit into the budget you allocate to tune your own LLM.
 
-## The text generation task
+In most setting we cannot allocate unlimited resources for instruction-tuning LLMs. Therefore, the DEITA authors investigated how to select qualitative data for instruction-tuning based on a principle of fewer high quality samples. Liu et al. tackle the issue of first defining good data and second identifying it to respect an initial budget to instruct-tune your LLM.
 
-The first `Task` that we will present is the most general one: [`TextGeneration`][distilabel.steps.tasks.text_generation.TextGeneration]. This is a pre-defined task that defines the `instruction` as the input and `generation` as the output. We can make use of this task for example with a dataset that already has all the instructions ready to be sent to be used:
+The strategy utilizes **LLMs to replace human effort in time-intensive data quality tasks on instruction tuning datasets**. DEITA introduces a way to measure data quality across three critical dimensions: complexity, quality and diversity.
 
-```python
-import os
+![DEITA pipeline overview](../../../assets/tutorials-assets/deita/overview.png)
 
-from distilabel.pipeline import Pipeline
-from distilabel.llms.mistral import MistralLLM
-from distilabel.steps.tasks.text_generation import TextGeneration
+You can see that we see again the dataset of instructions/responses and we kind of reproducing the second step when we learn how to optimize the responses according to an instruction by comparing several possibilities.
 
-text_generation = TextGeneration(
-    name="text-generation",
-    llm=MistralLLM(
-        model="mistral-tiny",
-        api_key=os.getenv("MISTRALAI_API_KEY"),  # type: ignore
-    ),
-    input_batch_size=8,
-    pipeline=Pipeline(name="text-gen-pipeline")
-)
+### Datasets and budget
 
-# remember to call .load() if testing outside of a Pipeline context
-text_generation.load()
-```
+We will dive deeper into the whole process. We will investigate each stage to efficiently select the final dataset used for supervised fine-tuning with a budget constraint. We will tackle technical challenges by explaining exactly how you would assess good data as presented in the paper.
 
-We can just pass a simple task to test it:
+As a reminder, we're looking for a strategy to automatically select good data for the instruction-tuning step when you want to fine-tune an LLM to your own use case taking into account a resource constraint. This means that you cannot blindly train a model on any data you encounter on the internet.
 
-```python
-result = next(
-    text_generation.process(
-        [
-            {
-                "instruction": "What if the Beatles had never formed as a band?",
-            },
-        ] 
-    )
-)
-```
+The DEITA authors assume that you have access to open-source datasets that fit your use case. This may not be the case entirely. But with open-source communities tackling many use cases, with projects such as [BLOOM](https://arxiv.org/pdf/2110.08207.pdf) or [AYA](https://cohere.com/research/aya), it's likely that your use case will be tackled at some point. Furthermore, you could generate your own instruction/response pairs with methods such as [self-generated instructions](https://aclanthology.org/2023.acl-long.754/) using distilabel. This tutorial assumes that we have a data pool with excessive samples for the project's cost constraint. In short, we aim to achieve adequate performance from fewer samples.
 
-And this is what `mistral-tiny` has to tell us to the question:
+The authors claim that the subsample size "correlates proportionally with the computation consumed in instruction tuning". Hence on a first approximation, reducing the sample size means reducing computation consumption and so the total development cost. Reproducing the paper notations, we will associate the budget m to a number of instruction/response pairs that you can set depending on your real budget.
 
-```python
-print(result[0]["generation"])
-# The formation of The Beatles in 1960 marked the beginning of a musical revolution that would last for decades. Their innovative songwriting, unique harmonies, and groundbreaking recordings continue to influence musicians and shape the music industry. However, had they never formed as a band, the musical landscape would have looked very different.
+![Datasets table](../../../assets/tutorials-assets/deita/datasets.png)
 
-# In the absence of The Beatles, other bands and artists would have taken the lead in the British Invasion of the US music charts. Some possibilities include:
+To match the experimental set-up, dataset *X\_sota* is a meta-dataset combining major open-source datasets available to instruct-tune LLMs. This dataset is composed of [ShareGPT](https://huggingface.co/datasets/shibing624/sharegpt_gpt4) (58k instruction/response pairs), [UltraChat](https://huggingface.co/datasets/stingning/ultrachat) (105k instruction/response pairs) and [WizardLM](https://github.com/nlpxucan/WizardLM) (143k instruction/response pairs). It sums to more than 300k instruction/response pairs. We aim to reduce the final subsample to 6k instruction/response pairs.
 
-# 1. The Rolling Stones: The Rolling Stones emerged as a major rival to The Beatles, and they were also a crucial part of the British Invasion. They developed their own unique sound, with a raw, edgier approach that contrasted with The Beatles' more polished style.
-# 2. The Who: The Who was another influential British band that rose to prominence during the same period as The Beatles. They were known for their powerful live performances and innovative approach to rock music.
-# 3. Gerry & The Pacemakers: Gerry & The Pacemakers were an early Merseybeat band, and they had several hits in the UK and the US before The Beatles. Had The Beatles not formed, they might have continued to be a major force in the music world.
-# 4. Cliff Richard: Cliff Richard was a successful pop singer in the UK before The Beatles, and he continued to have hits throughout the 1960s and beyond. He might have remained the dominant British pop star had The Beatles never emerged.
-# 5. Motown: The Beatles' influence extended beyond rock music, and their success paved the way for other genres to gain mainstream acceptance in the US. Motown, for instance, would have faced more resistance in breaking into the US market without The Beatles' paving the way.
+## Setup the notebook and packages
 
-# It's also worth noting that The Beatles' influence extends far beyond their music. They were trendsetters in fashion, hairstyles, and cultural norms. Their break-up in 1970 marked the end of an era in popular culture, and the music industry has never been the same since. So, even if other bands and artists had taken their place, The Beatles' impact on music and culture would still be felt.
-```
+Let's prepare our dependencies:
 
-Let's see now how we can tweak this task to adhere a bit more to another more customized task.
+```bash
+pip install "distilabel[openai,hf-transformers]>=1.0.0"
+pip install pynvml huggingface_hub argilla
+```
 
-### Using a custom prompt
+Import distilabel:
 
-The general `TextGeneration` task assumes our instructions need no further processing, and that we don't want to further process the response of the task for example. Let's see how we can customize the `TextGeneration` task to fit our use case.
+```python
+from distilabel.llms import TransformersLLM, OpenAILLM
+from distilabel.pipeline import Pipeline
+from distilabel.steps import ConversationTemplate, DeitaFiltering, ExpandColumns, LoadHubDataset
+from distilabel.steps.tasks import ComplexityScorer, EvolInstruct, EvolQuality, GenerateEmbeddings, QualityScorer
+```
 
-For the following example we will implement a step presented in [`WizardLM: Empowering Large Language Models to Follow Complex Instructions`](https://arxiv.org/abs/2304.12244), which asks an `LLM` to check whether two instructions are equal or not to decide if we should keep or remove them as redundant:
+Define the distilabel Pipeline and load the dataset from the Hugging Face Hub.
 
 ```python
-import string
-from typing import Dict, Any, List
-
-from distilabel.steps.tasks.text_generation import TextGeneration
+pipeline = Pipeline(name="DEITA")
 
-system_prompt = "You are an AI judge in charge of determining the equality of two instructions. "
+load_data = LoadHubDataset(
+    name="load_data", batch_size=100, output_mappings={"prompt": "instruction"}, pipeline=pipeline
+)
+```
 
-wizardllm_equal_prompt = """Here are two Instructions, do you think they are equal to each other and meet the following requirements?:
-1. They have the same constraints and requirements.
-2. They have the same depth and breadth of the inquiry.
-The First Prompt: {instruction_1}
-The Second Prompt: {instruction_2}
-Your Judgement (Just answer: Equal or Not Equal. No need to explain the reason):"""
+## EVOL-INSTRUCT: Generate Instructions with an LLM
 
+[Evol-Instruct](https://arxiv.org/abs/2304.12244) automates the creation of complex instruction data for training large language models (LLMs) by progressively rewriting an initial set of instructions into more complex forms. This generated data is then used to fine-tune a model named WizardLM.
 
-class WizardLMEqualPrompts(TextGeneration):
-    _template: str = wizardllm_equal_prompt
+Evaluations show that instructions from Evol-Instruct are superior to human-created ones, and WizardLM achieves performance close to or exceeding GPT3.5-turbo in many skills. In distilabel, we initialise each step of the data generation pipeline. Later, we'll connect them together.
 
-    @property
-    def inputs(self) -> List[str]:
-        return ["instruction_1", "instruction_2"]
+```python
+evol_instruction_complexity = EvolInstruct(
+    name="evol_instruction_complexity",
+    llm=OpenAILLM(model="gpt-3.5-turbo"),
+    num_evolutions=5,
+    store_evolutions=True,
+    generate_answers=True,
+    include_original_instruction=True,
+    pipeline=pipeline,
+)
 
-    @property
-    def outputs(self) -> List[str]:
-        return ["response"]
+evol_instruction_complexity.load()
 
-    def format_input(self, input: Dict[str, Any]) -> "ChatType":
-        return [
-            {
-                "role": "system", "content": system_prompt,
-                "role": "user", "content": self._template.format(**input)
-            }
-        ]
+_evolved_instructions = next(evol_instruction_complexity.process(
+    ([{"instruction": "How many fish are there in a dozen fish?"}]))
+)
 
-    def format_output(self, output: str | None, input: Dict[str, Any]) -> Dict[str, str]:
-        return {"response": output.translate(str.maketrans("", "", string.punctuation))}
+print(*_evolved_instructions, sep="\n")
 ```
 
-Now that we have our brand new task, let's use instantiate it (will use [`MistralLLM`][distilabel.llms.mistral.MistralLLM]):
+Output:
 
-```python
-import os
+```bash
+( 1, 'How many fish are there in a dozen fish?')
+( 2, 'How many rainbow trout are there in a dozen rainbow trout?')
+( 3, 'What is the average weight in pounds of a dozen rainbow trout caught in a specific river in Alaska during the month of May?')
+```
 
-from distilabel.pipeline import Pipeline
-from distilabel.llms.mistral import MistralLLM
+## EVOL COMPLEXITY: Evaluate complexity of generated instructions
 
-wizardlm_equality = WizardLMEqualPrompts(
-    name="wizardlm_equality",
-    llm=MistralLLM(
-        model="mistral-small",
-        api_key=os.getenv("MISTRALAI_API_KEY"),  # type: ignore
-    ),
-    input_batch_size=8,
-    pipeline=Pipeline(name="wizardlm-equality-pipeline")
-)
+The second step is the evaluation of *complexity* for an instruction in a given instruction-response pair. Like EVOL-INSTRUCT, this method uses LLMs instead of humans to automatically improve instructions, specifically through their complexity. From any instruction-response pair, $(I, R)$, we first generate new instructions following the In-Depth Evolving Response. We generate more complex instructions through prompting, as explained by authors, by adding some constraints or reasoning steps. Let\'s take an example from [GPT-4-LLM](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM) which aims to generate observations by GPT-4 to instruct-tune LLMs with supervised fine-tuning. And, we have the instruction $instruction_0$:
 
-# remember to call .load() if testing outside of a Pipeline context
-wizardlm_equality.load()
+```python
+instruction_0 = "Give three tips for staying healthy."
 ```
 
-Let's ask it to compare to random instructions:
+To make it more complex, you can use, as the authors did, some prompt templates to add constraints or deepen the instruction. They provided some prompts in the paper appendix. For instance, this one was used to add constraints:
 
 ```python
-result = next(
-    wizardlm_equality.process(
-        [
-            {
-                "instruction_1": "What if the Beatles had never formed as a band?",
-                "instruction_2": "What are The Simpsons?"
-            },
-        ] 
-    )
-)
+PROMPT = """I want you act as a Prompt Rewriter.
+Your objective is to rewrite a given prompt into a more complex version to
+make those famous AI systems (e.g., ChatGPT and GPT4) a bit harder to handle.
+But the rewritten prompt must be reasonable and must be understood and
+responded by humans.
+Your rewriting cannot omit the non-text parts such as the table and code in
+#Given Prompt#:. Also, please do not omit the input in #Given Prompt#.
+You SHOULD complicate the given prompt using the following method:
+Please add one more constraints/requirements into #Given Prompt#
+You should try your best not to make the #Rewritten Prompt# become verbose,
+#Rewritten Prompt# can only add 10 to 20 words into #Given Prompt#.
+‘#Given Prompt#’, ‘#Rewritten Prompt#’, ‘given prompt’ and ‘rewritten prompt’
+are not allowed to appear in #Rewritten Prompt#
+#Given Prompt#:
+<Here is instruction>
+#Rewritten Prompt#:
+"""
 ```
 
-And see what we have in return:
+Prompting this to an LLM, you automatically get a more complex instruction, called $instruction_1$, from an initial instruction $instruction_0$:
 
 ```python
-import json
-print(json.dumps(result, indent=2))
-# [
-#   {
-#     "instruction_1": "What if the Beatles had never formed as a band?",
-#     "instruction_2": "What are The Simpsons?",
-#     "model_name": "mistral-small",
-#     "response": "Not Equal The first prompt is a counterfactual question that invites exploration of the Beatles impact on music and culture if they had not formed while the second prompt asks for an explanation or definition of a longrunning TV show The Simpsons They do not share the same constraints requirements depth or breadth of inquiry"
-#   }
-# ]
+instruction_1 = "Provide three recommendations for maintaining well-being, ensuring one focuses on mental health."
 ```
 
-!!! Note
-    We can see the `response` contains "Not Equal", but it didn't strictly followed the prompt as requested. This can be a hint that a more powerful model is required, or the prompt needs some extra tuning.
-
-## Guided text generation
+With sequences of evolved instructions, we use a further LLM to automatically rank and score them. We provide the 6 instructions at the same time. By providing all instructions together, we force the scoring model to look at minor complexity differences between evolved instructions. Encouraging the model to discriminate between instructions. Taking the example below, $instruction_0$ and $instruction_1$ could deserve the same score independently, but when compared together we would notice the slight difference that makes $instruction_1$ more complex.
 
-Other than the base generation tasks, the literature has proposed some `Tasks` to provide extra functionality, like the following:
-
-### Self Instruct
-
-The first we are going to look at is [`SelfInstruct`][distilabel.steps.tasks.self_instruct.SelfInstruct]. This pre-defined task is inspired by [`Self-Instruct: Aligning Language Models with Self-Generated Instructions`](https://arxiv.org/abs/2212.10560), and has the following intent: given a number of instructions, a certain criteria for query generations, an application description, and an input, generates a number of instruction related to the given input and following what is stated in the criteria for query generation and the application description.
+In `distilabel`, we implement this like so:
 
 ```python
-import os
-
-from distilabel.pipeline import Pipeline
-from distilabel.llms.mistral import MistralLLM
-from distilabel.steps.tasks.self_instruct import SelfInstruct
+instruction_complexity_scorer = ComplexityScorer(
+    name="instruction_complexity_scorer",
+    llm=OpenAILLM(model="gpt-3.5-turbo"),
+    input_mappings={"instructions": "evolved_instructions"},
+    pipeline=pipeline,
+)
 
-self_instruct = SelfInstruct(
-    name="text-generation",
-    num_instructions=3,
-    input_batch_size=8,
-    llm=MistralLLM(
-        model="mistral-medium",
-        api_key=os.getenv("MISTRALAI_API_KEY"),  # type: ignore
-    ),
-    pipeline=Pipeline(name="self-instruct-pipeline")
+expand_evolved_instructions = ExpandColumns(
+    name="expand_evolved_instructions",
+    columns=["evolved_instructions", "answers", "scores"],
+    output_mappings={
+        "evolved_instructions": "evolved_instruction",
+        "answers": "answer",
+        "scores": "evol_instruction_score",
+    },
+    pipeline=pipeline,
 )
 
-# remember to call .load() if testing outside of a Pipeline context
-self_instruct.load()
-```
+instruction_complexity_scorer.load()
 
-Let's pass a simple input:
+_evolved_instructions = next(instruction_complexity_scorer.process(([{"evolved_instructions": [PROMPT + instruction_1]}])))
 
-```python
-result = next(
-    self_instruct.process(
-        [
-            {
-                "input": "What are fantasy novels?",
-            },
-        ] 
-    )
-)
+print("Original Instruction:")
+print(instruction_1)
+print("\nEvolved Instruction:")
+print(_evolved_instructions[0]["evolved_instructions"][0].split("#Rewritten Prompt#:\n")[1])
 ```
 
-And this is what we have in return:
+Output:
 
-```python
-import json
-print(json.dumps(result[0]["instructions"], indent=2))
-# [
-#   "1. Can you explain the common elements found in fantasy novels and their role in storytelling?",
-#   "2. Generate a brief summary of a popular fantasy novel, highlighting its unique features.",
-#   "3. Compare and contrast the world-building techniques used by two renowned fantasy authors."
-# ]
 ```
+Original Instruction:
+Provide three recommendations for maintaining well-being, ensuring one focuses on mental health.
 
-By tweaking the `num_instructions` and the `criteria_for_query_generation` we can see how this is a really powerful `Task` to generate synthetic data starting from a small amount of initial instructions.
+Evolved Instruction:
+Suggest three strategies for nurturing overall well-being, with the stipulation that at least one explicitly addresses the enhancement of mental health, incorporating evidence-based practices.
+```
 
-### Evol Instruct
+## EVOL-QUALITY: Quality Evaluation
 
-This `Task` was defined in [WizardLM: Empowering Large Language Models to Follow Complex Instructions](https://arxiv.org/abs/2304.12244), the idea is, starting from a series of initial instructions, evolve them according to a scheme of prompts to obtain more complex ones. Let's see how we can use [`EvolInstruct`][distilabel.steps.tasks.evol_instruct.base.EvolInstruct]:
+Now that we have scored the *complexity* of the instructions, we will focus on the *quality* of the responses. Similar to *EVOL COMPLEXITY*, the authors introduced *EVOL QUALITY, a method* based on LLMs, instead of humans, to automatically score the quality of the response.
 
-```python
-import os
-
-from distilabel.pipeline import Pipeline
-from distilabel.llms.mistral import MistralLLM
-from distilabel.steps.tasks.evol_instruct.base import EvolInstruct
+From an instruction-response pair, $(I, R)$, the goal is to make the response evolve into a more helpful and relevant response. The key difference is that we need to also provide the first instruction to guide evolution. Let's take back our example from [GPT-4-LLM](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM).
 
-evol_instruct = EvolInstruct(
-    name="evol-instruct",
-    num_evolutions=2,
-    store_evolutions=True,
-    input_batch_size=8,
-    llm=MistralLLM(
-        model="mistral-small",
-        api_key=os.getenv("MISTRALAI_API_KEY"),  # type: ignore
-    ),
-    pipeline=Pipeline(name="evol-instruct-pipeline")
-)
+Here we have the response $response_0$ and its initial instruction $instruction_0$:
 
-# remember to call .load() if testing outside of a Pipeline context
-evol_instruct.load()
+```python
+instruction_0 = "Give three tips for staying healthy."
+reponse_0 = "1. Eat a balanced and nutritious diet: Make sure your meals are inclusive of a variety of fruits and vegetables, lean protein, whole grains, and healthy fats. This helps to provide your body with the essential nutrients to function at its best and can help prevent chronic diseases. 2. Engage in regular physical activity: Exercise is crucial for maintaining strong bones, muscles, and cardiovascular health. Aim for at least 150 minutes of moderate aerobic exercise or 75 minutes of vigorous exercise each week. 3. Get enough sleep: Getting enough quality sleep is crucial for physical and mental well-being. It helps to regulate mood, improve cognitive function, and supports healthy growth and immune function. Aim for 7-9 hours of sleep each night."
 ```
 
-We can now use a sample instruction to see what that yields:
+Again the authors provided several prompts you could use to make your response evolve according to some guidelines. For example, this one was used to enrich the answer:
 
 ```python
-result = next(
-    evol_instruct.process(
-        [
-            {
-                "instruction": "What are fantasy novels?",
-            },
-        ] 
-    )
-)
+PROMPT = """I want you to act as a Response Rewriter
+Your goal is to enhance the quality of the response given by an AI assistant
+to the #Given Prompt# through rewriting.
+But the rewritten response must be reasonable and must be understood by humans.
+Your rewriting cannot omit the non-text parts such as the table and code in
+#Given Prompt# and #Given Response#. Also, please do not omit the input
+in #Given Prompt#.
+You Should enhance the quality of the response using the following method:
+Please make the Response more in-depth
+You should try your best not to make the #Rewritten Response# become verbose,
+#Rewritten Response# can only add 10 to 20 words into #Given Response#.
+‘#Given Response#’, ‘#Rewritten Response#’, ‘given response’ and ‘rewritten response’
+are not allowed to appear in #Rewritten Response#
+#Given Prompt#:
+<instruction_0>
+#Given Response#:
+<response_0>
+#Rewritten Response#:
+"""
 ```
 
-!!! Note
-    As we used `store_evolutions=True`, we now can see the evolution from the starting point. Remember to visit the [`API Reference`][distilabel.steps.tasks.evol_instruct.base.EvolInstruct] to take into account all the parameters.
-
-Let's see the evolved instructions we obtained:
+Prompting this to an LLM, you will automatically get a more enriched response, called $response_1$, from an initial response $response_0$ and initial instruction $instruction_0$:
 
 ```python
-import json
-print(json.dumps(result[0]["evolved_instructions"], indent=2))
-# [
-#   "Can you name some lesser-known literary genres that explore imaginary worlds, magical elements, and epic adventures, similar to fantasy novels, but with a unique twist and a smaller readership?",
-#   "How about you suggest some under-the-radar literary categories that, much like fantasy literature, delve into fictional realms, incorporate magical aspects, and narrate grand journeys, but with a distinct flavor and a more limited, devoted readership?"
-# ]
-```
+evol_response_quality = EvolQuality(
+    name="evol_response_quality",
+    llm=OpenAILLM(model="gpt-3.5-turbo"),
+    num_evolutions=5,
+    store_evolutions=True,
+    include_original_response=True,
+    input_mappings={
+        "instruction": "evolved_instruction",
+        "response": "answer",
+    },
+    pipeline=pipeline,
+)
 
-This strategy of evolving a set of instructions synthetically has yielded strong results as can be seen in the original paper, leading to the family of [WizardLM](https://github.com/nlpxucan/WizardLM).
+evol_response_quality.load()
 
-We will now take a look at some `EvolInstruct` *inspired* tasks that have been used for [`DEITA`]([`What Makes Good Data for Alignment? A Comprehensive Study of Automatic Data Selection in Instruction Tuning`](https://arxiv.org/abs/2312.15685)) datasets.
+_evolved_responses = next(evol_response_quality.process([{"instruction": PROMPT + instruction_0, "response": reponse_0}]))
 
-#### Evol Complexity
+print("Original Response:")
+print(reponse_0)
+print("\nEvolved Response:")
+print(*_evolved_responses[0]['evolved_responses'], sep="\n")
+```
 
-[`EvolComplexity`][distilabel.steps.tasks.evol_instruct.evol_complexity.base.EvolComplexity] evolves the instructions to make them specifically more complex. It follows the evolutionary approach from `EvolInstruct` but with slightly different prompts.
+And now, as in EVOL COMPLEXITY you iterate through this path and use different prompts to make your responses more relevant, helpful or creative. In the paper, they make 4 more iterations to get 5 evolved responses $(R0, R1, R2, R3, R4)$ which makes 5 different responses for one initial instruction at the end of this step.
 
 ```python
-import os
-
-from distilabel.pipeline import Pipeline
-from distilabel.llms.mistral import MistralLLM
-from distilabel.steps.tasks.evol_instruct.evol_complexity.base import EvolComplexity
+response_quality_scorer = QualityScorer(
+    name="response_quality_scorer",
+    llm=OpenAILLM(model="gpt-3.5-turbo"),
+    input_mappings={
+        "instruction": "evolved_instruction",
+        "responses": "evolved_responses",
+    },
+    pipeline=pipeline,
+)
 
-evol_complexity = EvolComplexity(
-    name="evol-complexity",
-    num_evolutions=1,
-    input_batch_size=8,
-    llm=MistralLLM(
-        model="mistral-small",
-        api_key=os.getenv("MISTRALAI_API_KEY"),  # type: ignore
-    ),
-    pipeline=Pipeline(name="evol-complexity-pipeline")
+expand_evolved_responses = ExpandColumns(
+    name="expand_evolved_responses",
+    columns=["evolved_responses", "scores"],
+    output_mappings={
+        "evolved_responses": "evolved_response",
+        "scores": "evol_response_score",
+    },
+    pipeline=pipeline,
 )
 
-# remember to call .load() if testing outside of a Pipeline context
-evol_complexity.load()
-```
+response_quality_scorer.load()
 
-Let's see it with the same previous example from `EvolInstruct`, this time with a single evolution and keeping the last generation:
+_scored_responses = next(response_quality_scorer.process([{"instruction": PROMPT + instruction_0, "responses": _evolved_responses[0]['evolved_responses']}]))
 
-```python
-result = next(
-    evol_complexity.process(
-        [
-            {
-                "instruction": "What are fantasy novels?",
-            },
-        ] 
-    )
-)
+print("Original Response:")
+print(reponse_0)
+
+print("\nScore, Evolved Response:")
+print(*zip(_scored_responses[0]["scores"], _evolved_responses[0]['evolved_responses']), sep="\n")
 ```
 
-This would be the evolved instruction:
+Output:
 
-```python
-print(result[0]["evolved_instruction"])
-# Could you explain the literary genre of fantasy novels, providing examples and discussing how they differ from science fiction?
+```bash
+Original Response:
+1. Eat a balanced and nutritious diet: Make sure your meals are inclusive of a variety of fruits and vegetables, lean protein, whole grains, and healthy fats. This helps to provide your body with the essential nutrients to function at its best and can help prevent chronic diseases. 2. Engage in regular physical activity: Exercise is crucial for maintaining strong bones, muscles, and cardiovascular health. Aim for at least 150 minutes of moderate aerobic exercise or 75 minutes of vigorous exercise each week. 3. Get enough sleep: Getting enough quality sleep is crucial for physical and mental well-being. It helps to regulate mood, improve cognitive function, and supports healthy growth and immune function. Aim for 7-9 hours of sleep each night.
 
-# (Note: I added a requirement to discuss the differences between fantasy novels and science fiction, and tried to keep the prompt reasonably concise.)
+Score, Evolved Response:
+(4.0, 'Here are three essential tips for maintaining good health: \n1. Prioritize regular exercise \n2. Eat a balanced diet with plenty of fruits and vegetables \n3. Get an adequate amount of sleep each night.')
+(2.0, 'Here are three effective strategies to maintain a healthy lifestyle.')
+(5.0, 'Here are three practical tips to maintain good health: Ensure a balanced diet, engage in regular exercise, and prioritize sufficient sleep. These practices support overall well-being.')
 ```
 
-And we have similar results to what we obtained with `EvolInstruct`, with a slight modification in the inner prompts used.
+## Improving Data Diversity
 
-!!! Note
-    Take into account there isn't just randomness from the `LLM`, but also from the mutation selected (the prompt used to evolve the instruction).
+One main component of good data to instruct-tune LLMs is diversity. Real world data can often contain [redundancy](https://openreview.net/forum?id=u96ZBg_Shna) due repetitive and homogeneous data.
 
-#### Evol Quality
+The authors of the DEITA paper tackle the challenge of ensuring data diversity in the instruction tuning LLMs to avoid the pitfalls of data redundancy that can lead to over-fitting or poor generalization. They propose an embedding-based method to filter data for diversity. This method, called Repr Filter, uses embeddings generated by the *Llama 1 13B* model to represent instruction-response pairs in a vector space. The diversity of a new data sample is assessed based on the cosine distance between its embedding and that of its nearest neighbor in the already selected dataset. If this distance is greater than a specified threshold, the sample is considered diverse and is added to the selection. This process prioritizes diversity by assessing each sample's contribution to the variety of the dataset until the data selection budget is met. This approach effectively maintains the diversity of the data used for instruction tuning, as demonstrated by the DEITA models outperforming or matching state-of-the-art models with significantly less training data. In this implementation of DEITA we use the hidden state of the last layer of the Llama 2 model to generate embeddings, instead of a sentence transformer model, because we found that it improved the diversity of the data selection.
 
-The [`EvolQuality`][distilabel.steps.tasks.evol_quality.base.EvolQuality] `Task` appeared in [`What Makes Good Data for Alignment? A Comprehensive Study of Automatic Data Selection in Instruction Tuning`](https://arxiv.org/abs/2312.15685), as a posterior step to the previous [`EvolComplexityGenerator`][distilabel.steps.tasks.evol_instruct.evol_complexity.generator.EvolComplexityGenerator]. It takes a different approach: we evolve the **quality** of the **responses** given a prompt. Let's see an example:
+![jdjd](../../../assets/tutorials-assets/deita/diversity.png)
 
 ```python
-import os
-
-from distilabel.pipeline import Pipeline
-from distilabel.llms.mistral import MistralLLM
-from distilabel.steps.tasks.evol_quality.base import EvolQuality
+generate_conversation = ConversationTemplate(
+    name="generate_conversation",
+    input_mappings={
+        "instruction": "evolved_instruction",
+        "response": "evolved_response",
+    },
+    pipeline=pipeline,
+)
 
-evol_quality = EvolQuality(
-    name="evol-quality",
-    num_evolutions=1,
-    input_batch_size=8,
-    llm=MistralLLM(
-        model="mistral-small",
-        api_key=os.getenv("MISTRALAI_API_KEY"),  # type: ignore
+generate_embeddings = GenerateEmbeddings(
+    name="generate_embeddings",
+    llm=TransformersLLM(
+        model="TinyLlama/TinyLlama-1.1B-Chat-v1.0",
+        device="cuda",
+        torch_dtype="float16",
     ),
-    pipeline=Pipeline(name="evol-quality-pipeline")
+    input_mappings={"text": "conversation"},
+    input_batch_size=5,
+    pipeline=pipeline,
 )
 
-# remember to call .load() if testing outside of a Pipeline context
-evol_quality.load()
+deita_filtering = DeitaFiltering(name="deita_filtering", pipeline=pipeline)
 ```
 
-We will use it on the output from `EvolComplexity` task:
+## Build the ⚗ distilabel `Pipeline`
+
+Now we're ready to build a `distilabel` pipeline using the DEITA method:
 
 ```python
-result = next(
-    evol_quality.process(
-        [
-            {
-                "instruction": "What are fantasy novels?",
-                "response": "Could you explain the literary genre of fantasy novels, providing examples and discussing how they differ from science fiction?\n\n(Note: I added a requirement to discuss the differences between fantasy novels and science fiction, and tried to keep the prompt reasonably concise.)"
-            },
-        ] 
-    )
+load_data.connect(evol_instruction_complexity)
+evol_instruction_complexity.connect(instruction_complexity_scorer)
+instruction_complexity_scorer.connect(expand_evolved_instructions)
+expand_evolved_instructions.connect(evol_response_quality)
+evol_response_quality.connect(response_quality_scorer)
+response_quality_scorer.connect(expand_evolved_responses)
+expand_evolved_responses.connect(generate_conversation)
+generate_conversation.connect(generate_embeddings)
+generate_embeddings.connect(deita_filtering)
+```
+
+Now we can run the pipeline. We use the step names to reference them in the pipeline configuration:
+
+```python
+distiset = pipeline.run(
+    parameters={
+        "load_data": {
+            "repo_id": "distilabel-internal-testing/instruction-dataset-50",
+            "split": "train",
+        },
+        "evol_instruction_complexity": {
+            "llm": {"generation_kwargs": {"max_new_tokens": 512, "temperature": 0.7}}
+        },
+        "instruction_complexity_scorer": {
+            "llm": {"generation_kwargs": {"temperature": 0.0}}
+        },
+        "evol_response_quality": {
+            "llm": {"generation_kwargs": {"max_new_tokens": 512, "temperature": 0.7}}
+        },
+        "response_quality_scorer": {"llm": {"generation_kwargs": {"temperature": 0.0}}},
+        "deita_filtering": {"data_budget": 500, "diversity_threshold": 0.04},
+    },
+    use_cache=False,
 )
 ```
 
-And we obtain in return an evolution from the previous response with a *mutation* applied to the response:
+We can push the results to the Hugging Face Hub:
 
 ```python
-print(result[0]["evolved_response"])
-# Fantasy novels are a captivating genre of literature, immersing readers in imaginary worlds filled with magical elements, mythical creatures, and epic adventures. They often feature complex plotlines and unique characters, offering a delightful escape from reality.
+distiset.push_to_hub("distilabel-internal-testing/deita-colab")
 ```
 
-!!! Note
-    Take into account that just as we had with the `EvolComplexity` task, there is randomness involved with the inner mutation prompt used.
+## Results
+
+Again, to show the relevance of EVOL QUALITY method, the authors evaluated on the MT-bench models fine-tuned with different data selections according to how we defined quality responses according to an instruction. Each time they selected 6k data according to the quality score:
+
+![DEITA results](../../../assets/tutorials-assets/deita/results.png)
+
+Credit: Liu et al. (2023)
+
+The score is much better when selecting data with the EVOL QUALITY method than when we select randomly or according to the length, making a more qualitative response if longer. Nevertheless, we see that the margin we may have seen in the complexity score is thinner. And we'll discuss the strategy in a later part. Nevertheless, this strategy looks to improve the fine-tuning compared to the baselines and now we're interested in mixing quality and complexity assessment with a diversity evaluation to find the right trade-off in our selection process.
+
+## Conclusion
+
+In conclusion, if you are looking for some efficient method to align an open-source LLM to your business case with a constrained budget, the solutions provided by DEITA are really worth the shot. This data-centric approach enables one to focus on the content of the dataset to have the best results instead of "just" scaling the instruction-tuning with more, and surely less qualitative, data. In a nutshell, the strategy developed, through automatically scoring instructions-responses, aims to substitute the human preference step proprietary models such as GPT-4 have been trained with. There are a few improvements we could think about when it comes to how to select the good data, but it opens a really great way in instruct-tuning LLM with lower computational needs making the whole process intellectually relevant and more sustainable than most of the other methods. We'd be happy to help you out with aligning an LLM with your business case drawing inspiration from such a methodology.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `distilabel-1.0.3/docs/sections/papers/instruction_backtranslation.md` & `distilabel-1.1.0/tests/unit/steps/tasks/test_instruction_backtranslation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,113 +1,90 @@
-Self Alignment with Instruction Backtranslation presents a scalable method to build a high quality instruction following language model by automatically labelling human-written text with corresponding instructions. Their approach, named instruction backtranslation, starts with a language model finetuned on a small amount of seed data, and a given web corpus. The seed model is used to construct training examples by generating instruction prompts for web documents (self-augmentation), and then selecting high quality examples from among these candidates (self-curation). This data is then used to finetune a stronger model.
-
-Their self-training approach assumes access to a base language model, a small amount of seed data, and a collection of unlabelled examples, e.g. a web corpus. The unlabelled data is a large, diverse set of human-written documents which includes writing about all manner of topics humans are interested in – but crucially is not paired with instructions.
-
-A first key assumption is that there exists some subset of this very large human-written text that would be suitable as gold generations for some user instructions. A second key assumption is that they can predict instructions for these candidate gold answers that can be used as high quality example pairs to train an instruction following model.
-
-Their overall process, called instruction backtranslation performs two core steps:
-1. Self-augment: Generate instructions for unlabelled data, i.e. the web corpus, to produce candidate training data of (instruction, output) pairs for instruction tuning.
-2. Self-curate: Self-select high quality demonstration examples as training data to finetune the base model to follow instructions. This approach is done iteratively where a better intermediate instruction-following model can improve on selecting data for finetuning in the next iteration.
-
-### Replication
-
-To replicate the paper we will be using `distilabel` and a smaller dataset created by the Hugging Face H4 team named [`HuggingFaceH4/instruction-dataset`](https://huggingface.co/datasets/HuggingFaceH4/instruction-dataset) for testing purposes.
-
-#### Installation
-
-To replicate Self Alignment with Instruction Backtranslation one will need to install `distilabel` as it follows:
-
-```bash
-pip install "distilabel[hf-inference-endpoints,openai]>=1.0.0"
-```
-
-And since we will be using `hf-inference-endpoints` we will need deploy those in advance either locally or in the Hugging Face Hub (alternatively also the serverless endpoints can be used, but most of the times the inference times are slower, and there's a limited quota to use those as those are free) and set both the `HF_TOKEN` (to use the `InferenceEndpointsLLM`) and the `OPENAI_API_KEY` environment variable value (to use the `OpenAILLM`).
-
-#### Building blocks
-
-* `LoadHubDataset`: Generator Step to load a dataset from the Hugging Face Hub.
-* `TextGeneration`: Task to generate responses for a given instruction using an LLM.
-    * `InferenceEndpointsLLM`: LLM that runs a model from an Inference Endpoint in the Hugging Face Hub.
-* `InstructionBacktranslation`: Task that generates a score and a reason for a response for a given instruction using the Self Alignment with Instruction Backtranslation prompt.
-    * `OpenAILLM`: LLM that loads a model from OpenAI using `OpenAILLM`.
-
-#### Code
-
-As mentioned before, we will put the previously mentioned building blocks together to replicate Self Alignment with Instruction Backtranslation.
-
-```python
-from distilabel.llms import InferenceEndpointsLLM, OpenAILLM
-from distilabel.pipeline import Pipeline
-from distilabel.steps import LoadHubDataset
-from distilabel.steps.tasks import InstructionBacktranslation, TextGeneration
-
-
-with Pipeline(name="self-alignment-with-instruction-backtranslation") as pipeline:
-    load_hub_dataset = LoadHubDataset(
-        name="load_dataset",
-        output_mappings={"prompt": "instruction"},
-    )
-
-    text_generation = TextGeneration(
-        name="text_generation",
-        llm=InferenceEndpointsLLM(
-            base_url="<INFERENCE_ENDPOINT_URL>",
-            tokenizer_id="argilla/notus-7b-v1",
-            model_display_name="argilla/notus-7b-v1",
-        ),
-        input_batch_size=10,
-        output_mappings={"model_name": "generation_model"},
-    )
-    load_hub_dataset.connect(text_generation)
-
-    instruction_backtranslation = InstructionBacktranslation(
-        name="instruction_backtranslation",
-        llm=OpenAILLM(model="gpt-4"),
-        input_batch_size=10,
-        output_mappings={"model_name": "scoring_model"},
-    )
-    text_generation.connect(instruction_backtranslation)
-
-    keep_columns = KeepColumns(
-        name="keep_columns",
-        columns=[
-            "instruction",
-            "generation",
-            "generation_model",
-            "score",
-            "reason",
-            "scoring_model",
-        ],
-    )
-    instruction_backtranslation.connect(keep_columns)
-```
-
-Then we need to call `pipeline.run` with the runtime parameters so that the pipeline can be launched.
-
-```python
-dataset = pipeline.run(
-    parameters={
-        "load_dataset": {
-            "repo_id": "HuggingFaceH4/instruction-dataset",
-            "split": "test",
-        },
-        "text_generation": {
-            "generation_kwargs": {
-                "max_new_tokens": 1024,
-                "temperature": 0.7,
-            },
-        },
-        "instruction_backtranslation": {
-            "generation_kwargs": {
-                "max_new_tokens": 1024,
-                "temperature": 0.7,
-            },
-        },
-    }
+# Copyright 2023-present, Argilla, Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from typing import Any, List
+
+from distilabel.llms.base import LLM
+from distilabel.llms.typing import GenerateOutput
+from distilabel.pipeline.local import Pipeline
+from distilabel.steps.tasks.instruction_backtranslation import (
+    InstructionBacktranslation,
 )
-```
+from distilabel.steps.tasks.typing import ChatType
 
-Finally, we can optionally push the generated dataset, named `Distiset`, to the Hugging Face Hub via the `push_to_hub` method, so that each subset generated in the leaf steps is pushed to the Hub.
 
-```python
-dataset.push_to_hub("distilabel-internal-testing/instruction-backtranslation-instruction-dataset", private=True)
-```
+class InstructionBacktranslationLLM(LLM):
+    def load(self) -> None:
+        pass
+
+    @property
+    def model_name(self) -> str:
+        return "instruction-backtranslation-model"
+
+    def generate(
+        self, inputs: List[ChatType], num_generations: int = 1, **kwargs: Any
+    ) -> List[GenerateOutput]:
+        return [
+            ["This is the reason. Score: 1" for _ in range(num_generations)]
+            for _ in inputs
+        ]
+
+
+class TestInstructionBacktranslation:
+    def test_format_input(self) -> None:
+        task = InstructionBacktranslation(
+            name="instruction-backtranslation",
+            llm=InstructionBacktranslationLLM(),
+            pipeline=Pipeline(name="unit-test-pipeline"),
+        )
+        task.load()
+
+        assert task.format_input(
+            {"instruction": "instruction", "generation": "generation"}
+        ) == [
+            {
+                "role": "user",
+                "content": 'Below is an instruction from an user and a candidate answer. Evaluate whether or not the answer is a good example of how AI Assistant should respond to the user’s instruction. Please assign a score using the following 5-point scale:\n1: It means the answer is incomplete, vague, off-topic, controversial, or not exactly what the user asked for. For example, some content seems missing, numbered list does not start from the beginning, the opening sentence repeats user’s question. Or the response is from another person’s perspective with their personal experience (e.g. taken from blog posts), or looks like an answer from a forum. Or it contains promotional text, navigation text, or other irrelevant information.\n2: It means the answer addresses most of the asks from the user. It does not directly address the user’s question. For example, it only provides a high-level methodology instead of the exact solution to user’s question.\n3: It means the answer is helpful but not written by an AI Assistant. It addresses all the basic asks from the user. It is complete and self contained with the drawback that the response is not written from an AI assistant’s perspective, but from other people’s perspective. The content looks like an excerpt from a blog post, web page, or web search results. For example, it contains personal experience or opinion, mentions comments section, or share on social media, etc.\n4: It means the answer is written from an AI assistant’s perspective with a clear focus of addressing the instruction. It provide a complete, clear, and comprehensive response to user’s question or instruction without missing or irrelevant information. It is well organized, self-contained, and written in a helpful tone. It has minor room for improvement, e.g. more concise and focused.\n5: It means it is a perfect answer from an AI Assistant. It has a clear focus on being a helpful AI Assistant, where the response looks like intentionally written to address the user’s question or instruction without any irrelevant sentences. The answer provides high quality content, demonstrating expert knowledge in the area, is very well written, logical, easy-to-follow, engaging and insightful.\nPlease first provide a brief reasoning you used to derive the rating score, and then write "Score: <rating>" in the last line.\n\ninstruction\ngeneration\n',
+            }
+        ]
+
+    def test_format_output(self) -> None:
+        task = InstructionBacktranslation(
+            name="instruction-backtranslation",
+            llm=InstructionBacktranslationLLM(),
+            pipeline=Pipeline(name="unit-test-pipeline"),
+        )
+        task.load()
+
+        assert task.format_output("This is the reason. Score: 1", {}) == {
+            "score": 1,
+            "reason": "This is the reason.",
+        }
+
+    def test_process(self) -> None:
+        task = InstructionBacktranslation(
+            name="instruction-backtranslation",
+            llm=InstructionBacktranslationLLM(),
+            pipeline=Pipeline(name="unit-test-pipeline"),
+        )
+        task.load()
+
+        assert next(task.process([{"instruction": "test", "generation": "A"}])) == [
+            {
+                "instruction": "test",
+                "generation": "A",
+                "score": 1,
+                "reason": "This is the reason.",
+                "model_name": "instruction-backtranslation-model",
+            }
+        ]
```

### Comparing `distilabel-1.0.3/src/distilabel/__init__.py` & `distilabel-1.1.0/src/distilabel/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,10 +10,10 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from rich import traceback as rich_traceback
 
-__version__ = "1.0.3"
+__version__ = "1.1.0"
 
 rich_traceback.install(show_locals=True)
```

### Comparing `distilabel-1.0.3/src/distilabel/__main__.py` & `distilabel-1.1.0/src/distilabel/__main__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/distiset.py` & `distilabel-1.1.0/src/distilabel/distiset.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from pathlib import Path
 from typing import Any, Dict, Optional
 
 from datasets import load_dataset
 from huggingface_hub import DatasetCardData, HfApi
 from pyarrow.lib import ArrowInvalid
 
+from distilabel.steps.tasks.base import DISTILABEL_METADATA_KEY
 from distilabel.utils.card.dataset_card import (
     DistilabelDatasetCard,
     size_categories_parser,
 )
 from distilabel.utils.files import list_files_in_dir
 
 
@@ -32,17 +33,20 @@
     """Convenient wrapper around `datasets.Dataset` to push to the Hugging Face Hub.
 
     It's a dictionary where the keys correspond to the different leaf_steps from the internal
     `DAG` and the values are `datasets.Dataset`.
 
     Attributes:
         pipeline_path: Optional path to the pipeline.yaml file that generated the dataset.
+        log_filename_path: Optional path to the pipeline.log file that generated was written by the
+            pipeline.
     """
 
     pipeline_path: Optional[Path] = None
+    log_filename_path: Optional[Path] = None
 
     def push_to_hub(
         self,
         repo_id: str,
         private: bool = False,
         token: Optional[str] = None,
         generate_card: bool = True,
@@ -118,14 +122,23 @@
             HfApi().upload_file(
                 path_or_fileobj=self.pipeline_path,
                 path_in_repo="pipeline.yaml",
                 repo_id=repo_id,
                 repo_type="dataset",
                 token=token,
             )
+        if self.log_filename_path:
+            # The same we had with "pipeline.yaml" but with the log file.
+            HfApi().upload_file(
+                path_or_fileobj=self.log_filename_path,
+                path_in_repo="pipeline.log",
+                repo_id=repo_id,
+                repo_type="dataset",
+                token=token,
+            )
 
     def _extract_readme_metadata(
         self, repo_id: str, token: Optional[str]
     ) -> Dict[str, Any]:
         """Extracts the metadata from the README.md file of the dataset repository.
 
         We have to download the previous README.md file in the repo, extract the metadata from it,
@@ -183,59 +196,79 @@
     def __repr__(self):
         # Copy from `datasets.DatasetDict.__repr__`.
         repr = "\n".join([f"{k}: {v}" for k, v in self.items()])
         repr = re.sub(r"^", " " * 4, repr, count=0, flags=re.M)
         return f"Distiset({{\n{repr}\n}})"
 
 
-def create_distiset(data_dir: Path, pipeline_path: Optional[Path] = None) -> Distiset:
+def create_distiset(  # noqa: C901
+    data_dir: Path,
+    pipeline_path: Optional[Path] = None,
+    log_filename_path: Optional[Path] = None,
+    enable_metadata: bool = False,
+) -> Distiset:
     """Creates a `Distiset` from the buffer folder.
 
     Args:
         data_dir: Folder where the data buffers were written by the `_WriteBuffer`.
             It should correspond to `CacheLocation.data`.
         pipeline_path: Optional path to the pipeline.yaml file that generated the dataset.
             Internally this will be passed to the `Distiset` object on creation to allow
             uploading the `pipeline.yaml` file to the repo upon `Distiset.push_to_hub`.
+        log_filename_path: Optional path to the pipeline.log file that was generated during the pipeline run.
+            Internally this will be passed to the `Distiset` object on creation to allow
+            uploading the `pipeline.log` file to the repo upon `Distiset.push_to_hub`.
+        enable_metadata: Whether to include the distilabel metadata column in the dataset or not.
+            Defaults to `False`.
 
     Returns:
         The dataset created from the buffer folder, where the different leaf steps will
         correspond to different configurations of the dataset.
     """
     logger = logging.getLogger("distilabel.distiset")
 
     data_dir = Path(data_dir)
 
     distiset = Distiset()
     for file in data_dir.iterdir():
         if file.is_file():
             continue
 
-        try:
-            files = [str(file) for file in list_files_in_dir(file)]
-            if files:
-                distiset[file.stem] = load_dataset(
+        files = [str(file) for file in list_files_in_dir(file)]
+        if files:
+            try:
+                ds = load_dataset(
                     "parquet", name=file.stem, data_files={"train": files}
                 )
-            else:
-                logger.warning(
-                    f"No output files for step '{file.stem}', can't create a dataset."
-                    " Did the step produce any data?"
-                )
-        except ArrowInvalid:
-            logger.warning(f"❌ Failed to load the subset from '{file}' directory.")
-            continue
+                if not enable_metadata and DISTILABEL_METADATA_KEY in ds.column_names:
+                    ds = ds.remove_columns(DISTILABEL_METADATA_KEY)
+                distiset[file.stem] = ds
+            except ArrowInvalid:
+                logger.warning(f"❌ Failed to load the subset from '{file}' directory.")
+                continue
+        else:
+            logger.warning(
+                f"No output files for step '{file.stem}', can't create a dataset."
+                " Did the step produce any data?"
+            )
 
     # If there's only one dataset i.e. one config, then set the config name to `default`
     if len(distiset.keys()) == 1:
         distiset["default"] = distiset.pop(list(distiset.keys())[0])
 
     if pipeline_path:
         distiset.pipeline_path = pipeline_path
     else:
         # If the pipeline path is not provided, try to find it in the parent directory
         # and assume that's the wanted file.
         pipeline_path = data_dir.parent / "pipeline.yaml"
         if pipeline_path.exists():
             distiset.pipeline_path = pipeline_path
 
+    if log_filename_path:
+        distiset.log_filename_path = log_filename_path
+    else:
+        log_filename_path = data_dir.parent / "pipeline.log"
+        if log_filename_path.exists():
+            distiset.log_filename_path = log_filename_path
+
     return distiset
```

### Comparing `distilabel-1.0.3/src/distilabel/cli/__init__.py` & `distilabel-1.1.0/src/distilabel/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/cli/app.py` & `distilabel-1.1.0/src/distilabel/cli/app.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/cli/pipeline/__init__.py` & `distilabel-1.1.0/src/distilabel/cli/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/cli/pipeline/app.py` & `distilabel-1.1.0/src/distilabel/cli/pipeline/app.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/cli/pipeline/utils.py` & `distilabel-1.1.0/src/distilabel/cli/pipeline/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Tuple
 
 import requests
 import yaml
 from pydantic import HttpUrl, ValidationError
 from pydantic.type_adapter import TypeAdapter
 
+from distilabel.pipeline.constants import (
+    ROUTING_BATCH_FUNCTION_ATTR_NAME,
+    STEP_ATTR_NAME,
+)
 from distilabel.pipeline.local import Pipeline
 
 if TYPE_CHECKING:
     from rich.panel import Panel
 
     from distilabel.pipeline.base import BasePipeline
 
@@ -159,14 +163,25 @@
             "\n",
             _build_steps_panel(pipeline),
             "\n",
             _build_steps_connection_panel(pipeline),
         ]
     )
 
+    if any(
+        pipeline.dag.get_step(step).get(ROUTING_BATCH_FUNCTION_ATTR_NAME) is not None
+        for step in pipeline.dag.G.nodes
+    ):
+        information.extend(
+            [
+                "\n",
+                _build_routing_batch_function_panel(pipeline),
+            ]
+        )
+
     return Panel(
         Group(*information),
         title="[magenta]Pipeline Information[/magenta]",
         expand=False,
         style="light_cyan3",
     )
 
@@ -210,15 +225,15 @@
             if optional != "":
                 optional = "Yes" if optional else "No"
 
             table.add_row(prefix + param["name"], param.get("description"), optional)
 
     steps = []
     for step_name, runtime_params in pipeline.get_runtime_parameters_info().items():
-        step = pipeline.dag.get_step(step_name)["step"]
+        step = pipeline.dag.get_step(step_name)[STEP_ATTR_NAME]
         class_name = step.__class__.__name__
 
         table = Table(
             title=f"{step.name} ([bold][magenta]{class_name}[/bold][/magenta])",
             show_header=True,
             header_style="bold magenta",
             expand=True,
@@ -270,7 +285,44 @@
 
     return Panel(
         table,
         title="[magenta]Steps connections[/magenta]",
         style="light_cyan3",
         expand=True,
     )
+
+
+def _build_routing_batch_function_panel(pipeline: "BasePipeline") -> "Panel":
+    """Builds a panel to display the routing batch function of the pipeline.
+
+    Args:
+        pipeline: The pipeline
+
+    Returns:
+        A `rich.panel.Panel` containing the routing batch function of the pipeline.
+    """
+    from rich.panel import Panel
+    from rich.table import Table
+
+    table = Table(show_header=True, header_style="bold magenta", expand=True)
+    table.add_column("Step", style="dim", width=18)
+    table.add_column("Function", style="dim")
+    table.add_column("Description", width=90)
+
+    G = pipeline.dag.G
+
+    for step_name in G.nodes:
+        node = pipeline.dag.get_step(step_name)
+        if routing_batch_function := node.get(ROUTING_BATCH_FUNCTION_ATTR_NAME):
+            table.add_row(
+                step_name,
+                routing_batch_function.routing_function.__name__,
+                routing_batch_function.description,
+            )
+            continue
+
+    return Panel(
+        table,
+        title="[magenta]Routing Batch Function[/magenta]",
+        style="light_cyan3",
+        expand=True,
+    )
```

### Comparing `distilabel-1.0.3/src/distilabel/llms/__init__.py` & `distilabel-1.1.0/src/distilabel/llms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 from distilabel.llms.anthropic import AnthropicLLM
 from distilabel.llms.anyscale import AnyscaleLLM
 from distilabel.llms.azure import AzureOpenAILLM
 from distilabel.llms.base import LLM, AsyncLLM
 from distilabel.llms.cohere import CohereLLM
+from distilabel.llms.groq import GroqLLM
 from distilabel.llms.huggingface import InferenceEndpointsLLM, TransformersLLM
 from distilabel.llms.litellm import LiteLLM
 from distilabel.llms.llamacpp import LlamaCppLLM
 from distilabel.llms.mistral import MistralLLM
 from distilabel.llms.mixins import CudaDevicePlacementMixin
 from distilabel.llms.ollama import OllamaLLM
 from distilabel.llms.openai import OpenAILLM
@@ -32,14 +33,15 @@
 __all__ = [
     "AnthropicLLM",
     "AnyscaleLLM",
     "AzureOpenAILLM",
     "LLM",
     "AsyncLLM",
     "CohereLLM",
+    "GroqLLM",
     "InferenceEndpointsLLM",
     "LiteLLM",
     "LlamaCppLLM",
     "MistralLLM",
     "CudaDevicePlacementMixin",
     "OllamaLLM",
     "OpenAILLM",
```

### Comparing `distilabel-1.0.3/src/distilabel/llms/anthropic.py` & `distilabel-1.1.0/src/distilabel/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/llms/anyscale.py` & `distilabel-1.1.0/src/distilabel/llms/anyscale.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,16 +20,15 @@
 from distilabel.llms.openai import OpenAILLM
 from distilabel.mixins.runtime_parameters import RuntimeParameter
 
 _ANYSCALE_API_KEY_ENV_VAR_NAME = "ANYSCALE_API_KEY"
 
 
 class AnyscaleLLM(OpenAILLM):
-    """Anyscale LLM implementation running the async API client of OpenAI because of
-    duplicate API behavior.
+    """Anyscale LLM implementation running the async API client of OpenAI.
 
     Attributes:
         model: the model name to use for the LLM, e.g., `google/gemma-7b-it`. See the
             supported models under the "Text Generation -> Supported Models" section
             [here](https://docs.endpoints.anyscale.com/).
         base_url: the base URL to use for the Anyscale API requests. Defaults to `None`, which
             means that the value set for the environment variable `ANYSCALE_BASE_URL` will be used, or
```

### Comparing `distilabel-1.0.3/src/distilabel/llms/azure.py` & `distilabel-1.1.0/src/distilabel/llms/azure.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,28 +25,30 @@
     from openai import AsyncAzureOpenAI
 
 _AZURE_OPENAI_ENDPOINT_ENV_VAR_NAME = "AZURE_OPENAI_ENDPOINT"
 _AZURE_OPENAI_API_KEY_ENV_VAR_NAME = "AZURE_OPENAI_API_KEY"
 
 
 class AzureOpenAILLM(OpenAILLM):
-    """Azure OpenAI LLM implementation running the async API client of OpenAI because of
-    duplicate API behavior, but with Azure-specific parameters.
+    """Azure OpenAI LLM implementation running the async API client.
 
     Attributes:
         model: the model name to use for the LLM i.e. the name of the Azure deployment.
         base_url: the base URL to use for the Azure OpenAI API can be set with `AZURE_OPENAI_ENDPOINT`.
             Defaults to `None` which means that the value set for the environment variable
             `AZURE_OPENAI_ENDPOINT` will be used, or `None` if not set.
         api_key: the API key to authenticate the requests to the Azure OpenAI API. Defaults to `None`
             which means that the value set for the environment variable `AZURE_OPENAI_API_KEY` will be
             used, or `None` if not set.
         api_version: the API version to use for the Azure OpenAI API. Defaults to `None` which means
             that the value set for the environment variable `OPENAI_API_VERSION` will be used, or
             `None` if not set.
+
+    Icon:
+        `:simple-microsoftazure:`
     """
 
     base_url: Optional[RuntimeParameter[str]] = Field(
         default_factory=lambda: os.getenv(_AZURE_OPENAI_ENDPOINT_ENV_VAR_NAME),
         description="The base URL to use for the Azure OpenAI API requests i.e. the Azure OpenAI endpoint.",
     )
     api_key: Optional[RuntimeParameter[SecretStr]] = Field(
```

### Comparing `distilabel-1.0.3/src/distilabel/llms/base.py` & `distilabel-1.1.0/src/distilabel/llms/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,18 +29,18 @@
 from distilabel.utils.docstring import parse_google_docstring
 from distilabel.utils.notebook import in_notebook
 from distilabel.utils.serialization import _Serializable
 
 if TYPE_CHECKING:
     from distilabel.llms.typing import GenerateOutput, HiddenState
     from distilabel.mixins.runtime_parameters import RuntimeParametersNames
+    from distilabel.steps.tasks.structured_outputs.outlines import StructuredOutputType
     from distilabel.steps.tasks.typing import ChatType
     from distilabel.utils.docstring import Docstring
 
-
 if in_notebook():
     import nest_asyncio
 
     nest_asyncio.apply()
 
 
 class LLM(RuntimeParametersMixin, BaseModel, _Serializable, ABC):
@@ -51,35 +51,39 @@
             so the `_logger` attribute is initialized.
         - `model_name` property to return the model name used for the LLM.
         - `generate` method to generate `num_generations` per input in `inputs`.
 
     Attributes:
         generation_kwargs: the kwargs to be propagated to either `generate` or `agenerate`
             methods within each `LLM`.
+        structured_output: a dictionary containing the structured output configuration or if more
+            fine-grained control is needed, an instance of `OutlinesStructuredOutput`. Defaults to None.
         _logger: the logger to be used for the `LLM`. It will be initialized when the `load`
             method is called.
     """
 
     model_config = ConfigDict(
         arbitrary_types_allowed=True,
         protected_namespaces=(),
         validate_default=True,
         validate_assignment=True,
+        extra="forbid",
     )
 
     generation_kwargs: Optional[RuntimeParameter[Dict[str, Any]]] = Field(
         default_factory=dict,
         description="The kwargs to be propagated to either `generate` or `agenerate`"
         " methods within each `LLM`.",
     )
+    structured_output: Optional[Any] = None
 
     _logger: Union[logging.Logger, None] = PrivateAttr(...)
 
     def load(self) -> None:
-        """Method to be called to initialize the `LLM` and its logger."""
+        """Method to be called to initialize the `LLM`, its logger and optionally the structured output generator."""
         self._logger = logging.getLogger(f"distilabel.llm.{self.model_name}")
 
     @property
     @abstractmethod
     def model_name(self) -> str:
         """Returns the model name used for the LLM."""
         pass
@@ -190,14 +194,32 @@
             A list containing the last hidden state for each sequence using a NumPy array
                 with shape [num_tokens, hidden_size].
         """
         raise NotImplementedError(
             f"Method `get_last_hidden_states` is not implemented for `{self.__class__.__name__}`"
         )
 
+    def _prepare_structured_output(
+        self, structured_output: Optional["StructuredOutputType"] = None
+    ) -> Union[Any, None]:
+        """Method in charge of preparing the structured output generator.
+
+        By default will raise a `NotImplementedError`, subclasses that allow it must override this
+        method with the implementation.
+
+        Args:
+            structured_output: the config to prepare the guided generation.
+
+        Returns:
+            The structure to be used for the guided generation.
+        """
+        raise NotImplementedError(
+            f"Guided generation is not implemented for `{type(self).__name__}`"
+        )
+
 
 class AsyncLLM(LLM):
     """Abstract class for asynchronous LLMs, so as to benefit from the async capabilities
     of each LLM implementation. This class is meant to be subclassed by each LLM, and the
     method `agenerate` needs to be implemented to provide the asynchronous generation of
     responses.
```

### Comparing `distilabel-1.0.3/src/distilabel/llms/chat_templates.py` & `distilabel-1.1.0/src/distilabel/llms/chat_templates.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/llms/cohere.py` & `distilabel-1.1.0/src/distilabel/llms/cohere.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 
 _COHERE_API_KEY_ENV_VAR_NAME = "COHERE_API_KEY"
 
 
 class CohereLLM(AsyncLLM):
     """Cohere API implementation using the async client for concurrent text generation.
 
-
     Attributes:
         model: the name of the model from the Cohere API to use for the generation.
         base_url: the base URL to use for the Cohere API requests. Defaults to
             `"https://api.cohere.ai/v1"`.
         api_key: the API key to authenticate the requests to the Cohere API. Defaults to
             the value of the `COHERE_API_KEY` environment variable.
         timeout: the maximum time in seconds to wait for a response from the API. Defaults
```

### Comparing `distilabel-1.0.3/src/distilabel/llms/litellm.py` & `distilabel-1.1.0/src/distilabel/llms/litellm.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,16 @@
     from litellm import Choices
 
 
 class LiteLLM(AsyncLLM):
     """LiteLLM implementation running the async API client.
 
     Attributes:
-        model: the model name to use for the LLM e.g. "gpt-3.5-turbo" or "mistral/mistral-large", etc.
+        model: the model name to use for the LLM e.g. "gpt-3.5-turbo" or "mistral/mistral-large",
+            etc.
         verbose: whether to log the LiteLLM client's logs. Defaults to `False`.
 
     Runtime parameters:
         - `verbose`: whether to log the LiteLLM client's logs. Defaults to `False`.
     """
 
     model: str
```

### Comparing `distilabel-1.0.3/src/distilabel/llms/llamacpp.py` & `distilabel-1.1.0/src/distilabel/llms/ollama.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,124 +8,147 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import TYPE_CHECKING, List, Optional
+from typing import TYPE_CHECKING, List, Literal, Optional, Sequence, Union
 
-from pydantic import Field, FilePath, PrivateAttr, validate_call
+from pydantic import Field, PrivateAttr, validate_call
+from typing_extensions import TypedDict
 
-from distilabel.llms.base import LLM
-from distilabel.llms.typing import GenerateOutput
+from distilabel.llms.base import AsyncLLM
 from distilabel.mixins.runtime_parameters import RuntimeParameter
 from distilabel.steps.tasks.typing import ChatType
 
 if TYPE_CHECKING:
-    from llama_cpp import CreateChatCompletionResponse, Llama
+    from ollama import AsyncClient
 
 
-class LlamaCppLLM(LLM):
-    """llama.cpp LLM implementation running the Python bindings for the C++ code.
+# Copied from `ollama._types.Options`
+class Options(TypedDict, total=False):
+    # load time options
+    numa: bool
+    num_ctx: int
+    num_batch: int
+    num_gqa: int
+    num_gpu: int
+    main_gpu: int
+    low_vram: bool
+    f16_kv: bool
+    logits_all: bool
+    vocab_only: bool
+    use_mmap: bool
+    use_mlock: bool
+    embedding_only: bool
+    rope_frequency_base: float
+    rope_frequency_scale: float
+    num_thread: int
+
+    # runtime options
+    num_keep: int
+    seed: int
+    num_predict: int
+    top_k: int
+    top_p: float
+    tfs_z: float
+    typical_p: float
+    repeat_last_n: int
+    temperature: float
+    repeat_penalty: float
+    presence_penalty: float
+    frequency_penalty: float
+    mirostat: int
+    mirostat_tau: float
+    mirostat_eta: float
+    penalize_newline: bool
+    stop: Sequence[str]
+
+
+class OllamaLLM(AsyncLLM):
+    """Ollama LLM implementation running the Async API client.
 
     Attributes:
-        chat_format: the chat format to use for the model. Defaults to `chatml`.
-        model_path: contains the path to the GGUF quantized model, compatible with the
-            installed version of the `llama.cpp` Python bindings.
-        n_gpu_layers: the number of layers to use for the GPU. Defaults to `-1`, meaning that
-            the available GPU device will be used.
-        verbose: whether to print verbose output. Defaults to `False`.
-        _model: the Llama model instance. This attribute is meant to be used internally and
-            should not be accessed directly. It will be set in the `load` method.
+        model: the model name to use for the LLM e.g. "notus".
+        host: the Ollama server host.
+        timeout: the timeout for the LLM. Defaults to `120`.
+        _aclient: the `AsyncClient` to use for the Ollama API. It is meant to be used internally.
+            Set in the `load` method.
 
     Runtime parameters:
-        - `model_path`: the path to the GGUF quantized model.
-        - `n_gpu_layers`: the number of layers to use for the GPU. Defaults to `-1`.
-        - `verbose`: whether to print verbose output. Defaults to `False`.
+        - `host`: the Ollama server host.
+        - `timeout`: the client timeout for the Ollama API. Defaults to `120`.
     """
 
-    chat_format: str = "chatml"
-    model_path: RuntimeParameter[FilePath] = Field(
-        default=None, description="The path to the GGUF quantized model."
-    )
-    n_gpu_layers: RuntimeParameter[int] = Field(
-        default=-1,
-        description="The number of layers that will be loaded in the GPU.",
+    model: str
+    host: Optional[RuntimeParameter[str]] = Field(
+        default=None, description="The host of the Ollama API."
     )
-    verbose: RuntimeParameter[bool] = Field(
-        default=False,
-        description="Whether to print verbose output from llama.cpp library.",
+    timeout: RuntimeParameter[int] = Field(
+        default=120, description="The timeout for the Ollama API."
     )
+    follow_redirects: bool = True
 
-    _model: Optional["Llama"] = PrivateAttr(...)
+    _aclient: Optional["AsyncClient"] = PrivateAttr(...)
 
     def load(self) -> None:
-        """Loads the `Llama` model from the `model_path`."""
+        """Loads the `AsyncClient` to use Ollama async API."""
+        super().load()
 
         try:
-            from llama_cpp import Llama
-        except ImportError as ie:
-            raise ImportError(
-                "The `llama_cpp` package is required to use the `LlamaCppLLM` class."
-            ) from ie
+            from ollama import AsyncClient
 
-        self._model = Llama(
-            model_path=self.model_path.as_posix(),
-            chat_format=self.chat_format,
-            n_gpu_layers=self.n_gpu_layers,
-            verbose=self.verbose,
-        )
-
-        super().load()
+            self._aclient = AsyncClient(
+                host=self.host,
+                timeout=self.timeout,
+                follow_redirects=self.follow_redirects,
+            )
+        except ImportError as e:
+            raise ImportError(
+                "Ollama Python client is not installed. Please install it using"
+                " `pip install ollama`."
+            ) from e
 
     @property
     def model_name(self) -> str:
         """Returns the model name used for the LLM."""
-        return self._model.model_path  # type: ignore
+        return self.model
 
     @validate_call
-    def generate(  # type: ignore
+    async def agenerate(  # type: ignore
         self,
-        inputs: List[ChatType],
+        input: ChatType,
         num_generations: int = 1,
-        max_new_tokens: int = 128,
-        frequency_penalty: float = 0.0,
-        presence_penalty: float = 0.0,
-        temperature: float = 1.0,
-        top_p: float = 1.0,
-    ) -> List[GenerateOutput]:
-        """Generates `num_generations` responses for the given input using the Llama model.
+        format: Literal["", "json"] = "",
+        # TODO: include relevant options from `Options` in `agenerate` method.
+        options: Union[Options, None] = None,
+        keep_alive: Union[bool, None] = None,
+    ) -> List[str]:
+        """
+        Generates a response asynchronously, using the [Ollama Async API definition](https://github.com/ollama/ollama-python).
 
         Args:
-            inputs: a list of inputs in chat format to generate responses for.
-            num_generations: the number of generations to create per input. Defaults to
-                `1`.
-            max_new_tokens: the maximum number of new tokens that the model will generate.
-                Defaults to `128`.
-            frequency_penalty: the repetition penalty to use for the generation. Defaults
-                to `0.0`.
-            presence_penalty: the presence penalty to use for the generation. Defaults to
-                `0.0`.
-            temperature: the temperature to use for the generation. Defaults to `0.1`.
-            top_p: the top-p value to use for the generation. Defaults to `1.0`.
+            input: the input to use for the generation.
+            num_generations: the number of generations to produce. Defaults to `1`.
+            format: the format to use for the generation. Defaults to `""`.
+            options: the options to use for the generation. Defaults to `None`.
+            keep_alive: whether to keep the connection alive. Defaults to `None`.
 
         Returns:
-            A list of lists of strings containing the generated responses for each input.
+            A list of strings as completion for the given input.
         """
-        batch_outputs = []
-        for input in inputs:
-            outputs = []
-            for _ in range(num_generations):
-                chat_completions: "CreateChatCompletionResponse" = (
-                    self._model.create_chat_completion(  # type: ignore
-                        messages=input,  # type: ignore
-                        max_tokens=max_new_tokens,
-                        frequency_penalty=frequency_penalty,
-                        presence_penalty=presence_penalty,
-                        temperature=temperature,
-                        top_p=top_p,
-                    )
-                )
-                outputs.append(chat_completions["choices"][0]["message"]["content"])
-            batch_outputs.append(outputs)
-        return batch_outputs
+        generations = []
+        # TODO: remove this for-loop and override the `generate` method
+        for _ in range(num_generations):
+            completion = await self._aclient.chat(  # type: ignore
+                model=self.model,
+                messages=input,  # type: ignore
+                stream=False,
+                format=format,
+                options=options,
+                keep_alive=keep_alive,
+            )
+            # TODO: improve error handling
+            generations.append(completion["message"]["content"])
+
+        return generations
```

### Comparing `distilabel-1.0.3/src/distilabel/llms/mistral.py` & `distilabel-1.1.0/src/distilabel/llms/mistral.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/llms/mixins.py` & `distilabel-1.1.0/src/distilabel/llms/mixins.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/llms/ollama.py` & `distilabel-1.1.0/src/distilabel/steps/tasks/self_instruct.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,147 +8,124 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import TYPE_CHECKING, List, Literal, Optional, Sequence, Union
+import sys
 
-from pydantic import Field, PrivateAttr, validate_call
-from typing_extensions import TypedDict
+if sys.version_info < (3, 9):
+    import importlib_resources
+else:
+    import importlib.resources as importlib_resources
 
-from distilabel.llms.base import AsyncLLM
-from distilabel.mixins.runtime_parameters import RuntimeParameter
-from distilabel.steps.tasks.typing import ChatType
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
-if TYPE_CHECKING:
-    from ollama import AsyncClient
+from jinja2 import Template
+from pydantic import PrivateAttr
+
+from distilabel.steps.tasks.base import Task
 
+if TYPE_CHECKING:
+    from distilabel.steps.tasks.typing import ChatType
 
-# Copied from `ollama._types.Options`
-class Options(TypedDict, total=False):
-    # load time options
-    numa: bool
-    num_ctx: int
-    num_batch: int
-    num_gqa: int
-    num_gpu: int
-    main_gpu: int
-    low_vram: bool
-    f16_kv: bool
-    logits_all: bool
-    vocab_only: bool
-    use_mmap: bool
-    use_mlock: bool
-    embedding_only: bool
-    rope_frequency_base: float
-    rope_frequency_scale: float
-    num_thread: int
-
-    # runtime options
-    num_keep: int
-    seed: int
-    num_predict: int
-    top_k: int
-    top_p: float
-    tfs_z: float
-    typical_p: float
-    repeat_last_n: int
-    temperature: float
-    repeat_penalty: float
-    presence_penalty: float
-    frequency_penalty: float
-    mirostat: int
-    mirostat_tau: float
-    mirostat_eta: float
-    penalize_newline: bool
-    stop: Sequence[str]
 
+class SelfInstruct(Task):
+    """Generate instructions based on a given input using an `LLM`.
 
-class OllamaLLM(AsyncLLM):
-    """Ollama LLM implementation running the Async API client.
+    `SelfInstruct` is a pre-defined task that, given a number of instructions, a
+    certain criteria for query generations, an application description, and an input,
+    generates a number of instruction related to the given input and following what
+    is stated in the criteria for query generation and the application description.
+    It is based in the SelfInstruct framework from the paper "Self-Instruct: Aligning
+    Language Models with Self-Generated Instructions".
 
     Attributes:
-        model: the model name to use for the LLM e.g. "notus".
-        host: the Ollama server host.
-        timeout: the timeout for the LLM. Defaults to `120`.
-        _aclient: the `AsyncClient` to use for the Ollama API. It is meant to be used internally.
-            Set in the `load` method.
-
-    Runtime parameters:
-        - `host`: the Ollama server host.
-        - `timeout`: the client timeout for the Ollama API. Defaults to `120`.
+        num_instructions: The number of instructions to be generated. Defaults to 5.
+        criteria_for_query_generation: The criteria for the query generation. Defaults
+            to the criteria defined within the paper.
+        application_description: The description of the AI application that one want
+            to build with these instructions. Defaults to `AI assistant`.
+
+    Input columns:
+        - input (`str`): The input to generate the instructions. It's also called seed in
+            the paper.
+
+    Output columns:
+        - instructions (`List[str]`): The generated instructions.
+        - model_name (`str`): The model name used to generate the instructions.
+
+    Categories:
+        - text-generation
+
+    Reference:
+        - [`Self-Instruct: Aligning Language Models with Self-Generated Instructions`](https://arxiv.org/abs/2212.10560)
     """
 
-    model: str
-    host: Optional[RuntimeParameter[str]] = Field(
-        default=None, description="The host of the Ollama API."
+    num_instructions: int = 5
+    criteria_for_query_generation: str = (
+        "Incorporate a diverse range of verbs, avoiding repetition.\n"
+        "Ensure queries are compatible with AI model's text generation functions and are limited to 1-2 sentences.\n"
+        "Design queries to be self-contained and standalone.\n"
+        'Blend interrogative (e.g., "What is the significance of x?") and imperative (e.g., "Detail the process of x.") styles.'
     )
-    timeout: RuntimeParameter[int] = Field(
-        default=120, description="The timeout for the Ollama API."
-    )
-    follow_redirects: bool = True
+    application_description: str = "AI assistant"
 
-    _aclient: Optional["AsyncClient"] = PrivateAttr(...)
+    _template: Union[Template, None] = PrivateAttr(...)
 
     def load(self) -> None:
-        """Loads the `AsyncClient` to use Ollama async API."""
+        """Loads the Jinja2 template."""
         super().load()
 
-        try:
-            from ollama import AsyncClient
+        _path = str(
+            importlib_resources.files("distilabel")
+            / "steps"
+            / "tasks"
+            / "templates"
+            / "self-instruct.jinja2"
+        )
+
+        self._template = Template(open(_path).read())
 
-            self._aclient = AsyncClient(
-                host=self.host,
-                timeout=self.timeout,
-                follow_redirects=self.follow_redirects,
-            )
-        except ImportError as e:
-            raise ImportError(
-                "Ollama Python client is not installed. Please install it using"
-                " `pip install ollama`."
-            ) from e
+    @property
+    def inputs(self) -> List[str]:
+        """The input for the task is the `input` i.e. seed text."""
+        return ["input"]
+
+    def format_input(self, input: Dict[str, Any]) -> "ChatType":
+        """The input is formatted as a `ChatType` assuming that the instruction
+        is the first interaction from the user within a conversation."""
+        return [
+            {
+                "role": "user",
+                "content": self._template.render(
+                    input=input["input"],
+                    application_description=self.application_description,
+                    criteria_for_query_generation=self.criteria_for_query_generation,
+                    num_instructions=self.num_instructions,
+                ),
+            }
+        ]
 
     @property
-    def model_name(self) -> str:
-        """Returns the model name used for the LLM."""
-        return self.model
+    def outputs(self):
+        """The output for the task is a list of `instructions` containing the generated instructions."""
+        return ["instructions", "model_name"]
 
-    @validate_call
-    async def agenerate(  # type: ignore
+    def format_output(
         self,
-        input: ChatType,
-        num_generations: int = 1,
-        format: Literal["", "json"] = "",
-        # TODO: include relevant options from `Options` in `agenerate` method.
-        options: Union[Options, None] = None,
-        keep_alive: Union[bool, None] = None,
-    ) -> List[str]:
-        """
-        Generates a response asynchronously, using the [Ollama Async API definition](https://github.com/ollama/ollama-python).
+        output: Union[str, None],
+        input: Optional[Dict[str, Any]] = None,
+    ) -> Dict[str, Any]:
+        """The output is formatted as a list with the generated instructions.
 
         Args:
-            input: the input to use for the generation.
-            num_generations: the number of generations to produce. Defaults to `1`.
-            format: the format to use for the generation. Defaults to `""`.
-            options: the options to use for the generation. Defaults to `None`.
-            keep_alive: whether to keep the connection alive. Defaults to `None`.
+            output: the raw output of the LLM.
+            input: the input to the task. Used for obtaining the number of responses.
 
         Returns:
-            A list of strings as completion for the given input.
+            A dict with containing the generated instructions.
         """
-        generations = []
-        # TODO: remove this for-loop and override the `generate` method
-        for _ in range(num_generations):
-            completion = await self._aclient.chat(  # type: ignore
-                model=self.model,
-                messages=input,  # type: ignore
-                stream=False,
-                format=format,
-                options=options,
-                keep_alive=keep_alive,
-            )
-            # TODO: improve error handling
-            generations.append(completion["message"]["content"])
-
-        return generations
+        if output is None:
+            return {"instructions": []}
+        return {"instructions": [line for line in output.split("\n") if line != ""]}
```

### Comparing `distilabel-1.0.3/src/distilabel/llms/openai.py` & `distilabel-1.1.0/src/distilabel/llms/openai.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,23 +41,28 @@
         api_key: the API key to authenticate the requests to the OpenAI API. Defaults to
             `None` which means that the value set for the environment variable `OPENAI_API_KEY`
             will be used, or `None` if not set.
         max_retries: the maximum number of times to retry the request to the API before
             failing. Defaults to `6`.
         timeout: the maximum time in seconds to wait for a response from the API. Defaults
             to `120`.
+        structured_output: a dictionary containing the structured output configuration or if more
+            fine-grained control is needed, an instance of `OutlinesStructuredOutput`. Defaults to None.
 
     Runtime parameters:
         - `base_url`: the base URL to use for the OpenAI API requests. Defaults to `None`.
         - `api_key`: the API key to authenticate the requests to the OpenAI API. Defaults
             to `None`.
         - `max_retries`: the maximum number of times to retry the request to the API before
             failing. Defaults to `6`.
         - `timeout`: the maximum time in seconds to wait for a response from the API. Defaults
             to `120`.
+
+    Icon:
+        `:simple-openai:`
     """
 
     model: str
     base_url: Optional[RuntimeParameter[str]] = Field(
         default_factory=lambda: os.getenv(
             "OPENAI_BASE_URL", "https://api.openai.com/v1"
         ),
@@ -117,14 +122,15 @@
         num_generations: int = 1,
         max_new_tokens: int = 128,
         frequency_penalty: float = 0.0,
         presence_penalty: float = 0.0,
         temperature: float = 1.0,
         top_p: float = 1.0,
         stop: Optional[Union[str, List[str]]] = None,
+        response_format: str = "text",
     ) -> GenerateOutput:
         """Generates `num_generations` responses for the given input using the OpenAI async
         client.
 
         Args:
             input: a single input in chat format to generate responses for.
             num_generations: the number of generations to create per input. Defaults to
@@ -135,29 +141,43 @@
                 to `0.0`.
             presence_penalty: the presence penalty to use for the generation. Defaults to
                 `0.0`.
             temperature: the temperature to use for the generation. Defaults to `0.1`.
             top_p: the top-p value to use for the generation. Defaults to `1.0`.
             stop: a string or a list of strings to use as a stop sequence for the generation.
                 Defaults to `None`.
+            response_format: the format of the response to return. Must be one of
+                "text" or "json". Read the documentation [here](https://platform.openai.com/docs/guides/text-generation/json-mode)
+                for more information on how to use the JSON model from OpenAI. Defaults to `text`.
+
+        Note:
+            If response_format
 
         Returns:
             A list of lists of strings containing the generated responses for each input.
         """
+        if response_format == "json":
+            response_format = "json_object"
+        elif response_format != "text":
+            raise ValueError(
+                f"Invalid response format '{response_format}'. Must be either 'text' or 'json'."
+            )
+
         completion = await self._aclient.chat.completions.create(  # type: ignore
             messages=input,  # type: ignore
             model=self.model,
             max_tokens=max_new_tokens,
             n=num_generations,
             frequency_penalty=frequency_penalty,
             presence_penalty=presence_penalty,
             temperature=temperature,
             top_p=top_p,
             stop=stop,
             timeout=50,
+            response_format={"type": response_format},
         )
         generations = []
         for choice in completion.choices:
             if (content := choice.message.content) is None:
                 self._logger.warning(  # type: ignore
                     f"Received no response using OpenAI client (model: '{self.model}')."
                     f" Finish reason was: {choice.finish_reason}"
```

### Comparing `distilabel-1.0.3/src/distilabel/llms/together.py` & `distilabel-1.1.0/src/distilabel/llms/together.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,16 +20,15 @@
 from distilabel.llms.openai import OpenAILLM
 from distilabel.mixins.runtime_parameters import RuntimeParameter
 
 _TOGETHER_API_KEY_ENV_VAR_NAME = "TOGETHER_API_KEY"
 
 
 class TogetherLLM(OpenAILLM):
-    """TogetherLLM LLM implementation running the async API client of OpenAI because of
-    duplicate API behavior.
+    """TogetherLLM LLM implementation running the async API client of OpenAI.
 
     Attributes:
         model: the model name to use for the LLM e.g. "mistralai/Mixtral-8x7B-Instruct-v0.1".
             Supported models can be found [here](https://api.together.xyz/models).
         base_url: the base URL to use for the Together API can be set with `TOGETHER_BASE_URL`.
             Defaults to `None` which means that the value set for the environment variable
             `TOGETHER_BASE_URL` will be used, or "https://api.together.xyz/v1" if not set.
```

### Comparing `distilabel-1.0.3/src/distilabel/llms/typing.py` & `distilabel-1.1.0/src/distilabel/llms/typing.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/llms/vertexai.py` & `distilabel-1.1.0/src/distilabel/llms/vertexai.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,21 @@
     - Using `gcloud auth application-default login` command
     - Using `vertexai.init` function from the `google-cloud-aiplatform` library
 
     Attributes:
         model: the model name to use for the LLM e.g. "gemini-1.0-pro". [Supported models](https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models).
         _aclient: the `GenerativeModel` to use for the Vertex AI Gemini API. It is meant
             to be used internally. Set in the `load` method.
+
+    Icon:
+        `:simple-googlecloud:`
     """
 
     model: str
+
     _aclient: Optional["GenerativeModel"] = PrivateAttr(...)
 
     def load(self) -> None:
         """Loads the `GenerativeModel` class which has access to `generate_content_async` to benefit from async requests."""
         super().load()
 
         try:
```

### Comparing `distilabel-1.0.3/src/distilabel/llms/vllm.py` & `distilabel-1.1.0/src/distilabel/llms/vllm.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,66 +8,100 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import TYPE_CHECKING, Any, Dict, List, Optional
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Literal, Optional, Union
 
 from pydantic import Field, PrivateAttr, validate_call
 
 from distilabel.llms.base import LLM
 from distilabel.llms.chat_templates import CHATML_TEMPLATE
 from distilabel.llms.mixins import CudaDevicePlacementMixin
 from distilabel.llms.typing import GenerateOutput
 from distilabel.mixins.runtime_parameters import RuntimeParameter
 from distilabel.steps.tasks.typing import ChatType
 
 if TYPE_CHECKING:
     from transformers import PreTrainedTokenizer
     from vllm import LLM as _vLLM
 
+    from distilabel.steps.tasks.structured_outputs.outlines import StructuredOutputType
+
 
 SamplingParams = None
 
 
 class vLLM(LLM, CudaDevicePlacementMixin):
     """`vLLM` library LLM implementation.
 
     Attributes:
         model: the model Hugging Face Hub repo id or a path to a directory containing the
             model weights and configuration files.
-        model_kwargs: additional dictionary of keyword arguments that will be passed to
-            the `LLM` class of `vllm` library.
+        dtype: the data type to use for the model. Defaults to `auto`.
+        trust_remote_code: whether to trust the remote code when loading the model. Defaults
+            to `False`.
+        quantization: the quantization mode to use for the model. Defaults to `None`.
+        revision: the revision of the model to load. Defaults to `None`.
+        tokenizer: the tokenizer Hugging Face Hub repo id or a path to a directory containing
+            the tokenizer files. If not provided, the tokenizer will be loaded from the
+            model directory. Defaults to `None`.
+        tokenizer_mode: the mode to use for the tokenizer. Defaults to `auto`.
+        tokenizer_revision: the revision of the tokenizer to load. Defaults to `None`.
+        skip_tokenizer_init: whether to skip the initialization of the tokenizer. Defaults
+            to `False`.
         chat_template: a chat template that will be used to build the prompts before
             sending them to the model. If not provided, the chat template defined in the
             tokenizer config will be used. If not provided and the tokenizer doesn't have
             a chat template, then ChatML template will be used. Defaults to `None`.
+        structured_output: a dictionary containing the structured output configuration or if more
+            fine-grained control is needed, an instance of `OutlinesStructuredOutput`. Defaults to None.
+        seed: the seed to use for the random number generator. Defaults to `0`.
+        extra_kwargs: additional dictionary of keyword arguments that will be passed to the
+            `LLM` class of `vllm` library. Defaults to `{}`.
         _model: the `vLLM` model instance. This attribute is meant to be used internally
             and should not be accessed directly. It will be set in the `load` method.
         _tokenizer: the tokenizer instance used to format the prompt before passing it to
             the `LLM`. This attribute is meant to be used internally and should not be
             accessed directly. It will be set in the `load` method.
 
+    References:
+        - https://github.com/vllm-project/vllm/blob/main/vllm/entrypoints/llm.py
+
     Runtime parameters:
-        - `model_kwargs`: additional dictionary of keyword arguments that will be passed to
+        - `extra_kwargs`: additional dictionary of keyword arguments that will be passed to
             the `LLM` class of `vllm` library.
     """
 
     model: str
-    model_kwargs: Optional[RuntimeParameter[Dict[str, Any]]] = Field(
+    dtype: str = "auto"
+    trust_remote_code: bool = False
+    quantization: Optional[str] = None
+    revision: Optional[str] = None
+
+    tokenizer: Optional[str] = None
+    tokenizer_mode: Literal["auto", "slow"] = "auto"
+    tokenizer_revision: Optional[str] = None
+    skip_tokenizer_init: bool = False
+    chat_template: Optional[str] = None
+
+    seed: int = 0
+
+    extra_kwargs: Optional[RuntimeParameter[Dict[str, Any]]] = Field(
         default_factory=dict,
         description="Additional dictionary of keyword arguments that will be passed to the"
-        " `LLM` class of `vllm` library.",
+        " `vLLM` class of `vllm` library. See all the supported arguments at: "
+        "https://github.com/vllm-project/vllm/blob/main/vllm/entrypoints/llm.py",
     )
-    chat_template: Optional[str] = None
 
     _model: Optional["_vLLM"] = PrivateAttr(...)
     _tokenizer: Optional["PreTrainedTokenizer"] = PrivateAttr(...)
+    _logits_processor: Optional[Callable] = PrivateAttr(default=None)
 
     def load(self) -> None:
         """Loads the `vLLM` model using either the path or the Hugging Face Hub repository id.
         Additionally, this method also sets the `chat_template` for the tokenizer, so as to properly
         parse the list of OpenAI formatted inputs using the expected format by the model, otherwise, the
         default value is ChatML format, unless explicitly provided.
         """
@@ -82,25 +116,42 @@
             global SamplingParams
             SamplingParams = _SamplingParams
         except ImportError as ie:
             raise ImportError(
                 "vLLM is not installed. Please install it using `pip install vllm`."
             ) from ie
 
-        self._model = _vLLM(self.model, **self.model_kwargs)  # type: ignore
-        self._tokenizer = self._model.get_tokenizer()  # type: ignore
+        self._model = _vLLM(
+            self.model,
+            dtype=self.dtype,
+            trust_remote_code=self.trust_remote_code,
+            quantization=self.quantization,
+            revision=self.revision,
+            tokenizer=self.tokenizer,
+            tokenizer_mode=self.tokenizer_mode,
+            tokenizer_revision=self.tokenizer_revision,
+            skip_tokenizer_init=self.skip_tokenizer_init,
+            seed=self.seed,
+            **self.extra_kwargs,
+        )
 
+        self._tokenizer = self._model.get_tokenizer()  # type: ignore
         if self.chat_template is not None:
             self._tokenizer.chat_template = self.chat_template  # type: ignore
         elif (
             self._tokenizer.chat_template is None  # type: ignore
             and self._tokenizer.default_chat_template is None  # type: ignore
         ):
             self._tokenizer.chat_template = CHATML_TEMPLATE
 
+        if self.structured_output:
+            self._logits_processor = self._prepare_structured_output(
+                self.structured_output
+            )
+
     @property
     def model_name(self) -> str:
         """Returns the model name used for the LLM."""
         return self.model
 
     def prepare_input(self, input: "ChatType") -> str:
         """Prepares the input by applying the chat template to the input, which is formatted
@@ -143,30 +194,52 @@
             top_k: the top-k value to use for the generation. Defaults to `0`.
             extra_sampling_params: dictionary with additional arguments to be passed to
                 the `SamplingParams` class from `vllm`.
 
         Returns:
             A list of lists of strings containing the generated responses for each input.
         """
+        prepared_inputs = [self.prepare_input(input) for input in inputs]
+
         if extra_sampling_params is None:
             extra_sampling_params = {}
 
         sampling_params = SamplingParams(  # type: ignore
             n=num_generations,
             presence_penalty=presence_penalty,
             frequency_penalty=frequency_penalty,
             temperature=temperature,
             top_p=top_p,
             top_k=top_k,
             max_tokens=max_new_tokens,
+            logits_processors=[self._logits_processor],
             **extra_sampling_params,
         )
 
-        prepared_inputs = [self.prepare_input(input) for input in inputs]
         batch_outputs = self._model.generate(  # type: ignore
             prepared_inputs,
             sampling_params,
             use_tqdm=False,  # type: ignore
         )
         return [
             [output.text for output in outputs.outputs] for outputs in batch_outputs
         ]
+
+    def _prepare_structured_output(
+        self, structured_output: Optional["StructuredOutputType"] = None
+    ) -> Union[Callable, None]:
+        """Creates the appropriate function to filter tokens to generate structured outputs.
+
+        Args:
+            structured_output: the configuration dict to prepare the structured output.
+
+        Returns:
+            The callable that will be used to guide the generation of the model.
+        """
+        from distilabel.steps.tasks.structured_outputs.outlines import (
+            prepare_guided_output,
+        )
+
+        result = prepare_guided_output(structured_output, "vllm", self._model)
+        if schema := result.get("schema"):
+            self.structured_output["schema"] = schema
+        return result["processor"]
```

### Comparing `distilabel-1.0.3/src/distilabel/llms/huggingface/__init__.py` & `distilabel-1.1.0/src/distilabel/llms/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/llms/huggingface/inference_endpoints.py` & `distilabel-1.1.0/src/distilabel/llms/huggingface/inference_endpoints.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,47 +40,80 @@
     from transformers import PreTrainedTokenizer
 
 
 _INFERENCE_ENDPOINTS_API_KEY_ENV_VAR_NAME = "HF_TOKEN"
 
 
 class InferenceEndpointsLLM(AsyncLLM):
-    """InferenceEndpoints LLM implementation running the async API client via either
-    the `huggingface_hub.AsyncInferenceClient` or via `openai.AsyncOpenAI`.
+    """InferenceEndpoints LLM implementation running the async API client.
+
+    This LLM will internally use `huggingface_hub.AsyncInferenceClient` or `openai.AsyncOpenAI`
+    depending on the `use_openai_client` attribute.
 
     Attributes:
         model_id: the model ID to use for the LLM as available in the Hugging Face Hub, which
             will be used to resolve the base URL for the serverless Inference Endpoints API requests.
             Defaults to `None`.
         endpoint_name: the name of the Inference Endpoint to use for the LLM. Defaults to `None`.
         endpoint_namespace: the namespace of the Inference Endpoint to use for the LLM. Defaults to `None`.
         base_url: the base URL to use for the Inference Endpoints API requests.
         api_key: the API key to authenticate the requests to the Inference Endpoints API.
         tokenizer_id: the tokenizer ID to use for the LLM as available in the Hugging Face Hub.
             Defaults to `None`, but defining one is recommended to properly format the prompt.
         model_display_name: the model display name to use for the LLM. Defaults to `None`.
         use_openai_client: whether to use the OpenAI client instead of the Hugging Face client.
 
+    Icon:
+        `:hugging:`
+
     Examples:
+
+        Free serverless Inference API:
+
         ```python
         from distilabel.llms.huggingface import InferenceEndpointsLLM
 
-        # Free serverless Inference API
         llm = InferenceEndpointsLLM(
             model_id="mistralai/Mistral-7B-Instruct-v0.2",
         )
 
-        # Dedicated Inference Endpoints
+        llm.load()
+
+        # Synchrounous request
+        output = llm.generate(inputs=[[{"role": "user", "content": "Hello world!"}]])
+
+        # Asynchronous request
+        output = await llm.agenerate(input=[{"role": "user", "content": "Hello world!"}])
+        ```
+
+        Dedicated Inference Endpoints:
+
+        ```python
+        from distilabel.llms.huggingface import InferenceEndpointsLLM
+
         llm = InferenceEndpointsLLM(
             endpoint_name="<ENDPOINT_NAME>",
             api_key="<HF_API_KEY>",
             endpoint_namespace="<USER|ORG>",
         )
 
-        # Dedicated Inference Endpoints or TGI
+        llm.load()
+
+        # Synchrounous request
+        output = llm.generate(inputs=[[{"role": "user", "content": "Hello world!"}]])
+
+        # Asynchronous request
+        output = await llm.agenerate(input=[{"role": "user", "content": "Hello world!"}])
+        ```
+
+        Dedicated Inference Endpoints or TGI:
+
+        ```python
+        from distilabel.llms.huggingface import InferenceEndpointsLLM
+
         llm = InferenceEndpointsLLM(
             api_key="<HF_API_KEY>",
             base_url="<BASE_URL>",
         )
 
         llm.load()
 
@@ -296,14 +329,17 @@
         repetition_penalty: Optional[float] = None,
         temperature: float = 1.0,
         do_sample: bool = False,
         top_k: Optional[int] = None,
         top_p: Optional[float] = None,
         typical_p: Optional[float] = None,
         stop_sequences: Optional[Union[str, List[str]]] = None,
+        return_full_text: bool = False,
+        seed: Optional[int] = None,
+        watermark: bool = False,
     ) -> "GenerateOutput":
         """Generates completions for the given input using the OpenAI async client.
 
         Args:
             input: a single input in chat format to generate responses for.
             max_new_tokens: the maximum number of new tokens that the model will generate.
                 Defaults to `128`.
@@ -319,14 +355,19 @@
             top_k: the top-k value to use for the generation. Defaults to `0.8`, since neither
                 `0.0` nor `1.0` are valid values in TGI.
             top_p: the top-p value to use for the generation. Defaults to `1.0`.
             typical_p: the typical-p value to use for the generation. Defaults to `0.5`.
             stop_sequences: either a single string or a list of strings containing the sequences
                 to stop the generation at. Defaults to `None`, but will be set to the
                 `tokenizer.eos_token` if available.
+            return_full_text: whether to return the full text of the completion or just the
+                generated text. Defaults to `False`, meaning that only the generated text will be
+                returned.
+            seed: the seed to use for the generation. Defaults to `None`.
+            watermark: whether to add the watermark to the generated text. Defaults to `None`.
 
         Returns:
             A list of lists of strings containing the generated responses for each input.
         """
         if stop_sequences is not None:
             if isinstance(stop_sequences, str):
                 stop_sequences = [stop_sequences]
@@ -352,30 +393,33 @@
         if self._tokenizer is not None:
             prompt = self._tokenizer.apply_chat_template(  # type: ignore
                 conversation=input,  # type: ignore
                 tokenize=False,
                 add_generation_prompt=True,
             )
         else:
+            # TODO: should we apply a default chat template here instead? e.g. ChatML
             prompt = "\n".join([message["content"] for message in input])
 
         try:
             completion = await self._aclient.text_generation(  # type: ignore
                 prompt=prompt,  # type: ignore
                 max_new_tokens=max_new_tokens,
                 do_sample=do_sample,
                 typical_p=typical_p,
                 repetition_penalty=repetition_penalty,
                 temperature=temperature,
                 top_p=top_p,
                 top_k=top_k,
+                stop_sequences=stop_sequences,
+                return_full_text=return_full_text,
+                watermark=watermark,
                 # NOTE: here to ensure that the cache is not used and a different response is
                 # generated every time
-                seed=random.randint(0, 2147483647),
-                stop_sequences=stop_sequences,
+                seed=seed or random.randint(0, 2147483647),
             )
             return [completion]
         except Exception as e:
             self._logger.warning(  # type: ignore
                 f"⚠️ Received no response using Inference Client (model: '{self.model_name}')."
                 f" Finish reason was: {e}"
             )
```

### Comparing `distilabel-1.0.3/src/distilabel/llms/huggingface/transformers.py` & `distilabel-1.1.0/src/distilabel/llms/huggingface/transformers.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Union
 
 from pydantic import PrivateAttr, validate_call
 
 from distilabel.llms.base import LLM
 from distilabel.llms.chat_templates import CHATML_TEMPLATE
 from distilabel.llms.mixins import CudaDevicePlacementMixin
 from distilabel.llms.typing import GenerateOutput
@@ -25,14 +25,15 @@
 
 if TYPE_CHECKING:
     from transformers import Pipeline
     from transformers.modeling_utils import PreTrainedModel
     from transformers.tokenization_utils import PreTrainedTokenizer
 
     from distilabel.llms.typing import HiddenState
+    from distilabel.steps.tasks.structured_outputs.outlines import StructuredOutputType
 
 
 class TransformersLLM(LLM, CudaDevicePlacementMixin):
     """Hugging Face `transformers` library LLM implementation using the text generation
     pipeline.
 
     Attributes:
@@ -57,14 +58,17 @@
         device: the name or index of the device where the model will be loaded. Defaults
             to `None`.
         device_map: a dictionary mapping each layer of the model to a device, or a mode
             like `"sequential"` or `"auto"`. Defaults to `None`.
         token: the Hugging Face Hub token that will be used to authenticate to the Hugging
             Face Hub. If not provided, the `HF_TOKEN` environment or `huggingface_hub` package
             local configuration will be used. Defaults to `None`.
+
+    Icon:
+        `:hugging:`
     """
 
     model: str
     revision: str = "main"
     torch_dtype: str = "auto"
     trust_remote_code: bool = False
     model_kwargs: Optional[Dict[str, Any]] = None
@@ -72,20 +76,19 @@
     use_fast: bool = True
     chat_template: Optional[str] = None
     device: Optional[Union[str, int]] = None
     device_map: Optional[Union[str, Dict[str, Any]]] = None
     token: Optional[str] = None
 
     _pipeline: Optional["Pipeline"] = PrivateAttr(...)
+    _prefix_allowed_tokens_fn: Union[Callable, None] = PrivateAttr(default=None)
 
     def load(self) -> None:
         """Loads the model and tokenizer and creates the text generation pipeline. In addition,
         it will configure the tokenizer chat template."""
-        super().load()
-
         if self.device == "cuda":
             CudaDevicePlacementMixin.load(self)
 
         try:
             from transformers import pipeline
         except ImportError as ie:
             raise ImportError(
@@ -111,14 +114,21 @@
             self._pipeline.tokenizer.chat_template = self.chat_template  # type: ignore
         elif (
             self._pipeline.tokenizer.chat_template is None  # type: ignore
             and self._pipeline.tokenizer.default_chat_template is None  # type: ignore
         ):
             self._pipeline.tokenizer.chat_template = CHATML_TEMPLATE  # type: ignore
 
+        if self.structured_output:
+            self._prefix_allowed_tokens_fn = self._prepare_structured_output(
+                self.structured_output
+            )
+
+        super().load()
+
     @property
     def model_name(self) -> str:
         """Returns the model name used for the LLM."""
         return self.model
 
     def prepare_input(self, input: "ChatType") -> str:
         """Prepares the input by applying the chat template to the input, which is formatted
@@ -157,23 +167,26 @@
             top_p: the top-p value to use for the generation. Defaults to `1.0`.
             top_k: the top-k value to use for the generation. Defaults to `0`.
             do_sample: whether to use sampling or not. Defaults to `True`.
 
         Returns:
             A list of lists of strings containing the generated responses for each input.
         """
+        prepared_inputs = [self.prepare_input(input=input) for input in inputs]
+
         outputs: List[List[Dict[str, str]]] = self._pipeline(  # type: ignore
-            [self.prepare_input(input=input) for input in inputs],
+            prepared_inputs,
             max_new_tokens=max_new_tokens,
             temperature=temperature,
             repetition_penalty=repetition_penalty,
             top_p=top_p,
             top_k=top_k,
             do_sample=do_sample,
             num_return_sequences=num_generations,
+            prefix_allowed_tokens_fn=self._prefix_allowed_tokens_fn,
         )
         return [
             [generation["generated_text"] for generation in output]
             for output in outputs
         ]
 
     def get_last_hidden_states(self, inputs: List["ChatType"]) -> List["HiddenState"]:
@@ -203,7 +216,29 @@
         return [
             seq_last_hidden_state[attention_mask.bool(), :].detach().cpu().numpy()
             for seq_last_hidden_state, attention_mask in zip(
                 last_hidden_states,
                 input_ids["attention_mask"],  # type: ignore
             )
         ]
+
+    def _prepare_structured_output(
+        self, structured_output: Optional["StructuredOutputType"] = None
+    ) -> Union[Callable, None]:
+        """Creates the appropriate function to filter tokens to generate structured outputs.
+
+        Args:
+            structured_output: the configuration dict to prepare the structured output.
+
+        Returns:
+            The callable that will be used to guide the generation of the model.
+        """
+        from distilabel.steps.tasks.structured_outputs.outlines import (
+            prepare_guided_output,
+        )
+
+        result = prepare_guided_output(
+            structured_output, "transformers", self._pipeline
+        )
+        if schema := result.get("schema"):
+            self.structured_output["schema"] = schema
+        return result["processor"]
```

### Comparing `distilabel-1.0.3/src/distilabel/mixins/__init__.py` & `distilabel-1.1.0/src/distilabel/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/mixins/runtime_parameters.py` & `distilabel-1.1.0/src/distilabel/mixins/runtime_parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import difflib
 import inspect
 from typing import TYPE_CHECKING, Any, Dict, List, Tuple, TypeVar, Union
 
 from pydantic import BaseModel, Field, PrivateAttr
 from pydantic.types import _SecretField
 from typing_extensions import Annotated, get_args, get_origin
 
@@ -101,16 +102,30 @@
         to be set is a `RuntimeParametersMixin`, it will call `set_runtime_parameters` on
         the attr.
 
         Args:
             runtime_parameters: A dictionary containing the values of the runtime parameters
                 to set.
         """
+        runtime_parameters_names = list(self.runtime_parameters_names.keys())
         for name, value in runtime_parameters.items():
             if name not in self.runtime_parameters_names:
+                # Check done just to ensure the unit tests for the mixin run
+                if getattr(self, "pipeline", None):
+                    closest = difflib.get_close_matches(
+                        name, runtime_parameters_names, cutoff=0.5
+                    )
+                    msg = (
+                        f"⚠️  Runtime parameter '{name}' unknown in step '{self.name}'."
+                    )
+                    if closest:
+                        msg += f" Did you mean any of: {closest}"
+                    else:
+                        msg += f" Available runtime parameters for the step: {runtime_parameters_names}."
+                    self.pipeline._logger.warning(msg)
                 continue
 
             attr = getattr(self, name)
             if isinstance(attr, RuntimeParametersMixin):
                 attr.set_runtime_parameters(value)
                 self._runtime_parameters[name] = value
                 continue
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `distilabel-1.0.3/src/distilabel/pipeline/__init__.py` & `distilabel-1.1.0/src/distilabel/pipeline/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,9 +9,13 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from distilabel.pipeline.local import Pipeline
+from distilabel.pipeline.routing_batch_function import (
+    routing_batch_function,
+    sample_n_steps,
+)
 
-__all__ = ["Pipeline"]
+__all__ = ["Pipeline", "routing_batch_function", "sample_n_steps"]
```

### Comparing `distilabel-1.0.3/src/distilabel/pipeline/base.py` & `distilabel-1.1.0/src/distilabel/pipeline/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,57 +8,74 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import copy
 import hashlib
 import logging
 import os
+from collections import defaultdict
 from dataclasses import asdict, dataclass, field
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     Iterable,
     List,
     Optional,
     Set,
+    Tuple,
     TypedDict,
     Union,
 )
 
 import pyarrow as pa
 import pyarrow.parquet as pq
 from typing_extensions import Self
 
 from distilabel import __version__
 from distilabel.pipeline._dag import DAG
+from distilabel.pipeline.constants import (
+    RECEIVES_ROUTED_BATCHES_ATTR_NAME,
+    ROUTING_BATCH_FUNCTION_ATTR_NAME,
+    STEP_ATTR_NAME,
+)
 from distilabel.utils.files import list_files_in_dir
 from distilabel.utils.serialization import TYPE_INFO_KEY, _Serializable
 
 if TYPE_CHECKING:
     from os import PathLike
 
     from distilabel.distiset import Distiset
+    from distilabel.pipeline.routing_batch_function import RoutingBatchFunction
     from distilabel.steps.base import _Step
     from distilabel.utils.serialization import SaveFormats, StrOrPath
 
 
 BASE_CACHE_DIR = Path.home() / ".cache" / "distilabel" / "pipelines"
 
 
-class CacheLocation(TypedDict):
-    """Dictionary to store the filenames and directories of a cached pipeline."""
+class _CacheLocation(TypedDict):
+    """Dictionary to store the filenames and directories of a cached pipeline.
+
+    Attributes:
+        pipeline: The filename where the pipeline content will be serialized.
+        batch_manager: The filename where the batch manager content will be serialized.
+        data: The directory where the output data of each leaf step will be stored.
+        log_file: The filename where the logs will be stored.
+    """
 
     pipeline: Path
     batch_manager: Path
     data: Path
+    log_file: Path
 
 
 class _GlobalPipelineManager:
     """Class to manage the global pipeline instance that will be used by the steps when
     created within a pipeline context.
 
     Attributes:
@@ -100,37 +117,44 @@
     """
 
     def __init__(
         self,
         name: str,
         description: Optional[str] = None,
         cache_dir: Optional["PathLike"] = None,
+        enable_metadata: bool = False,
     ) -> None:
         """Initialize the `BasePipeline` instance.
 
         Args:
             name: The name of the pipeline.
             description: A description of the pipeline. Defaults to `None`.
             cache_dir: A directory where the pipeline will be cached. Defaults to `None`.
+            enable_metadata: Whether to include the distilabel metadata column for the pipeline
+                in the final `Distiset`. It contains metadata used by distilabel, for example
+                the raw outputs of the `LLM` without processing would be here, inside `raw_output_...`
+                field. Defaults to `False`.
         """
         self.name = name
         self.description = description
+        self._enable_metadata = enable_metadata
         self.dag = DAG()
 
         if cache_dir:
             self._cache_dir = Path(cache_dir)
         elif env_cache_dir := os.getenv("DISTILABEL_CACHE_DIR"):
             self._cache_dir = Path(env_cache_dir)
         else:
             self._cache_dir = BASE_CACHE_DIR
 
         self._logger = logging.getLogger("distilabel.pipeline")
 
         # It's set to None here, will be created in the call to run
         self._batch_manager: Optional["_BatchManager"] = None
+        self._dry_run: bool = False
 
     def __enter__(self) -> Self:
         """Set the global pipeline instance when entering a pipeline context."""
         _GlobalPipelineManager.set_pipeline(self)
         return self
 
     def __exit__(self, exc_type, exc_value, traceback) -> None:
@@ -145,23 +169,19 @@
         Returns:
             int: Signature of the pipeline.
         """
         hasher = hashlib.sha1()
 
         steps_info = []
         pipeline_dump = self.dump()["pipeline"]
+
         for step in pipeline_dump["steps"]:
             step_info = step["name"]
-            for argument, value in sorted(step["step"].items()):
-                if (
-                    (argument == TYPE_INFO_KEY)
-                    or (argument == "llm")
-                    or (value is None)
-                ):
-                    # NOTE: Should we include the LLM info at this stage??
+            for argument, value in sorted(step[STEP_ATTR_NAME].items()):
+                if (argument == TYPE_INFO_KEY) or (value is None):
                     continue
 
                 if isinstance(value, dict):
                     # input_mappings/output_mappings
                     step_info += "-".join(
                         [f"{str(k)}-{str(v)}" for k, v in value.items()]
                     )
@@ -177,15 +197,29 @@
                     )
 
             steps_info.append(step_info)
 
         connections_info = [
             f"{c['from']}-{'-'.join(c['to'])}" for c in pipeline_dump["connections"]
         ]
-        hasher.update(",".join(steps_info + connections_info).encode())
+
+        routing_batch_functions_info = []
+        for function in pipeline_dump["routing_batch_functions"]:
+            step = function["step"]
+            routing_batch_function: "RoutingBatchFunction" = self.dag.get_step(step)[
+                ROUTING_BATCH_FUNCTION_ATTR_NAME
+            ]
+            if type_info := routing_batch_function._get_type_info():
+                step += f"-{type_info}"
+
+        hasher.update(
+            ",".join(
+                steps_info + connections_info + routing_batch_functions_info
+            ).encode()
+        )
 
         return hasher.hexdigest()
 
     def run(
         self,
         parameters: Optional[Dict[str, Dict[str, Any]]] = None,
         use_cache: bool = True,
@@ -206,24 +240,59 @@
             The `Distiset` created by the pipeline.
         """
         if use_cache:
             self._load_from_cache()
         self._set_runtime_parameters(parameters or {})
         self.dag.validate()
 
+    def dry_run(
+        self,
+        parameters: Optional[Dict[str, Dict[str, Any]]] = None,
+        batch_size: int = 1,
+    ) -> "Distiset":
+        """Do a dry run to test the pipeline runs as expected.
+
+        Running a `Pipeline` in dry run mode will set all the `batch_size` of generator steps
+        to the specified batch_size, and run just with a single batch, effectively
+        running the whole pipeline with a single example. The cache will be set to False.
+
+        Args:
+            parameters: The same parameters variable from `BasePipeline.run`. Defaults to None.
+                Will be passed to the parent method, but with the batch_size of the generator steps
+                fixed to 1.
+            batch_size: The batch size to test the pipeline. Defaults to 1.
+
+        Returns:
+            Will return the `Distiset` as the main run method would do.
+        """
+        self._dry_run = True
+
+        for step_name in self.dag:
+            step = self.dag.get_step(step_name)[STEP_ATTR_NAME]
+            if step.is_generator:
+                if parameters.get(step_name) and parameters[step_name].get(
+                    "batch_size"
+                ):
+                    parameters[step_name]["batch_size"] = batch_size
+
+        distiset = self.run(parameters, use_cache=False)
+
+        self._dry_run = False
+        return distiset
+
     def get_runtime_parameters_info(self) -> Dict[str, List[Dict[str, Any]]]:
         """Get the runtime parameters for the steps in the pipeline.
 
         Returns:
             A dictionary with the step name as the key and a list of dictionaries with
             the parameter name and the parameter info as the value.
         """
         runtime_parameters = {}
         for step_name in self.dag:
-            step: "_Step" = self.dag.get_step(step_name)["step"]
+            step: "_Step" = self.dag.get_step(step_name)[STEP_ATTR_NAME]
             runtime_parameters[step_name] = step.get_runtime_parameters_info()
         return runtime_parameters
 
     def _add_step(self, step: "_Step") -> None:
         """Add a step to the pipeline.
 
         Args:
@@ -236,24 +305,56 @@
 
         Args:
             from_step: The name of the step that will generate the input for `to_step`.
             to_step: The name of the step that will receive the input from `from_step`.
         """
         self.dag.add_edge(from_step, to_step)
 
+        # Check if `from_step` has a `routing_batch_function`. If it does, then mark
+        # `to_step` as a step that will receive a routed batch.
+        node = self.dag.get_step(from_step)  # type: ignore
+        routing_batch_function = node.get(ROUTING_BATCH_FUNCTION_ATTR_NAME, None)
+        self.dag.set_step_attr(
+            name=to_step,
+            attr=RECEIVES_ROUTED_BATCHES_ATTR_NAME,
+            value=routing_batch_function is not None,
+        )
+
+    def _add_routing_batch_function(
+        self, step_name: str, routing_batch_function: "RoutingBatchFunction"
+    ) -> None:
+        """Add a routing batch function to a step.
+
+        Args:
+            step_name: The name of the step that will receive the routed batch.
+            routing_batch_function: The function that will route the batch to the step.
+        """
+        self.dag.set_step_attr(
+            name=step_name,
+            attr=ROUTING_BATCH_FUNCTION_ATTR_NAME,
+            value=routing_batch_function,
+        )
+
     def _set_runtime_parameters(self, parameters: Dict[str, Dict[str, Any]]) -> None:
         """Set the runtime parameters for the steps in the pipeline.
 
         Args:
             parameters: A dictionary with the step name as the key and a dictionary with
             the parameter name as the key and the parameter value as the value.
         """
+        step_names = set(self.dag.G)
         for step_name, step_parameters in parameters.items():
-            step: "_Step" = self.dag.get_step(step_name)["step"]
-            step.set_runtime_parameters(step_parameters)
+            if step_name not in step_names:
+                self._logger.warning(
+                    f"❓ Step '{step_name}' provided in `Pipeline.run(parameters={{...}})` not found in the pipeline."
+                    f" Available steps are: {step_names}."
+                )
+            else:
+                step: "_Step" = self.dag.get_step(step_name)[STEP_ATTR_NAME]
+                step.set_runtime_parameters(step_parameters)
 
     def _model_dump(self, obj: Any, **kwargs: Any) -> Dict[str, Any]:
         """Dumps the DAG content to a dict.
 
         Args:
             obj (Any): Unused, just kept to match the signature of the parent method.
             kwargs (Any): Unused, just kept to match the signature of the parent method.
@@ -289,53 +390,48 @@
         name = data["pipeline"]["name"]
         description = data["pipeline"].get("description")
         with cls(name=name, description=description) as pipe:
             pipe.dag = DAG.from_dict(data["pipeline"])
         return pipe
 
     @property
-    def _cache_location(self) -> CacheLocation:
+    def _cache_location(self) -> _CacheLocation:
         """Dictionary containing the the object that will stored and the location,
         whether it is a filename or a folder.
 
         Returns:
             Path: Filenames where the pipeline content will be serialized.
         """
-        folder = self._cache_dir / self._create_signature()
+        folder = self._cache_dir / self.name / self._create_signature()
         return {
             "pipeline": folder / "pipeline.yaml",
             "batch_manager": folder / "batch_manager.json",
             "data": folder / "data",
+            "log_file": folder / "pipeline.log",
         }
 
     def _cache(self) -> None:
         """Saves the `BasePipeline` using the `_cache_filename`."""
         self.save(
             path=self._cache_location["pipeline"],
-            format=self._cache_location["pipeline"].suffix.replace(".", ""),
+            format=self._cache_location["pipeline"].suffix.replace(".", ""),  # type: ignore
         )
         if self._batch_manager is not None:
             self._batch_manager.save(
                 self._cache_location["batch_manager"],
-                format=self._cache_location["batch_manager"].suffix.replace(".", ""),
+                format=self._cache_location["batch_manager"].suffix.replace(".", ""),  # type: ignore
             )
         self._logger.debug("Pipeline and batch manager saved to cache.")
 
     def _load_from_cache(self) -> None:
         """Will try to load the `BasePipeline` from the cache dir if found, updating
         the internal `DAG` and `_BatchManager`.
         """
         cache_loc = self._cache_location
         if cache_loc["pipeline"].exists():
-            # Refresh the DAG to avoid errors when it's created within a context manager
-            # (it will check the steps aren't already defined for the DAG).
-            self.dag = DAG()
-            new_class = self.from_yaml(cache_loc["pipeline"])
-            # Update the internal dag and batch_manager
-            self.dag.G = new_class.dag.G
             if cache_loc["batch_manager"].exists():
                 self._batch_manager = _BatchManager.from_json(
                     cache_loc["batch_manager"]
                 )
             self._logger.info("💾 Load pipeline from cache")
 
 
@@ -345,63 +441,49 @@
 
     Attributes:
         seq_no: The sequence number of the batch.
         step_name: The name of the step that will process the batch.
         last_batch: A flag to indicate if the batch is the last one.
         data: The data to be processed.
         accumulated: A flag to indicate if the batch is accumulated.
+        created_from: A dictionary containing the `seq_no` of the batches of the steps that
+            were used to create this batch.
+        size: The size of the batch.
     """
 
     seq_no: int
     step_name: str
     last_batch: bool
     data: List[List[Dict[str, Any]]] = field(default_factory=list, repr=False)
     accumulated: bool = False
+    created_from: Dict[str, List[Tuple[int, int]]] = field(default_factory=dict)
+    batch_routed_to: List[str] = field(default_factory=list)
+    size: int = 0
 
     def next_batch(self) -> "_Batch":
         """Create a new `_Batch` instance with the next batch of data.
+
         Args:
             data: The data to be processed.
+
         Returns:
             A `_Batch` instance.
         """
         return _Batch(
             seq_no=self.seq_no + 1, step_name=self.step_name, last_batch=self.last_batch
         )
 
-    @property
-    def empty(self) -> bool:
-        """Checks if the batch is empty.
-
-        Returns:
-            `True` if the batch is empty. Otherwise, `False`.
-        """
-        return all(len(rows) == 0 for rows in self.data)
-
-    @classmethod
-    def from_batches(cls, step_name: str, batches: List["_Batch"]) -> "_Batch":
-        """Create a `_Batch` instance with the outputs from the list of batches that
-        were received from another steps. All the batches must have the same sequence
-        number.
+    def set_data(self, data: List[List[Dict[str, Any]]]) -> None:
+        """Sets the data of the batch and updates the size of the batch.
 
         Args:
-            step_name: The name of the step that will process the batch.
-            batches: A list of `_Batch` instances.
-
-        Returns:
-            A `_Batch` instance.
+            data: The data of the batch.
         """
-
-        seq_no = batches[0].seq_no
-        if not all(batch.seq_no == seq_no for batch in batches):
-            raise ValueError("All batches must have the same sequence number")
-
-        data = [batch.data[0] for batch in batches]
-        last_batch = batches[-1].last_batch
-        return cls(seq_no, step_name, last_batch, data)
+        self.data = data
+        self.size = len(data[0])
 
     @classmethod
     def accumulate(cls, step_name: str, batches: List[List["_Batch"]]) -> "_Batch":
         """Creates a `_Batch` instance using the data from the list of batches that
         were received from another steps. The batches will be accumulated in a single
         list of data.
 
@@ -421,22 +503,30 @@
             seq_no=0, step_name=step_name, last_batch=True, data=data, accumulated=True
         )
 
     def _model_dump(self, obj: Any, **kwargs: Any) -> Dict[str, Any]:
         """Dumps the content of the `_Batch` to a dictionary, using the `dataclass` helper function.
 
         Args:
-            obj (Any): Unused, just kept to match the signature of the parent method.
-            kwargs (Any): Additional arguments that are kept to match the signature of the parent method.
+            obj: Unused, just kept to match the signature of the parent method.
+            kwargs: Additional arguments that are kept to match the signature of the parent method.
 
         Returns:
-            Dict[str, Any]: Internal representation of the `_Batch`.
+            A `dict` containing the internal representation of the `_Batch`.
         """
         return asdict(self)
 
+    def copy(self) -> "_Batch":
+        """Creates a copy of the `_Batch` instance.
+
+        Returns:
+            A copy of the `_Batch` instance.
+        """
+        return copy.deepcopy(self)
+
 
 @dataclass
 class _BatchManagerStep(_Serializable):
     """A class that will accumulate data for a step from the predecessors and create
     batches for the step to process when there is enough data.
 
     Attributes:
@@ -448,57 +538,85 @@
             If `None`, then `accumulate` must be `True`. Defaults to `None`.
         data: A dictionary with the predecessor step name as the key and a list of
             dictionaries (rows) as the value.
         seq_no: The sequence number of the next batch to be created. It will be
             incremented for each batch created.
         last_batch_received: A list with the names of the steps that sent the last
             batch of data.
+        convergence_step: A flag to indicate if the step is a convergence step. An
+            `Step` is a convergence step if all its predecessors are receiving routed
+            batches. Defaults to `False`.
+        convergence_step_batches_consumed: A dictionary in which the key is the `seq_no`
+            of the batch created by step A, that was used by step B and C and obtained from
+            the `created_from` of the batches created by them. It's used to know if all
+            the batches from B and C steps created from batches of A have been consumed
+            by D, in order to not mess up the order of the batches. Only used if `convergence_step=True`.
+            Defaults to an empty dictionary.
+        next_expected_created_from_batch_seq_no: The next expected sequence number of the
+            batch from step A used by steps B and C and obtained from the `created_from`
+            of the batches created by them. It's used to avoid messing up the order of the
+            batches. Only used if `convergence_step=True`. Defaults to `0`.
     """
 
     step_name: str
     accumulate: bool
     input_batch_size: Union[int, None] = None
-    data: Dict[str, List[Dict[str, Any]]] = field(default_factory=dict)
+    data: Dict[str, List[_Batch]] = field(default_factory=dict)
     seq_no: int = 0
     last_batch_received: List[str] = field(default_factory=list)
+    convergence_step: bool = False
+    convergence_step_batches_consumed: Dict[int, Dict[str, int]] = field(
+        default_factory=dict
+    )
+    next_expected_created_from_batch_seq_no: int = 0
 
     def add_batch(self, batch: _Batch, prepend: bool = False) -> None:
         """Add a batch of data from `batch.step_name` to the step. It will accumulate the
         data and keep track of the last batch received from the predecessors.
 
         Args:
             batch: The output batch of an step to be processed by the step.
             prepend: If `True`, the content of the batch will be added at the start of
                 the buffer.
         """
         from_step = batch.step_name
+
         if prepend:
-            self.data[from_step] = batch.data[0] + self.data[from_step]
+            self.data[from_step].insert(0, batch)
         else:
-            self.data[from_step].extend(batch.data[0])
+            self.data[from_step].append(batch)
+
         if batch.last_batch:
             self.last_batch_received.append(from_step)
 
     def get_batch(self) -> Union[_Batch, None]:
         """Create a new batch of data for the step to process. It will return `None` if
         there is not enough data to create a batch.
 
         Returns:
             A `_Batch` instance if there is enough data to create a batch. Otherwise,
             `None`.
         """
         if not self._ready_to_create_batch():
             return None
 
+        # `_last_batch` must be called before `_get_data`, as `_get_data` will update the
+        # list of data which is used to determine if the batch to be created is the last one.
+        # TODO: remove `_last_batch` method and integrate logic in `_get_data`
+        last_batch = self._last_batch()
+        data, created_from, batch_routed_to = self._get_data()
+
         return _Batch(
             seq_no=self._get_seq_no(),
             step_name=self.step_name,
-            last_batch=self._last_batch(),
-            data=self._get_data(),
+            last_batch=last_batch,
+            data=data,
             accumulated=self.accumulate,
+            created_from=created_from,
+            batch_routed_to=batch_routed_to,
         )
 
     def empty_buffers(self) -> List[str]:
         """Checks if the input buffer for the step is empty.
 
         Returns:
             The name of the previous steps for which the input buffer for this step is
@@ -509,140 +627,428 @@
                 previous_step
                 for previous_step in self.data.keys()
                 if previous_step not in self.last_batch_received
             ]
 
         return [
             previous_step
-            for previous_step, buffer in self.data.items()
+            for previous_step, batches in self.data.items()
             if previous_step not in self.last_batch_received
-            and len(buffer) < self.input_batch_size
+            and sum(len(batch.data[0]) for batch in batches) < self.input_batch_size  # type: ignore
         ]
 
     @classmethod
     def from_step(
-        cls, step: "_Step", predecessors: Iterable[str]
+        cls, step: "_Step", predecessors: Iterable[str], convergence_step: bool = False
     ) -> "_BatchManagerStep":
         """Creates a `_BatchManagerStep` instance from a `_Step` instance and its
         predecessors.
 
+        Args:
+            step: The `_Step` instance.
+            predecessors: The names of the predecessors of the step.
+            convergence_step: A flag to indicate if the step is a convergence step. An
+                `Step` is a convergence step if all its predecessors are receiving routed
+                batches. Defaults to `False`.
+
         Returns:
             A `_BatchManagerStep` instance.
         """
         return cls(
-            step_name=step.name,
+            step_name=step.name,  # type: ignore
             accumulate=step.is_global,
             input_batch_size=getattr(step, "input_batch_size", None),
             data={predecessor: [] for predecessor in predecessors},
+            convergence_step=convergence_step,
         )
 
     def _get_seq_no(self) -> int:
         """Gets the sequence number for the next batch to be created and increments it.
 
         Returns:
             The sequence number for the next batch to be created.
         """
         seq_no = self.seq_no
         self.seq_no += 1
         return seq_no
 
-    def _get_data(self) -> List[List[Dict[str, Any]]]:
+    def _get_data(
+        self,
+    ) -> Tuple[List[List[Dict[str, Any]]], Dict[str, List[Tuple[int, int]]], List[str]]:
         """Gets the data needed to create a batch for the step to process. If the step is
         accumulating data, then it will return a list with all the data received from the
         predecessors. Otherwise, it will return a list of data with the `input_batch_size`
         for each predecessor. In addition, it will remove the data used to create the
         batch from the step's data.
 
         Returns:
-            The list of data needed to create a batch for the step to process.
+            A tuple containing the list of data needed to create a batch for the step to
+            process, a dictionary with the sequence numbers of the batches that were used
+            to create the batch and the list of steps to which the batch was routed to if
+            the step is a normal step.
         """
         if self.accumulate:
-            data = list(self.data.values())
-            self.data = {step_name: [] for step_name in self.data}
-            return data
+            # Steps accumulating cannot receive routed batches
+            return self._get_data_for_accumulate() + ([],)
+
+        if self.convergence_step:
+            # Convergence steps will receive routed batches, but we need to clean the
+            # `batch_routed_to` list
+            return self._get_data_for_convergence_step() + ([],)
+
+        return self._get_data_normal()
+
+    def _get_data_for_accumulate(
+        self,
+    ) -> Tuple[List[List[Dict[str, Any]]], Dict[str, List[Tuple[int, int]]]]:
+        """Gets the data needed to create a batch for the step to process when the step
+        is accumulating data. It will return a list with all the data received from the
+        predecessors. In addition, it will remove the data used to create the batch from
+        the step's data.
 
+        Returns:
+            A tuple containing the list of data needed to create a batch for the step to
+            process and a dictionary with the sequence numbers of the batches that were
+            used to create the batch.
+        """
         data = []
-        for step_name in self.data:
-            step_data = self.data[step_name]
-            data_for_batch, self.data[step_name] = (
-                step_data[: self.input_batch_size],
-                step_data[self.input_batch_size :],
+        batches_used = {}
+        for step_name, batches in self.data.items():
+            batches_used[step_name] = []
+            for batch in batches:
+                batches_used[step_name].append((batch.seq_no, batch.size))
+            data.append([row for batch in batches for row in batch.data[0]])
+        # Reset the data buffer
+        self.data = {step_name: [] for step_name in self.data}
+        return data, batches_used
+
+    def _get_data_for_convergence_step(
+        self,
+    ) -> Tuple[List[List[Dict[str, Any]]], Dict[str, List[Tuple[int, int]]]]:
+        """Gets the data needed to create a batch for the step to process when the step is
+        a convergence step.
+
+        Returns:
+            A tuple containing the list of data needed to create a batch for the step to
+            process and a dictionary with the sequence numbers of the batches that were
+            used to create the batch.
+        """
+        grouped_batches = self._group_batches_by_created_from()
+        seq_no, batches = grouped_batches[0]
+
+        remaining_rows_per_step = {
+            step_name: self.input_batch_size for step_name in self.data
+        }
+        batches_used = defaultdict(list)
+        data = defaultdict(list)
+        for batch, batch_size in batches:
+            batch_data = batch.data[0]
+            remaining_rows = remaining_rows_per_step[batch.step_name]
+            selected_data = batch_data[:remaining_rows]
+            data[batch.step_name].extend(selected_data)
+
+            # If A -> [B, C] -> D, then in D (this step) we keep track of the remaining
+            # rows from the batches of A that B and C used to create the `batches`.
+            batch_size = self.convergence_step_batches_consumed.setdefault(
+                seq_no, {}
+            ).get(batch.step_name, batch_size)
+            remaining_rows_in_batch = batch_size - len(selected_data)
+            self.convergence_step_batches_consumed[seq_no].update(
+                {batch.step_name: remaining_rows_in_batch}
             )
-            data.append(data_for_batch)
-        return data
+
+            # Update the remaining rows
+            num_rows = len(selected_data)
+            remaining_rows_per_step[batch.step_name] -= num_rows  # type: ignore
+
+            # Keep track of the batches used to create the batch
+            batches_used[batch.step_name].append((batch.seq_no, batch.size))
+
+            # If the batch was entirely consumed, then remove it from the buffer
+            if num_rows >= len(batch_data):
+                self.data[batch.step_name].remove(batch)
+                continue
+
+            # The batch was not entirely consumed. so we need to update the batch
+            # with the remaining data
+            batch_idx = self.data[batch.step_name].index(batch)
+            batch_ref = self.data[batch.step_name][batch_idx]
+            batch_ref.data[0] = batch_data[len(selected_data) :]
+
+        # If all the batches grouped by the `seq_no` in `created_from` were consumed, then
+        # we can update the `next_expected_created_from_batch_seq_no` to the next one
+        # to avoid skipping batches.
+        no_remaining_rows = all(
+            count == 0
+            for count in self.convergence_step_batches_consumed[seq_no].values()
+        )
+        if no_remaining_rows:
+            self.next_expected_created_from_batch_seq_no += 1
+
+        return list(data.values()), dict(batches_used)
+
+    def _get_data_normal(
+        self,
+    ) -> Tuple[List[List[Dict[str, Any]]], Dict[str, List[Tuple[int, int]]], List[str]]:
+        """Gets the data needed to create a batch for the step to process when the step is
+        not accumulating data. It will return a list of data with the `input_batch_size`
+        for each predecessor. In addition, it will remove the data used to create the batch
+        from the step's data.
+
+        Returns:
+            A tuple containing the list of data needed to create a batch for the step to
+            process, a dictionary with the sequence numbers of the batches that were used
+            to create the batch and the list of steps to which the batch was routed to if
+            the step is a convergence step.
+        """
+        data = []
+        batches_used = defaultdict(list)
+        batch_routed_to = []
+        for step_name in self.data:
+            # For each step batches buffer, we will create a batch with the `input_batch_size`
+            # using the data from the buffer. We will remove the consumed batches (no data
+            # left) and update the batch data with the remaining data.
+            step_data = []
+            idx_drop_batches = []
+            remaining_rows: int = self.input_batch_size  # type: ignore
+            for idx, batch in enumerate(self.data[step_name]):
+                if remaining_rows == 0:
+                    break
+
+                # Get `remaining_rows` or the remaining rows in the batch and add it to
+                # the step data that will be used to create the batch
+                batch_data = batch.data[0]
+                selected_data = batch_data[:remaining_rows]
+                step_data.extend(selected_data)
+                batch_routed_to = batch.batch_routed_to
+
+                # Update the remaining rows
+                num_rows = len(selected_data)
+                remaining_rows -= num_rows
+
+                # Keep track of the batches used to create the batch
+                batches_used[step_name].append((batch.seq_no, batch.size))
+
+                # If the batch was entirely consumed, then remove it from the buffer
+                if num_rows >= len(batch_data):
+                    idx_drop_batches.append(idx)
+                    continue
+
+                # The batch was not entirely consumed. so we need to update the batch
+                # with the remaining data
+                batch.data[0] = batch_data[len(selected_data) :]
+
+            # Remove the batches that were entirely consumed
+            idx_drop_batches.reverse()
+            for idx in idx_drop_batches:
+                self.data[step_name].pop(idx)
+
+            data.append(step_data)
+
+        return data, dict(batches_used), batch_routed_to
 
     def _ready_to_create_batch(self) -> bool:
-        """Checks if there is enough data to create a batch for the step. If the step is
-        accumulating data, then it will return `True` if the last batch was received from
-        all the predecessors. Otherwise, it will return `True` if there is enough data to
-        create a batch for the step based on the `input_batch_size`.
+        """Checks if there is enough data to create a batch for the step.
 
         Returns:
             `True` if there is enough data to create a batch for the step. Otherwise,
             `False`.
         """
         if self.accumulate:
-            return all(
-                step in self.last_batch_received and len(rows) >= 0
-                for step, rows in self.data.items()
-            )
+            return self._ready_to_create_batch_accumulate()
+
+        if self.convergence_step:
+            return self._ready_to_create_batch_convergence_step()
+
+        return self._ready_to_create_batch_normal()
+
+    def _ready_to_create_batch_accumulate(self) -> bool:
+        """Checks if there is enough data for an step accumulating data. It will return
+        `True` if the last batch was received from all the predecessors.
+
+        Returns:
+            `True` if ready to create a batch, `False` otherwise.
+        """
+        return all(
+            step in self.last_batch_received
+            and sum(len(batch.data[0]) for batch in batches) >= 0
+            for step, batches in self.data.items()
+        )
+
+    def _ready_to_create_batch_convergence_step(self) -> bool:
+        """Checks if there is enough data for creating a batch for an step in which output
+        batches that were generated by steps that received routed batches are received.
+        It will return `True`, if all the output batches that were generated from a routed
+        batch have been received.
+
+        Returns:
+            `True` if ready to create a batch, `False` otherwise.
+        """
+        grouped_batches = self._group_batches_by_created_from()
+        if not grouped_batches:
+            return False
+        seq_no, batches = grouped_batches[0]
+
+        # If the `seq_no` from the `created_from` field is not the expected one, then
+        # we cannot create a batch yet or the order will be messed up
+        if seq_no != self.next_expected_created_from_batch_seq_no:
+            return False
+
+        # Not all output batches to which the input batch was routed to haven't been
+        # received
+        batch_routed_to = batches[0][0].batch_routed_to
+        batches_received_from = {batch.step_name for batch, _ in batches}
+        if any(step_name not in batches_received_from for step_name in batch_routed_to):
+            return False
+
+        # There are output batches to which the input batch was routed to from all
+        # the steps. Check if there is enough data for creating a batch with `input_batch_size`
+        rows_per_step = defaultdict(lambda: 0)
+        for batch, _ in batches:
+            num_rows = len(batch.data[0])
+            rows_per_step[batch.step_name] += num_rows
+
+        # If there aren't at least `input_batch_size` rows from each step, then there
+        # isn't enough data to create a batch
+        if not all(
+            num_rows >= self.input_batch_size or step_name in self.last_batch_received  # type: ignore
+            for step_name, num_rows in rows_per_step.items()
+        ):
+            return False
+
+        return True
+
+    def _ready_to_create_batch_normal(self) -> bool:
+        """Checks if there is enough data for creating a batch for a normal step. It will
+        be `True` it there are at least `input_batch_size` rows from each predecessor step.
+
+        Returns:
+            `True` if ready to create a batch, `False` otherwise.
+        """
+        for step_name, batches in self.data.items():
+            num_rows = sum(len(batch.data[0]) for batch in batches)
 
-        for step_name, rows in self.data.items():
             # If there are now rows but the last batch was already received, then there
             # are no more batch to be created
-            if len(rows) == 0 and step_name in self.last_batch_received:
+            if num_rows == 0 and step_name in self.last_batch_received:
                 return False
 
             # If there are not enough rows and the last batch was not received yet, then
             # there is not enough data yet to creata a batch
             if (
                 self.input_batch_size
-                and len(rows) < self.input_batch_size
+                and num_rows < self.input_batch_size
                 and step_name not in self.last_batch_received
             ):
                 return False
 
         return True
 
     def _last_batch(self) -> bool:
         """Checks if the batch to be created is the last one i.e. if the last batch was
         received from all the predecessors.
 
         Returns:
             `True` if the batch to be created is the last one. Otherwise, `False`.
         """
         if self.accumulate:
-            return all(step in self.last_batch_received for step in self.data.keys())
+            return self._last_batch_accumulate()
+
+        if self.convergence_step:
+            return self._last_batch_convergence_step()
 
-        for step_name, rows in self.data.items():
+        return self._last_batch_normal()
+
+    def _last_batch_accumulate(self) -> bool:
+        """Checks if the batch to be created is the last one for an step accumulating data.
+        `True` if the last batch was received from all the predecessors.
+
+        Returns:
+            `True` if the batch to be created is the last one. Otherwise, `False`.
+        """
+        return all(step in self.last_batch_received for step in self.data.keys())
+
+    def _last_batch_convergence_step(self) -> bool:
+        """Checks if the batch to be created is the last one for a convergence step. `True`
+        if the last batch of all the steps (`batch_routed_to`) in the last routed batch
+        have been received.
+
+        Returns:
+            `True` if the batch to be created is the last one. Otherwise, `False`.
+        """
+        grouped_batches = self._group_batches_by_created_from()
+        if not grouped_batches:
+            return False
+        _, batches = grouped_batches[0]
+
+        for batch, _ in batches:
+            if not batch.last_batch:
+                return False
+
+            if len(batch.data[0]) > self.input_batch_size:  # type: ignore
+                return False
+
+        return True
+
+    def _last_batch_normal(self) -> bool:
+        """Checks if the batch to be created is the last one for a normal step. `True` if
+        there is no more data to be received from the predecessors.
+
+        Returns:
+            `True` if the batch to be created is the last one. Otherwise, `False`.
+        """
+        for step_name, batches in self.data.items():
             if step_name not in self.last_batch_received:
                 return False
 
+            num_rows = sum(len(batch.data[0]) for batch in batches)
+
             if (
                 self.input_batch_size
-                and len(rows) > self.input_batch_size
+                and num_rows > self.input_batch_size
                 and step_name in self.last_batch_received
             ):
                 return False
 
         return True
 
+    def _group_batches_by_created_from(
+        self,
+    ) -> List[Tuple[int, List[Tuple["_Batch", int]]]]:
+        """Group the batches by the first key of `created_from` field. This method is
+        meant to be used only with a `convergence_step`.
+
+        Returns:
+            A list of the batches grouped by the `seq_no` of the first step name in `created_from`.
+            The list is sorted by the `seq_no`.
+        """
+        grouped_batches: Dict[int, List[Tuple["_Batch", int]]] = defaultdict(list)
+        for batches in self.data.values():
+            for batch in batches:
+                first_key = next(iter(batch.created_from))
+                batch_seq_no, batch_size = batch.created_from[first_key][0]
+                grouped_batches[batch_seq_no].append((batch, batch_size))
+        return sorted((seq_no, batches) for seq_no, batches in grouped_batches.items())
+
     def _model_dump(self, obj: Any, **kwargs: Any) -> Dict[str, Any]:
         """Dumps the content of the `_BatchManagerStep` to a dictionary, using the `dataclass` helper function.
 
         Args:
-            obj (Any): Unused, just kept to match the signature of the parent method.
-            kwargs (Any): Additional arguments that are kept to match the signature of the parent method.
+            obj: Unused, just kept to match the signature of the parent method.
+            kwargs: Additional arguments that are kept to match the signature of the parent method.
 
         Returns:
-            Dict[str, Any]: Internal representation of the `_BatchManagerStep`.
+            Internal representation of the `_BatchManagerStep`.
         """
         return asdict(self)
 
 
+LAST_BATCH_SENT_FLAG = "last_batch_sent"
+
+
 class _BatchManager(_Serializable):
     """Class to manage the batches received from the steps. It keeps track of the
     received batches and returns new batches for the steps to process based on their
     input batch size and the batches received from the predecessors.
 
     Attributes:
         steps: A dictionary with the step name as the key and a `_BatchManagerStep`
@@ -651,63 +1057,74 @@
             indicate whether we received the last batch from the step.
     """
 
     def __init__(
         self,
         steps: Dict[str, _BatchManagerStep],
         last_batch_received: Dict[str, Union[_Batch, None]],
+        last_batch_sent: Dict[str, Union[_Batch, None]],
+        last_batch_flag_sent_to: List[str],
     ) -> None:
         """Initialize the `_BatchManager` instance.
 
         Args:
             steps: A dictionary with the step name as the key and a dictionary with the
                 predecessor step name as the key and a list of batches as the value.
             last_batch_received: A dictionary with the step name as the key and a the last
                 `_Batch` received from the step.
+            last_batch_sent: A dictionary with the step name as the key and a the last
+                `_Batch` sent to the step.
+            last_batch_flag_sent_to: A list with the names of the steps to which `LAST_BATCH_SENT_FLAG`
+                was sent.
         """
+
         self._steps = steps
         self._last_batch_received = last_batch_received
+        self._last_batch_sent = last_batch_sent
+        self._last_batch_flag_sent_to = last_batch_flag_sent_to
 
     def can_generate(self) -> bool:
         """Checks if there are still batches to be processed by the steps.
 
         Returns:
             `True` if there are still batches to be processed by the steps. Otherwise,
             `False`.
         """
 
-        # Check if any step that hasn't finished producing data (we haven't received its
-        # last batch) still needs data from its predecessors, and those predecessors have
-        # already sent their last batch and it's empty. In this case, we cannot continue
-        # the pipeline.
-        for batch_manager_step in self._steps.values():
-            for predecessor in batch_manager_step.data.keys():
-                batch = self._last_batch_received.get(predecessor)
-                if (
-                    batch
-                    and batch.last_batch
-                    and batch.empty
-                    and batch_manager_step.data[predecessor] == []
-                ):
-                    return False
+        for step_name, batch in self._last_batch_received.items():
+            if step_name not in self._last_batch_flag_sent_to:
+                if not batch:
+                    return True
 
-        return not all(
-            batch and batch.last_batch for batch in self._last_batch_received.values()
-        )
+                if not batch.last_batch:
+                    return True
+
+                if not self.get_last_batch_sent(step_name):
+                    return True
+
+        return False
 
     def register_batch(self, batch: _Batch) -> None:
         """Method to register a batch received from a step. It will keep track of the
         sequence number and the last batch received from the step in the internal maps.
 
         Args:
             batch: _Batch from which we will register the sequence number and the last batch received.
         """
         self._last_batch_received[batch.step_name] = batch
 
     def get_last_batch(self, step_name: str) -> Union[_Batch, None]:
+        """Gets the last batch received from a step.
+
+        Args:
+            step_name: The name of the step.
+
+        Returns:
+            The last batch received from the step or `None` if no batch was received.
+        """
         return self._last_batch_received.get(step_name)
 
     def add_batch(self, to_step: str, batch: _Batch, prepend: bool = False) -> None:
         """Add an output batch from `batch.step_name` to `to_step`.
 
         Args:
             to_step: The name of the step that will process the batch.
@@ -747,36 +1164,72 @@
 
         Returns:
             The name of the previous steps for which the input buffer for this step is
             empty.
         """
         return self._steps[step_name].empty_buffers()
 
+    def set_last_batch_sent(self, batch: "_Batch") -> None:
+        """Set the last batch sent to a step.
+
+        Args:
+            batch: The last batch sent to a step.
+        """
+        self._last_batch_sent[batch.step_name] = batch
+
+    def get_last_batch_sent(self, step_name: str) -> Union["_Batch", None]:
+        """Get the last batch sent to a step.
+
+        Args:
+            step_name: The name of the step.
+
+        Returns:
+            The last batch sent to a step or `None` if no batch was sent.
+        """
+        return self._last_batch_sent.get(step_name, None)
+
+    def set_last_batch_flag_sent_to(self, step_name: str) -> None:
+        """Set the flag to indicate that the last batch was sent to a step.
+
+        Args:
+            step_name: The name of the step.
+        """
+        self._last_batch_flag_sent_to.append(step_name)
+
     @classmethod
     def from_dag(cls, dag: "DAG") -> "_BatchManager":
         """Create a `_BatchManager` instance from a `DAG` instance.
 
         Args:
             dag: The `DAG` instance.
 
         Returns:
             A `_BatchManager` instance.
         """
         steps = {}
         last_batch_received = {}
+        last_batch_sent = {}
         for step_name in dag:
-            step: "_Step" = dag.get_step(step_name)["step"]
+            step: "_Step" = dag.get_step(step_name)[STEP_ATTR_NAME]
             last_batch_received[step.name] = None
+            last_batch_sent[step.name] = None
             if step.is_generator:
                 continue
+            predecessors = list(dag.get_step_predecessors(step_name))
+            convergence_step = all(
+                dag.get_step(predecessor).get(RECEIVES_ROUTED_BATCHES_ATTR_NAME, False)
+                for predecessor in predecessors
+            )
             batch_manager_step = _BatchManagerStep.from_step(
-                step, dag.get_step_predecessors(step_name)
+                step=step,
+                predecessors=predecessors,
+                convergence_step=convergence_step,
             )
             steps[step_name] = batch_manager_step
-        return cls(steps, last_batch_received)
+        return cls(steps, last_batch_received, last_batch_sent, [])
 
     def _model_dump(self, obj: Any, **kwargs: Any) -> Dict[str, Any]:
         """Dumps the content of the `_BatchManager` to a dictionary.
 
         Args:
             obj (Any): Unused, just kept to match the signature of the parent method.
             kwargs (Any): Additional arguments that are kept to match the signature of the parent method.
@@ -786,39 +1239,49 @@
         """
         return {
             "steps": {name: step.dump() for name, step in self._steps.items()},
             "last_batch_received": {
                 step_name: batch.dump() if batch is not None else None
                 for step_name, batch in self._last_batch_received.items()
             },
+            "last_batch_sent": {
+                step_name: batch.dump() if batch is not None else None
+                for step_name, batch in self._last_batch_sent.items()
+            },
+            "last_batch_flag_sent_to": self._last_batch_flag_sent_to,
         }
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "_BatchManager":
         """Loads a `_BatchManager` from its serialized content in a dictionary.
 
         Args:
             data: The serialized batch manager.
 
         Returns:
             A `_BatchManager` instance.
         """
-        # Remove the type info, we already know its a _BatchManager, and there aren't subclasses of it
+        # Remove the type info, we already know its a `_BatchManager`, and there aren't subclasses of it
         data.pop(TYPE_INFO_KEY)
-        # Also there is only one type of _BatchManagerStep, so we can call it directly instead of generically
-        # via _get_class
+        # Also there is only one type of `_BatchManagerStep`, so we can call it directly instead of generically
+        # via `_get_module_attr`
         return cls(
             {
                 name: _BatchManagerStep.from_file(step_path)
                 for name, step_path in data["steps"].items()
             },
             {
                 step_name: _Batch.from_dict(batch) if batch is not None else None
                 for step_name, batch in data["last_batch_received"].items()
             },
+            {
+                step_name: _Batch.from_dict(batch) if batch is not None else None
+                for step_name, batch in data["last_batch_sent"].items()
+            },
+            data["last_batch_flag_sent_to"],
         )
 
     def save(
         self,
         path: Union["StrOrPath", None] = None,
         format: "SaveFormats" = "json",
         dump: Optional[Dict[str, Any]] = None,
```

### Comparing `distilabel-1.0.3/src/distilabel/pipeline/local.py` & `distilabel-1.1.0/src/distilabel/pipeline/local.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,41 +14,54 @@
 
 import logging
 import multiprocessing as mp
 import signal
 import threading
 import time
 import traceback
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union, cast
 
 import tblib
 
 from distilabel.distiset import create_distiset
 from distilabel.llms.mixins import CudaDevicePlacementMixin
-from distilabel.pipeline.base import BasePipeline, _Batch, _BatchManager, _WriteBuffer
+from distilabel.pipeline.base import (
+    LAST_BATCH_SENT_FLAG,
+    BasePipeline,
+    _Batch,
+    _BatchManager,
+    _WriteBuffer,
+)
+from distilabel.pipeline.constants import (
+    CONVERGENCE_STEP_ATTR_NAME,
+    INPUT_QUEUE_ATTR_NAME,
+    ROUTING_BATCH_FUNCTION_ATTR_NAME,
+    STEP_ATTR_NAME,
+)
 from distilabel.steps.base import Step
 from distilabel.utils.logging import setup_logging, stop_logging
 
 if TYPE_CHECKING:
     from multiprocessing.managers import DictProxy, SyncManager
     from multiprocessing.pool import Pool
     from queue import Queue
 
     from distilabel.distiset import Distiset
-    from distilabel.steps.base import GeneratorStep
+    from distilabel.steps.base import GeneratorStep, _Step
 
 
 _STEPS_LOADED_KEY = "steps_loaded"
 _STEPS_LOADED_LOCK_KEY = "steps_loaded_lock"
 _STEPS_LOADED_ERROR_CODE = -1
 _CUDA_LLM_DEVICE_PLACEMENT_KEY = "cuda_llm_device_placement"
 _CUDA_LLM_DEVICE_PLACEMENT_LOCK_KEY = "cuda_llm_device_placement_lock"
 
 _STOP_CALLED = False
 _STOP_CALLED_LOCK = threading.Lock()
+_STOP_CALLS = 0
 
 _STEPS_LOADED = set()
 _STEPS_LOADED_LOCK = threading.Lock()
 
 _STEPS_FINISHED = set()
 _STEPS_FINISHED_LOCK = threading.Lock()
 
@@ -78,23 +91,23 @@
 
         Returns:
             The `Distiset` created by the pipeline.
 
         Raises:
             RuntimeError: If the pipeline fails to load all the steps.
         """
-        try:
-            mp.set_start_method("forkserver")
-        except RuntimeError:
-            pass
         log_queue = mp.Queue()
-        setup_logging(log_queue)  # type: ignore
+        # We must place the runtime parameters before calling setup_logging to ensure consistency
+        super().run(parameters, use_cache)
+        setup_logging(log_queue, filename=str(self._cache_location["log_file"]))  # type: ignore
         self._logger = logging.getLogger("distilabel.pipeline.local")
 
-        super().run(parameters, use_cache)
+        if self._dry_run:
+            # This message is placed here to ensure we are using the already setup logger.
+            self._logger.info("🌵 Dry run mode")
 
         if self._batch_manager is None:
             self._batch_manager = _BatchManager.from_dag(self.dag)
 
         # If the batch manager is not able to generate batches, that means that the loaded
         # `_BatchManager` from cache didn't have any remaining batches to process i.e.
         # the previous pipeline execution was completed successfully.
@@ -103,28 +116,32 @@
                 "💾 Loaded batch manager from cache doesn't have any remaining data. Returning"
                 " `Distiset` from cache data..."
             )
             stop_logging()
             return create_distiset(
                 self._cache_location["data"],
                 pipeline_path=self._cache_location["pipeline"],
+                log_filename_path=self._cache_location["log_file"],
+                enable_metadata=self._enable_metadata,
             )
 
         buffer_data_path = self._cache_location["data"]
         self._logger.info(f"📝 Pipeline data will be written to '{buffer_data_path}'")
         write_buffer = _WriteBuffer(buffer_data_path, self.dag.leaf_steps)
 
         num_processes = len(self.dag)
-        ctx = mp.get_context("forkserver")  # type: ignore
+        ctx = mp.get_context()  # type: ignore
         with ctx.Manager() as manager, ctx.Pool(
-            num_processes, initializer=_init_worker, initargs=(log_queue,)
+            num_processes,
+            initializer=_init_worker,
+            initargs=(log_queue,),
         ) as pool:
             self.output_queue: "Queue[Any]" = manager.Queue()
             self.shared_info = self._create_shared_info_dict(manager)
-            self._handle_keyboard_interrupt()
+            self._handle_keyboard_interrupt(manager=manager, pool=pool)
 
             # Run the steps using the pool of processes
             self._run_steps_in_loop(pool, manager, self.output_queue, self.shared_info)
 
             # Wait for all the steps to be loaded correctly
             if not self._all_steps_loaded():
                 write_buffer.close()
@@ -145,15 +162,18 @@
             self._notify_steps_to_stop()
 
             pool.close()
             pool.join()
 
         write_buffer.close()
         distiset = create_distiset(
-            self._cache_location["data"], pipeline_path=self._cache_location["pipeline"]
+            self._cache_location["data"],
+            pipeline_path=self._cache_location["pipeline"],
+            log_filename_path=self._cache_location["log_file"],
+            enable_metadata=self._enable_metadata,
         )
         stop_logging()
         return distiset
 
     def _run_output_queue_loop_in_thread(self, write_buffer: "_WriteBuffer") -> None:
         """Runs the output queue loop in a separate thread to receive the output batches
         from the steps. This is done to avoid the signal handler to block the loop, which
@@ -166,15 +186,15 @@
         thread.start()
         thread.join()
 
     def _notify_steps_to_stop(self) -> None:
         """Notifies the steps to stop their infinite running loop by sending `None` to
         their input queues."""
         for step_name in self.dag:
-            if input_queue := self.dag.get_step(step_name).get("input_queue"):
+            if input_queue := self.dag.get_step(step_name).get(INPUT_QUEUE_ATTR_NAME):
                 input_queue.put(None)
 
     def _output_queue_loop(self, write_buffer: "_WriteBuffer") -> None:
         """Loop to receive the output batches from the steps and manage the flow of the
         batches through the pipeline.
 
         Args:
@@ -214,77 +234,156 @@
         requested to send a new batch.
 
         Args:
             batch: The batch that was processed.
         """
         assert self._batch_manager, "Batch manager is not set"
 
-        self._batch_manager.register_batch(batch)
-        self._logger.debug(
-            f"Batch {batch.seq_no} from step '{batch.step_name}' registered in batch"
-            " manager"
-        )
+        # Make sure to send the `LAST_BATCH_SENT_FLAG` to the predecessors of the convergence
+        # step if the batch is the last one, so they stop their processing loop even if
+        # they haven't received the last batch because of the routing function.
+        if self._is_convergence_step(batch.step_name) and batch.last_batch:
+            for step_name in self.dag.get_step_predecessors(batch.step_name):
+                self._send_last_batch_flag_to_step(step_name)
+
+        route_to, routed = self._get_successors(batch)
+
+        # Keep track of the steps that the batch was routed to
+        if routed:
+            batch.batch_routed_to = route_to
+
+        self._register_batch(batch)
 
-        step: "Step" = self.dag.get_step(batch.step_name)["step"]
+        step = self._get_step_from_batch(batch)
 
-        for successor in self.dag.get_step_successors(step.name):
-            self._batch_manager.add_batch(successor, batch)
+        # Add the batch to the successors input buffers
+        for successor in route_to:
+            # Copy batch to avoid modifying the same reference in the batch manager
+            batch_to_add = batch.copy() if len(route_to) > 1 else batch
+
+            self._batch_manager.add_batch(successor, batch_to_add)
 
             # Check if the step is a generator and if there are successors that need data
             # from this step. This usually happens when the generator `batch_size` is smaller
             # than the `input_batch_size` of the successor steps.
             if (
                 step.is_generator
                 and step.name in self._batch_manager.step_empty_buffers(successor)
             ):
-                last_batch = self._batch_manager.get_last_batch(step.name)
-                self._send_batch_to_step(last_batch.next_batch())  # type: ignore
+                last_batch_sent = self._batch_manager.get_last_batch_sent(step.name)
+                self._send_batch_to_step(last_batch_sent.next_batch())  # type: ignore
 
+            # If successor step has enough data in its buffer to create a new batch, then
+            # send the batch to the step.
             if new_batch := self._batch_manager.get_batch(successor):
                 self._send_batch_to_step(new_batch)
 
         if step.is_generator:
             return
 
-        # Step has enough data on its buffers to create a new batch
-        if next_batch := self._batch_manager.get_batch(step.name):
-            self._send_batch_to_step(next_batch)
-            return
+        # Step ("this", the one from which the batch was received) has enough data on its
+        # buffers to create a new batch
+        if new_batch := self._batch_manager.get_batch(step.name):  # type: ignore
+            self._send_batch_to_step(new_batch)
+        else:
+            self._request_more_batches_if_needed(step)
+
+        self._cache()
+
+    def _register_batch(self, batch: "_Batch") -> None:
+        """Registers a batch in the batch manager.
+
+        Args:
+            batch: The batch to register.
+        """
+        self._batch_manager.register_batch(batch)  # type: ignore
+        self._logger.debug(
+            f"Batch {batch.seq_no} from step '{batch.step_name}' registered in batch"
+            " manager"
+        )
+
+    def _get_successors(self, batch: "_Batch") -> Tuple[List[str], bool]:
+        """Gets the successors and the successors to which the batch has to be routed.
 
-        # Request more batches to the predecessors generator steps
-        empty_buffers = self._batch_manager.step_empty_buffers(step.name)
+        Args:
+            batch: The batch to which the successors will be determined.
+
+        Returns:
+            The successors to route the batch to and whether the batch was routed using
+            a routing function.
+        """
+        node = self.dag.get_step(batch.step_name)
+        step: "Step" = node[STEP_ATTR_NAME]
+        successors = list(self.dag.get_step_successors(step.name))  # type: ignore
+        route_to = successors
+
+        # Check if the step has a routing function to send the batch to specific steps
+        if routing_batch_function := node.get(ROUTING_BATCH_FUNCTION_ATTR_NAME):
+            route_to = routing_batch_function(batch, successors)
+            successors_str = ", ".join(f"'{successor}'" for successor in route_to)
+            self._logger.info(
+                f"🚏 Using '{step.name}' routing function to send batch {batch.seq_no} to steps: {successors_str}"
+            )
+
+        return route_to, route_to != successors
+
+    def _get_step_from_batch(self, batch: "_Batch") -> "Step":
+        """Gets the `Step` instance from a batch.
+
+        Args:
+            batch: The batch to get the step from.
+
+        Returns:
+            The `Step` instance.
+        """
+        return self.dag.get_step(batch.step_name)[STEP_ATTR_NAME]
+
+    def _request_more_batches_if_needed(self, step: "Step") -> None:
+        """Request more batches to the predecessors steps of `step` if needed.
+
+        Args:
+            step: The step of which it has to be checked if more batches are needed from
+                its predecessors.
+        """
+        empty_buffers = self._batch_manager.step_empty_buffers(step.name)  # type: ignore
         for previous_step_name in empty_buffers:
             if previous_step_name not in self.dag.root_steps:
                 continue
 
-            if last_batch := self._batch_manager.get_last_batch(previous_step_name):
-                self._logger.debug(
-                    f"Step '{step.name}' input buffer for step '{previous_step_name}' is"
-                    " empty. Requesting new batch..."
-                )
-                self._send_batch_to_step(last_batch.next_batch())
+            last_batch = self._batch_manager.get_last_batch_sent(previous_step_name)  # type: ignore
+            if last_batch is None:
+                continue
 
-        self._cache()
+            self._logger.debug(
+                f"Step '{step.name}' input buffer for step '{previous_step_name}' is"
+                " empty. Requesting new batch..."
+            )
+            self._send_batch_to_step(last_batch.next_batch())
 
     def _handle_stop(self, write_buffer: "_WriteBuffer") -> None:
         """Handles the stop of the pipeline execution, which will stop the steps from
         processing more batches and wait for the output queue to be empty, to not lose
         any data that was already processed by the steps before the stop was called.
 
         Args:
             write_buffer: The write buffer to write the data from the leaf steps to disk.
         """
         self._logger.debug("Handling stop of the pipeline execution...")
 
-        # Send `None` to the input queues of all the steps to notify them to stop
-        # processing batches.
+        # Add the remaining batches in the input queues back to the batch manager
         for step_name in self.dag:
-            if input_queue := self.dag.get_step(step_name).get("input_queue"):
+            node = self.dag.get_step(step_name)
+            step: "_Step" = node[STEP_ATTR_NAME]
+            if step.is_generator:
+                continue
+            if input_queue := node.get(INPUT_QUEUE_ATTR_NAME):
                 while not input_queue.empty():
                     batch = input_queue.get()
+                    if batch is None:
+                        continue
                     self._batch_manager.add_batch(  # type: ignore
                         to_step=step_name, batch=batch, prepend=True
                     )
                     self._logger.debug(
                         f"Adding batch back to the batch manager: {batch}"
                     )
                 input_queue.put(None)
@@ -294,45 +393,49 @@
         for step_name in self.dag:
             self._wait_step_input_queue_empty(step_name)
 
         # Consume the output queue until it's empty to not lose any data that was already
         # processed by the steps before stop was called.
         while not self.output_queue.empty():
             batch = self.output_queue.get()
+            if batch is None:
+                continue
+
             if batch.step_name in self.dag.leaf_steps:
                 write_buffer.add_batch(batch)
+
             self._handle_batch_on_stop(batch)
 
         self._cache()
 
     def _handle_batch_on_stop(self, batch: "_Batch") -> None:
         """Handles a batch that was received from the output queue when the pipeline was
         stopped. It will add and register the batch in the batch manager.
 
         Args:
             batch: The batch to handle.
         """
         self._batch_manager.register_batch(batch)  # type: ignore
-        step: "Step" = self.dag.get_step(batch.step_name)["step"]
-        for successor in self.dag.get_step_successors(step.name):
+        step: "Step" = self.dag.get_step(batch.step_name)[STEP_ATTR_NAME]
+        for successor in self.dag.get_step_successors(step.name):  # type: ignore
             self._batch_manager.add_batch(successor, batch)  # type: ignore
 
     def _wait_step_input_queue_empty(self, step_name: str) -> Union["Queue[Any]", None]:
         """Waits for the input queue of a step to be empty.
 
         Args:
             step_name: The name of the step.
 
         Returns:
             The input queue of the step if it's not loaded or finished, `None` otherwise.
         """
         if self._check_step_not_loaded_or_finished(step_name):
             return None
 
-        if input_queue := self.dag.get_step(step_name).get("input_queue"):
+        if input_queue := self.dag.get_step(step_name).get(INPUT_QUEUE_ATTR_NAME):
             while input_queue.qsize() != 0:
                 pass
             return input_queue
 
     def _create_shared_info_dict(self, manager: "SyncManager") -> "DictProxy[str, Any]":
         """Creates the shared information dictionary to be used by the processes.
 
@@ -405,32 +508,63 @@
                 )
                 self._send_batch_to_step(batch)
 
         for step_name in self.dag.root_steps:
             seq_no = 0
             if last_batch := self._batch_manager.get_last_batch(step_name):
                 seq_no = last_batch.seq_no + 1
-            batch = _Batch(seq_no=seq_no, step_name=step_name, last_batch=False)
+            batch = _Batch(seq_no=seq_no, step_name=step_name, last_batch=self._dry_run)
             self._logger.debug(
                 f"Requesting initial batch to '{step_name}' generator step: {batch}"
             )
             self._send_batch_to_step(batch)
 
     def _send_batch_to_step(self, batch: "_Batch") -> None:
         """Sends a batch to the input queue of a step.
 
         Args:
             batch: The batch to send.
         """
         self._logger.debug(
+            f"Setting batch {batch.seq_no} as last batch sent to '{batch.step_name}': {batch}"
+        )
+        self._batch_manager.set_last_batch_sent(batch)  # type: ignore
+
+        self._logger.debug(
             f"Sending batch {batch.seq_no} to step '{batch.step_name}': {batch}"
         )
-        input_queue = self.dag.get_step(batch.step_name)["input_queue"]
+        input_queue = self.dag.get_step(batch.step_name)[INPUT_QUEUE_ATTR_NAME]
         input_queue.put(batch)
 
+    def _is_convergence_step(self, step_name: str) -> None:
+        """Checks if a step is a convergence step.
+
+        Args:
+            step_name: The name of the step.
+        """
+        return self.dag.get_step(step_name).get(CONVERGENCE_STEP_ATTR_NAME)
+
+    def _send_last_batch_flag_to_step(self, step_name: str) -> None:
+        """Sends the `LAST_BATCH_SENT_FLAG` to a step to stop processing batches.
+
+        Args:
+            step_name: The name of the step.
+        """
+        batch = self._batch_manager.get_last_batch_sent(step_name)  # type: ignore
+        if batch and batch.last_batch:
+            return
+
+        self._logger.debug(
+            f"Sending `LAST_BATCH_SENT_FLAG` to '{step_name}' step to stop processing"
+            " batches..."
+        )
+        input_queue = self.dag.get_step(step_name)[INPUT_QUEUE_ATTR_NAME]
+        input_queue.put(LAST_BATCH_SENT_FLAG)
+        self._batch_manager.set_last_batch_flag_sent_to(step_name)  # type: ignore
+
     def _run_steps_in_loop(
         self,
         pool: "Pool",
         manager: "SyncManager",
         output_queue: "Queue[_Batch]",
         shared_info: "DictProxy[str, Any]",
     ) -> None:
@@ -444,28 +578,29 @@
         Args:
             pool: The pool of processes.
             manager: The manager to create the queues.
             output_queue: The queue to send the output batches.
             shared_info: The shared information between the processes.
         """
         for step_name in self.dag:
-            step: "Step" = self.dag.get_step(step_name)["step"]
+            step: "Step" = self.dag.get_step(step_name)[STEP_ATTR_NAME]
             input_queue = manager.Queue()
-            self.dag.set_step_attr(step.name, "input_queue", input_queue)
+            self.dag.set_step_attr(step.name, INPUT_QUEUE_ATTR_NAME, input_queue)
 
             # Set `pipeline` to `None` as in some Python environments the pipeline is not
             # picklable and it will raise an error when trying to send the step to the process.
             # `TypeError: cannot pickle 'code' object`
             step.pipeline = None
 
             process_wrapper = _ProcessWrapper(
                 step=step,
                 input_queue=input_queue,
                 output_queue=output_queue,
                 shared_info=shared_info,
+                dry_run=self._dry_run,
             )
 
             pool.apply_async(
                 process_wrapper.run,
                 callback=self._finished_callback,
                 error_callback=self._error_callback,
             )  # type: ignore
@@ -540,48 +675,75 @@
 
         with _STEPS_FINISHED_LOCK:
             if step_name in _STEPS_FINISHED:
                 return True
 
         return False
 
-    def _stop(self) -> None:
+    def _stop(
+        self, manager: Optional["SyncManager"] = None, pool: Optional["Pool"] = None
+    ) -> None:
         """Stops the pipeline execution. It will first send `None` to the input queues
         of all the steps and then wait until the output queue is empty i.e. all the steps
         finished processing the batches that were sent before the stop flag. Then it will
         send `None` to the output queue to notify the pipeline to stop."""
 
         global _STOP_CALLED
 
         with _STOP_CALLED_LOCK:
             if _STOP_CALLED:
-                self._logger.warning(
-                    "🛑 Stop has already been called. Ignoring subsequent calls and waiting"
-                    " for the pipeline to finish..."
-                )
+                global _STOP_CALLS
+                _STOP_CALLS += 1
+                # if _STOP_CALLS == 1:
+                #     self._logger.warning(
+                #         "🛑 Stop has already been called. Ignoring subsequent calls and waiting"
+                #         " for the pipeline to finish..."
+                #     )
+                if _STOP_CALLS == 1:
+                    self._logger.warning(
+                        "🛑 Press again to force the pipeline to stop."
+                    )
+                elif _STOP_CALLS > 1:
+                    self._logger.warning("🛑 Forcing pipeline interruption.")
+                    import gc
+                    import sys
+
+                    if manager:
+                        manager.shutdown()
+
+                    if pool:
+                        pool.close()
+                        pool.terminate()
+
+                    gc.collect()
+
+                    sys.exit(1)
+
                 return
             _STOP_CALLED = True
 
         self._logger.debug(f"Steps loaded before calling `stop`: {_STEPS_LOADED}")
         self._logger.info(
             "🛑 Stopping pipeline. Waiting for steps to finish processing batches..."
         )
         self._logger.debug("Sending `None` to the output queue to notify stop...")
         self.output_queue.put(None)
 
-    def _handle_keyboard_interrupt(self) -> None:
+    def _handle_keyboard_interrupt(
+        self, manager: Optional["SyncManager"] = None, pool: Optional["Pool"] = None
+    ) -> None:
         """Handles KeyboardInterrupt signal sent during the Pipeline.run method.
 
         It will try to call self._stop (if the pipeline didn't started yet, it won't
         have any effect), and if the pool is already started, will close it before exiting
         the program.
         """
 
         def signal_handler(signumber: int, frame: Any) -> None:
-            self._stop()
+            self._stop(manager=manager, pool=pool)
 
         signal.signal(signal.SIGINT, signal_handler)
 
 
 class _ProcessWrapperException(Exception):
     """Exception to be raised when an error occurs in the `Step` process.
 
@@ -648,27 +810,30 @@
 
     def __init__(
         self,
         step: "Step",
         input_queue: "Queue[_Batch]",
         output_queue: "Queue[_Batch]",
         shared_info: "DictProxy[str, Any]",
+        dry_run: bool = False,
     ) -> None:
         """Initializes the `_ProcessWrapper`.
 
         Args:
             step: The step to run.
             input_queue: The queue to receive the input data.
             output_queue: The queue to send the output data.
             shared_info: The shared information between the processes.
+            dry_run: Flag to ensure we are forcing to run the last batch.
         """
         self.step = step
         self.input_queue = input_queue
         self.output_queue = output_queue
         self.shared_info = shared_info
+        self._dry_run = dry_run
 
         # If step is a task, and it's using a `CUDALLM`, then set the CUDA device map
         # and the lock for that map.
         if hasattr(self.step, "llm") and isinstance(
             self.step.llm, CudaDevicePlacementMixin
         ):
             self.step.llm.set_device_placement_info(
@@ -710,15 +875,15 @@
         try:
             self.input_queue.get(block=False)
         except Exception:
             pass
 
         self.step._logger.info(f"🏁 Finished running step '{self.step.name}'")
 
-        return self.step.name
+        return self.step.name  # type: ignore
 
     def _notify_load(self) -> None:
         """Notifies that the step has finished executing its `load` function successfully."""
         with self.shared_info[_STEPS_LOADED_LOCK_KEY]:
             self.shared_info[_STEPS_LOADED_KEY].append(self.step.name)
 
     def _generator_step_process_loop(self) -> None:
@@ -730,32 +895,31 @@
         process will finish.
 
         Raises:
             _ProcessWrapperException: If an error occurs during the execution of the
                 `process` method.
         """
         step = cast("GeneratorStep", self.step)
-
         try:
             if (batch := self.input_queue.get()) is None:
                 self.step._logger.info(
                     f"🛑 Stopping yielding batches from step '{self.step.name}'"
                 )
                 return
 
-            offset = batch.seq_no * step.batch_size
+            offset = batch.seq_no * step.batch_size  # type: ignore
 
             self.step._logger.info(
                 f"🧬 Starting yielding batches from generator step '{self.step.name}'."
                 f" Offset: {offset}"
             )
 
             for data, last_batch in step.process_applying_mappings(offset=offset):
-                batch.data = [data]
-                batch.last_batch = last_batch
+                batch.set_data([data])
+                batch.last_batch = self._dry_run or last_batch
                 self._send_batch(batch)
 
                 if batch.last_batch:
                     return
 
                 self.step._logger.debug(
                     f"Step '{self.step.name}' waiting for next batch request..."
@@ -785,40 +949,49 @@
         while True:
             if (batch := self.input_queue.get()) is None:
                 self.step._logger.info(
                     f"🛑 Stopping processing batches from step '{self.step.name}'"
                 )
                 break
 
+            if batch == LAST_BATCH_SENT_FLAG:
+                self.step._logger.debug("Received `LAST_BATCH_SENT_FLAG`. Stopping...")
+                break
+
             self.step._logger.info(
                 f"📦 Processing batch {batch.seq_no} in '{batch.step_name}'"
             )
-            # `result` is initially an empty list so f `process` method raises an exception
-            # an empty batch will be sent to the `output_queue`
             result = []
             try:
                 if self.step.has_multiple_inputs:
                     result = next(self.step.process_applying_mappings(*batch.data))
                 else:
                     result = next(self.step.process_applying_mappings(batch.data[0]))
             except Exception as e:
                 if self.step.is_global:
                     raise _ProcessWrapperException(str(e), self.step, 2, e) from e
 
+                # Impute step outputs columns with `None`
+                for row in batch.data[0]:
+                    data = row.copy()
+                    for output in self.step.outputs:
+                        data[output] = None
+                    result.append(data)
+
                 # if the step is not global then we can skip the batch which means sending
                 # an empty batch to the output queue
                 self.step._logger.warning(
                     f"⚠️ Processing batch {batch.seq_no} with step '{self.step.name}' failed."
-                    " Sending empty batch..."
+                    " Sending empty batch filled with `None`s..."
                 )
                 self.step._logger.warning(
                     f"Subprocess traceback:\n\n{traceback.format_exc()}"
                 )
             finally:
-                batch.data = [result]
+                batch.set_data([result])
                 self._send_batch(batch)
 
             if batch.last_batch:
                 break
 
     def _send_batch(self, batch: _Batch) -> None:
         """Sends a batch to the `output_queue`."""
```

### Comparing `distilabel-1.0.3/src/distilabel/pipeline/utils.py` & `distilabel-1.1.0/src/distilabel/pipeline/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,27 @@
 
 
 def combine_dicts(
     *inputs: StepInput,
     merge_keys: List[str],
     output_merge_keys: Optional[List[str]] = None,
 ) -> StepInput:
+    """Combines multiple list of dictionaries into a single list of dictionaries on the
+    specified `merge_keys`. If `output_merge_keys` are provided, then it will also rename
+    `merge_keys`.
+
+    Args:
+        inputs: list of dictionaries to combine.
+        merge_keys: list of keys to merge on.
+        output_merge_keys: list of keys to rename the merge keys to. Defaults to `None`.
+
+    Returns:
+        A list of dictionaries where the values of the `merge_keys` are combined into a
+        list and renamed to `output_merge_keys`.
+    """
     if output_merge_keys is not None and len(output_merge_keys) != len(merge_keys):
         raise ValueError(
             "The length of output_merge_keys must be the same as the length of merge_keys"
         )
     if output_merge_keys is None:
         output_merge_keys = [f"merged_{key}" for key in merge_keys]
     merge_keys_dict = dict(zip(merge_keys, output_merge_keys))
```

### Comparing `distilabel-1.0.3/src/distilabel/steps/base.py` & `distilabel-1.1.0/src/distilabel/steps/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,43 +10,89 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import inspect
 import logging
+import re
 from abc import ABC, abstractmethod
 from enum import Enum
 from functools import cached_property
-from typing import TYPE_CHECKING, Any, Dict, List, Tuple, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union, overload
 
 from pydantic import BaseModel, ConfigDict, Field, PositiveInt, PrivateAttr
-from typing_extensions import Annotated
+from typing_extensions import Annotated, Self
 
 from distilabel.mixins.runtime_parameters import (
     RuntimeParameter,
     RuntimeParametersMixin,
 )
 from distilabel.utils.serialization import TYPE_INFO_KEY, _Serializable
 from distilabel.utils.typing_ import is_parameter_annotated_with
 
 if TYPE_CHECKING:
     from logging import Logger
 
+    from distilabel.pipeline.base import BasePipeline
+    from distilabel.pipeline.routing_batch_function import RoutingBatchFunction
+    from distilabel.pipeline.typing import (
+        DownstreamConnectable,
+        DownstreamConnectableSteps,
+        UpstreamConnectableSteps,
+    )
     from distilabel.steps.typing import GeneratorStepOutput, StepOutput
 
+
 DEFAULT_INPUT_BATCH_SIZE = 50
 
 
 _STEP_INPUT_ANNOTATION = "distilabel_step_input"
 StepInput = Annotated[List[Dict[str, Any]], _STEP_INPUT_ANNOTATION]
 """StepInput is just an `Annotated` alias of the typing `List[Dict[str, Any]]` with
 extra metadata that allows `distilabel` to perform validations over the `process` step
 method defined in each `Step`"""
 
+# Pattern to convert PascalCase to snake_case
+PATTERN_PASCAL_NAME = re.compile(r"(?<!^)(?=[A-Z])")
+
+
+def _infer_step_name(
+    step_cls_name: str, pipeline: Optional["BasePipeline"] = None
+) -> str:
+    """Infer the name of the step based on the class name and the pipeline.
+
+    If a `Pipeline` is given (the general case), it will check if the name already exists
+    in the steps of the `DAG`, to add a number at the end of the name.
+
+    Args:
+        step_cls_name: The step class name, as obtained by `type(cls).__name__`.
+        pipeline: The `Pipeline` the step belongs to, can be `None` if the step is created
+            outside of a `Pipeline`.
+
+    Returns:
+        A name for the step.
+
+    Example:
+        ```python
+        >>> _infer_step_name("StepWithOnePreviousStep", None)
+        'step_with_one_previous_step'
+        ```
+    """
+    name = re.sub(PATTERN_PASCAL_NAME, "_", step_cls_name).lower() + "_0"
+    if pipeline:
+        # Check the name doesn't already exist in the pipeline
+        step_names = set(pipeline.dag.G)
+        parts = name.split("_")
+        base_name = "_".join(parts[:-1])
+        while name in step_names:
+            idx = int(name.split("_")[-1])
+            name = f"{base_name}_{idx+1}"
+    return name
+
 
 class _Step(RuntimeParametersMixin, BaseModel, _Serializable, ABC):
     """Base class for the steps that can be included in a `Pipeline`.
 
     A `Step` is a class defining some processing logic. The input and outputs for this
     processing logic are lists of dictionaries with the same keys:
 
@@ -89,59 +135,174 @@
     connection to a database, etc.
 
     Finally, the `Step` class inherits from `pydantic.BaseModel`, so attributes can be easily
     defined, validated, serialized and included in the `__init__` method of the step.
     """
 
     model_config = ConfigDict(
-        arbitrary_types_allowed=True, validate_default=True, validate_assignment=True
+        arbitrary_types_allowed=True,
+        validate_default=True,
+        validate_assignment=True,
+        extra="forbid",
     )
 
-    name: str = Field(pattern=r"^[a-zA-Z0-9_-]+$")
-    pipeline: Annotated[Any, Field(exclude=True, repr=False)] = None
+    name: Optional[str] = Field(default=None, pattern=r"^[a-zA-Z0-9_-]+$")
+    pipeline: Any = Field(default=None, exclude=True, repr=False)
     input_mappings: Dict[str, str] = {}
     output_mappings: Dict[str, str] = {}
 
     _built_from_decorator: bool = PrivateAttr(default=False)
-    _logger: Union["Logger", None] = PrivateAttr(...)
+    _logger: "Logger" = PrivateAttr(None)
 
     def model_post_init(self, __context: Any) -> None:
         from distilabel.pipeline.base import _GlobalPipelineManager
 
         super().model_post_init(__context)
 
         if self.pipeline is None:
             self.pipeline = _GlobalPipelineManager.get_pipeline()
 
         if self.pipeline is None:
-            raise ValueError(
+            _logger = logging.getLogger(f"distilabel.step.{self.name}")
+            _logger.warning(
                 f"Step '{self.name}' hasn't received a pipeline, and it hasn't been"
                 " created within a `Pipeline` context. Please, use"
                 " `with Pipeline() as pipeline:` and create the step within the context."
             )
 
-        self.pipeline._add_step(self)
+        if not self.name:
+            # This must be done before the check for repeated names, but assuming
+            # we are passing the pipeline from the _GlobalPipelineManager, should
+            # be done after that.
+            self.name = _infer_step_name(type(self).__name__, self.pipeline)
+
+        if self.pipeline is not None:
+            # If not set an error will be raised in `Pipeline.run` parent
+            self.pipeline._add_step(self)
 
     def connect(
-        self, step: "_Step", input_mappings: Union[Dict[str, str], None] = None
+        self,
+        *steps: "_Step",
+        routing_batch_function: Optional["RoutingBatchFunction"] = None,
     ) -> None:
         """Connects the current step to another step in the pipeline, which means that
         the output of this step will be the input of the other step.
 
         Args:
-            step: The step to connect to.
-            input_mappings: A dictionary with the mapping of the columns from the output
-                of the current step to the input of the other step. If `None`, the
-                columns will be mapped by name. This is useful when the names of the
-                output columns of the current step are different from the names of the
-                input columns of the other step. Defaults to `None`.
-        """
-        if input_mappings is not None:
-            step.input_mappings = input_mappings
-        self.pipeline._add_edge(self.name, step.name)  # type: ignore
+            steps: The steps to connect to the current step.
+            routing_batch_function: A function that receives a list of steps and returns
+                a list of steps to which the output batch generated by this step should be
+                routed. It should be used to define the routing logic of the pipeline. If
+                not provided, the output batch will be routed to all the connected steps.
+                Defaults to `None`.
+        """
+        assert self.pipeline is not None
+
+        if routing_batch_function:
+            self._set_routing_batch_function(routing_batch_function)
+
+        for step in steps:
+            self.pipeline._add_edge(from_step=self.name, to_step=step.name)  # type: ignore
+
+    def _set_routing_batch_function(
+        self, routing_batch_function: "RoutingBatchFunction"
+    ) -> None:
+        """Sets a routing batch function for the batches generated by this step, so they
+        get routed to specific downstream steps.
+
+        Args:
+            routing_batch_function: The routing batch function that will be used to route
+                the batches generated by this step.
+        """
+        self.pipeline._add_routing_batch_function(
+            step_name=self.name,  # type: ignore
+            routing_batch_function=routing_batch_function,
+        )
+        routing_batch_function._step = self
+
+    @overload
+    def __rshift__(self, other: "RoutingBatchFunction") -> "RoutingBatchFunction":
+        ...
+
+    @overload
+    def __rshift__(
+        self, other: List["DownstreamConnectableSteps"]
+    ) -> List["DownstreamConnectableSteps"]:
+        ...
+
+    @overload
+    def __rshift__(self, other: "DownstreamConnectable") -> "DownstreamConnectable":
+        ...
+
+    def __rshift__(
+        self,
+        other: Union[
+            "DownstreamConnectable",
+            "RoutingBatchFunction",
+            List["DownstreamConnectableSteps"],
+        ],
+    ) -> Union[
+        "DownstreamConnectable",
+        "RoutingBatchFunction",
+        List["DownstreamConnectableSteps"],
+    ]:
+        """Allows using the `>>` operator to connect steps in the pipeline.
+
+        Args:
+            other: The step to connect, a list of steps to connect to or a routing batch
+                function to be set for the step.
+
+        Returns:
+            The connected step, the list of connected steps or the routing batch function.
+
+        Example:
+            ```python
+            step1 >> step2
+            # Would be equivalent to:
+            step1.connect(step2)
+
+            # It also allows to connect a list of steps
+            step1 >> [step2, step3]
+            ```
+        """
+        # Here to avoid circular imports
+        from distilabel.pipeline.routing_batch_function import RoutingBatchFunction
+
+        if isinstance(other, list):
+            self.connect(*other)
+            return other
+
+        if isinstance(other, RoutingBatchFunction):
+            self._set_routing_batch_function(other)
+            return other
+
+        self.connect(other)
+        return other
+
+    def __rrshift__(self, other: List["UpstreamConnectableSteps"]) -> Self:
+        """Allows using the [step1, step2] >> step3 operator to connect a list of steps in the pipeline
+        to a single step, as the list doesn't have the __rshift__ operator.
+
+        Args:
+            other: The step to connect to.
+
+        Returns:
+            The connected step
+
+        Example:
+            ```python
+            [step2, step3] >> step1
+            # Would be equivalent to:
+            step2.connect(step1)
+            step3.connect(step1)
+            ```
+        """
+        for o in other:
+            o.connect(self)
+        return self
 
     def load(self) -> None:
         """Method to perform any initialization logic before the `process` method is
         called. For example, to load an LLM, stablish a connection to a database, etc.
         """
         self._logger = logging.getLogger(f"distilabel.step.{self.name}")
 
@@ -310,26 +471,29 @@
         if TYPE_INFO_KEY in _data.keys():
             _data.pop(TYPE_INFO_KEY)
 
         # Before passing the data to instantiate the general step, we have to instantiate
         # some of the internal objects. For the moment we only take into account the LLM,
         # we should take care if we update any of the objects.
         if llm := _data.get("llm"):
-            from distilabel.utils.serialization import _get_class
+            from distilabel.utils.serialization import _get_module_attr
 
-            nested_cls = _get_class(**llm.pop(TYPE_INFO_KEY))
+            nested_cls = _get_module_attr(**llm.pop(TYPE_INFO_KEY))
             # Load the LLM and update the _data inplace
             nested_cls = nested_cls(**llm)
             _data.update({"llm": nested_cls})
 
         # Enums need a specific restoring process
         for k, v in _data.items():
             if isinstance(v, dict) and "_type" in v and v["_type"] == "enum":
                 _data[k] = Enum(v["_name"], v["_values"], type=eval(v["_enum_type"]))
 
+        # Skip `runtime_parameters_info` since extras are not allowed
+        _data.pop("runtime_parameters_info", None)
+
         # Every step needs the pipeline, and the remaining arguments are general
         step = cls(**_data)
 
         return step
 
     def _model_dump(self, obj: Any, **kwargs: Any) -> Dict[str, Any]:
         dump = super()._model_dump(obj, **kwargs)
```

### Comparing `distilabel-1.0.3/src/distilabel/steps/combine.py` & `distilabel-1.1.0/src/distilabel/steps/combine.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,28 +20,31 @@
 from distilabel.steps.base import Step, StepInput
 
 if TYPE_CHECKING:
     from distilabel.steps.typing import StepOutput
 
 
 class CombineColumns(Step):
-    """CombineColumns is a Step that implements the `process` method that calls the `combine_dicts`
+    """Combines columns from a list of `StepInput`.
+
+    `CombineColumns` is a `Step` that implements the `process` method that calls the `combine_dicts`
     function to handle and combine a list of `StepInput`. Also `CombineColumns` provides two attributes
     `columns` and `output_columns` to specify the columns to merge and the output columns
     which will override the default value for the properties `inputs` and `outputs`, respectively.
 
     Attributes:
         columns: List of strings with the names of the columns to merge.
         output_columns: Optional list of strings with the names of the output columns.
 
     Input columns:
-        - dynamic, based on the `columns` value provided.
+        - dynamic (determined by `columns` attribute): The columns to merge.
 
     Output columns:
-        - dynamic, based on the `output_columns` value provided or `merged_{column}` for each column in `columns`.
+        - dynamic (determined by `columns` and `output_columns` attributes): The columns
+            that were merged.
     """
 
     columns: List[str]
     output_columns: Optional[List[str]] = None
 
     @property
     def inputs(self) -> List[str]:
```

### Comparing `distilabel-1.0.3/src/distilabel/steps/conversation.py` & `distilabel-1.1.0/src/distilabel/steps/formatting/conversation.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,14 +25,19 @@
 
     Input columns:
         - instruction (`str`): The instruction to be used in the conversation.
         - response (`str`): The response to be used in the conversation.
 
     Output columns:
         - conversation (`ChatType`): The conversation template.
+
+    Categories:
+        - format
+        - chat
+        - template
     """
 
     @property
     def inputs(self) -> List[str]:
         """The instruction and response."""
         return ["instruction", "response"]
```

### Comparing `distilabel-1.0.3/src/distilabel/steps/decorator.py` & `distilabel-1.1.0/src/distilabel/steps/decorator.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/steps/deita.py` & `distilabel-1.1.0/src/distilabel/steps/deita.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 from distilabel.steps.base import GlobalStep, StepInput
 
 if TYPE_CHECKING:
     from distilabel.steps.typing import StepOutput
 
 
 class DeitaFiltering(GlobalStep):
-    """Filter the dataset based on the DEITA score and the cosine distance between the embeddings.
+    """Filter dataset rows using DEITA filtering strategy.
+
+    Filter the dataset based on the DEITA score and the cosine distance between the embeddings.
     It's an implementation of the filtering step from the paper 'What Makes Good Data
     for Alignment? A Comprehensive Study of Automatic Data Selection in Instruction Tuning'.
 
     Attributes:
         data_budget: The desired size of the dataset after filtering.
         diversity_threshold: If a row has a cosine distance with respect to it's nearest
             neighbor greater than this value, it will be included in the filtered dataset.
@@ -53,14 +55,17 @@
     Output columns:
         - deita_score (`float`): The DEITA score for the instruction-response pair.
         - deita_score_computed_with (`List[str]`): The scores used to compute the DEITA
             score.
         - nearest_neighbor_distance (`float`): The cosine distance between the embeddings
             of the instruction-response pair.
 
+    Categories:
+        - filtering
+
     References:
         - [`What Makes Good Data for Alignment? A Comprehensive Study of Automatic Data Selection in Instruction Tuning`](https://arxiv.org/abs/2312.15685)
     """
 
     data_budget: RuntimeParameter[int] = Field(
         default=None, description="The desired size of the dataset after filtering."
     )
```

### Comparing `distilabel-1.0.3/src/distilabel/steps/expand.py` & `distilabel-1.1.0/src/distilabel/steps/expand.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,24 +22,29 @@
 if TYPE_CHECKING:
     from distilabel.steps.typing import StepOutput
 
 
 class ExpandColumns(Step):
     """Expand columns that contain lists into multiple rows.
 
+    `ExpandColumns` is a `Step` that takes a list of columns and expands them into multiple
+    rows. The new rows will have the same data as the original row, except for the expanded
+    column, which will contain a single item from the original list.
+
     Attributes:
         columns: A dictionary that maps the column to be expanded to the new column name
             or a list of columns to be expanded. If a list is provided, the new column name
             will be the same as the column name.
 
     Input columns:
-        - The columns to be expanded.
+        - dynamic (determined by `columns` attribute): The columns to be expanded into
+            multiple rows.
 
     Output columns:
-        - The expanded columns.
+        - dynamic (determined by `columns` attribute):  The expanded columns.
     """
 
     columns: Union[Dict[str, str], List[str]]
 
     @field_validator("columns")
     @classmethod
     def always_dict(cls, value: Union[Dict[str, str], List[str]]) -> Dict[str, str]:
```

### Comparing `distilabel-1.0.3/src/distilabel/steps/keep.py` & `distilabel-1.1.0/src/distilabel/steps/keep.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,32 +19,34 @@
 from distilabel.steps.base import Step, StepInput
 
 if TYPE_CHECKING:
     from distilabel.steps.typing import StepOutput
 
 
 class KeepColumns(Step):
-    """KeepColumns is a Step that implements the `process` method that keeps only the columns
+    """Keeps selected columns in the dataset.
+
+    `KeepColumns` is a `Step` that implements the `process` method that keeps only the columns
     specified in the `columns` attribute. Also `KeepColumns` provides an attribute `columns` to
     specify the columns to keep which will override the default value for the properties `inputs`
     and `outputs`.
 
     Note:
         The order in which the columns are provided is important, as the output will be sorted
         using the provided order, which is useful before pushing either a `dataset.Dataset` via
         the `PushToHub` step or a `distilabel.Distiset` via the `Pipeline.run` output variable.
 
     Attributes:
         columns: List of strings with the names of the columns to keep.
 
     Input columns:
-        - dynamic, based on the `columns` value provided.
+        - dynamic (determined by `columns` attribute): The columns to keep.
 
     Output columns:
-        - dynamic, based on the `columns` value provided.
+        - dynamic (determined by `columns` attribute): The columns that were kept.
     """
 
     columns: List[str]
 
     @property
     def inputs(self) -> List[str]:
         """The inputs for the task are the column names in `columns`."""
```

### Comparing `distilabel-1.0.3/src/distilabel/steps/typing.py` & `distilabel-1.1.0/src/distilabel/steps/typing.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/steps/argilla/__init__.py` & `distilabel-1.1.0/src/distilabel/steps/argilla/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/steps/argilla/base.py` & `distilabel-1.1.0/src/distilabel/steps/argilla/base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/steps/argilla/preference.py` & `distilabel-1.1.0/src/distilabel/steps/argilla/preference.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,17 @@
         TextQuestion,
     )
 
     from distilabel.steps.typing import StepOutput
 
 
 class PreferenceToArgilla(Argilla):
-    """Step that creates a dataset in Argilla during the load phase, and then pushes the input
+    """Creates a preference dataset in Argilla.
+
+    Step that creates a dataset in Argilla during the load phase, and then pushes the input
     batches into it as records. This dataset is a preference dataset, where there's one field
     for the instruction and one extra field per each generation within the same record, and then
     a rating question per each of the generation fields. The rating question asks the annotator to
     set a rating from 1 to 5 for each of the provided generations.
 
     Note:
         This step is meant to be used in conjunction with the `UltraFeedback` step, or any other step
@@ -124,15 +126,16 @@
                     rg.TextField(name=self._id, title=self._id),  # type: ignore
                     rg.TextField(name=self._instruction, title=self._instruction),  # type: ignore
                     *self._generation_fields(),  # type: ignore
                 ],
                 questions=self._rating_rationale_pairs(),  # type: ignore
             )
             self._rg_dataset = _rg_dataset.push_to_argilla(
-                name=self.dataset_name, workspace=self.dataset_workspace
+                name=self.dataset_name,  # type: ignore
+                workspace=self.dataset_workspace,
             )
 
     def _generation_fields(self) -> List["TextField"]:
         """Method to generate the fields for each of the generations."""
         return [
             rg.TextField(  # type: ignore
                 name=f"{self._generations}-{idx}",
@@ -148,15 +151,15 @@
         """Method to generate the rating and rationale questions for each of the generations."""
         questions = []
         for idx in range(self.num_generations):
             questions.extend(
                 [
                     rg.RatingQuestion(  # type: ignore
                         name=f"{self._generations}-{idx}-rating",
-                        title=f"Rate {self._generations}-{idx} given {self._instruction} based on the annotation guidelines.",
+                        title=f"Rate {self._generations}-{idx} given {self._instruction}.",
                         description=f"Ignore this question if the corresponding `{self._generations}-{idx}` field is not available."
                         if idx != 0
                         else None,
                         values=[1, 2, 3, 4, 5],
                         required=True if idx == 0 else False,
                     ),
                     rg.TextQuestion(  # type: ignore
```

### Comparing `distilabel-1.0.3/src/distilabel/steps/argilla/text_generation.py` & `distilabel-1.1.0/src/distilabel/steps/argilla/text_generation.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 from distilabel.steps.base import StepInput
 
 if TYPE_CHECKING:
     from distilabel.steps.typing import StepOutput
 
 
 class TextGenerationToArgilla(Argilla):
-    """Step that creates a dataset in Argilla during the load phase, and then pushes the input
+    """Creates a text generation dataset in Argilla.
+
+    `Step` that creates a dataset in Argilla during the load phase, and then pushes the input
     batches into it as records. This dataset is a text-generation dataset, where there's one field
     per each input, and then a label question to rate the quality of the completion in either bad
     (represented with 👎) or good (represented with 👍).
 
     Note:
         This step is meant to be used in conjunction with a `TextGeneration` step and no column mapping
         is needed, as it will use the default values for the `instruction` and `generation` columns.
@@ -69,15 +71,15 @@
         """
         super().load()
 
         self._instruction = self.input_mappings.get("instruction", "instruction")
         self._generation = self.input_mappings.get("generation", "generation")
 
         if self._rg_dataset_exists():
-            _rg_dataset = rg.FeedbackDataset.from_argilla(
+            _rg_dataset = rg.FeedbackDataset.from_argilla(  # type: ignore
                 name=self.dataset_name,
                 workspace=self.dataset_workspace,
             )
 
             for field in _rg_dataset.fields:
                 if (
                     field.name not in [self._id, self._instruction, self._generation]
@@ -87,30 +89,31 @@
                         f"The dataset {self.dataset_name} in the workspace {self.dataset_workspace} already exists,"
                         f" but contains at least a required field that is neither `{self._id}`, `{self._instruction}`"
                         f", nor `{self._generation}`."
                     )
 
             self._rg_dataset = _rg_dataset
         else:
-            _rg_dataset = rg.FeedbackDataset(
+            _rg_dataset = rg.FeedbackDataset(  # type: ignore
                 fields=[
                     rg.TextField(name=self._id, title=self._id),  # type: ignore
                     rg.TextField(name=self._instruction, title=self._instruction),  # type: ignore
                     rg.TextField(name=self._generation, title=self._generation),  # type: ignore
                 ],
                 questions=[
                     rg.LabelQuestion(  # type: ignore
                         name="quality",
                         title=f"What's the quality of the {self._generation} for the given {self._instruction}?",
                         labels={"bad": "👎", "good": "👍"},
                     )
                 ],
             )
             self._rg_dataset = _rg_dataset.push_to_argilla(
-                name=self.dataset_name, workspace=self.dataset_workspace
+                name=self.dataset_name,  # type: ignore
+                workspace=self.dataset_workspace,
             )
 
     @property
     def inputs(self) -> List[str]:
         """The inputs for the step are the `instruction` and the `generation`."""
         return ["instruction", "generation"]
 
@@ -144,15 +147,15 @@
                 # If the generation is already in the set, then skip it
                 if generation in generations_set:
                     continue
                 # Otherwise, add it to the set
                 generations_set.add(generation)
 
                 records.append(
-                    rg.FeedbackRecord(
+                    rg.FeedbackRecord(  # type: ignore
                         fields={
                             self._id: instruction_id,
                             self._instruction: input["instruction"],
                             self._generation: generation,
                         },
                     )
                 )
```

### Comparing `distilabel-1.0.3/src/distilabel/steps/generators/__init__.py` & `distilabel-1.1.0/src/distilabel/utils/card/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/steps/generators/data.py` & `distilabel-1.1.0/src/distilabel/steps/generators/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,26 +19,31 @@
 from distilabel.steps.base import GeneratorStep
 
 if TYPE_CHECKING:
     from distilabel.steps.typing import GeneratorStepOutput
 
 
 class LoadDataFromDicts(GeneratorStep):
-    """A generator step that loads a dataset from a list of dictionaries.
+    """Loads a dataset from a list of dictionaries.
 
-    This step will load the dataset and yield the transformed data as it is loaded from the list of dictionaries.
+    `GeneratorStep` that loads a dataset from a list of dictionaries and yields it in
+    batches.
 
     Attributes:
         data: The list of dictionaries to load the data from.
 
     Runtime parameters:
         - `batch_size`: The batch size to use when processing the data.
 
     Output columns:
-        Dynamic, based on the keys found on the first dictionary of the list
+        - dynamic (based on the keys found on the first dictionary of the list): The columns
+            of the dataset.
+
+    Categories:
+        - load
     """
 
     data: List[Dict[str, Any]]
 
     @override
     def process(self, offset: int = 0) -> "GeneratorStepOutput":  # type: ignore
         """Yields batches from a list of dictionaries.
```

### Comparing `distilabel-1.0.3/src/distilabel/steps/generators/huggingface.py` & `distilabel-1.1.0/src/distilabel/steps/generators/huggingface.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,83 +13,54 @@
 # limitations under the License.
 
 import os
 from functools import lru_cache
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 import requests
-from datasets import IterableDataset, load_dataset
+from datasets import DatasetInfo, IterableDataset, load_dataset
 from pydantic import Field, PrivateAttr
+from requests.exceptions import ConnectionError
 
 from distilabel.mixins.runtime_parameters import RuntimeParameter
 from distilabel.steps.base import GeneratorStep
 
 if TYPE_CHECKING:
     from distilabel.steps.typing import GeneratorStepOutput
 
 
-@lru_cache
-def _get_hf_dataset_info(
-    repo_id: str, config: Union[str, None] = None
-) -> Dict[str, Any]:
-    """Calls the Datasets Server API from Hugging Face to obtain the dataset information.
-    The results are cached to avoid making multiple requests to the server.
-
-    Args:
-        repo_id: The Hugging Face Hub repository ID of the dataset.
-        config: The configuration of the dataset. This is optional and only needed if the
-            dataset has multiple configurations.
-
-    Returns:
-        The dataset information.
-    """
-
-    params = {"dataset": repo_id}
-    if config is not None:
-        params["config"] = config
-
-    if "HF_TOKEN" in os.environ:
-        headers = {"Authorization": f"Bearer {os.environ['HF_TOKEN']}"}
-    else:
-        headers = None
-
-    response = requests.get(
-        "https://datasets-server.huggingface.co/info", params=params, headers=headers
-    )
-
-    assert (
-        response.status_code == 200
-    ), f"Failed to get '{repo_id}' dataset info. Make sure you have set the HF_TOKEN environment variable if it is a private dataset."
-
-    return response.json()["dataset_info"]
-
-
 class LoadHubDataset(GeneratorStep):
-    """A generator step that loads a dataset from the Hugging Face Hub using the `datasets`
-    library.
+    """Loads a dataset from the Hugging Face Hub.
 
-    This step will load the dataset in streaming mode, which means that it will not load the
-    entire dataset into memory at once. Instead, it will load the dataset in chunks and yield
-    the transformed data as it is loaded from the Hugging Face Hub.
+    `GeneratorStep` that loads a dataset from the Hugging Face Hub using the `datasets`
+    library.
 
     Attributes:
         repo_id: The Hugging Face Hub repository ID of the dataset to load.
         split: The split of the dataset to load.
         config: The configuration of the dataset to load. This is optional and only needed
             if the dataset has multiple configurations.
 
     Runtime parameters:
         - `batch_size`: The batch size to use when processing the data.
         - `repo_id`: The Hugging Face Hub repository ID of the dataset to load.
         - `split`: The split of the dataset to load. Defaults to 'train'.
         - `config`: The configuration of the dataset to load. This is optional and only
             needed if the dataset has multiple configurations.
+        - `streaming`: Whether to load the dataset in streaming mode or not. Defaults to
+            `False`.
+        - `num_examples`: The number of examples to load from the dataset.
+            By default will load all examples.
+
+    Output columns:
+        - dynamic (`all`): The columns that will be generated by this step, based on the
+            datasets loaded from the Hugging Face Hub.
 
-    Output columns
-        - dynamic, based on the dataset being loaded
+    Categories:
+        - load
     """
 
     repo_id: RuntimeParameter[str] = Field(
         default=None,
         description="The Hugging Face Hub repository ID of the dataset to load.",
     )
     split: RuntimeParameter[str] = Field(
@@ -97,50 +68,64 @@
         description="The split of the dataset to load. Defaults to 'train'.",
     )
     config: Optional[RuntimeParameter[str]] = Field(
         default=None,
         description="The configuration of the dataset to load. This is optional and only"
         " needed if the dataset has multiple configurations.",
     )
+    streaming: RuntimeParameter[bool] = Field(
+        default=False,
+        description="Whether to load the dataset in streaming mode or not. Defaults to False.",
+    )
+    num_examples: Optional[RuntimeParameter[int]] = Field(
+        default=None,
+        description="The number of examples to load from the dataset. By default will load all examples.",
+    )
 
     _dataset: Union[IterableDataset, None] = PrivateAttr(...)
 
     def load(self) -> None:
         """Load the dataset from the Hugging Face Hub"""
         super().load()
 
         self._dataset = load_dataset(
             self.repo_id,  # type: ignore
             self.config,
             split=self.split,
-            streaming=True,
+            streaming=self.streaming,
+        )
+        num_examples = self._get_dataset_num_examples()
+        self.num_examples = (
+            min(self.num_examples, num_examples) if self.num_examples else num_examples
         )
 
+        if not self.streaming:
+            self._dataset = self._dataset.select(range(self.num_examples))
+
     def process(self, offset: int = 0) -> "GeneratorStepOutput":
         """Yields batches from the loaded dataset from the Hugging Face Hub.
 
         Args:
             offset: The offset to start yielding the data from. Will be used during the caching
                 process to help skipping already processed data.
 
         Yields:
             A tuple containing a batch of rows and a boolean indicating if the batch is
             the last one.
         """
-        num_examples = self._get_dataset_num_examples()
         num_returned_rows = 0
         for batch_num, batch in enumerate(
             self._dataset.iter(batch_size=self.batch_size)  # type: ignore
         ):
             if batch_num * self.batch_size < offset:
                 continue
             transformed_batch = self._transform_batch(batch)
             batch_size = len(transformed_batch)
             num_returned_rows += batch_size
-            yield transformed_batch, num_returned_rows == num_examples
+            yield transformed_batch, num_returned_rows >= self.num_examples
 
     @property
     def outputs(self) -> List[str]:
         """The columns that will be generated by this step, based on the datasets loaded
         from the Hugging Face Hub.
 
         Returns:
@@ -179,20 +164,71 @@
     def _get_dataset_columns(self) -> List[str]:
         """Get the columns of the dataset, based on the `config` runtime parameter provided.
 
         Returns:
             The columns of the dataset.
         """
         dataset_info = self._get_dataset_info()
+
+        if isinstance(dataset_info, DatasetInfo):
+            if self.config:
+                return list(self._dataset[self.config].info.features.keys())
+            return list(self._dataset.info.features.keys())
+
         if self.config:
             return list(dataset_info["features"].keys())
         return list(dataset_info["default"]["features"].keys())
 
     def _get_dataset_info(self) -> Dict[str, Any]:
         """Calls the Datasets Server API from Hugging Face to obtain the dataset information.
 
         Returns:
             The dataset information.
         """
         repo_id = self.repo_id
         config = self.config
-        return _get_hf_dataset_info(repo_id, config)
+
+        try:
+            return _get_hf_dataset_info(repo_id, config)
+        except ConnectionError:
+            # The previous could fail in case of a internet connection issues.
+            # Assuming the dataset is already loaded and we can get the info from the loaded dataset, otherwise it will fail anyway.
+            self.load()
+            if config:
+                return self._dataset[config].info
+            return self._dataset.info
+
+
+@lru_cache
+def _get_hf_dataset_info(
+    repo_id: str, config: Union[str, None] = None
+) -> Dict[str, Any]:
+    """Calls the Datasets Server API from Hugging Face to obtain the dataset information.
+    The results are cached to avoid making multiple requests to the server.
+
+    Args:
+        repo_id: The Hugging Face Hub repository ID of the dataset.
+        config: The configuration of the dataset. This is optional and only needed if the
+            dataset has multiple configurations.
+
+    Returns:
+        The dataset information.
+    """
+
+    params = {"dataset": repo_id}
+    if config is not None:
+        params["config"] = config
+
+    if "HF_TOKEN" in os.environ:
+        headers = {"Authorization": f"Bearer {os.environ['HF_TOKEN']}"}
+    else:
+        headers = None
+
+    response = requests.get(
+        "https://datasets-server.huggingface.co/info", params=params, headers=headers
+    )
+
+    assert (
+        response.status_code == 200
+    ), f"Failed to get '{repo_id}' dataset info. Make sure you have set the HF_TOKEN environment variable if it is a private dataset."
+
+    return response.json()["dataset_info"]
```

### Comparing `distilabel-1.0.3/src/distilabel/steps/globals/__init__.py` & `distilabel-1.1.0/src/distilabel/steps/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/steps/globals/huggingface.py` & `distilabel-1.1.0/src/distilabel/steps/globals/huggingface.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 from distilabel.steps.base import GlobalStep, StepInput
 
 if TYPE_CHECKING:
     from distilabel.steps.typing import StepOutput
 
 
 class PushToHub(GlobalStep):
-    """A `GlobalStep` which creates a `datasets.Dataset` with the input data and pushes
+    """Push data to a Hugging Face Hub dataset.
+
+    A `GlobalStep` which creates a `datasets.Dataset` with the input data and pushes
     it to the Hugging Face Hub.
 
     Attributes:
         repo_id: The Hugging Face Hub repository ID where the dataset will be uploaded.
         split: The split of the dataset that will be pushed. Defaults to `"train"`.
         private: Whether the dataset to be pushed should be private or not. Defaults to
             `False`.
@@ -44,15 +46,20 @@
     Runtime parameters:
         - `repo_id`: The Hugging Face Hub repository ID where the dataset will be uploaded.
         - `split`: The split of the dataset that will be pushed.
         - `private`: Whether the dataset to be pushed should be private or not.
         - `token`: The token that will be used to authenticate in the Hub.
 
     Input columns:
-        - dynamic, based on the existing data within inputs
+        - dynamic (`all`): all columns from the input will be used to create the dataset.
+
+    Categories:
+        - save
+        - dataset
+        - huggingface
     """
 
     repo_id: RuntimeParameter[str] = Field(
         default=None,
         description="The Hugging Face Hub repository ID where the dataset will be uploaded.",
     )
     split: RuntimeParameter[str] = Field(
```

### Comparing `distilabel-1.0.3/src/distilabel/steps/tasks/__init__.py` & `distilabel-1.1.0/src/distilabel/steps/tasks/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,36 +18,41 @@
 from distilabel.steps.tasks.evol_instruct.evol_complexity.base import EvolComplexity
 from distilabel.steps.tasks.evol_instruct.evol_complexity.generator import (
     EvolComplexityGenerator,
 )
 from distilabel.steps.tasks.evol_instruct.generator import EvolInstructGenerator
 from distilabel.steps.tasks.evol_quality.base import EvolQuality
 from distilabel.steps.tasks.generate_embeddings import GenerateEmbeddings
+from distilabel.steps.tasks.genstruct import Genstruct
 from distilabel.steps.tasks.instruction_backtranslation import (
     InstructionBacktranslation,
 )
 from distilabel.steps.tasks.pair_rm import PairRM
+from distilabel.steps.tasks.prometheus_eval import PrometheusEval
 from distilabel.steps.tasks.quality_scorer import QualityScorer
 from distilabel.steps.tasks.self_instruct import SelfInstruct
-from distilabel.steps.tasks.text_generation import TextGeneration
+from distilabel.steps.tasks.text_generation import ChatGeneration, TextGeneration
 from distilabel.steps.tasks.typing import ChatItem, ChatType
 from distilabel.steps.tasks.ultrafeedback import UltraFeedback
 
 __all__ = [
     "Task",
     "GeneratorTask",
+    "ChatGeneration",
     "ChatItem",
     "ChatType",
     "ComplexityScorer",
     "EvolInstruct",
     "EvolComplexity",
     "EvolComplexityGenerator",
     "EvolInstructGenerator",
     "EvolQuality",
     "GenerateEmbeddings",
+    "Genstruct",
     "InstructionBacktranslation",
     "PairRM",
+    "PrometheusEval",
     "QualityScorer",
     "SelfInstruct",
     "TextGeneration",
     "UltraFeedback",
 ]
```

### Comparing `distilabel-1.0.3/src/distilabel/steps/tasks/base.py` & `distilabel-1.1.0/src/distilabel/steps/tasks/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,29 +29,36 @@
 
 if TYPE_CHECKING:
     from distilabel.llms.typing import GenerateOutput
     from distilabel.steps.tasks.typing import ChatType
     from distilabel.steps.typing import StepOutput
 
 
+DISTILABEL_METADATA_KEY = "distilabel_metadata"
+
+
 class _Task(_Step, ABC):
     """_Task is an abstract class that implements the `_Step` interface and adds the
     `format_input` and `format_output` methods to format the inputs and outputs of the
     task. It also adds a `llm` attribute to be used as the LLM to generate the outputs.
 
-    Args:
+    Attributes:
         llm: the `LLM` to be used to generate the outputs of the task.
         group_generations: whether to group the `num_generations` generated per input in
             a list or create a row per generation. Defaults to `False`.
+        add_raw_output: whether to include a field with the raw output of the LLM in the
+            `distilabel_metadata` field of the output. Can be helpful to not loose data
+            with `Tasks` that need to format the output of the `LLM`. Defaults to `False`.
         num_generations: The number of generations to be produced per input.
     """
 
     llm: LLM
 
     group_generations: bool = False
+    add_raw_output: bool = False
     num_generations: RuntimeParameter[int] = Field(
         default=1, description="The number of generations to be produced per input."
     )
 
     def load(self) -> None:
         """Loads the LLM via the `LLM.load()` method (done for safer serialization)."""
         super().load()
@@ -81,25 +88,52 @@
 
         Returns:
             A list containing a dictionary with the outputs of the task for each input.
         """
         formatted_outputs = []
         for output, input in zip(outputs, inputs * len(outputs)):
             try:
-                formatted_outputs.append(self.format_output(output, input))
+                formatted_output = self.format_output(output, input)
+                formatted_output = self._maybe_add_raw_output(
+                    formatted_output, output, add_raw_output=self.add_raw_output
+                )
+                formatted_outputs.append(formatted_output)
             except Exception as e:
                 self._logger.warning(  # type: ignore
-                    f"Task '{self.name}' failed to format output: {e}. Using empty dict."  # type: ignore
+                    f"Task '{self.name}' failed to format output: {e}. Saving raw response."  # type: ignore
                 )
-                formatted_outputs.append(self._outputs_empty_dict())
+                formatted_outputs.append(self._output_on_failure(output, input))
         return formatted_outputs
 
-    def _outputs_empty_dict(self) -> Dict[str, None]:
-        """Returns a dictionary with the outputs of the task set to `None`."""
-        return {output: None for output in self.outputs}  # type: ignore
+    def _output_on_failure(
+        self, output: Union[str, None], input: Dict[str, Any]
+    ) -> Dict[str, Any]:
+        """In case of failure to format the output, this method will return a dictionary including
+        a new field `distilabel_meta` with the raw output of the LLM.
+        """
+        # Create a dictionary with the outputs of the task (every output set to None)
+        outputs = {output: None for output in self.outputs}
+        outputs["model_name"] = self.llm.model_name
+        outputs = self._maybe_add_raw_output(
+            outputs, output, add_raw_output=self.add_raw_output
+        )
+        return outputs
+
+    def _maybe_add_raw_output(
+        self,
+        output: Dict[str, Any],
+        raw_output: Union[str, None],
+        add_raw_output: bool = True,
+    ) -> Dict[str, Any]:
+        """Adds the raw output of the LLM to the output dictionary if `add_raw_output` is True."""
+        if add_raw_output:
+            meta = output.get(DISTILABEL_METADATA_KEY, {})
+            meta[f"raw_output_{self.name}"] = raw_output
+            output[DISTILABEL_METADATA_KEY] = meta
+        return output
 
 
 class Task(_Task, Step):
     """Task is a class that implements the `_Task` abstract class and adds the `Step`
     interface to be used as a step in the pipeline.
 
     Attributes:
```

### Comparing `distilabel-1.0.3/src/distilabel/steps/tasks/complexity_scorer.py` & `distilabel-1.1.0/src/distilabel/steps/tasks/complexity_scorer.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,83 +9,116 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import re
+import sys
+
+if sys.version_info < (3, 9):
+    import importlib_resources
+else:
+    import importlib.resources as importlib_resources
+
 from typing import TYPE_CHECKING, Any, Dict, List, Union
 
 from jinja2 import Template
 from pydantic import PrivateAttr
 
 from distilabel.steps.tasks.base import Task
 
 if TYPE_CHECKING:
     from distilabel.steps.tasks.typing import ChatType
 
-_COMPLEXITY_SCORER_TEMPLATE = """
-Ranking the following questions according to the difficulty and complexity. Score 1-{{ instructions|length }}.
-You can give a score of {{ (instructions|length) + 1 }} if the question is too complex for you to answer it. You should
-respond with the format:
-[1] Score: 1
-[2] Score: 2
-...
-{% for instruction in instructions %}
-[{{ loop.index }}] {{ instruction }}
-{%- endfor %}
-""".lstrip()
 
 _PARSE_SCORE_LINE_REGEX = re.compile(r"\[\d+\] score: (\d+)", re.IGNORECASE)
 
 
 class ComplexityScorer(Task):
-    """This task is used to rank a list of instructions based on their complexity. It's
-    an implementation of the complexity score task from the paper 'What Makes Good Data
-    for Alignment? A Comprehensive Study of Automatic Data Selection in Instruction Tuning'.
+    """Score instructions based on their complexity using an `LLM`.
+
+    `ComplexityScorer` is a pre-defined task used to rank a list of instructions based in
+    their complexity. It's an implementation of the complexity score task from the paper
+    'What Makes Good Data for Alignment? A Comprehensive Study of Automatic Data Selection
+    in Instruction Tuning'.
 
     Attributes:
-        _template: The Jinja2 template used to format the input data.
+        _template: a Jinja2 template used to format the input for the LLM.
 
     Input columns:
         - instructions (`List[str]`): The list of instructions to be scored.
 
     Output columns:
-        - complexity_score (`List[float]`): The complexity score for each instruction.
+        - scores (`List[float]`): The score for each instruction.
+        - model_name (`str`): The model name used to generate the scores.
+
+    Categories:
+        - scorer
+        - complexity
+        - instruction
 
     References:
         - [`What Makes Good Data for Alignment? A Comprehensive Study of Automatic Data Selection in Instruction Tuning`](https://arxiv.org/abs/2312.15685)
     """
 
     _template: Union[Template, None] = PrivateAttr(...)
 
     def load(self) -> None:
+        """Loads the Jinja2 template."""
         super().load()
-        self._template = Template(_COMPLEXITY_SCORER_TEMPLATE)
+
+        _path = str(
+            importlib_resources.files("distilabel")
+            / "steps"
+            / "tasks"
+            / "templates"
+            / "complexity-scorer.jinja2"
+        )
+
+        self._template = Template(open(_path).read())
 
     @property
     def inputs(self) -> List[str]:
+        """The inputs for the task are the `instructions`."""
         return ["instructions"]
 
+    def format_input(self, input: Dict[str, Any]) -> "ChatType":
+        """The input is formatted as a `ChatType` assuming that the instruction
+        is the first interaction from the user within a conversation."""
+        return [
+            {
+                "role": "user",
+                "content": self._template.render(instructions=input["instructions"]),  # type: ignore
+            }
+        ]
+
     @property
     def outputs(self) -> List[str]:
-        return ["scores"]
-
-    def format_input(self, input: Dict[str, Any]) -> "ChatType":
-        return [{"role": "user", "content": self._template.render(**input)}]  # type: ignore
+        """The output for the task are: a list of `scores` containing the complexity score for each
+        instruction in `instructions`, and the `model_name`."""
+        return ["scores", "model_name"]
 
     def format_output(
         self, output: Union[str, None], input: Dict[str, Any]
     ) -> Dict[str, Any]:
+        """The output is formatted as a list with the score of each instruction.
+
+        Args:
+            output: the raw output of the LLM.
+            input: the input to the task. Used for obtaining the number of responses.
+
+        Returns:
+            A dict with the key `scores` containing the scores for each instruction.
+        """
         if output is None:
             return {"scores": [None] * len(input["instructions"])}
 
         scores = []
         score_lines = output.split("\n")
         for i, line in enumerate(score_lines):
             match = _PARSE_SCORE_LINE_REGEX.match(line)
             score = float(match.group(1)) if match else None
             scores.append(score)
             if i == len(input["instructions"]) - 1:
                 break
-
         return {"scores": scores}
```

### Comparing `distilabel-1.0.3/src/distilabel/steps/tasks/generate_embeddings.py` & `distilabel-1.1.0/src/distilabel/steps/tasks/generate_embeddings.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,50 +20,58 @@
 
 if TYPE_CHECKING:
     from distilabel.steps.tasks.typing import ChatType
     from distilabel.steps.typing import StepOutput
 
 
 class GenerateEmbeddings(Step):
-    """Generate embeddings for a text input using the last hidden state of an `LLM`, as
+    """Generate embeddings using the last hidden state of an `LLM`.
+
+    Generate embeddings for a text input using the last hidden state of an `LLM`, as
     described in the paper 'What Makes Good Data for Alignment? A Comprehensive Study of
     Automatic Data Selection in Instruction Tuning'.
 
     Attributes:
         llm: The `LLM` to use to generate the embeddings.
 
     Input columns:
         - text (`str`, `List[Dict[str, str]]`): The input text or conversation to generate
             embeddings for.
 
     Output columns:
         - embedding (`List[float]`): The embedding of the input text or conversation.
+        - model_name (`str`): The model name used to generate the embeddings.
+
+    Categories:
+        - embedding
+        - llm
 
     References:
         - [What Makes Good Data for Alignment? A Comprehensive Study of Automatic Data Selection in Instruction Tuning](https://arxiv.org/abs/2312.15685)
     """
 
     llm: LLM
 
     def load(self) -> None:
         """Loads the `LLM` used to generate the embeddings."""
         super().load()
+
         self.llm.load()
 
     @property
     def inputs(self) -> List[str]:
         """The inputs for the task is a `text` column containing either a string or a
         list of dictionaries in OpenAI chat-like format."""
         return ["text"]
 
     @property
     def outputs(self) -> List[str]:
         """The outputs for the task is an `embedding` column containing the embedding of
         the `text` input."""
-        return ["embedding"]
+        return ["embedding", "model_name"]
 
     def format_input(self, input: Dict[str, Any]) -> "ChatType":
         """Formats the input to be used by the LLM to generate the embeddings. The input
         can be in `ChatType` format or a string. If a string, it will be converted to a
         list of dictionaries in OpenAI chat-like format.
 
         Args:
@@ -95,8 +103,9 @@
         Yields:
             A list of Python dictionaries with the outputs of the task.
         """
         formatted_inputs = [self.format_input(input) for input in inputs]
         last_hidden_states = self.llm.get_last_hidden_states(formatted_inputs)
         for input, hidden_state in zip(inputs, last_hidden_states):
             input["embedding"] = hidden_state[-1].tolist()
+            input["model_name"] = self.llm.model_name
         yield inputs
```

### Comparing `distilabel-1.0.3/src/distilabel/steps/tasks/instruction_backtranslation.py` & `distilabel-1.1.0/src/distilabel/steps/tasks/instruction_backtranslation.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,23 +37,28 @@
 
     Input columns:
         - instruction (`str`): The reference instruction to evaluate the text output.
         - generation (`str`): The text output to evaluate for the given instruction.
 
     Output columns:
         - score (`str`): The score for the generation based on the given instruction.
+        - reason (`str`): The reason for the provided score.
+        - model_name (`str`): The model name used to score the generation.
+
+    Categories:
+        - critique
 
     References:
         - [`Self-Alignment with Instruction Backtranslation`](https://arxiv.org/abs/2308.06259)
     """
 
     _template: Optional["Template"] = PrivateAttr(default=...)
 
     def load(self) -> None:
-        """Loads the Jinja2 template with the Instruction Backtranslation prompt."""
+        """Loads the Jinja2 template."""
         super().load()
 
         _path = str(
             importlib_resources.files("distilabel")
             / "steps"
             / "tasks"
             / "templates"
```

### Comparing `distilabel-1.0.3/src/distilabel/steps/tasks/pair_rm.py` & `distilabel-1.1.0/src/distilabel/steps/tasks/pair_rm.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,79 +24,84 @@
 
 
 class PairRM(Step):
     """Rank the candidates based on the input using the `LLM` model.
 
     Attributes:
         model: The model to use for the ranking. Defaults to `"llm-blender/PairRM"`.
-        input_batch_size: The batch size to use when processing the input. Defaults to `8`.
         instructions: The instructions to use for the model. Defaults to `None`.
 
     Input columns:
         - inputs (`List[Dict[str, Any]]`): The input text or conversation to rank the candidates for.
         - candidates (`List[Dict[str, Any]]`): The candidates to rank.
 
     Output columns:
         - ranks (`List[int]`): The ranks of the candidates based on the input.
         - ranked_candidates (`List[Dict[str, Any]]`): The candidates ranked based on the input.
+        - model_name (`str`): The model name used to rank the candidate responses. Defaults to `"llm-blender/PairRM"`.
 
     References:
         - [LLM-Blender: Ensembling Large Language Models with Pairwise Ranking and Generative Fusion](https://arxiv.org/abs/2306.02561).
         - [Pair Ranking Model](https://huggingface.co/llm-blender/PairRM).
 
+    Categories:
+        - preference
+
     Note:
         This step differs to other tasks as there is a single implementation of this model
         currently, and we will use a specific `LLM`.
     """
 
     model: str = "llm-blender/PairRM"
-    input_batch_size: int = 8
     instructions: Optional[str] = None
 
     def load(self) -> None:
+        """Loads the PairRM model provided via `model` with `llm_blender.Blender`, which is the
+        custom library for running the inference for the PairRM models."""
         try:
             import llm_blender
         except ImportError as e:
             raise ImportError(
                 "The `llm_blender` package is required to use the `PairRM` class."
                 "Please install it with `pip install git+https://github.com/yuchenlin/LLM-Blender.git`."
             ) from e
+
         self._blender = llm_blender.Blender()
         self._blender.loadranker(self.model)
 
     @property
     def inputs(self) -> List[str]:
         """The input columns correspond to the two required arguments from `Blender.rank`:
         `inputs` and `candidates`."""
         return ["input", "candidates"]
 
     @property
     def outputs(self) -> List[str]:
         """The outputs will include the `ranks` and the `ranked_candidates`."""
-        return ["ranks", "ranked_candidates"]
+        return ["ranks", "ranked_candidates", "model_name"]
 
     def format_input(self, input: Dict[str, Any]) -> Dict[str, Any]:
         """The input is expected to be a dictionary with the keys `input` and `candidates`,
         where the `input` corresponds to the instruction of a model and `candidates` are a
         list of responses to be ranked.
         """
-        return input
+        return {"input": input["input"], "candidates": input["candidates"]}
 
     def process(self, inputs: StepInput) -> "StepOutput":  # type: ignore
         """Generates the ranks for the candidates based on the input.
 
         The ranks are the positions of the candidates, where lower is better,
         and the ranked candidates correspond to the candidates sorted according to the
         ranks obtained.
 
         Args:
             inputs: A list of Python dictionaries with the inputs of the task.
 
         Yields:
-            An iterator with the inputs containing the `ranks` and the `ranked_candidates`.
+            An iterator with the inputs containing the `ranks`, `ranked_candidates`, and `model_name`.
         """
         input_texts = []
         candidates = []
         for input in inputs:
             formatted_input = self.format_input(input)
             input_texts.append(formatted_input["input"])
             candidates.append(formatted_input["candidates"])
@@ -116,9 +121,10 @@
         ranked_candidates = np.take_along_axis(
             np.array(candidates), ranks - 1, axis=1
         ).tolist()
         ranks = ranks.tolist()
         for input, rank, ranked_candidate in zip(inputs, ranks, ranked_candidates):
             input["ranks"] = rank
             input["ranked_candidates"] = ranked_candidate
+            input["model_name"] = self.model
 
         yield inputs
```

### Comparing `distilabel-1.0.3/src/distilabel/steps/tasks/quality_scorer.py` & `distilabel-1.1.0/src/distilabel/steps/tasks/quality_scorer.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,102 +9,119 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import re
+import sys
+
+if sys.version_info < (3, 9):
+    import importlib_resources
+else:
+    import importlib.resources as importlib_resources
+
 from typing import Any, Dict, List, Union
 
 from jinja2 import Template
 from pydantic import PrivateAttr
 
 from distilabel.steps.tasks.base import Task
 from distilabel.steps.tasks.typing import ChatType
 
-_QUALITY_SCORER_TEMPLATE = """
-Rank the following pair of instructions and responses according to their quality. Your evaluation should consider factors such as helpfulness, relevance, accuracy, depth, creativity, and level of detail of the response. Score 1-{{ responses|length }}.
-Score each response from 1 to {{ responses|length }}, with {{ (responses|length) + 1}} reserved for responses that are already very well written and cannot be improved further. You should respond with the format:
-[1] Score: 1
-[2] Score: 2
-...
-#Question#: {{ instruction }}
-#Response List#:
-{% for response in responses %}
-[{{ loop.index }}] {{ response }}
-{%- endfor %}
-""".lstrip()
-
 _PARSE_SCORE_LINE_REGEX = re.compile(r"\[\d+\] score: (\d+)", re.IGNORECASE)
 
 
 class QualityScorer(Task):
-    """QualityScorer is a pre-defined task that defines the `instruction` as the input
+    """Score responses based on their quality using an `LLM`.
+
+    `QualityScorer` is a pre-defined task that defines the `instruction` as the input
     and `score` as the output. This task is used to rate the quality of instructions and responses.
     It's an implementation of the quality score task from the paper 'What Makes Good Data
     for Alignment? A Comprehensive Study of Automatic Data Selection in Instruction Tuning'.
     The task follows the same scheme as the Complexity Scorer, but the instruction-response pairs
     are scored in terms of quality, obtaining a quality score for each instruction.
 
     Attributes:
         _template: a Jinja2 template used to format the input for the LLM.
 
     Input columns:
         - instruction (`str`): The instruction that was used to generate the `responses`.
         - responses (`List[str]`): The responses to be scored. Each response forms a pair with the instruction.
 
     Output columns:
-        - quality_score (`List[float]`): The quality score for each instruction.
+        - scores (`List[float]`): The score for each instruction.
+        - model_name (`str`): The model name used to generate the scores.
+
+    Categories:
+        - scorer
+        - quality
+        - response
 
     References:
         - [`What Makes Good Data for Alignment? A Comprehensive Study of Automatic Data Selection in Instruction Tuning`](https://arxiv.org/abs/2312.15685)
     """
 
     _template: Union[Template, None] = PrivateAttr(...)
 
     def load(self) -> None:
+        """Loads the Jinja2 template."""
         super().load()
-        self._template = Template(_QUALITY_SCORER_TEMPLATE)
+
+        _path = str(
+            importlib_resources.files("distilabel")
+            / "steps"
+            / "tasks"
+            / "templates"
+            / "quality-scorer.jinja2"
+        )
+
+        self._template = Template(open(_path).read())
 
     @property
     def inputs(self) -> List[str]:
-        """The input for the task are `instruction` and `responses`."""
+        """The inputs for the task are `instruction` and `responses`."""
         return ["instruction", "responses"]
 
     def format_input(self, input: Dict[str, Any]) -> ChatType:  # type: ignore
         """The input is formatted as a `ChatType` assuming that the instruction
         is the first interaction from the user within a conversation."""
-        return [{"role": "user", "content": self._template.render(**input)}]  # type: ignore
+        return [
+            {
+                "role": "user",
+                "content": self._template.render(  # type: ignore
+                    instruction=input["instruction"], responses=input["responses"]
+                ),
+            }
+        ]
 
     @property
     def outputs(self):
-        """The output for the task is a list of `quality_scores` containing the quality score for each
+        """The output for the task is a list of `scores` containing the quality score for each
         response in `responses`."""
-        return ["scores"]
+        return ["scores", "model_name"]
 
     def format_output(
         self, output: Union[str, None], input: Dict[str, Any]
     ) -> Dict[str, Any]:
         """The output is formatted as a list with the score of each instruction-response pair.
 
         Args:
             output: the raw output of the LLM.
             input: the input to the task. Used for obtaining the number of responses.
 
         Returns:
-            A dict with containing the scores for each instruction-response pair.
+            A dict with the key `scores` containing the scores for each instruction-response pair.
         """
-
         if output is None:
-            return {self.outputs[0]: [None] * len(input["responses"])}
+            return {"scores": [None] * len(input["responses"])}
 
         scores = []
         score_lines = output.split("\n")
 
         for i, line in enumerate(score_lines):
             match = _PARSE_SCORE_LINE_REGEX.match(line)
             score = float(match.group(1)) if match else None
             scores.append(score)
             if i == len(input["responses"]) - 1:
                 break
-
-        return {self.outputs[0]: scores}
+        return {"scores": scores}
```

### Comparing `distilabel-1.0.3/src/distilabel/steps/tasks/text_generation.py` & `distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,60 +8,59 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Any, Dict, List, Union
+from typing import Dict
 
-from distilabel.steps.tasks.base import Task
-from distilabel.steps.tasks.typing import ChatType
-from distilabel.utils.chat import is_openai_format
-
-
-class TextGeneration(Task):
-    """TextGeneration is a pre-defined task that defines the `instruction` as the input
-    and `generation` as the output. This task is used to generate text based on the input
-    instruction. The model_name is also returned as part of the output in order to enhance it.
+from distilabel.steps.tasks.evol_instruct.base import EvolInstruct
+from distilabel.steps.tasks.evol_instruct.evol_complexity.utils import (
+    MUTATION_TEMPLATES,
+)
+
+
+class EvolComplexity(EvolInstruct):
+    """Evolve instructions to make them more complex using an `LLM`.
+
+    `EvolComplexity` is a task that evolves instructions to make them more complex,
+    and it is based in the EvolInstruct task, but using slight different prompts, but the
+    exact same evolutionary approach.
+
+    Attributes:
+        num_instructions: The number of instructions to be generated.
+        generate_answers: Whether to generate answers for the instructions or not. Defaults
+            to `False`.
+        mutation_templates: The mutation templates to be used for the generation of the
+            instructions.
+        min_length: Defines the length (in bytes) that the generated instruction needs to
+            be higher than, to be considered valid. Defaults to `512`.
+        max_length: Defines the length (in bytes) that the generated instruction needs to
+            be lower than, to be considered valid. Defaults to `1024`.
+        seed: The seed to be set for `numpy` in order to randomly pick a mutation method.
+            Defaults to `42`.
+
+    Runtime parameters:
+        - `min_length`: Defines the length (in bytes) that the generated instruction needs to be higher than, to be considered valid.
+        - `max_length`: Defines the length (in bytes) that the generated instruction needs to be lower than, to be considered valid.
+        - `seed`: The number of evolutions to be run.
 
     Input columns:
-        - instruction (`str`): The instruction to generate text from.
+        - instruction (`str`): The instruction to evolve.
 
     Output columns:
-        - generation (`str`): The generated text.
-        - model_name (`str`): The model name used to generate the text.
+        - evolved_instruction (`str`): The evolved instruction.
+        - answer (`str`, optional): The answer to the instruction if `generate_answers=True`.
+        - model_name (`str`): The name of the LLM used to evolve the instructions.
+
+    Categories:
+        - evol
+        - instruction
+        - deita
+
+    References:
+        - [What Makes Good Data for Alignment? A Comprehensive Study of Automatic Data Selection in Instruction Tuning](https://arxiv.org/abs/2312.15685)
+        - [WizardLM: Empowering Large Language Models to Follow Complex Instructions](https://arxiv.org/abs/2304.12244)
     """
 
-    @property
-    def inputs(self) -> List[str]:
-        """The input for the task is the `instruction`."""
-        return ["instruction"]
-
-    def format_input(self, input: Dict[str, Any]) -> ChatType:
-        """The input is formatted as a `ChatType` assuming that the instruction
-        is the first interaction from the user within a conversation."""
-
-        instruction = input["instruction"]
-
-        if isinstance(instruction, str):
-            return [{"role": "user", "content": input["instruction"]}]
-
-        if not is_openai_format(instruction):
-            raise ValueError(
-                f"Input `instruction` must be a string or an OpenAI chat-like format. "
-                f"Got: {instruction}. Please check: 'https://cookbook.openai.com/examples/how_to_format_inputs_to_chatgpt_models'."
-            )
-
-        return instruction
-
-    @property
-    def outputs(self) -> List[str]:
-        """The output for the task is the `generation` and the `model_name`."""
-        return ["generation", "model_name"]
-
-    def format_output(
-        self, output: Union[str, None], input: Dict[str, Any]
-    ) -> Dict[str, Any]:
-        """The output is formatted as a dictionary with the `generation`. The `model_name`
-        will be automatically included within the `process` method of `Task`."""
-        return {"generation": output}
+    mutation_templates: Dict[str, str] = MUTATION_TEMPLATES
```

### Comparing `distilabel-1.0.3/src/distilabel/steps/tasks/typing.py` & `distilabel-1.1.0/src/distilabel/steps/tasks/typing.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/steps/tasks/ultrafeedback.py` & `distilabel-1.1.0/src/distilabel/utils/serialization.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,225 +8,314 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import re
+import importlib
+import json
+import os
 import sys
+from enum import Enum
 
-from distilabel.utils.dicts import combine_dicts
-
-if sys.version_info < (3, 9):
-    import importlib_resources
+if sys.version_info < (3, 11):
+    from enum import EnumMeta as EnumType
 else:
-    import importlib.resources as importlib_resources
+    from enum import EnumType
 
-from typing import Any, Dict, List, Literal, Optional, Union
+from pathlib import Path
+from typing import Any, Dict, List, Literal, Optional, Type, TypeVar, Union, get_args
 
-from jinja2 import Template
-from pydantic import PrivateAttr
+import yaml
+from pydantic import BaseModel
+from typing_extensions import Self
 
-from distilabel.steps.tasks.base import Task
-from distilabel.steps.tasks.typing import ChatType
-
-
-class UltraFeedback(Task):
-    """UltraFeedback: Boosting Language Models with High-quality Feedback.
-
-    Attributes:
-        aspect: The aspect to perform with the `UltraFeedback` model. The available aspects are:
-            - `helpfulness`: Evaluate text outputs based on helpfulness.
-            - `honesty`: Evaluate text outputs based on honesty.
-            - `instruction-following`: Evaluate text outputs based on given instructions.
-            - `truthfulness`: Evaluate text outputs based on truthfulness.
-            Additionally, a custom aspect has been defined by Argilla, so as to evaluate the overall
-            assessment of the text outputs within a single prompt. The custom aspect is:
-            - `overall-rating`: Evaluate text outputs based on an overall assessment.
-
-    Input columns:
-        - instruction (`str`): The reference instruction to evaluate the text outputs.
-        - generations (`List[str]`): The text outputs to evaluate for the given instruction.
-
-    Output columns:
-        - ratings (`List[float]`): The ratings for each of the provided text outputs.
-        - rationales (`List[str]`): The rationales for each of the provided text outputs.
-        - model_name (`str`): The name of the model used to generate the ratings and rationales.
-
-    References:
-        - [`UltraFeedback: Boosting Language Models with High-quality Feedback`](https://arxiv.org/abs/2310.01377)
-        - [`UltraFeedback - GitHub Repository`](https://github.com/OpenBMB/UltraFeedback)
-    """
-
-    aspect: Literal[
-        "helpfulness",
-        "honesty",
-        "instruction-following",
-        "truthfulness",
-        # Custom aspects
-        "overall-rating",
-    ]
-
-    _system_prompt: str = PrivateAttr(
-        default=(
-            "Your role is to evaluate text quality based on given criteria.\n"
-            'You\'ll receive an instructional description ("Instruction") and {no_texts} text outputs ("Text").\n'
-            "Understand and interpret instructions to evaluate effectively.\n"
-            "Provide annotations for each text with a rating and rationale.\n"
-            "The {no_texts} texts given are independent, and should be evaluated separately.\n"
-        )
-    )
-    _template: Optional["Template"] = PrivateAttr(default=...)
+T = TypeVar("T")
 
-    def load(self) -> None:
-        """Loads the Jinja2 template for the given `aspect`."""
-        super().load()
-
-        _path = str(
-            importlib_resources.files("distilabel")
-            / "steps"
-            / "tasks"
-            / "templates"
-            / "ultrafeedback"
-            / f"{self.aspect}.jinja2"
-        )
+DISTILABEL_FILENAME = "distilabel-file.json"
+TYPE_INFO_KEY = "type_info"
 
-        self._template = Template(open(_path).read())
 
-    @property
-    def inputs(self) -> List[str]:
-        """The input for the task is the `instruction`, and the `generations` for it."""
-        return ["instruction", "generations"]
-
-    def format_input(self, input: Dict[str, Any]) -> ChatType:
-        """The input is formatted as a `ChatType` assuming that the instruction
-        is the first interaction from the user within a conversation."""
-        return [
-            {
-                "role": "system",
-                "content": self._system_prompt.format(
-                    no_texts=len(input["generations"])
-                ),
-            },
-            {
-                "role": "user",
-                "content": self._template.render(  # type: ignore
-                    instruction=input["instruction"], generations=input["generations"]
-                ),
-            },
-        ]
-
-    @property
-    def outputs(self) -> List[str]:
-        """The output for the task is the `generation` and the `model_name`."""
-        columns = []
-        if self.aspect in ["honesty", "instruction-following", "overall-rating"]:
-            columns = ["ratings", "rationales"]
-        elif self.aspect in ["helpfulness", "truthfulness"]:
-            columns = ["types", "rationales", "ratings", "rationales-for-ratings"]
-        return columns + ["model_name"]
-
-    def format_output(
-        self, output: Union[str, None], input: Dict[str, Any]
-    ) -> Dict[str, Any]:
-        """The output is formatted as a dictionary with the `ratings` and `rationales` for
-        each of the provided `generations` for the given `instruction`. The `model_name`
-        will be automatically included within the `process` method of `Task`.
-
-        Args:
-            output: a string representing the output of the LLM via the `process` method.
-            input: the input to the task, as required by some tasks to format the output.
-
-        Returns:
-            A dictionary containing either the `ratings` and `rationales` for each of the provided
-            `generations` for the given `instruction` if the provided aspect is either `honesty`,
-            `instruction-following`, or `overall-rating`; or the `types`, `rationales`,
-            `ratings`, and `rationales-for-ratings` for each of the provided `generations` for the
-            given `instruction` if the provided aspect is either `helpfulness` or `truthfulness`.
-        """
-        if self.aspect in [
-            "honesty",
-            "instruction-following",
-            "overall-rating",
-        ]:
-            return self._format_ratings_rationales_output(output, input)
-        else:
-            return self._format_types_ratings_rationales_output(output, input)
+StrOrPath = Union[str, os.PathLike]
+SaveFormats = Literal["json", "yaml"]
+
+
+def _get_module_attr(module: str, name: str) -> Type:
+    """Gets a class given the module and the name of the class.
+
+    Returns:
+        The type of the class.
+    """
+    mod = importlib.import_module(module)
+    return getattr(mod, name)
+
+
+def load_from_dict(class_: Dict[str, Any]) -> Any:
+    """Creates an instance of a class from a dictionary containing the type info and the
+    serialized data of the class.
+
+    Args:
+        class_: dictionary containing the type info and the serialized data of the class.
+
+    Returns:
+        An instance of the class with the data loaded from the dictionary.
+    """
+    type_info = class_.pop(TYPE_INFO_KEY)
+    if TYPE_INFO_KEY in type_info:
+        # There is a nested type_info, load the class recursively
+        type_info = load_from_dict(type_info)
+
+    cls = _get_module_attr(type_info["module"], type_info["name"])
+
+    for k, v in class_.items():
+        if isinstance(v, dict) and "_type" in v and v["_type"] == "enum":
+            class_[k] = Enum(v["_name"], v["_values"], type=eval(v["_enum_type"]))
+
+    instance = cls(**class_)
+    return instance
+
+
+def write_json(filename: Path, data: Any) -> None:
+    """Writes a JSON file to the given path, creating the parent dir if needed.
+
+    Args:
+        filename: the path to the file.
+        data: the data to write to the file.
+    """
+    filename.parent.mkdir(parents=True, exist_ok=True)
+    with open(filename, "w") as file:
+        json.dump(data, file, indent=2)
 
-    def _format_ratings_rationales_output(
-        self, output: Union[str, None], input: Dict[str, Any]
-    ) -> Dict[str, List[Any]]:
-        """Formats the output when the aspect is either `honesty`, `instruction-following`, or `overall-rating`."""
-        if output is None:
-            return {
-                "ratings": [None] * len(input["generations"]),
-                "rationales": [None] * len(input["generations"]),
-            }
-
-        pattern = r"Rating: (.+?)\nRationale: (.+)"
-        sections = output.split("\n\n")
-
-        formatted_outputs = []
-        for section in sections:
-            matches = None
-            if section is not None and section != "":
-                matches = re.search(pattern, section, re.DOTALL)
-            if not matches:
-                formatted_outputs.append({"ratings": None, "rationales": None})
-                continue
-
-            formatted_outputs.append(
-                {
-                    "ratings": int(re.findall(r"\b\d+\b", matches.group(1))[0])
-                    if matches.group(1) not in ["None", "N/A"]
-                    else None,
-                    "rationales": matches.group(2),
-                }
-            )
-        return combine_dicts(*formatted_outputs)
 
-    def _format_types_ratings_rationales_output(
-        self, output: Union[str, None], input: Dict[str, Any]
-    ) -> Dict[str, List[Any]]:
-        """Formats the output when the aspect is either `helpfulness` or `truthfulness`."""
-        if output is None:
-            return {
-                "types": [None] * len(input["generations"]),
-                "rationales": [None] * len(input["generations"]),
-                "ratings": [None] * len(input["generations"]),
-                "rationales-for-ratings": [None] * len(input["generations"]),
-            }
-
-        pattern = r"Type: (.+?)\nRationale: (.+?)\nRating: (.+?)\nRationale: (.+)"
-
-        sections = output.split("\n\n")
-
-        formatted_outputs = []
-        for section in sections:
-            matches = None
-            if section is not None and section != "":
-                matches = re.search(pattern, section, re.DOTALL)
-            if not matches:
-                formatted_outputs.append(
-                    {
-                        "types": None,
-                        "rationales": None,
-                        "ratings": None,
-                        "rationales-for-ratings": None,
-                    }
-                )
-                continue
-
-            formatted_outputs.append(
-                {
-                    "types": int(re.findall(r"\b\d+\b", matches.group(1))[0])
-                    if matches.group(1) not in ["None", "N/A"]
-                    else None,
-                    "rationales": matches.group(2),
-                    "ratings": int(re.findall(r"\b\d+\b", matches.group(3))[0])
-                    if matches.group(3) not in ["None", "N/A"]
-                    else None,
-                    "rationales-for-ratings": matches.group(4),
+def read_json(filename: StrOrPath) -> Any:
+    """Reads a JSON file.
+
+    Args:
+        filename: the path to the JSON file.
+
+    Returns:
+        The data from the file.
+    """
+    with open(filename, "r") as file:
+        return json.load(file)
+
+
+def write_yaml(filename: Path, data: Dict[str, Any]) -> None:
+    """Writes a YAML file to the given path, creating the parent dir if needed.
+
+    Args:
+        filename: the path to the file.
+        data: the data to write to the file.
+    """
+    filename.parent.mkdir(parents=True, exist_ok=True)
+    with open(filename, "w") as file:
+        yaml.dump(data, file, default_flow_style=False, sort_keys=False)
+
+
+def read_yaml(filename: StrOrPath) -> Dict[str, Any]:
+    """Reads a YAML file.
+
+    Args:
+        filename: the path to the YAML file.
+
+    Returns:
+        The data from the file.
+    """
+    with open(filename, "r") as file:
+        return yaml.load(file, Loader=yaml.FullLoader)
+
+
+class _Serializable:
+    """Base class for serializable classes. It provides the means to serialize and deserialize."""
+
+    _type_info: Dict[str, Any] = {}
+
+    def _model_dump(self, obj: Any, **kwargs: Any) -> Dict[str, Any]:
+        """Method in charge of serializing the object.
+
+        This method works for `pydantic.BaseModel`s. Other classes will have to reimplement
+        this method, like the `DAG` class.
+
+        The signature must be respected, `obj` represents the object to serialize and `kwargs` are
+        the optional parameters for the method used.
+
+        Args:
+            obj: the object to be serialized.
+
+        Returns:
+            A dictionary containing the serializable content of the class.
+        """
+        # Any parameter named api_key will be excluded from the dump (those are supposed to be SecretStr anyway,
+        # and will remove them afterwards)
+        dump = obj.model_dump(exclude="api_key", **kwargs)
+
+        # Check if any attribute in value within the `dump` is an `EnumType`,
+        # as it needs a specific serialization.
+        for k, v in dump.items():
+            if isinstance(v, EnumType):
+                dump[k] = {
+                    "_type": "enum",
+                    "_enum_type": type(next(iter(v)).value).__name__,  # type: ignore
+                    "_name": getattr(obj, k).__name__,
+                    "_values": {x.name: x.value for x in v},  # type: ignore
                 }
+        # Grab the fields that need extra care (LLMs from inside tasks)
+        to_update = _extra_serializable_fields(obj)
+        # Update those in the dumped dict
+        [dump.update(field) for field in to_update]
+
+        return dump
+
+    def dump(self, **kwargs: Any) -> Dict[str, Any]:
+        """Transforms the class into a dict including the type info to be serialized.
+
+        Args:
+            kwargs: optional parameters to be used in the serialization process.
+
+        Returns:
+            A dictionary containing the serializable content of the class.
+        """
+        _dict = self._model_dump(self, **kwargs)
+
+        # Remove private variables from the dump
+        _dict = {k: v for k, v in _dict.items() if not k.startswith("_")}
+        _dict[TYPE_INFO_KEY] = {
+            "module": type(self).__module__,
+            "name": type(self).__name__,
+        }
+        return _dict
+
+    def save(
+        self,
+        path: Union[StrOrPath, None] = None,
+        format: SaveFormats = "json",
+        dump: Optional[Dict[str, Any]] = None,
+        **kwargs: Any,
+    ) -> None:
+        """Serialized the object and saves it to a file.
+
+        Args:
+            path: filename of the object to save. If a folder is given, will create the object
+                inside. If None is given, the file will be created at the current
+                working directory. Defaults to None.
+            format: the format to use when saving the file. Valid options are 'json' and
+                'yaml'. Defaults to `"json"`.
+            dump: the serialized object to save. If None, the object will be serialized using
+                the default self.dump. This variable is here to allow extra customization, in
+                general should be set as None.
+
+        Raises:
+            ValueError: if the provided `format` is not valid.
+        """
+        if path is None:
+            path = Path.cwd() / DISTILABEL_FILENAME
+        path = Path(path)
+        if path.suffix == "":
+            # If the path has no suffix, assume the user just wants a folder to write the task
+            path = path / DISTILABEL_FILENAME
+
+        if dump is None:
+            dump = self.dump(**kwargs)
+
+        if format == "json":
+            write_json(path, dump)
+        elif format == "yaml":
+            write_yaml(path, dump)
+        else:
+            raise ValueError(
+                f"Invalid format: '{format}', must be one of {get_args(SaveFormats)}."
             )
-        return combine_dicts(*formatted_outputs)
+
+    @classmethod
+    def from_dict(cls, data: Dict[str, Any]) -> Self:
+        """Creates a class from a dict containing the type info and the serialized data
+        of the class.
+
+        Args:
+            data: dictionary containing the type info and the serialized data of the class.
+
+        Returns:
+            An instance of the class with the data loaded from the dictionary.
+        """
+        return load_from_dict(data)
+
+    @classmethod
+    def from_json(cls, path: StrOrPath) -> Self:
+        """Loads a class type info and the serialized data from a JSON file and returns
+        an instance of the class.
+
+        Args:
+            path: the path to the file containing the serialized class.
+
+        Raises:
+            ValueError: if the path is a directory.
+
+        Returns:
+            An instance of the class.
+        """
+        _check_is_dir(path)
+        content = read_json(path)
+        return cls.from_dict(content)
+
+    @classmethod
+    def from_yaml(cls, path: StrOrPath) -> Self:
+        """Loads a class type info and the serialized data from a YAML file and returns
+        an instance of the class.
+
+        Args:
+            path: the path to the file containing the serialized class.
+
+        Raises:
+            ValueError: if the path is a directory.
+
+        Returns:
+            An instance of the class.
+        """
+        _check_is_dir(path)
+        content = read_yaml(path)
+        return cls.from_dict(content)
+
+    @classmethod
+    def from_file(cls, path: StrOrPath) -> Self:
+        """Loads a class from a file.
+
+        Args:
+            path: the path to the file containing the serialized class.
+
+        Returns:
+            An instance of the class.
+        """
+        path = Path(path)
+        if path.suffix == ".json":
+            return cls.from_json(path)
+
+        if path.suffix == ".yaml" or path.suffix == ".yml":
+            return cls.from_yaml(path)
+
+        raise ValueError(
+            f"Invalid file format: '{path.suffix}', must be one of {get_args(SaveFormats)}."
+        )
+
+
+def _check_is_dir(path: StrOrPath) -> None:
+    if Path(path).is_dir():
+        raise ValueError(f"You must provide a file path, not a directory: {path}")
+
+
+def _extra_serializable_fields(obj: BaseModel) -> List[Dict[str, Dict[str, Any]]]:
+    # This function is here to loop over objects that contains nested _Serializable objects.
+    # Cannot work recursively due to the mix between models that inherit from BaseModel and
+    # those that don't, so we loop over the classes and update those that are _Serializable.
+    # Extra introspection to dump nested objects.
+    # Mainly for the LLMs inside a Task for the moment.
+    # This way we ensure the "type_info" is inserted in those objects.
+    from distilabel.pipeline.base import BasePipeline
+
+    to_update = []
+    for k in obj.model_fields.keys():
+        field = getattr(obj, k)
+        # Have to remove the Pipeline as it will be inside the Step objects but is really
+        # in a higher level hierarchy.
+        if isinstance(field, _Serializable) and (not isinstance(field, BasePipeline)):
+            to_update.append({k: getattr(obj, k).dump()})
+    return to_update
```

### Comparing `distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/__init__.py` & `distilabel-1.1.0/src/distilabel/steps/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/base.py` & `distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,17 @@
 from distilabel.utils.lists import flatten_responses
 
 if TYPE_CHECKING:
     from distilabel.steps.typing import StepOutput
 
 
 class EvolInstruct(Task):
-    """WizardLM: Empowering Large Language Models to Follow Complex Instructions
+    """Evolve instructions using an `LLM`.
+
+    WizardLM: Empowering Large Language Models to Follow Complex Instructions
 
     Attributes:
         num_evolutions: The number of evolutions to be performed.
         store_evolutions: Whether to store all the evolutions or just the last one. Defaults
             to `False`.
         generate_answers: Whether to generate answers for the evolved instructions. Defaults
             to `False`.
@@ -56,14 +58,18 @@
         - evolved_instructions (`List[str]`): The evolved instructions if `store_evolutions=True`.
         - model_name (`str`): The name of the LLM used to evolve the instructions.
         - answer (`str`): The answer to the evolved instruction if `generate_answers=True`
             and `store_evolutions=False`.
         - answers (`List[str]`): The answers to the evolved instructions if `generate_answers=True`
             and `store_evolutions=True`.
 
+    Categories:
+        - evol
+        - instruction
+
     References:
         - [WizardLM: Empowering Large Language Models to Follow Complex Instructions](https://arxiv.org/abs/2304.12244)
         - [GitHub: h2oai/h2o-wizardlm](https://github.com/h2oai/h2o-wizardlm)
     """
 
     num_evolutions: int
     store_evolutions: bool = False
```

### Comparing `distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/english_nouns.txt` & `distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/english_nouns.txt`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/generator.py` & `distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,17 @@
 
 if TYPE_CHECKING:
     from distilabel.steps.tasks.typing import ChatType
     from distilabel.steps.typing import GeneratorStepOutput
 
 
 class EvolInstructGenerator(GeneratorTask):
-    """WizardLM: Empowering Large Language Models to Follow Complex Instructions
+    """Generate evolved instructions using an `LLM`.
+
+    WizardLM: Empowering Large Language Models to Follow Complex Instructions
 
     Attributes:
         num_instructions: The number of instructions to be generated.
         generate_answers: Whether to generate answers for the instructions or not. Defaults
             to `False`.
         mutation_templates: The mutation templates to be used for the generation of the
             instructions.
@@ -61,14 +63,19 @@
 
     Output columns:
         - instruction (`str`): The generated instruction if `generate_answers=False`.
         - answer (`str`): The generated answer if `generate_answers=True`.
         - instructions (`List[str]`): The generated instructions if `generate_answers=True`.
         - model_name (`str`): The name of the LLM used to generate and evolve the instructions.
 
+    Categories:
+        - evol
+        - instruction
+        - generation
+
     References:
         - [WizardLM: Empowering Large Language Models to Follow Complex Instructions](https://arxiv.org/abs/2304.12244)
         - [GitHub: h2oai/h2o-wizardlm](https://github.com/h2oai/h2o-wizardlm)
     """
 
     num_instructions: int
     generate_answers: bool = False
```

### Comparing `distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/utils.py` & `distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/evol_complexity/__init__.py` & `distilabel-1.1.0/src/distilabel/steps/globals/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/evol_complexity/base.py` & `distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/generator.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,24 +10,26 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Dict
 
-from distilabel.steps.tasks.evol_instruct.base import EvolInstruct
 from distilabel.steps.tasks.evol_instruct.evol_complexity.utils import (
-    MUTATION_TEMPLATES,
+    GENERATION_MUTATION_TEMPLATES,
 )
+from distilabel.steps.tasks.evol_instruct.generator import EvolInstructGenerator
 
 
-class EvolComplexity(EvolInstruct):
-    """EvolComplexity is a task that evolves instructions to make them more complex,
-    and it is based in the EvolInstruct task, but using slight different prompts, but the
-    exact same evolutionary approach.
+class EvolComplexityGenerator(EvolInstructGenerator):
+    """Generate evolved instructions with increased complexity using an `LLM`.
+
+    `EvolComplexityGenerator` is a generation task that evolves instructions to make
+    them more complex, and it is based in the EvolInstruct task, but using slight different
+    prompts, but the exact same evolutionary approach.
 
     Attributes:
         num_instructions: The number of instructions to be generated.
         generate_answers: Whether to generate answers for the instructions or not. Defaults
             to `False`.
         mutation_templates: The mutation templates to be used for the generation of the
             instructions.
@@ -39,21 +41,24 @@
             Defaults to `42`.
 
     Runtime parameters:
         - `min_length`: Defines the length (in bytes) that the generated instruction needs to be higher than, to be considered valid.
         - `max_length`: Defines the length (in bytes) that the generated instruction needs to be lower than, to be considered valid.
         - `seed`: The number of evolutions to be run.
 
-    Input columns:
-        - instruction (`str`): The instruction to evolve.
-
     Output columns:
-        - evolved_instruction (`str`): The evolved instruction.
+        - instruction (`str`): The evolved instruction.
         - answer (`str`, optional): The answer to the instruction if `generate_answers=True`.
         - model_name (`str`): The name of the LLM used to evolve the instructions.
 
+    Categories:
+        - evol
+        - instruction
+        - generation
+        - deita
+
     References:
         - [What Makes Good Data for Alignment? A Comprehensive Study of Automatic Data Selection in Instruction Tuning](https://arxiv.org/abs/2312.15685)
         - [WizardLM: Empowering Large Language Models to Follow Complex Instructions](https://arxiv.org/abs/2304.12244)
     """
 
-    mutation_templates: Dict[str, str] = MUTATION_TEMPLATES
+    mutation_templates: Dict[str, str] = GENERATION_MUTATION_TEMPLATES
```

### Comparing `distilabel-1.0.3/src/distilabel/steps/tasks/evol_instruct/evol_complexity/utils.py` & `distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/steps/tasks/evol_quality/__init__.py` & `distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/steps/tasks/evol_quality/base.py` & `distilabel-1.1.0/src/distilabel/steps/tasks/evol_quality/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,17 @@
 from distilabel.steps.tasks.typing import ChatType
 
 if TYPE_CHECKING:
     from distilabel.steps.typing import StepOutput
 
 
 class EvolQuality(Task):
-    """The `EvolQuality` task is used to evolve the quality of the responses given a prompt,
+    """Evolve the quality of the responses using an `LLM`.
+
+    `EvolQuality` task is used to evolve the quality of the responses given a prompt,
     by generating a new response with a language model. This step implements the evolution
     quality task from the paper 'What Makes Good Data for Alignment? A Comprehensive Study of
     Automatic Data Selection in Instruction Tuning'.
 
     Attributes:
         num_evolutions: The number of evolutions to be performed on the responses.
         store_evolutions: Whether to store all the evolved responses or just the last one.
@@ -52,14 +54,19 @@
         - response (`str`): The responses to be rewritten.
 
     Output columns:
         - evolved_response (`str`): The evolved response if `store_evolutions=False`.
         - evolved_responses (`List[str]`): The evolved responses if `store_evolutions=True`.
         - model_name (`str`): The name of the LLM used to evolve the responses.
 
+    Categories:
+        - evol
+        - response
+        - deita
+
     References:
         - [`What Makes Good Data for Alignment? A Comprehensive Study of Automatic Data Selection in Instruction Tuning`](https://arxiv.org/abs/2312.15685)
     """
 
     num_evolutions: int
     store_evolutions: bool = False
     include_original_response: bool = False
```

### Comparing `distilabel-1.0.3/src/distilabel/steps/tasks/evol_quality/utils.py` & `distilabel-1.1.0/src/distilabel/steps/tasks/evol_quality/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/steps/tasks/templates/instruction-backtranslation.jinja2` & `distilabel-1.1.0/src/distilabel/steps/tasks/templates/instruction-backtranslation.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/steps/tasks/templates/ultrafeedback/helpfulness.jinja2` & `distilabel-1.1.0/src/distilabel/steps/tasks/templates/ultrafeedback/helpfulness.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/steps/tasks/templates/ultrafeedback/honesty.jinja2` & `distilabel-1.1.0/src/distilabel/steps/tasks/templates/ultrafeedback/honesty.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/steps/tasks/templates/ultrafeedback/instruction-following.jinja2` & `distilabel-1.1.0/src/distilabel/steps/tasks/templates/ultrafeedback/instruction-following.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/steps/tasks/templates/ultrafeedback/overall-rating.jinja2` & `distilabel-1.1.0/src/distilabel/steps/tasks/templates/ultrafeedback/overall-rating.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/steps/tasks/templates/ultrafeedback/truthfulness.jinja2` & `distilabel-1.1.0/src/distilabel/steps/tasks/templates/ultrafeedback/truthfulness.jinja2`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/utils/__init__.py` & `distilabel-1.1.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/utils/chat.py` & `distilabel-1.1.0/src/distilabel/utils/chat.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/utils/dicts.py` & `distilabel-1.1.0/src/distilabel/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/utils/files.py` & `distilabel-1.1.0/tests/unit/cli/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,21 +8,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from pathlib import Path
-from typing import List
+import os
 
+current_dir = os.path.dirname(os.path.abspath(__file__))
 
-def list_files_in_dir(dir_path: Path) -> List[Path]:
-    """List all files in a directory.
-
-    Args:
-        dir_path: Path to the directory.
-
-    Returns:
-        A list of file names in the directory.
-    """
-    return [f for f in dir_path.iterdir() if f.is_file()]
+TEST_PIPELINE_PATH = os.path.join(current_dir, "test_pipeline.yaml")
```

### Comparing `distilabel-1.0.3/src/distilabel/utils/itertools.py` & `distilabel-1.1.0/src/distilabel/utils/itertools.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/utils/lists.py` & `distilabel-1.1.0/src/distilabel/utils/lists.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/utils/logging.py` & `distilabel-1.1.0/src/distilabel/utils/logging.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 import multiprocessing as mp
 import os
 import warnings
+from logging import FileHandler
 from logging.handlers import QueueHandler, QueueListener
-from typing import TYPE_CHECKING, Any, Union
+from pathlib import Path
+from typing import TYPE_CHECKING, Any, Optional, Union
 
 from rich.logging import RichHandler
 
 if TYPE_CHECKING:
     from queue import Queue
 
 
@@ -36,30 +38,41 @@
     "fsspec",
     "asyncio",
 ]
 
 queue_listener: Union[QueueListener, None] = None
 
 
-def setup_logging(log_queue: "Queue[Any]") -> None:
+def setup_logging(log_queue: "Queue[Any]", filename: Optional[str] = None) -> None:
     """Sets up logging to use a queue across all processes."""
     global queue_listener
 
     # Disable overly verbose loggers
     logging.getLogger("argilla.client.feedback.dataset.local.mixins").disabled = True
     for logger in _SILENT_LOGGERS:
         logging.getLogger(logger).setLevel(logging.CRITICAL)
 
     # If the current process is the main process, set up a `QueueListener`
     # to handle logs from all subprocesses
     if mp.current_process().name == "MainProcess":
         formatter = logging.Formatter("['%(name)s'] %(message)s")
         handler = RichHandler(rich_tracebacks=True)
         handler.setFormatter(formatter)
-        queue_listener = QueueListener(log_queue, handler, respect_handler_level=True)
+        if not Path(filename).parent.exists():
+            Path(filename).parent.mkdir(parents=True, exist_ok=True)
+
+        file_handler = FileHandler(filename, delay=True)
+        file_formatter = logging.Formatter(
+            "[%(asctime)s] %(levelname)-8s %(message)s", datefmt="%Y-%m-%d %H:%M:%S"
+        )
+        file_handler.setFormatter(file_formatter)
+
+        queue_listener = QueueListener(
+            log_queue, handler, file_handler, respect_handler_level=True
+        )
         queue_listener.start()
 
     log_level = os.environ.get("DISTILABEL_LOG_LEVEL", "INFO").upper()
     if log_level not in ["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]:
         warnings.warn(
             f"Invalid log level '{log_level}', using default 'INFO' instead.",
             stacklevel=2,
```

### Comparing `distilabel-1.0.3/src/distilabel/utils/notebook.py` & `distilabel-1.1.0/src/distilabel/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/utils/typing_.py` & `distilabel-1.1.0/src/distilabel/utils/typing_.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/utils/card/__init__.py` & `distilabel-1.1.0/src/distilabel/utils/mkdocs/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/utils/card/dataset_card.py` & `distilabel-1.1.0/src/distilabel/utils/card/dataset_card.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/src/distilabel/utils/card/distilabel_template.md` & `distilabel-1.1.0/src/distilabel/utils/card/distilabel_template.md`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/__init__.py` & `distilabel-1.1.0/src/distilabel/steps/tasks/evol_quality/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/integration/test_pipe_llms.py` & `distilabel-1.1.0/tests/integration/test_pipe_llms.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/integration/test_pipe_simple.py` & `distilabel-1.1.0/tests/integration/test_pipe_simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,18 +153,14 @@
         )
 
         load_dataset.connect(rename_columns)
         rename_columns.connect(generate_response)
 
     return pipeline.run(
         parameters={
-            "load_dataset": {
-                "repo_id": "plaguss/test",
-                "split": "train",
-            },
             "rename_columns": {
                 "rename_mappings": {
                     "prompt": "instruction",
                 },
             },
         }
     )
```

### Comparing `distilabel-1.0.3/tests/unit/__init__.py` & `distilabel-1.1.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/test_distiset.py` & `distilabel-1.1.0/tests/unit/test_distiset.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/test_imports.py` & `distilabel-1.1.0/tests/unit/test_imports.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,22 +38,26 @@
     from distilabel.pipeline import Pipeline
 
     from distilabel.steps import (
         CombineColumns,
         ConversationTemplate,
         DeitaFiltering,
         ExpandColumns,
+        FormatChatGenerationDPO,
+        FormatChatGenerationSFT,
+        FormatTextGenerationDPO,
+        FormatTextGenerationSFT,
         GeneratorStep,
         GlobalStep,
+        GeneratorStepOutput,
         KeepColumns,
         LoadDataFromDicts,
         LoadHubDataset,
         PushToHub,
         Step,
-        GeneratorStepOutput,
         StepOutput,
         PreferenceToArgilla,
         TextGenerationToArgilla,
         step,
     )
 
     from distilabel.steps.tasks import (
@@ -63,14 +67,16 @@
         ChatType,
         ComplexityScorer,
         EvolInstruct,
         EvolComplexity,
         EvolComplexityGenerator,
         EvolInstructGenerator,
         GenerateEmbeddings,
+        Genstruct,
         InstructionBacktranslation,
         PairRM,
+        PrometheusEval,
         QualityScorer,
         SelfInstruct,
         TextGeneration,
         UltraFeedback,
     )
```

### Comparing `distilabel-1.0.3/tests/unit/cli/__init__.py` & `distilabel-1.1.0/src/distilabel/steps/tasks/structured_outputs/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/cli/test_pipeline.yaml` & `distilabel-1.1.0/tests/unit/cli/test_pipeline.yaml`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/cli/utils.py` & `distilabel-1.1.0/tests/unit/helpers.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,10 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 
-current_dir = os.path.dirname(os.path.abspath(__file__))
-
-TEST_PIPELINE_PATH = os.path.join(current_dir, "test_pipeline.yaml")
+DISTILABEL_RUN_SLOW_TESTS = os.getenv("DISTILABEL_RUN_SLOW_TESTS", False)
```

### Comparing `distilabel-1.0.3/tests/unit/cli/pipeline/__init__.py` & `distilabel-1.1.0/src/distilabel/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/cli/pipeline/test_app.py` & `distilabel-1.1.0/tests/unit/cli/pipeline/test_app.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/cli/pipeline/utils.py` & `distilabel-1.1.0/tests/unit/cli/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/llms/__init__.py` & `distilabel-1.1.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/llms/test_anthropic.py` & `distilabel-1.1.0/tests/unit/llms/test_anthropic.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 
         _dump = {
             "base_url": "https://api.anthropic.com",
             "generation_kwargs": {},
             "max_retries": 6,
             "model": "claude-3-opus-20240229",
             "timeout": 600.0,
+            "structured_output": None,
             "type_info": {
                 "module": "distilabel.llms.anthropic",
                 "name": "AnthropicLLM",
             },
         }
 
         assert llm.dump() == _dump
```

### Comparing `distilabel-1.0.3/tests/unit/llms/test_anyscale.py` & `distilabel-1.1.0/tests/unit/llms/test_anyscale.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 
         _dump = {
             "model": self.model_id,
             "generation_kwargs": {},
             "max_retries": 6,
             "base_url": "https://api.endpoints.anyscale.com/v1",
             "timeout": 120,
+            "structured_output": None,
             "type_info": {
                 "module": "distilabel.llms.anyscale",
                 "name": "AnyscaleLLM",
             },
         }
 
         assert llm.dump() == _dump
```

### Comparing `distilabel-1.0.3/tests/unit/llms/test_azure.py` & `distilabel-1.1.0/tests/unit/llms/test_azure.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,11 +64,12 @@
         _dump = {
             "generation_kwargs": {},
             "model": "gpt-4",
             "base_url": "https://example-resource.azure.openai.com/",
             "max_retries": 6,
             "timeout": 120,
             "api_version": "preview",
+            "structured_output": None,
             "type_info": {"module": "distilabel.llms.azure", "name": "AzureOpenAILLM"},
         }
         assert llm.dump() == _dump
         assert isinstance(AzureOpenAILLM.from_dict(_dump), AzureOpenAILLM)
```

### Comparing `distilabel-1.0.3/tests/unit/llms/test_cohere.py` & `distilabel-1.1.0/tests/unit/llms/test_cohere.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,15 @@
 
         dump = {
             "model": "command-r",
             "generation_kwargs": {},
             "base_url": "https://api.cohere.ai/v1",
             "timeout": 120,
             "client_name": "distilabel",
+            "structured_output": None,
             "type_info": {
                 "module": "distilabel.llms.cohere",
                 "name": "CohereLLM",
             },
         }
 
         assert llm.dump() == dump
```

### Comparing `distilabel-1.0.3/tests/unit/llms/test_litellm.py` & `distilabel-1.1.0/tests/unit/llms/test_litellm.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 
     def test_serialization(self, _: MagicMock, model: str) -> None:
         llm = LiteLLM(model=model)  # type: ignore
 
         _dump = {
             "model": model,
             "verbose": False,
+            "structured_output": None,
             "type_info": {
                 "module": "distilabel.llms.litellm",
                 "name": "LiteLLM",
             },
             "generation_kwargs": {},
         }
```

### Comparing `distilabel-1.0.3/tests/unit/llms/test_llamacpp.py` & `distilabel-1.1.0/tests/unit/llms/test_llamacpp.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,33 +17,33 @@
 from typing import Generator
 
 import pytest
 from distilabel.llms.llamacpp import LlamaCppLLM
 
 
 @pytest.fixture(scope="module")
-def llamacpp_llm() -> Generator[LlamaCppLLM, None, None]:
+def llm() -> Generator[LlamaCppLLM, None, None]:
     if not os.path.exists("tinyllama.gguf"):
         urllib.request.urlretrieve(
             "https://huggingface.co/TheBloke/TinyLlama-1.1B-Chat-v1.0-GGUF/resolve/main/tinyllama-1.1b-chat-v1.0.Q2_K.gguf",
             "tinyllama.gguf",
         )
 
     llm = LlamaCppLLM(model_path="tinyllama.gguf", n_gpu_layers=0)  # type: ignore
     llm.load()
 
     yield llm
 
 
 class TestLlamaCppLLM:
-    def test_model_name(self, llamacpp_llm: LlamaCppLLM) -> None:
-        assert llamacpp_llm.model_name == "tinyllama.gguf"
+    def test_model_name(self, llm: LlamaCppLLM) -> None:
+        assert llm.model_name == "tinyllama.gguf"
 
-    def test_generate(self, llamacpp_llm: LlamaCppLLM) -> None:
-        responses = llamacpp_llm.generate(
+    def test_generate(self, llm: LlamaCppLLM) -> None:
+        responses = llm.generate(
             inputs=[
                 [{"role": "user", "content": "Hello, how are you?"}],
                 [
                     {
                         "role": "user",
                         "content": "You're GPT2, you're old now but you still serves a purpose which is being used in unit tests.",
                     }
```

### Comparing `distilabel-1.0.3/tests/unit/llms/test_mistral.py` & `distilabel-1.1.0/tests/unit/llms/test_mistral.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
         _dump = {
             "model": "mistral-tiny",
             "endpoint": "https://api.mistral.ai",
             "generation_kwargs": {},
             "max_retries": 6,
             "timeout": 120,
             "max_concurrent_requests": 64,
+            "structured_output": None,
             "type_info": {
                 "module": "distilabel.llms.mistral",
                 "name": "MistralLLM",
             },
         }
 
         assert llm.dump() == _dump
```

### Comparing `distilabel-1.0.3/tests/unit/llms/test_mixins.py` & `distilabel-1.1.0/tests/unit/llms/test_mixins.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/llms/test_ollama.py` & `distilabel-1.1.0/tests/unit/llms/test_ollama.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 
         _dump = {
             "model": "notus",
             "host": None,
             "timeout": 120,
             "follow_redirects": True,
             "generation_kwargs": {},
+            "structured_output": None,
             "type_info": {
                 "module": "distilabel.llms.ollama",
                 "name": "OllamaLLM",
             },
         }
 
         assert llm.dump() == _dump
```

### Comparing `distilabel-1.0.3/tests/unit/llms/test_openai.py` & `distilabel-1.1.0/tests/unit/llms/test_openai.py`

 * *Files 7% similar despite different names*

```diff
@@ -83,23 +83,38 @@
                         "role": "user",
                         "content": "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
                     },
                 ]
             ]
         )
 
+        with pytest.raises(ValueError):
+            llm.generate(
+                inputs=[
+                    [
+                        {"role": "system", "content": ""},
+                        {
+                            "role": "user",
+                            "content": "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
+                        },
+                    ]
+                ],
+                response_format="unkown_format",
+            )
+
     def test_serialization(self, _: MagicMock) -> None:
         llm = OpenAILLM(model=self.model_id)
 
         _dump = {
             "model": self.model_id,
             "generation_kwargs": {},
             "max_retries": 6,
             "base_url": "https://api.openai.com/v1",
             "timeout": 120,
+            "structured_output": None,
             "type_info": {
                 "module": "distilabel.llms.openai",
                 "name": "OpenAILLM",
             },
         }
 
         assert llm.dump() == _dump
```

### Comparing `distilabel-1.0.3/tests/unit/llms/test_together.py` & `distilabel-1.1.0/tests/unit/llms/test_together.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 
         _dump = {
             "model": self.model_id,
             "generation_kwargs": {},
             "max_retries": 6,
             "base_url": "https://api.together.xyz/v1",
             "timeout": 120,
+            "structured_output": None,
             "type_info": {
                 "module": "distilabel.llms.together",
                 "name": "TogetherLLM",
             },
         }
 
         assert llm.dump() == _dump
```

### Comparing `distilabel-1.0.3/tests/unit/llms/test_vertexai.py` & `distilabel-1.1.0/tests/unit/llms/test_vertexai.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import os
 from unittest.mock import AsyncMock, MagicMock, Mock, patch
 
 import nest_asyncio
 import pytest
 from distilabel.llms.vertexai import VertexAILLM
 from vertexai.generative_models import (
     Content,
@@ -24,24 +23,24 @@
     Part,
 )
 
 
 @patch("vertexai.generative_models.GenerativeModel.generate_content_async")
 class TestVertexAILLM:
     def test_openai_llm(self, _: MagicMock) -> None:
-        llm = VertexAILLM(model="gemini-1.0-pro", api_key="api.key")  # type: ignore
+        llm = VertexAILLM(model="gemini-1.0-pro")
         assert isinstance(llm, VertexAILLM)
         assert llm.model_name == "gemini-1.0-pro"
 
     @pytest.mark.asyncio
     async def test_agenerate(self, mock_generative_model: MagicMock) -> None:
-        llm = VertexAILLM(model="gemini-1.0-pro", api_key="api.key")  # type: ignore
+        llm = VertexAILLM(model="gemini-1.0-pro")
         llm._aclient = mock_generative_model
-        llm._part_class = Part
-        llm._content_class = Content
+        llm._part_class = Part  # type: ignore
+        llm._content_class = Content  # type: ignore
         llm._generation_config_class = GenerationConfig
 
         mocked_completion = Mock(
             choices=[Mock(message=Mock(content=" Aenean hendrerit aliquam velit. ..."))]
         )
         llm._aclient.chat.completions.create = AsyncMock(return_value=mocked_completion)
 
@@ -66,18 +65,18 @@
                     "content": "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
                 },
             ]
         )
 
     @pytest.mark.asyncio
     async def test_generate(self, mock_generative_model: MagicMock) -> None:
-        llm = VertexAILLM(model="gemini-1.0-pro", api_key="api.key")  # type: ignore
+        llm = VertexAILLM(model="gemini-1.0-pro")
         llm._aclient = mock_generative_model
-        llm._part_class = Part
-        llm._content_class = Content
+        llm._part_class = Part  # type: ignore
+        llm._content_class = Content  # type: ignore
         llm._generation_config_class = GenerationConfig
 
         mocked_completion = Mock(
             choices=[Mock(message=Mock(content=" Aenean hendrerit aliquam velit. ..."))]
         )
         llm._aclient.chat.completions.create = AsyncMock(return_value=mocked_completion)
 
@@ -107,20 +106,20 @@
                         "content": "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
                     },
                 ]
             ]
         )
 
     def test_serialization(self, _: MagicMock) -> None:
-        os.environ["OPENAI_API_KEY"] = "api.key"
-        llm = VertexAILLM(model="gemini-1.0-pro")  # type: ignore
+        llm = VertexAILLM(model="gemini-1.0-pro")
 
         _dump = {
             "model": "gemini-1.0-pro",
             "generation_kwargs": {},
+            "structured_output": None,
             "type_info": {
                 "module": "distilabel.llms.vertexai",
                 "name": "VertexAILLM",
             },
         }
 
         assert llm.dump() == _dump
```

### Comparing `distilabel-1.0.3/tests/unit/llms/huggingface/__init__.py` & `distilabel-1.1.0/tests/unit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/llms/huggingface/test_inference_endpoints.py` & `distilabel-1.1.0/tests/unit/llms/huggingface/test_inference_endpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,14 +171,15 @@
             "endpoint_name": None,
             "endpoint_namespace": None,
             "base_url": None,
             "tokenizer_id": None,
             "generation_kwargs": {},
             "model_display_name": None,
             "use_openai_client": False,
+            "structured_output": None,
             "type_info": {
                 "module": "distilabel.llms.huggingface.inference_endpoints",
                 "name": "InferenceEndpointsLLM",
             },
         }
         assert llm.dump() == _dump
         assert isinstance(InferenceEndpointsLLM.from_dict(_dump), InferenceEndpointsLLM)
```

### Comparing `distilabel-1.0.3/tests/unit/llms/huggingface/test_transformers.py` & `distilabel-1.1.0/tests/unit/llms/huggingface/test_transformers.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/mixins/__init__.py` & `distilabel-1.1.0/tests/unit/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/mixins/test_runtime_parameters.py` & `distilabel-1.1.0/tests/unit/mixins/test_runtime_parameters.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/pipeline/__init__.py` & `distilabel-1.1.0/tests/unit/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/pipeline/conftest.py` & `distilabel-1.1.0/tests/unit/pipeline/conftest.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/pipeline/test_dag.py` & `distilabel-1.1.0/tests/unit/pipeline/test_dag.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,18 +15,20 @@
 import tempfile
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable, Dict, List
 
 import pytest
 from distilabel.mixins.runtime_parameters import RuntimeParameter
 from distilabel.pipeline._dag import DAG
+from distilabel.pipeline.constants import STEP_ATTR_NAME
 from distilabel.pipeline.local import Pipeline
+from distilabel.pipeline.routing_batch_function import routing_batch_function
 from distilabel.steps.base import GeneratorStep, Step, StepInput
 
-from .utils import DummyGeneratorStep
+from .utils import DummyGeneratorStep, DummyStep1, DummyStep2
 
 if TYPE_CHECKING:
     from distilabel.steps.typing import (
         GeneratorStepOutput,
         StepOutput,
     )
 
@@ -47,15 +49,15 @@
         ):
             dag.add_step(dummy_step_1)
 
     def test_get_step(self, dummy_step_1: "Step") -> None:
         dag = DAG()
         dag.add_step(dummy_step_1)
 
-        assert dag.get_step("dummy_step_1")["step"] == dummy_step_1
+        assert dag.get_step("dummy_step_1")[STEP_ATTR_NAME] == dummy_step_1
 
     def test_get_step_nonexistent(self) -> None:
         dag = DAG()
         with pytest.raises(
             ValueError, match="Step with name 'dummy_step_1' does not exist"
         ):
             dag.get_step("dummy_step_1")
@@ -358,15 +360,15 @@
         step.set_runtime_parameters({})
 
         dag = DAG()
         dag.add_step(step)
 
         dag.validate()
 
-    def test_step_invalid_input_mappings(self, pipeline: "Pipeline") -> None:
+    def test_validate_step_invalid_input_mappings(self, pipeline: "Pipeline") -> None:
         class DummyStep(Step):
             @property
             def inputs(self) -> List[str]:
                 return ["instruction"]
 
             @property
             def outputs(self) -> List[str]:
@@ -386,15 +388,15 @@
 
         with pytest.raises(
             ValueError,
             match="The input column 'i_do_not_exist' doesn't exist in the inputs",
         ):
             dag.validate()
 
-    def test_step_invalid_output_mappings(self, pipeline: "Pipeline") -> None:
+    def test_validate_step_invalid_output_mappings(self, pipeline: "Pipeline") -> None:
         class DummyStep(Step):
             @property
             def inputs(self) -> List[str]:
                 return ["instruction"]
 
             @property
             def outputs(self) -> List[str]:
@@ -414,15 +416,15 @@
 
         with pytest.raises(
             ValueError,
             match="The output column 'i_do_not_exist' doesn't exist in the outputs",
         ):
             dag.validate()
 
-    def test_generator_step_process_method_with_step_input(
+    def test_validate_generator_step_process_method_with_step_input(
         self, pipeline: "Pipeline"
     ) -> None:
         class DummyGeneratorStep(GeneratorStep):
             @property
             def inputs(self) -> List[str]:
                 return ["instruction"]
 
@@ -442,15 +444,15 @@
 
         with pytest.raises(
             ValueError,
             match="Generator step 'dummy_generator_step' should not have a parameter with type hint `StepInput`",
         ):
             dag.validate()
 
-    def test_generator_step_process_without_offset_parameter(
+    def test_validate_generator_step_process_without_offset_parameter(
         self, pipeline: "Pipeline"
     ) -> None:
         class DummyGeneratorStep(GeneratorStep):
             @property
             def inputs(self) -> List[str]:
                 return ["instruction"]
 
@@ -468,14 +470,159 @@
 
         with pytest.raises(
             ValueError,
             match="Generator step 'dummy_generator_step' should have an `offset` parameter",
         ):
             dag.validate()
 
+    def test_validate_convergence_step_receiving_from_same_routed_batch_function(
+        self, pipeline: "Pipeline"
+    ) -> None:
+        generator_step_1 = DummyGeneratorStep(pipeline=pipeline)
+        dummy_step_1 = DummyStep1(pipeline=pipeline)
+        dummy_step_2 = DummyStep1(pipeline=pipeline)
+
+        generator_step_2 = DummyGeneratorStep(pipeline=pipeline)
+        dummy_step_3 = DummyStep1(pipeline=pipeline)
+        dummy_step_4 = DummyStep1(pipeline=pipeline)
+
+        convergence_step = DummyStep2(name="convergence_step", pipeline=pipeline)
+
+        @routing_batch_function()
+        def routing_batch_function_1(steps: List[str]) -> List[str]:
+            return steps
+
+        @routing_batch_function()
+        def routing_batch_function_2(steps: List[str]) -> List[str]:
+            return steps
+
+        generator_step_1 >> routing_batch_function_1 >> [dummy_step_1, dummy_step_2]
+
+        generator_step_2 >> routing_batch_function_2 >> [dummy_step_3, dummy_step_4]
+
+        [dummy_step_1, dummy_step_2, dummy_step_3, dummy_step_4] >> convergence_step
+
+        with pytest.raises(
+            ValueError,
+            match=r"Convergence step 'convergence_step' should receive batches from steps receiving"
+            " routed batches from the same previous step and `routing_batch_function`.",
+        ):
+            pipeline.dag.validate()
+
+    def test_validate_convergence_step_input_batch_size(
+        self, pipeline: "Pipeline"
+    ) -> None:
+        generator_step_1 = DummyGeneratorStep(pipeline=pipeline)
+        dummy_step_1 = DummyStep1(pipeline=pipeline)
+        dummy_step_2 = DummyStep1(pipeline=pipeline)
+        convergence_step = DummyStep2(
+            name="convergence_step",
+            pipeline=pipeline,
+            input_batch_size=666,
+        )
+
+        @routing_batch_function()
+        def routing_batch_function_1(steps: List[str]) -> List[str]:
+            return steps
+
+        (
+            generator_step_1
+            >> routing_batch_function_1
+            >> [dummy_step_1, dummy_step_2]
+            >> convergence_step
+        )
+
+        with pytest.raises(
+            ValueError,
+            match="A convergence step should have an `input_batch_size` equal or lower",
+        ):
+            pipeline.dag.validate()
+
+    def test_validate_step_receiving_routed_batches_multiple_predecessors(
+        self, pipeline: "Pipeline"
+    ) -> None:
+        generator_step_1 = DummyGeneratorStep(pipeline=pipeline)
+        dummy_step_1 = DummyStep1(pipeline=pipeline)
+
+        generator_step_2 = DummyGeneratorStep(pipeline=pipeline)
+        dummy_step_2 = DummyStep1(pipeline=pipeline)
+
+        dummy_step_3 = DummyStep2(name="doomed", pipeline=pipeline)
+        dummy_step_4 = DummyStep2(pipeline=pipeline)
+
+        @routing_batch_function()
+        def routing_batch_function_1(steps: List[str]) -> List[str]:
+            return steps
+
+        (
+            generator_step_1
+            >> dummy_step_1
+            >> routing_batch_function_1
+            >> [dummy_step_3, dummy_step_4]
+        )
+
+        generator_step_2 >> dummy_step_2 >> dummy_step_3
+
+        with pytest.raises(
+            ValueError,
+            match="Step 'doomed' cannot have multiple predecessors when the batches of one"
+            " are being routed with a `routing_batch_function`.",
+        ):
+            pipeline.dag.validate()
+
+    def test_validate_step_receiving_routed_batches_input_batch_size(
+        self, pipeline: "Pipeline"
+    ) -> None:
+        generator_step_1 = DummyGeneratorStep(pipeline=pipeline)
+        dummy_step_1 = DummyStep1(pipeline=pipeline)
+        dummy_step_2 = DummyStep1(name="demon", pipeline=pipeline, input_batch_size=666)
+
+        @routing_batch_function()
+        def routing_batch_function_1(steps: List[str]) -> List[str]:
+            return steps
+
+        convergence_step = DummyStep2(name="convergence_step", pipeline=pipeline)
+
+        (
+            generator_step_1
+            >> routing_batch_function_1
+            >> [dummy_step_1, dummy_step_2]
+            >> convergence_step
+        )
+
+        with pytest.raises(
+            ValueError,
+            match="Step 'demon' should have an `input_batch_size` equal or lower",
+        ):
+            pipeline.dag.validate()
+
+    def test_validate_step_receiving_routed_batches_input_batch_size_multiple(
+        self, pipeline: "Pipeline"
+    ) -> None:
+        generator_step_1 = DummyGeneratorStep(pipeline=pipeline)
+        dummy_step_1 = DummyStep1(pipeline=pipeline)
+        dummy_step_2 = DummyStep1(name="demon", pipeline=pipeline, input_batch_size=7)
+
+        @routing_batch_function()
+        def routing_batch_function_1(steps: List[str]) -> List[str]:
+            return steps
+
+        convergence_step = DummyStep2(name="convergence_step", pipeline=pipeline)
+        (
+            generator_step_1
+            >> routing_batch_function_1
+            >> [dummy_step_1, dummy_step_2]
+            >> convergence_step
+        )
+        with pytest.raises(
+            ValueError,
+            match="Step 'demon' should have an `input_batch_size` that is a multiple of the `input_batch_size` or `batch_size`",
+        ):
+            pipeline.dag.validate()
+
 
 class TestDagSerialization:
     def test_dag_dump(self, dummy_step_1: "Step", dummy_step_2: "Step") -> None:
         dag = DAG()
         dag.add_step(dummy_step_1)
         dag.add_step(dummy_step_2)
         dag.add_edge("dummy_step_1", "dummy_step_2")
@@ -500,23 +647,26 @@
             new_dag = DAG.from_dict(dag.dump())
         assert isinstance(new_dag, DAG)
         assert "dummy_step_1" in new_dag.G
         assert "dummy_step_2" in new_dag.G
         assert "dummy_step_2" in new_dag.G["dummy_step_1"]
 
     def test_dag_from_dict_errored_without_pipeline(
-        self, dummy_step_1: "Step", dummy_step_2: "Step"
+        self,
+        caplog: pytest.LogCaptureFixture,
+        dummy_step_1: "Step",
+        dummy_step_2: "Step",
     ) -> None:
         dag = DAG()
         dag.add_step(dummy_step_1)
         dag.add_step(dummy_step_2)
         dag.add_edge("dummy_step_1", "dummy_step_2")
 
-        with pytest.raises(ValueError):
-            DAG.from_dict(dag.dump())
+        DAG.from_dict(dag.dump())
+        assert "Step 'dummy_step_1' hasn't received a pipeline" in caplog.text
 
     @pytest.mark.parametrize(
         "format, name, loader",
         [
             ("yaml", "dag.yaml", DAG.from_yaml),
             ("json", "dag.json", DAG.from_json),
             ("invalid", "dag.invalid", None),
```

### Comparing `distilabel-1.0.3/tests/unit/pipeline/test_local.py` & `distilabel-1.1.0/tests/unit/pipeline/test_local.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,19 +46,23 @@
 
         input_queue = mock.MagicMock()
         step = mock.MagicMock()
         step.__getitem__.return_value = input_queue
         get_step_mock = mock.MagicMock(return_value=step)
         pipeline.dag.get_step = get_step_mock  # type: ignore
 
+        batch_manager_mock = mock.MagicMock()
+        pipeline._batch_manager = batch_manager_mock  # type: ignore
+
         batch = _Batch(
             seq_no=0, step_name=dummy_generator_step.name, last_batch=False, data=[[]]
         )
         pipeline._send_batch_to_step(batch=batch)  # type: ignore
 
+        batch_manager_mock.set_last_batch_sent.assert_called_once_with(batch)
         get_step_mock.assert_called_once_with(dummy_generator_step.name)
         input_queue.put.assert_called_once_with(batch)
 
     @mock.patch("distilabel.pipeline.local._ProcessWrapper")
     def test_create_processes(self, process_wrapper_mock: mock.MagicMock) -> None:
         pool = mock.MagicMock()
         manager = mock.MagicMock()
@@ -80,26 +84,29 @@
         process_wrapper_mock.assert_has_calls(
             [
                 mock.call(
                     step=dummy_generator,
                     input_queue=mock.ANY,
                     output_queue=queue,
                     shared_info=shared_info,
+                    dry_run=False,
                 ),
                 mock.call(
                     step=dummy_step_1,
                     input_queue=mock.ANY,
                     output_queue=queue,
                     shared_info=shared_info,
+                    dry_run=False,
                 ),
                 mock.call(
                     step=dummy_step_2,
                     input_queue=mock.ANY,
                     output_queue=queue,
                     shared_info=shared_info,
+                    dry_run=False,
                 ),
             ],
         )
 
         pool.apply_async.assert_has_calls(
             [
                 mock.call(
```

### Comparing `distilabel-1.0.3/tests/unit/pipeline/utils.py` & `distilabel-1.1.0/tests/unit/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/steps/__init__.py` & `distilabel-1.1.0/tests/unit/cli/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/steps/test_base.py` & `distilabel-1.1.0/tests/unit/steps/test_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,21 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import List, Optional
 
 import pytest
 from distilabel.mixins.runtime_parameters import RuntimeParameter
+from distilabel.pipeline.constants import ROUTING_BATCH_FUNCTION_ATTR_NAME
 from distilabel.pipeline.local import Pipeline
-from distilabel.steps.base import (
-    GeneratorStep,
-    GlobalStep,
-    Step,
-    StepInput,
-)
+from distilabel.steps.base import GeneratorStep, GlobalStep, Step, StepInput
+from distilabel.steps.decorator import step
 from distilabel.steps.typing import GeneratorStepOutput, StepOutput
 from distilabel.utils.serialization import TYPE_INFO_KEY
 from pydantic import ValidationError
 
 
 class DummyStep(Step):
     @property
@@ -73,28 +70,36 @@
             DummyStep(
                 name="this-is-not-va.li.d-because-it-contains-dots", pipeline=pipeline
             )
 
         with pytest.raises(ValidationError):
             DummyStep(name="this is not valid because spaces", pipeline=pipeline)
 
+    def test_create_step_and_infer_name(self) -> None:
+        dummy_step = DummyStep(pipeline=Pipeline(name="unit-test-pipeline"))
+        assert dummy_step.name == "dummy_step_0"
+
     def test_create_step_passing_pipeline(self) -> None:
         pipeline = Pipeline(name="unit-test-pipeline")
         step = DummyStep(name="dummy", pipeline=pipeline)
         assert step.pipeline == pipeline
 
     def test_create_step_within_pipeline_context(self) -> None:
         with Pipeline(name="unit-test-pipeline") as pipeline:
             step = DummyStep(name="dummy")
 
         assert step.pipeline == pipeline
 
-    def test_creating_step_without_pipeline(self) -> None:
-        with pytest.raises(ValueError, match="Step 'dummy' hasn't received a pipeline"):
-            DummyStep(name="dummy")
+    def test_creating_step_without_pipeline(
+        self, caplog: pytest.LogCaptureFixture
+    ) -> None:
+        # This test is to ensure that the warning is raised when creating a step without a pipeline,
+        # vs the error we raised before.
+        dummy_step = DummyStep(name="dummy")
+        assert f"Step '{dummy_step.name}' hasn't received a pipeline" in caplog.text
 
     def test_is_generator(self) -> None:
         step = DummyStep(name="dummy", pipeline=Pipeline(name="unit-test-pipeline"))
         assert not step.is_generator
 
     def test_is_global(self) -> None:
         step = DummyStep(name="dummy", pipeline=Pipeline(name="unit-test-pipeline"))
@@ -213,14 +218,44 @@
 
         assert outputs == [
             {"prompt": "hello 1", "generation": "unit test"},
             {"prompt": "hello 2", "generation": "unit test"},
             {"prompt": "hello 3", "generation": "unit test"},
         ]
 
+    def test_connect(self) -> None:
+        @step(inputs=["instruction"], outputs=["generation"])
+        def GenerationStep(input: StepInput):
+            pass
+
+        def routing_batch_function(downstream_step_names: List[str]) -> List[str]:
+            return downstream_step_names
+
+        with Pipeline(name="unit-test-pipeline") as pipeline:
+            generator_step = DummyGeneratorStep(name="dummy_generator")
+
+            generate_1 = GenerationStep(name="generate_1")
+            generate_2 = GenerationStep(name="generate_2")
+            generate_3 = GenerationStep(name="generate_3")
+
+            generator_step.connect(
+                generate_1,
+                generate_2,
+                generate_3,
+                routing_batch_function=routing_batch_function,
+            )
+
+        assert "generate_1" in pipeline.dag.G["dummy_generator"]
+        assert "generate_2" in pipeline.dag.G["dummy_generator"]
+        assert "generate_3" in pipeline.dag.G["dummy_generator"]
+        assert (
+            pipeline.dag.get_step("dummy_generator")[ROUTING_BATCH_FUNCTION_ATTR_NAME]
+            == routing_batch_function
+        )
+
 
 class TestGeneratorStep:
     def test_is_generator(self) -> None:
         step = DummyGeneratorStep(
             name="dummy", pipeline=Pipeline(name="unit-test-pipeline")
         )
         assert step.is_generator
@@ -280,20 +315,22 @@
                         },
                     }
                 }
             )
 
         assert isinstance(step, DummyStep)
 
-    def test_step_from_dict_without_pipeline_context(self) -> None:
-        with pytest.raises(ValueError):
-            DummyStep.from_dict(
-                {
-                    **{
-                        "name": "dummy",
-                        TYPE_INFO_KEY: {
-                            "module": "tests.pipeline.step.test_base",
-                            "name": "DummyStep",
-                        },
-                    }
+    def test_step_from_dict_without_pipeline_context(
+        self, caplog: pytest.LogCaptureFixture
+    ) -> None:
+        dummy_step = DummyStep.from_dict(
+            {
+                **{
+                    "name": "dummy",
+                    TYPE_INFO_KEY: {
+                        "module": "tests.pipeline.step.test_base",
+                        "name": "DummyStep",
+                    },
                 }
-            )
+            }
+        )
+        assert f"Step '{dummy_step.name}' hasn't received a pipeline" in caplog.text
```

### Comparing `distilabel-1.0.3/tests/unit/steps/test_combine.py` & `distilabel-1.1.0/tests/unit/steps/test_combine.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/steps/test_conversation.py` & `distilabel-1.1.0/tests/unit/steps/formatting/test_conversation.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from distilabel.pipeline.local import Pipeline
-from distilabel.steps.conversation import ConversationTemplate
+from distilabel.steps.formatting.conversation import ConversationTemplate
 
 
 class TestConversationTemplate:
     def test_process(self) -> None:
         conversation_template = ConversationTemplate(
             name="conversation_template",
             pipeline=Pipeline(name="unit-test"),
```

### Comparing `distilabel-1.0.3/tests/unit/steps/test_decorator.py` & `distilabel-1.1.0/tests/unit/steps/test_decorator.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/steps/test_deita.py` & `distilabel-1.1.0/tests/unit/steps/test_deita.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/steps/test_expand.py` & `distilabel-1.1.0/tests/unit/steps/test_expand.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/steps/test_keep.py` & `distilabel-1.1.0/tests/unit/steps/test_keep.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/steps/argilla/__init__.py` & `distilabel-1.1.0/tests/unit/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/steps/argilla/test_base.py` & `distilabel-1.1.0/tests/unit/steps/argilla/test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,23 +67,23 @@
             assert step.name == "step"
             assert step.api_url == "https://example.com"
             assert step.api_key.get_secret_value() == "api.key"  # type: ignore
             assert step.dataset_name == "argilla"
             assert step.dataset_workspace == "argilla"
         assert step.pipeline is pipeline
 
-    def test_with_errors(self) -> None:
-        with pytest.raises(ValueError, match="Step 'step' hasn't received a pipeline"):
-            CustomArgilla(
-                name="step",
-                api_url="https://example.com",
-                api_key="api.key",  # type: ignore
-                dataset_name="argilla",
-                dataset_workspace="argilla",
-            )
+    def test_with_errors(self, caplog) -> None:
+        CustomArgilla(
+            name="step",
+            api_url="https://example.com",
+            api_key="api.key",  # type: ignore
+            dataset_name="argilla",
+            dataset_workspace="argilla",
+        )
+        assert "Step 'step' hasn't received a pipeline" in caplog.text
 
         with pytest.raises(
             TypeError,
             match="Can't instantiate abstract class Argilla with abstract methods inputs, process",
         ):
             Argilla(name="step", pipeline=Pipeline(name="unit-test-pipeline"))  # type: ignore
```

### Comparing `distilabel-1.0.3/tests/unit/steps/argilla/test_preference.py` & `distilabel-1.1.0/tests/unit/steps/argilla/test_preference.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,28 +27,28 @@
             rg.TextField(name="instruction", title="instruction"),  # type: ignore
             rg.TextField(name="generations-0", title="generations-0"),  # type: ignore
             rg.TextField(name="generations-1", title="generations-1"),  # type: ignore
         ],
         questions=[
             rg.RatingQuestion(  # type: ignore
                 name="generations-0-rating",
-                title="Rate generations-0 given instruction based on the annotation guidelines.",
+                title="Rate generations-0 given instruction.",
                 description=None,
                 values=[1, 2, 3, 4, 5],
                 required=True,
             ),
             rg.TextQuestion(  # type: ignore
                 name="generations-0-rationale",
                 title="Specify the rationale for generations-0's rating.",
                 description=None,
                 required=False,
             ),
             rg.RatingQuestion(  # type: ignore
                 name="generations-1-rating",
-                title="Rate generations-1 given instruction based on the annotation guidelines.",
+                title="Rate generations-1 given instruction.",
                 description="Ignore this question if the corresponding `generations-1` field is not available.",
                 values=[1, 2, 3, 4, 5],
                 required=False,
             ),
             rg.TextQuestion(  # type: ignore
                 name="generations-1-rationale",
                 title="Specify the rationale for generations-1's rating.",
```

### Comparing `distilabel-1.0.3/tests/unit/steps/argilla/test_text_generation.py` & `distilabel-1.1.0/tests/unit/steps/argilla/test_text_generation.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/steps/generators/test_data.py` & `distilabel-1.1.0/tests/unit/steps/generators/test_data.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/steps/tasks/__init__.py` & `distilabel-1.1.0/tests/unit/llms/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/steps/tasks/conftest.py` & `distilabel-1.1.0/tests/unit/steps/tasks/conftest.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/steps/tasks/test_base.py` & `distilabel-1.1.0/tests/unit/steps/tasks/test_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,17 +62,17 @@
         with Pipeline(name="unit-test-pipeline") as pipeline:
             llm = DummyLLM()
             task = DummyTask(name="task", llm=llm, pipeline=pipeline)
             assert task.name == "task"
             assert task.llm is llm
         assert task.pipeline == pipeline
 
-    def test_with_errors(self) -> None:
-        with pytest.raises(ValueError, match="Step 'task' hasn't received a pipeline"):
-            DummyTask(name="task", llm=DummyLLM())
+    def test_with_errors(self, caplog: pytest.LogCaptureFixture) -> None:
+        DummyTask(name="task", llm=DummyLLM())
+        assert "Step 'task' hasn't received a pipeline" in caplog.text
 
         with pytest.raises(
             ValidationError, match="llm\n  Field required \\[type=missing"
         ):
             DummyTask(name="task", pipeline=Pipeline(name="unit-test-pipeline"))  # type: ignore
 
         with pytest.raises(
@@ -83,17 +83,29 @@
 
     @pytest.mark.parametrize(
         "group_generations, expected",
         [
             (
                 False,
                 [
-                    {"instruction": "test", "output": "output", "model_name": "test"},
-                    {"instruction": "test", "output": "output", "model_name": "test"},
-                    {"instruction": "test", "output": "output", "model_name": "test"},
+                    {
+                        "instruction": "test",
+                        "output": "output",
+                        "model_name": "test",
+                    },
+                    {
+                        "instruction": "test",
+                        "output": "output",
+                        "model_name": "test",
+                    },
+                    {
+                        "instruction": "test",
+                        "output": "output",
+                        "model_name": "test",
+                    },
                 ],
             ),
             (
                 True,
                 [
                     {
                         "instruction": "test",
@@ -169,19 +181,21 @@
 
     def test_serialization(self) -> None:
         pipeline = Pipeline(name="unit-test-pipeline")
         llm = DummyLLM()
         task = DummyTask(name="task", llm=llm, pipeline=pipeline)
         assert task.dump() == {
             "name": "task",
+            "add_raw_output": False,
             "input_mappings": {},
             "output_mappings": {},
             "input_batch_size": 50,
             "llm": {
                 "generation_kwargs": {},
+                "structured_output": None,
                 "type_info": {
                     "module": "tests.unit.steps.tasks.utils",
                     "name": "DummyLLM",
                 },
             },
             "group_generations": False,
             "num_generations": 1,
```

### Comparing `distilabel-1.0.3/tests/unit/steps/tasks/test_complexity_scorer.py` & `distilabel-1.1.0/tests/unit/steps/tasks/test_complexity_scorer.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/steps/tasks/test_generate_embeddings.py` & `distilabel-1.1.0/tests/unit/steps/tasks/test_generate_embeddings.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/steps/tasks/test_pair_rm.py` & `distilabel-1.1.0/tests/unit/steps/tasks/test_pair_rm.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,30 +38,38 @@
 
         assert ranked == [
             {
                 "input": "Hello, how are you?",
                 "candidates": ["fine", "good", "bad"],
                 "ranks": [2, 1, 3],
                 "ranked_candidates": ["good", "fine", "bad"],
+                "model_name": "llm-blender/PairRM",
             },
             {
                 "input": "Anybody there?",
                 "candidates": ["get out", "yep", "nope"],
                 "ranks": [2, 1, 3],
                 "ranked_candidates": ["yep", "get out", "nope"],
+                "model_name": "llm-blender/PairRM",
             },
         ]
 
     def test_serialization(self, _: MagicMock) -> None:
         ranker = PairRM(
             name="pair_rm_ranker", pipeline=Pipeline(name="unit-test-pipeline")
         )
         assert ranker.dump() == {
             "name": ranker.name,
             "input_mappings": {},
             "output_mappings": {},
             "input_batch_size": ranker.input_batch_size,
             "model": ranker.model,
             "instructions": None,
-            "runtime_parameters_info": [],
+            "runtime_parameters_info": [
+                {
+                    "description": "The number of rows that will contain the batches processed by the step.",
+                    "name": "input_batch_size",
+                    "optional": True,
+                },
+            ],
             "type_info": {"module": "distilabel.steps.tasks.pair_rm", "name": "PairRM"},
         }
```

### Comparing `distilabel-1.0.3/tests/unit/steps/tasks/test_quality_scorer.py` & `distilabel-1.1.0/tests/unit/steps/tasks/test_quality_scorer.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/steps/tasks/test_self_instruct.py` & `distilabel-1.1.0/tests/unit/steps/tasks/test_self_instruct.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/steps/tasks/test_text_generation.py` & `distilabel-1.1.0/tests/unit/steps/tasks/test_genstruct.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,49 +8,72 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from typing import Any, Dict, Union
+
+import pytest
 from distilabel.pipeline.local import Pipeline
-from distilabel.steps.tasks.text_generation import TextGeneration
+from distilabel.steps.tasks.genstruct import Genstruct
 
 from tests.unit.steps.tasks.utils import DummyLLM
 
 
-class TestTextGeneration:
-    def test_format_input_with_str(self) -> None:
-        pipeline = Pipeline(name="unit-test-pipeline")
-        llm = DummyLLM()
-        task = TextGeneration(name="task", llm=llm, pipeline=pipeline)
-
-        assert task.format_input({"instruction": "test"}) == [
-            {"role": "user", "content": "test"}
-        ]
+class TestGenstruct:
+    def test_format_input(self) -> None:
+        task = Genstruct(
+            name="genstruct",
+            llm=DummyLLM(),
+            pipeline=Pipeline(name="unit-test-pipeline"),
+        )
+        task.load()
+
+        result = task.format_input(
+            input={"title": "This is the title.\n", "content": "This is the content.\n"}
+        )
 
-    def test_format_input_with_conversation(self) -> None:
-        pipeline = Pipeline(name="unit-test-pipeline")
-        llm = DummyLLM()
-        task = TextGeneration(name="task", llm=llm, pipeline=pipeline)
-
-        assert task.format_input(
+        assert result == [
             {
-                "instruction": [
-                    {"role": "system", "content": "You're a helpful assistant"},
-                    {"role": "user", "content": "How much is 2+2?"},
-                    {"role": "system", "content": "4"},
-                ]
+                "role": "user",
+                "content": "[[[Title]]] This is the title.\n[[[Content]]] This is the content.\n\nThe following is an interaction between a user and an AI assistant that is related to the above text.\n\n[[[User]]] ",
             }
-        ) == [
-            {"role": "system", "content": "You're a helpful assistant"},
-            {"role": "user", "content": "How much is 2+2?"},
-            {"role": "system", "content": "4"},
         ]
 
-    def test_process(self) -> None:
-        pipeline = Pipeline(name="unit-test-pipeline")
-        llm = DummyLLM()
-        task = TextGeneration(name="task", llm=llm, pipeline=pipeline)
-        assert next(task.process([{"instruction": "test"}])) == [
-            {"instruction": "test", "generation": "output", "model_name": "test"}
-        ]
+    @pytest.mark.parametrize(
+        "output, expected",
+        [
+            (
+                "This is the instruction.\n[[[Assistant]]] This is the response.\n",
+                {
+                    "user": "This is the instruction.",
+                    "assistant": "This is the response.",
+                },
+            ),
+            (
+                None,
+                {"user": None, "assistant": None},
+            ),
+        ],
+    )
+    def test_format_output(
+        self, output: Union[str, None], expected: Dict[str, Any]
+    ) -> None:
+        task = Genstruct(
+            name="genstruct",
+            llm=DummyLLM(),
+            pipeline=Pipeline(name="unit-test-pipeline"),
+        )
+        task.load()
+
+        assert (
+            task.format_output(
+                output=output,
+                input={
+                    "title": "This is the title.\n",
+                    "content": "This is the content.\n",
+                },
+            )
+            == expected
+        )
```

### Comparing `distilabel-1.0.3/tests/unit/steps/tasks/test_ultrafeedback.py` & `distilabel-1.1.0/tests/unit/steps/tasks/test_ultrafeedback.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/steps/tasks/utils.py` & `distilabel-1.1.0/tests/unit/steps/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/steps/tasks/evol_instruct/__init__.py` & `distilabel-1.1.0/tests/unit/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/steps/tasks/evol_instruct/test_base.py` & `distilabel-1.1.0/tests/unit/steps/tasks/evol_instruct/test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,22 +41,24 @@
             task = EvolInstruct(
                 name="task", llm=dummy_llm, num_evolutions=2, pipeline=pipeline
             )
             assert task.name == "task"
             assert task.llm is dummy_llm
         assert task.pipeline == pipeline
 
-    def test_with_errors(self, dummy_llm: LLM) -> None:
+    def test_with_errors(
+        self, caplog: pytest.LogCaptureFixture, dummy_llm: LLM
+    ) -> None:
         with pytest.raises(
             ValidationError, match="num_evolutions\n  Field required \\[type=missing"
         ):
             EvolInstruct(name="task", pipeline=Pipeline(name="unit-test-pipeline"))  # type: ignore
 
-        with pytest.raises(ValueError, match="Step 'task' hasn't received a pipeline"):
-            EvolInstruct(name="task", llm=dummy_llm, num_evolutions=2)
+        EvolInstruct(name="task", llm=dummy_llm, num_evolutions=2)
+        assert "Step 'task' hasn't received a pipeline" in caplog.text
 
     def test_process(self, dummy_llm: LLM) -> None:
         pipeline = Pipeline(name="unit-test-pipeline")
         task = EvolInstruct(
             name="task", llm=dummy_llm, num_evolutions=2, pipeline=pipeline
         )
         task.load()
@@ -115,19 +117,21 @@
         pipeline = Pipeline(name="unit-test-pipeline")
         task = EvolInstruct(
             name="task", llm=dummy_llm, num_evolutions=2, pipeline=pipeline
         )
         task.load()
         assert task.dump() == {
             "name": "task",
+            "add_raw_output": False,
             "input_mappings": task.input_mappings,
             "output_mappings": task.output_mappings,
             "input_batch_size": task.input_batch_size,
             "llm": {
                 "generation_kwargs": {},
+                "structured_output": None,
                 "type_info": {
                     "module": task.llm.__module__,
                     "name": task.llm.__class__.__name__,
                 },
             },
             "group_generations": task.group_generations,
             "num_generations": task.num_generations,
```

### Comparing `distilabel-1.0.3/tests/unit/steps/tasks/evol_instruct/test_generator.py` & `distilabel-1.1.0/tests/unit/steps/tasks/evol_instruct/test_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,24 +41,26 @@
             task = EvolInstructGenerator(
                 name="task", llm=dummy_llm, num_instructions=2, pipeline=pipeline
             )
             assert task.name == "task"
             assert task.llm is dummy_llm
         assert task.pipeline == pipeline
 
-    def test_with_errors(self, dummy_llm: LLM) -> None:
+    def test_with_errors(
+        self, caplog: pytest.LogCaptureFixture, dummy_llm: LLM
+    ) -> None:
         with pytest.raises(
             ValidationError, match="num_instructions\n  Field required \\[type=missing"
         ):
             EvolInstructGenerator(
                 name="task", pipeline=Pipeline(name="unit-test-pipeline")
             )  # type: ignore
 
-        with pytest.raises(ValueError, match="Step 'task' hasn't received a pipeline"):
-            EvolInstructGenerator(name="task", llm=dummy_llm, num_instructions=2)
+        EvolInstructGenerator(name="task", llm=dummy_llm, num_instructions=2)
+        assert "Step 'task' hasn't received a pipeline" in caplog.text
 
     def test_process(self, dummy_llm: LLM) -> None:
         pipeline = Pipeline(name="unit-test-pipeline")
         task = EvolInstructGenerator(
             name="task",
             llm=dummy_llm,
             num_instructions=1,
@@ -111,19 +113,21 @@
         )
         task.load()
 
         assert task.dump() == {
             "name": "task",
             "llm": {
                 "generation_kwargs": {},
+                "structured_output": None,
                 "type_info": {
                     "module": task.llm.__class__.__module__,
                     "name": task.llm.__class__.__name__,
                 },
             },
+            "add_raw_output": False,
             "input_mappings": task.input_mappings,
             "output_mappings": task.output_mappings,
             "batch_size": task.batch_size,
             "num_instructions": task.num_instructions,
             "generate_answers": task.generate_answers,
             "mutation_templates": {
                 "FRESH_START": "Write one question or request containing one or more of the following words: <PROMPT>",
```

### Comparing `distilabel-1.0.3/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/__init__.py` & `distilabel-1.1.0/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_base.py` & `distilabel-1.1.0/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_base.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_generator.py` & `distilabel-1.1.0/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_generator.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/steps/tasks/evol_quality/__init__.py` & `distilabel-1.1.0/tests/unit/steps/argilla/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/steps/tasks/evol_quality/test_base.py` & `distilabel-1.1.0/tests/unit/steps/tasks/evol_quality/test_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,22 +19,24 @@
     EvolQuality,
 )
 from distilabel.steps.tasks.evol_quality.utils import MUTATION_TEMPLATES
 from pydantic import ValidationError
 
 
 class TestEvolQuality:
-    def test_with_errors(self, dummy_llm: LLM) -> None:
+    def test_with_errors(
+        self, caplog: pytest.LogCaptureFixture, dummy_llm: LLM
+    ) -> None:
         with pytest.raises(
             ValidationError, match="num_evolutions\n  Field required \\[type=missing"
         ):
             EvolQuality(name="task", pipeline=Pipeline(name="unit-test-pipeline"))  # type: ignore
 
-        with pytest.raises(ValueError, match="Step 'task' hasn't received a pipeline"):
-            EvolQuality(name="task", llm=dummy_llm, num_evolutions=2)
+        EvolQuality(name="task", llm=dummy_llm, num_evolutions=2)
+        assert "Step 'task' hasn't received a pipeline" in caplog.text
 
     def test_process(self, dummy_llm: LLM) -> None:
         pipeline = Pipeline(name="unit-test-pipeline")
         task = EvolQuality(
             name="task", llm=dummy_llm, num_evolutions=2, pipeline=pipeline
         )
         task.load()
@@ -74,19 +76,21 @@
         pipeline = Pipeline(name="unit-test-pipeline")
         task = EvolQuality(
             name="task", llm=dummy_llm, num_evolutions=2, pipeline=pipeline
         )
         task.load()
         assert task.dump() == {
             "name": "task",
+            "add_raw_output": False,
             "input_mappings": task.input_mappings,
             "output_mappings": task.output_mappings,
             "input_batch_size": task.input_batch_size,
             "llm": {
                 "generation_kwargs": {},
+                "structured_output": None,
                 "type_info": {
                     "module": task.llm.__module__,
                     "name": task.llm.__class__.__name__,
                 },
             },
             "num_evolutions": task.num_evolutions,
             "store_evolutions": task.store_evolutions,
```

### Comparing `distilabel-1.0.3/tests/unit/utils/__init__.py` & `distilabel-1.1.0/tests/unit/steps/tasks/structured_outputs/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/utils/test_chat.py` & `distilabel-1.1.0/tests/unit/utils/test_chat.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/utils/test_lists.py` & `distilabel-1.1.0/tests/unit/utils/test_lists.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/tests/unit/utils/test_typing.py` & `distilabel-1.1.0/tests/unit/utils/test_typing.py`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/.gitignore` & `distilabel-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/LICENSE` & `distilabel-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/LICENSE_HEADER` & `distilabel-1.1.0/LICENSE_HEADER`

 * *Files identical despite different names*

### Comparing `distilabel-1.0.3/README.md` & `distilabel-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 <div align="center">
   <picture>
     <source media="(prefers-color-scheme: dark)" srcset="https://github.com/argilla-io/distilabel/blob/main/docs/assets/distilabel-white.png?raw=true">
     <img alt="Distilabel Logo" src="https://raw.githubusercontent.com/argilla-io/distilabel/main/docs/assets/distilabel-black.png">
   </picture>
 </div>
-<h3 align="center">Synthesize data for AI and add feedback on the fly!</h2>
+
+<h3 align="center">Synthesize data for AI and add feedback on the fly!</h3>
 
 <p align="center">
-<a  href="https://pypi.org/project/distilabel/">
-<img alt="CI" src="https://img.shields.io/pypi/v/distilabel.svg?style=flat-round&logo=pypi&logoColor=white">
-</a>
-<a href="https://pepy.tech/project/distilabel">
-<img alt="CI" src="https://static.pepy.tech/personalized-badge/distilabel?period=month&units=international_system&left_color=grey&right_color=blue&left_text=pypi%20downloads/month">
-</a>
+  <a  href="https://pypi.org/project/distilabel/">
+    <img alt="CI" src="https://img.shields.io/pypi/v/distilabel.svg?style=flat-round&logo=pypi&logoColor=white">
+  </a>
+  <a href="https://pepy.tech/project/distilabel">
+    <img alt="CI" src="https://static.pepy.tech/personalized-badge/distilabel?period=month&units=international_system&left_color=grey&right_color=blue&left_text=pypi%20downloads/month">
+  </a>
 </p>
 
 <p align="center">
-<a href="https://twitter.com/argilla_io">
-<img src="https://img.shields.io/badge/twitter-black?logo=x"/>
-</a>
-<a href="https://www.linkedin.com/company/argilla-io">
-<img src="https://img.shields.io/badge/linkedin-blue?logo=linkedin"/>
-</a>
-<a href="https://join.slack.com/t/rubrixworkspace/shared_invite/zt-whigkyjn-a3IUJLD7gDbTZ0rKlvcJ5g">
-<img src="https://img.shields.io/badge/slack-purple?logo=slack"/>
-</a>
+  <a href="https://twitter.com/argilla_io">
+    <img src="https://img.shields.io/badge/twitter-black?logo=x"/>
+  </a>
+  <a href="https://www.linkedin.com/company/argilla-io">
+    <img src="https://img.shields.io/badge/linkedin-blue?logo=linkedin"/>
+  </a>
+  <a href="https://join.slack.com/t/rubrixworkspace/shared_invite/zt-whigkyjn-a3IUJLD7gDbTZ0rKlvcJ5g">
+    <img src="https://img.shields.io/badge/slack-purple?logo=slack"/>
+  </a>
 </p>
 
+
 Distilabel is the **framework for synthetic data and AI feedback for AI engineers** that require **high-quality outputs, full data ownership, and overall efficiency**.
 
 If you just want to get started, we recommend you check the [documentation](http://distilabel.argilla.io/). Curious, and want to know more? Keep reading!
 <!-- ![overview](https://github.com/argilla-io/distilabel/assets/36760800/360110da-809d-4e24-a29b-1a1a8bc4f9b7)  -->
 
 ## Why use Distilabel?
 
@@ -75,14 +77,15 @@
 Requires Python 3.8+
 
 In addition, the following extras are available:
 
 - `anthropic`: for using models available in [Anthropic API](https://www.anthropic.com/api) via the `AnthropicLLM` integration.
 - `cohere`: for using models available in [Cohere](https://cohere.ai/) via the `CohereLLM` integration.
 - `argilla`: for exporting the generated datasets to [Argilla](https://argilla.io/).
+- `groq`: for using models available in [Groq](https://groq.com/) using [`groq`](https://github.com/groq/groq-python) Python client via the `GroqLLM` integration.
 - `hf-inference-endpoints`: for using the [Hugging Face Inference Endpoints](https://huggingface.co/inference-endpoints) via the `InferenceEndpointsLLM` integration.
 - `hf-transformers`: for using models available in [transformers](https://github.com/huggingface/transformers) package via the `TransformersLLM` integration.
 - `litellm`: for using [`LiteLLM`](https://github.com/BerriAI/litellm) to call any LLM using OpenAI format via the `LiteLLM` integration.
 - `llama-cpp`: for using [llama-cpp-python](https://github.com/abetlen/llama-cpp-python) Python bindings for `llama.cpp` via the `LlamaCppLLM` integration.
 - `mistralai`: for using models available in [Mistral AI API](https://mistral.ai/news/la-plateforme/) via the `MistralAILLM` integration.
 - `ollama`: for using [Ollama](https://ollama.com/) and their available models via `OllamaLLM` integration.
 - `openai`: for using [OpenAI API](https://openai.com/blog/openai-api) models via the `OpenAILLM` integration, or the rest of the integrations based on OpenAI and relying on its client as `AnyscaleLLM`, `AzureOpenAILLM`, and `TogetherLLM`.
@@ -105,33 +108,28 @@
 from distilabel.steps import LoadHubDataset
 from distilabel.steps.tasks import TextGeneration
 
 with Pipeline(
     name="simple-text-generation-pipeline",
     description="A simple text generation pipeline",
 ) as pipeline:
-    load_dataset = LoadHubDataset(
-        name="load_dataset",
-        output_mappings={"prompt": "instruction"},
-    )
-
-    generate_with_openai = TextGeneration(
-        name="generate_with_gpt35", llm=OpenAILLM(model="gpt-3.5-turbo")
-    )
+    load_dataset = LoadHubDataset(output_mappings={"prompt": "instruction"})
+
+    generate_with_openai = TextGeneration(llm=OpenAILLM(model="gpt-3.5-turbo"))
 
     load_dataset.connect(generate_with_openai)
 
 if __name__ == "__main__":
     distiset = pipeline.run(
         parameters={
-            "load_dataset": {
+            load_dataset.name: {
                 "repo_id": "distilabel-internal-testing/instruction-dataset-mini",
                 "split": "test",
             },
-            "generate_with_gpt35": {
+            generate_with_openai.name: {
                 "llm": {
                     "generation_kwargs": {
                         "temperature": 0.7,
                         "max_new_tokens": 512,
                     }
                 }
             },
```

#### html2text {}

 * *error from `html2text {}` (a):*

 * *File "/tmp/diffoscope_t8_gf1y__/tmpz4hwj601_TarContainer/0/253.md", line 7, column 75: Levels of opening and closing headings don't match*

```diff
@@ -49,18 +49,20 @@
 latest research papers** to improve the quality of the dataset. ##
 ð¨ð½âð» Installation ```sh pip install distilabel --upgrade ```
 Requires Python 3.8+ In addition, the following extras are available: -
 `anthropic`: for using models available in [Anthropic API](https://
 www.anthropic.com/api) via the `AnthropicLLM` integration. - `cohere`: for
 using models available in [Cohere](https://cohere.ai/) via the `CohereLLM`
 integration. - `argilla`: for exporting the generated datasets to [Argilla]
-(https://argilla.io/). - `hf-inference-endpoints`: for using the [Hugging Face
-Inference Endpoints](https://huggingface.co/inference-endpoints) via the
-`InferenceEndpointsLLM` integration. - `hf-transformers`: for using models
-available in [transformers](https://github.com/huggingface/transformers)
+(https://argilla.io/). - `groq`: for using models available in [Groq](https://
+groq.com/) using [`groq`](https://github.com/groq/groq-python) Python client
+via the `GroqLLM` integration. - `hf-inference-endpoints`: for using the
+[Hugging Face Inference Endpoints](https://huggingface.co/inference-endpoints)
+via the `InferenceEndpointsLLM` integration. - `hf-transformers`: for using
+models available in [transformers](https://github.com/huggingface/transformers)
 package via the `TransformersLLM` integration. - `litellm`: for using
 [`LiteLLM`](https://github.com/BerriAI/litellm) to call any LLM using OpenAI
 format via the `LiteLLM` integration. - `llama-cpp`: for using [llama-cpp-
 python](https://github.com/abetlen/llama-cpp-python) Python bindings for
 `llama.cpp` via the `LlamaCppLLM` integration. - `mistralai`: for using models
 available in [Mistral AI API](https://mistral.ai/news/la-plateforme/) via the
 `MistralAILLM` integration. - `ollama`: for using [Ollama](https://ollama.com/
@@ -73,24 +75,23 @@
 github.com/vllm-project/vllm) serving engine via the `vLLM` integration. ###
 Example To run the following example you must install `distilabel` with both
 `openai` extra: ```sh pip install "distilabel[openai]" --upgrade ``` Then run:
 ```python from distilabel.llms import OpenAILLM from distilabel.pipeline import
 Pipeline from distilabel.steps import LoadHubDataset from
 distilabel.steps.tasks import TextGeneration with Pipeline( name="simple-text-
 generation-pipeline", description="A simple text generation pipeline", ) as
-pipeline: load_dataset = LoadHubDataset( name="load_dataset", output_mappings=
-{"prompt": "instruction"}, ) generate_with_openai = TextGeneration
-( name="generate_with_gpt35", llm=OpenAILLM(model="gpt-3.5-turbo") )
-load_dataset.connect(generate_with_openai) if __name__ == "__main__": distiset
-= pipeline.run( parameters={ "load_dataset": { "repo_id": "distilabel-internal-
-testing/instruction-dataset-mini", "split": "test", }, "generate_with_gpt35":
-{ "llm": { "generation_kwargs": { "temperature": 0.7, "max_new_tokens": 512, }
-} }, }, ) ``` ## Badges If you build something cool with `distilabel` consider
-adding one of these badges to your dataset or model card. [[Built with
-Distilabel]](https://github.com/argilla-io/distilabel) [[Built with
-Distilabel]](https://github.com/argilla-io/distilabel) [[Built with
-Distilabel]](https://github.com/argilla-io/distilabel) [[Built with
-Distilabel]](https://github.com/argilla-io/distilabel) ## Contribute To
-directly contribute with `distilabel`, check our [good first issues](https://
-github.com/argilla-io/distilabel/
+pipeline: load_dataset = LoadHubDataset(output_mappings={"prompt":
+"instruction"}) generate_with_openai = TextGeneration(llm=OpenAILLM(model="gpt-
+3.5-turbo")) load_dataset.connect(generate_with_openai) if __name__ ==
+"__main__": distiset = pipeline.run( parameters={ load_dataset.name:
+{ "repo_id": "distilabel-internal-testing/instruction-dataset-mini", "split":
+"test", }, generate_with_openai.name: { "llm": { "generation_kwargs":
+{ "temperature": 0.7, "max_new_tokens": 512, } } }, }, ) ``` ## Badges If you
+build something cool with `distilabel` consider adding one of these badges to
+your dataset or model card. [[Built with Distilabel]](https://github.com/
+argilla-io/distilabel) [[Built with Distilabel]](https://github.com/argilla-io/
+distilabel) [[Built with Distilabel]](https://github.com/argilla-io/distilabel)
+[[Built with Distilabel]](https://github.com/argilla-io/distilabel) ##
+Contribute To directly contribute with `distilabel`, check our [good first
+issues](https://github.com/argilla-io/distilabel/
 issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22) or [open a new
 one](https://github.com/argilla-io/distilabel/issues/new/choose).
```

### Comparing `distilabel-1.0.3/pyproject.toml` & `distilabel-1.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "distilabel"
-description = "AI Feedback (AIF) framework"
+description = "Distilabel is an AI Feedback (AIF) framework for building datasets with and for LLMs."
 readme = "README.md"
 requires-python = ">=3.8"
-license = "MIT"
+license = "Apache-2.0"
 keywords = ["llm", "annotation", "alignment", "synthetic", "data", "rlaif"]
 authors = [{ name = "Argilla", email = "admin@argilla.io" }]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
@@ -35,40 +35,45 @@
     "tblib >= 3.0.0",
 ]
 dynamic = ["version"]
 
 [project.scripts]
 distilabel = "distilabel.cli.app:app"
 
+[project.entry-points."mkdocs.plugins"]
+"distilabel/components-gallery" = "distilabel.utils.mkdocs.components_gallery:ComponentsGalleryPlugin"
+
 [project.optional-dependencies]
 dev = ["ruff == 0.2.2", "pre-commit >= 3.5.0"]
 docs = [
     "mkdocs-material >= 9.5.0",
     "mkdocstrings[python] >= 0.24.0",
     "mkdocs-literate-nav >= 0.6.1",
     "mkdocs-section-index >= 0.3.8",
     "mkdocs-gen-files >= 0.5.0",
     "mike >= 2.0.0",
     "Pillow >= 9.5.0",
     "CairoSVG >= 2.7.1",
     "mknotebooks >= 0.8.0",
 ]
-tests = ["pytest >= 7.4.0", "pytest-asyncio", "nest-asyncio"]
+tests = ["pytest >= 7.4.0", "pytest-asyncio", "nest-asyncio", "pytest-timeout"]
 
 # Optional LLMs, integrations, etc
 anthropic = ["anthropic >= 0.20.0"]
 argilla = ["argilla >= 1.23.0"]
 cohere = ["cohere >= 5.2.0"]
+groq = ["groq >= 0.4.1"]
 hf-inference-endpoints = ["huggingface_hub >= 0.19.0"]
 hf-transformers = ["transformers >= 4.34.1", "torch >= 2.0.0"]
 litellm = ["litellm >= 1.30.0"]
 llama-cpp = ["llama-cpp-python >= 0.2.0"]
 mistralai = ["mistralai >= 0.1.0"]
 ollama = ["ollama >= 0.1.7"]
 openai = ["openai >= 1.0.0"]
+outlines = ["outlines >= 0.0.40"]
 vertexai = ["google-cloud-aiplatform >= 1.38.0"]
 vllm = ["vllm >= 0.2.1", "filelock >= 3.13.4"]
 
 [project.urls]
 Documentation = "https://distilabel.argilla.io/"
 Issues = "https://github.com/argilla/distilabel/issues"
 Source = "https://github.com/argilla/distilabel"
```

### Comparing `distilabel-1.0.3/PKG-INFO` & `distilabel-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.3
 Name: distilabel
-Version: 1.0.3
-Summary: AI Feedback (AIF) framework
+Version: 1.1.0
+Summary: Distilabel is an AI Feedback (AIF) framework for building datasets with and for LLMs.
 Project-URL: Documentation, https://distilabel.argilla.io/
 Project-URL: Issues, https://github.com/argilla/distilabel/issues
 Project-URL: Source, https://github.com/argilla/distilabel
 Author-email: Argilla <admin@argilla.io>
-License-Expression: MIT
+License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: LICENSE_HEADER
 Keywords: alignment,annotation,data,llm,rlaif,synthetic
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -46,14 +46,16 @@
 Requires-Dist: mkdocs-gen-files>=0.5.0; extra == 'docs'
 Requires-Dist: mkdocs-literate-nav>=0.6.1; extra == 'docs'
 Requires-Dist: mkdocs-material>=9.5.0; extra == 'docs'
 Requires-Dist: mkdocs-section-index>=0.3.8; extra == 'docs'
 Requires-Dist: mkdocstrings[python]>=0.24.0; extra == 'docs'
 Requires-Dist: mknotebooks>=0.8.0; extra == 'docs'
 Requires-Dist: pillow>=9.5.0; extra == 'docs'
+Provides-Extra: groq
+Requires-Dist: groq>=0.4.1; extra == 'groq'
 Provides-Extra: hf-inference-endpoints
 Requires-Dist: huggingface-hub>=0.19.0; extra == 'hf-inference-endpoints'
 Provides-Extra: hf-transformers
 Requires-Dist: torch>=2.0.0; extra == 'hf-transformers'
 Requires-Dist: transformers>=4.34.1; extra == 'hf-transformers'
 Provides-Extra: litellm
 Requires-Dist: litellm>=1.30.0; extra == 'litellm'
@@ -61,54 +63,59 @@
 Requires-Dist: llama-cpp-python>=0.2.0; extra == 'llama-cpp'
 Provides-Extra: mistralai
 Requires-Dist: mistralai>=0.1.0; extra == 'mistralai'
 Provides-Extra: ollama
 Requires-Dist: ollama>=0.1.7; extra == 'ollama'
 Provides-Extra: openai
 Requires-Dist: openai>=1.0.0; extra == 'openai'
+Provides-Extra: outlines
+Requires-Dist: outlines>=0.0.40; extra == 'outlines'
 Provides-Extra: tests
 Requires-Dist: nest-asyncio; extra == 'tests'
 Requires-Dist: pytest-asyncio; extra == 'tests'
+Requires-Dist: pytest-timeout; extra == 'tests'
 Requires-Dist: pytest>=7.4.0; extra == 'tests'
 Provides-Extra: vertexai
 Requires-Dist: google-cloud-aiplatform>=1.38.0; extra == 'vertexai'
 Provides-Extra: vllm
 Requires-Dist: filelock>=3.13.4; extra == 'vllm'
 Requires-Dist: vllm>=0.2.1; extra == 'vllm'
 Description-Content-Type: text/markdown
 
 <div align="center">
   <picture>
     <source media="(prefers-color-scheme: dark)" srcset="https://github.com/argilla-io/distilabel/blob/main/docs/assets/distilabel-white.png?raw=true">
     <img alt="Distilabel Logo" src="https://raw.githubusercontent.com/argilla-io/distilabel/main/docs/assets/distilabel-black.png">
   </picture>
 </div>
-<h3 align="center">Synthesize data for AI and add feedback on the fly!</h2>
+
+<h3 align="center">Synthesize data for AI and add feedback on the fly!</h3>
 
 <p align="center">
-<a  href="https://pypi.org/project/distilabel/">
-<img alt="CI" src="https://img.shields.io/pypi/v/distilabel.svg?style=flat-round&logo=pypi&logoColor=white">
-</a>
-<a href="https://pepy.tech/project/distilabel">
-<img alt="CI" src="https://static.pepy.tech/personalized-badge/distilabel?period=month&units=international_system&left_color=grey&right_color=blue&left_text=pypi%20downloads/month">
-</a>
+  <a  href="https://pypi.org/project/distilabel/">
+    <img alt="CI" src="https://img.shields.io/pypi/v/distilabel.svg?style=flat-round&logo=pypi&logoColor=white">
+  </a>
+  <a href="https://pepy.tech/project/distilabel">
+    <img alt="CI" src="https://static.pepy.tech/personalized-badge/distilabel?period=month&units=international_system&left_color=grey&right_color=blue&left_text=pypi%20downloads/month">
+  </a>
 </p>
 
 <p align="center">
-<a href="https://twitter.com/argilla_io">
-<img src="https://img.shields.io/badge/twitter-black?logo=x"/>
-</a>
-<a href="https://www.linkedin.com/company/argilla-io">
-<img src="https://img.shields.io/badge/linkedin-blue?logo=linkedin"/>
-</a>
-<a href="https://join.slack.com/t/rubrixworkspace/shared_invite/zt-whigkyjn-a3IUJLD7gDbTZ0rKlvcJ5g">
-<img src="https://img.shields.io/badge/slack-purple?logo=slack"/>
-</a>
+  <a href="https://twitter.com/argilla_io">
+    <img src="https://img.shields.io/badge/twitter-black?logo=x"/>
+  </a>
+  <a href="https://www.linkedin.com/company/argilla-io">
+    <img src="https://img.shields.io/badge/linkedin-blue?logo=linkedin"/>
+  </a>
+  <a href="https://join.slack.com/t/rubrixworkspace/shared_invite/zt-whigkyjn-a3IUJLD7gDbTZ0rKlvcJ5g">
+    <img src="https://img.shields.io/badge/slack-purple?logo=slack"/>
+  </a>
 </p>
 
+
 Distilabel is the **framework for synthetic data and AI feedback for AI engineers** that require **high-quality outputs, full data ownership, and overall efficiency**.
 
 If you just want to get started, we recommend you check the [documentation](http://distilabel.argilla.io/). Curious, and want to know more? Keep reading!
 <!-- ![overview](https://github.com/argilla-io/distilabel/assets/36760800/360110da-809d-4e24-a29b-1a1a8bc4f9b7)  -->
 
 ## Why use Distilabel?
 
@@ -153,14 +160,15 @@
 Requires Python 3.8+
 
 In addition, the following extras are available:
 
 - `anthropic`: for using models available in [Anthropic API](https://www.anthropic.com/api) via the `AnthropicLLM` integration.
 - `cohere`: for using models available in [Cohere](https://cohere.ai/) via the `CohereLLM` integration.
 - `argilla`: for exporting the generated datasets to [Argilla](https://argilla.io/).
+- `groq`: for using models available in [Groq](https://groq.com/) using [`groq`](https://github.com/groq/groq-python) Python client via the `GroqLLM` integration.
 - `hf-inference-endpoints`: for using the [Hugging Face Inference Endpoints](https://huggingface.co/inference-endpoints) via the `InferenceEndpointsLLM` integration.
 - `hf-transformers`: for using models available in [transformers](https://github.com/huggingface/transformers) package via the `TransformersLLM` integration.
 - `litellm`: for using [`LiteLLM`](https://github.com/BerriAI/litellm) to call any LLM using OpenAI format via the `LiteLLM` integration.
 - `llama-cpp`: for using [llama-cpp-python](https://github.com/abetlen/llama-cpp-python) Python bindings for `llama.cpp` via the `LlamaCppLLM` integration.
 - `mistralai`: for using models available in [Mistral AI API](https://mistral.ai/news/la-plateforme/) via the `MistralAILLM` integration.
 - `ollama`: for using [Ollama](https://ollama.com/) and their available models via `OllamaLLM` integration.
 - `openai`: for using [OpenAI API](https://openai.com/blog/openai-api) models via the `OpenAILLM` integration, or the rest of the integrations based on OpenAI and relying on its client as `AnyscaleLLM`, `AzureOpenAILLM`, and `TogetherLLM`.
@@ -183,33 +191,28 @@
 from distilabel.steps import LoadHubDataset
 from distilabel.steps.tasks import TextGeneration
 
 with Pipeline(
     name="simple-text-generation-pipeline",
     description="A simple text generation pipeline",
 ) as pipeline:
-    load_dataset = LoadHubDataset(
-        name="load_dataset",
-        output_mappings={"prompt": "instruction"},
-    )
-
-    generate_with_openai = TextGeneration(
-        name="generate_with_gpt35", llm=OpenAILLM(model="gpt-3.5-turbo")
-    )
+    load_dataset = LoadHubDataset(output_mappings={"prompt": "instruction"})
+
+    generate_with_openai = TextGeneration(llm=OpenAILLM(model="gpt-3.5-turbo"))
 
     load_dataset.connect(generate_with_openai)
 
 if __name__ == "__main__":
     distiset = pipeline.run(
         parameters={
-            "load_dataset": {
+            load_dataset.name: {
                 "repo_id": "distilabel-internal-testing/instruction-dataset-mini",
                 "split": "test",
             },
-            "generate_with_gpt35": {
+            generate_with_openai.name: {
                 "llm": {
                     "generation_kwargs": {
                         "temperature": 0.7,
                         "max_new_tokens": 512,
                     }
                 }
             },
```

#### html2text {}

 * *error from `html2text {}` (a):*

 * *File "/tmp/diffoscope_t8_gf1y__/tmpz4hwj601_TarContainer/0/255", line 85, column 75: Levels of opening and closing headings don't match*

```diff
@@ -1,12 +1,13 @@
-Metadata-Version: 2.3 Name: distilabel Version: 1.0.3 Summary: AI Feedback
-(AIF) framework Project-URL: Documentation, https://distilabel.argilla.io/
-Project-URL: Issues, https://github.com/argilla/distilabel/issues Project-URL:
-Source, https://github.com/argilla/distilabel Author-email: Argilla
-argilla.io> License-Expression: MIT License-File: LICENSE License-File:
+Metadata-Version: 2.3 Name: distilabel Version: 1.1.0 Summary: Distilabel is an
+AI Feedback (AIF) framework for building datasets with and for LLMs. Project-
+URL: Documentation, https://distilabel.argilla.io/ Project-URL: Issues, https:/
+/github.com/argilla/distilabel/issues Project-URL: Source, https://github.com/
+argilla/distilabel Author-email: Argilla
+argilla.io> License-Expression: Apache-2.0 License-File: LICENSE License-File:
 LICENSE_HEADER Keywords: alignment,annotation,data,llm,rlaif,synthetic
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.8
@@ -22,28 +23,31 @@
 Requires-Dist: ruff==0.2.2; extra == 'dev' Provides-Extra: docs Requires-Dist:
 cairosvg>=2.7.1; extra == 'docs' Requires-Dist: mike>=2.0.0; extra == 'docs'
 Requires-Dist: mkdocs-gen-files>=0.5.0; extra == 'docs' Requires-Dist: mkdocs-
 literate-nav>=0.6.1; extra == 'docs' Requires-Dist: mkdocs-material>=9.5.0;
 extra == 'docs' Requires-Dist: mkdocs-section-index>=0.3.8; extra == 'docs'
 Requires-Dist: mkdocstrings[python]>=0.24.0; extra == 'docs' Requires-Dist:
 mknotebooks>=0.8.0; extra == 'docs' Requires-Dist: pillow>=9.5.0; extra ==
-'docs' Provides-Extra: hf-inference-endpoints Requires-Dist: huggingface-
-hub>=0.19.0; extra == 'hf-inference-endpoints' Provides-Extra: hf-transformers
-Requires-Dist: torch>=2.0.0; extra == 'hf-transformers' Requires-Dist:
+'docs' Provides-Extra: groq Requires-Dist: groq>=0.4.1; extra == 'groq'
+Provides-Extra: hf-inference-endpoints Requires-Dist: huggingface-hub>=0.19.0;
+extra == 'hf-inference-endpoints' Provides-Extra: hf-transformers Requires-
+Dist: torch>=2.0.0; extra == 'hf-transformers' Requires-Dist:
 transformers>=4.34.1; extra == 'hf-transformers' Provides-Extra: litellm
 Requires-Dist: litellm>=1.30.0; extra == 'litellm' Provides-Extra: llama-cpp
 Requires-Dist: llama-cpp-python>=0.2.0; extra == 'llama-cpp' Provides-Extra:
 mistralai Requires-Dist: mistralai>=0.1.0; extra == 'mistralai' Provides-Extra:
 ollama Requires-Dist: ollama>=0.1.7; extra == 'ollama' Provides-Extra: openai
-Requires-Dist: openai>=1.0.0; extra == 'openai' Provides-Extra: tests Requires-
-Dist: nest-asyncio; extra == 'tests' Requires-Dist: pytest-asyncio; extra ==
-'tests' Requires-Dist: pytest>=7.4.0; extra == 'tests' Provides-Extra: vertexai
-Requires-Dist: google-cloud-aiplatform>=1.38.0; extra == 'vertexai' Provides-
-Extra: vllm Requires-Dist: filelock>=3.13.4; extra == 'vllm' Requires-Dist:
-vllm>=0.2.1; extra == 'vllm' Description-Content-Type: text/markdown
+Requires-Dist: openai>=1.0.0; extra == 'openai' Provides-Extra: outlines
+Requires-Dist: outlines>=0.0.40; extra == 'outlines' Provides-Extra: tests
+Requires-Dist: nest-asyncio; extra == 'tests' Requires-Dist: pytest-asyncio;
+extra == 'tests' Requires-Dist: pytest-timeout; extra == 'tests' Requires-Dist:
+pytest>=7.4.0; extra == 'tests' Provides-Extra: vertexai Requires-Dist: google-
+cloud-aiplatform>=1.38.0; extra == 'vertexai' Provides-Extra: vllm Requires-
+Dist: filelock>=3.13.4; extra == 'vllm' Requires-Dist: vllm>=0.2.1; extra ==
+'vllm' Description-Content-Type: text/markdown
                                [Distilabel Logo]
          ******** SSyynntthheessiizzee ddaattaa ffoorr AAII aanndd aadddd ffeeeeddbbaacckk oonn tthhee ffllyy!! ********
                                    _[_C_I_]_[_C_I_]
   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_t_w_i_t_t_e_r_-_b_l_a_c_k_?_l_o_g_o_=_x_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
     _b_a_d_g_e_/_l_i_n_k_e_d_i_n_-_b_l_u_e_?_l_o_g_o_=_l_i_n_k_e_d_i_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_s_l_a_c_k_-
                               _p_u_r_p_l_e_?_l_o_g_o_=_s_l_a_c_k_]
 Distilabel is the **framework for synthetic data and AI feedback for AI
@@ -91,18 +95,20 @@
 latest research papers** to improve the quality of the dataset. ##
 ð¨ð½âð» Installation ```sh pip install distilabel --upgrade ```
 Requires Python 3.8+ In addition, the following extras are available: -
 `anthropic`: for using models available in [Anthropic API](https://
 www.anthropic.com/api) via the `AnthropicLLM` integration. - `cohere`: for
 using models available in [Cohere](https://cohere.ai/) via the `CohereLLM`
 integration. - `argilla`: for exporting the generated datasets to [Argilla]
-(https://argilla.io/). - `hf-inference-endpoints`: for using the [Hugging Face
-Inference Endpoints](https://huggingface.co/inference-endpoints) via the
-`InferenceEndpointsLLM` integration. - `hf-transformers`: for using models
-available in [transformers](https://github.com/huggingface/transformers)
+(https://argilla.io/). - `groq`: for using models available in [Groq](https://
+groq.com/) using [`groq`](https://github.com/groq/groq-python) Python client
+via the `GroqLLM` integration. - `hf-inference-endpoints`: for using the
+[Hugging Face Inference Endpoints](https://huggingface.co/inference-endpoints)
+via the `InferenceEndpointsLLM` integration. - `hf-transformers`: for using
+models available in [transformers](https://github.com/huggingface/transformers)
 package via the `TransformersLLM` integration. - `litellm`: for using
 [`LiteLLM`](https://github.com/BerriAI/litellm) to call any LLM using OpenAI
 format via the `LiteLLM` integration. - `llama-cpp`: for using [llama-cpp-
 python](https://github.com/abetlen/llama-cpp-python) Python bindings for
 `llama.cpp` via the `LlamaCppLLM` integration. - `mistralai`: for using models
 available in [Mistral AI API](https://mistral.ai/news/la-plateforme/) via the
 `MistralAILLM` integration. - `ollama`: for using [Ollama](https://ollama.com/
@@ -115,24 +121,23 @@
 github.com/vllm-project/vllm) serving engine via the `vLLM` integration. ###
 Example To run the following example you must install `distilabel` with both
 `openai` extra: ```sh pip install "distilabel[openai]" --upgrade ``` Then run:
 ```python from distilabel.llms import OpenAILLM from distilabel.pipeline import
 Pipeline from distilabel.steps import LoadHubDataset from
 distilabel.steps.tasks import TextGeneration with Pipeline( name="simple-text-
 generation-pipeline", description="A simple text generation pipeline", ) as
-pipeline: load_dataset = LoadHubDataset( name="load_dataset", output_mappings=
-{"prompt": "instruction"}, ) generate_with_openai = TextGeneration
-( name="generate_with_gpt35", llm=OpenAILLM(model="gpt-3.5-turbo") )
-load_dataset.connect(generate_with_openai) if __name__ == "__main__": distiset
-= pipeline.run( parameters={ "load_dataset": { "repo_id": "distilabel-internal-
-testing/instruction-dataset-mini", "split": "test", }, "generate_with_gpt35":
-{ "llm": { "generation_kwargs": { "temperature": 0.7, "max_new_tokens": 512, }
-} }, }, ) ``` ## Badges If you build something cool with `distilabel` consider
-adding one of these badges to your dataset or model card. [[Built with
-Distilabel]](https://github.com/argilla-io/distilabel) [[Built with
-Distilabel]](https://github.com/argilla-io/distilabel) [[Built with
-Distilabel]](https://github.com/argilla-io/distilabel) [[Built with
-Distilabel]](https://github.com/argilla-io/distilabel) ## Contribute To
-directly contribute with `distilabel`, check our [good first issues](https://
-github.com/argilla-io/distilabel/
+pipeline: load_dataset = LoadHubDataset(output_mappings={"prompt":
+"instruction"}) generate_with_openai = TextGeneration(llm=OpenAILLM(model="gpt-
+3.5-turbo")) load_dataset.connect(generate_with_openai) if __name__ ==
+"__main__": distiset = pipeline.run( parameters={ load_dataset.name:
+{ "repo_id": "distilabel-internal-testing/instruction-dataset-mini", "split":
+"test", }, generate_with_openai.name: { "llm": { "generation_kwargs":
+{ "temperature": 0.7, "max_new_tokens": 512, } } }, }, ) ``` ## Badges If you
+build something cool with `distilabel` consider adding one of these badges to
+your dataset or model card. [[Built with Distilabel]](https://github.com/
+argilla-io/distilabel) [[Built with Distilabel]](https://github.com/argilla-io/
+distilabel) [[Built with Distilabel]](https://github.com/argilla-io/distilabel)
+[[Built with Distilabel]](https://github.com/argilla-io/distilabel) ##
+Contribute To directly contribute with `distilabel`, check our [good first
+issues](https://github.com/argilla-io/distilabel/
 issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22) or [open a new
 one](https://github.com/argilla-io/distilabel/issues/new/choose).
```

