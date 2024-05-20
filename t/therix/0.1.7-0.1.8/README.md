# Comparing `tmp/therix-0.1.7.tar.gz` & `tmp/therix-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "therix-0.1.7.tar", max compression
+gzip compressed data, was "therix-0.1.8.tar", max compression
```

## Comparing `therix-0.1.7.tar` & `therix-0.1.8.tar`

### file list

```diff
@@ -1,118 +1,119 @@
--rw-r--r--   0        0        0     1068 2024-03-20 09:19:32.105170 therix-0.1.7/LICENSE
--rw-r--r--   0        0        0     1218 2024-04-16 12:12:31.272029 therix-0.1.7/README.md
--rw-r--r--   0        0        0     1048 2024-05-14 09:55:14.710919 therix-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.275037 therix-0.1.7/therix/__init__.py
--rw-r--r--   0        0        0       38 2024-04-26 09:41:57.771370 therix-0.1.7/therix/alembic/README
--rw-r--r--   0        0        0     2912 2024-04-26 09:41:57.771506 therix-0.1.7/therix/alembic/env.py
--rw-r--r--   0        0        0      635 2024-04-26 09:41:57.771730 therix-0.1.7/therix/alembic/script.py.mako
--rw-r--r--   0        0        0     2619 2024-04-29 11:17:18.463236 therix-0.1.7/therix/alembic/versions/2024_04_26_0914-739c7981bdd8_added_config_type_for_cache_config.py
--rw-r--r--   0        0        0     2131 2024-05-03 12:50:17.295513 therix-0.1.7/therix/alembic/versions/2024_04_26_1644-b8fe483b5a71_add_type_column_in_pipeline_table.py
--rw-r--r--   0        0        0      880 2024-05-08 11:24:55.867083 therix-0.1.7/therix/alembic/versions/2024_05_06_1524-1e7f3dc15e9c_added_chat_history_fix.py
--rw-r--r--   0        0        0     2614 2024-05-14 09:23:25.311332 therix-0.1.7/therix/alembic/versions/2024_05_13_1842-f5c4562bcd86_added_config_type_for_system_prompt.py
--rw-r--r--   0        0        0     3092 2024-04-26 10:10:45.584242 therix-0.1.7/therix/alembic/versions/f5fb392e6b0a_initial_database_setup.py
--rw-r--r--   0        0        0     3599 2024-04-26 09:41:57.771233 therix-0.1.7/therix/alembic.ini
--rw-r--r--   0        0        0     2083 2024-04-16 12:12:31.275418 therix-0.1.7/therix/core/JSONLoader.py
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.275458 therix-0.1.7/therix/core/__init__.py
--rw-r--r--   0        0        0     2737 2024-05-13 10:00:13.299373 therix-0.1.7/therix/core/cache.py
--rw-r--r--   0        0        0     1399 2024-05-13 10:00:13.301278 therix-0.1.7/therix/core/chat_history/base_chat_history.py
--rw-r--r--   0        0        0     1649 2024-05-13 10:00:13.301411 therix-0.1.7/therix/core/constants.py
--rw-r--r--   0        0        0      854 2024-04-16 12:12:31.275897 therix-0.1.7/therix/core/data_sources.py
--rw-r--r--   0        0        0     1676 2024-04-16 12:12:31.276049 therix-0.1.7/therix/core/embedding_models.py
--rw-r--r--   0        0        0     2374 2024-05-13 10:00:13.301910 therix-0.1.7/therix/core/inference_models.py
--rw-r--r--   0        0        0      317 2024-05-13 10:00:13.302010 therix-0.1.7/therix/core/output_parser.py
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.276202 therix-0.1.7/therix/core/output_source.py
--rw-r--r--   0        0        0      251 2024-04-26 09:41:57.772340 therix-0.1.7/therix/core/pii_filter_config.py
--rw-r--r--   0        0        0     6884 2024-05-14 09:23:25.312293 therix-0.1.7/therix/core/pipeline.py
--rw-r--r--   0        0        0     1153 2024-04-16 12:12:31.276619 therix-0.1.7/therix/core/pipeline_component.py
--rw-r--r--   0        0        0      238 2024-05-08 11:24:55.868662 therix-0.1.7/therix/core/response.py
--rw-r--r--   0        0        0      594 2024-05-13 10:00:13.302774 therix-0.1.7/therix/core/summarizer_config.py
--rw-r--r--   0        0        0       98 2024-05-13 10:00:13.302847 therix-0.1.7/therix/core/summarizer_output_model.py
--rw-r--r--   0        0        0      328 2024-05-14 09:23:25.312543 therix-0.1.7/therix/core/system_prompt_config.py
--rw-r--r--   0        0        0      299 2024-04-16 12:12:31.276847 therix-0.1.7/therix/core/trace.py
--rw-r--r--   0        0        0        0 2024-04-23 08:07:48.247669 therix-0.1.7/therix/db/__init__.py
--rw-r--r--   0        0        0     3757 2024-05-14 09:52:11.737008 therix-0.1.7/therix/db/db_manager.py
--rw-r--r--   0        0        0      412 2024-04-26 09:41:57.773326 therix-0.1.7/therix/db/session.py
--rw-r--r--   0        0        0        0 2024-04-26 09:41:57.773383 therix-0.1.7/therix/db/tests/__init__.py
--rw-r--r--   0        0        0     1895 2024-04-26 09:41:57.773575 therix-0.1.7/therix/db/tests/test_db_manager.py
--rw-r--r--   0        0        0      235 2024-05-03 05:53:02.647293 therix-0.1.7/therix/docs/.gitignore
--rw-r--r--   0        0        0      768 2024-04-16 12:12:31.278162 therix-0.1.7/therix/docs/README.md
--rw-r--r--   0        0        0       89 2024-04-16 12:12:31.278296 therix-0.1.7/therix/docs/babel.config.js
--rw-r--r--   0        0        0      389 2024-04-16 12:12:31.278633 therix-0.1.7/therix/docs/blog/2019-05-28-first-blog-post.md
--rw-r--r--   0        0        0     3116 2024-04-16 12:12:31.278892 therix-0.1.7/therix/docs/blog/2019-05-29-long-blog-post.md
--rw-r--r--   0        0        0      439 2024-04-16 12:12:31.279136 therix-0.1.7/therix/docs/blog/2021-08-01-mdx-blog-post.mdx
--rw-r--r--   0        0        0    96122 2024-04-16 12:12:31.280182 therix-0.1.7/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg
--rw-r--r--   0        0        0      783 2024-04-16 12:12:31.280655 therix-0.1.7/therix/docs/blog/2021-08-26-welcome/index.md
--rw-r--r--   0        0        0      447 2024-04-16 12:12:31.280914 therix-0.1.7/therix/docs/blog/authors.yml
--rw-r--r--   0        0        0      162 2024-05-03 05:53:02.647798 therix-0.1.7/therix/docs/docs/LLM-Proxy/_category_.json
--rw-r--r--   0        0        0       66 2024-05-03 05:53:02.647994 therix-0.1.7/therix/docs/docs/LLM-Proxy/index.md
--rw-r--r--   0        0        0      168 2024-05-03 05:53:02.648275 therix-0.1.7/therix/docs/docs/core-components/_category_.json
--rw-r--r--   0        0        0      182 2024-05-03 05:53:02.648495 therix-0.1.7/therix/docs/docs/core-components/pipeline-configurations/_category_.json
--rw-r--r--   0        0        0     3533 2024-05-08 11:24:55.869158 therix-0.1.7/therix/docs/docs/core-components/pipeline-configurations/caching.md
--rw-r--r--   0        0        0     1288 2024-05-08 11:24:55.869292 therix-0.1.7/therix/docs/docs/core-components/pipeline-configurations/data-sources.md
--rw-r--r--   0        0        0     3959 2024-05-08 11:24:55.869587 therix-0.1.7/therix/docs/docs/core-components/pipeline-configurations/embedding-model.md
--rw-r--r--   0        0        0     5428 2024-05-13 10:00:13.303279 therix-0.1.7/therix/docs/docs/core-components/pipeline-configurations/inference-model.md
--rw-r--r--   0        0        0   101843 2024-05-08 11:24:55.870971 therix-0.1.7/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_dashboard.JPG
--rw-r--r--   0        0        0    87594 2024-05-08 11:24:55.871966 therix-0.1.7/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_settings_dashboard.JPG
--rw-r--r--   0        0        0     1409 2024-05-14 09:23:25.313707 therix-0.1.7/therix/docs/docs/core-components/pipeline-configurations/system-prompt.md
--rw-r--r--   0        0        0     1835 2024-05-08 11:24:55.872168 therix-0.1.7/therix/docs/docs/core-components/pipeline-configurations/trace.md
--rw-r--r--   0        0        0     1377 2024-05-08 11:24:55.868823 therix-0.1.7/therix/docs/docs/core-components/pipeline-configurations.md
--rw-r--r--   0        0        0       88 2024-05-03 05:53:02.649320 therix-0.1.7/therix/docs/docs/core-components/pipeline-templates.md
--rw-r--r--   0        0        0     3488 2024-05-08 11:24:55.872304 therix-0.1.7/therix/docs/docs/core-components/pipeline.md
--rw-r--r--   0        0        0      182 2024-05-03 05:53:02.649540 therix-0.1.7/therix/docs/docs/introduction/_category_.json
--rw-r--r--   0        0        0     1266 2024-05-03 05:53:02.649620 therix-0.1.7/therix/docs/docs/introduction/getting-started.md
--rw-r--r--   0        0        0      701 2024-05-03 05:53:02.649715 therix-0.1.7/therix/docs/docs/introduction/index.md
--rw-r--r--   0        0        0     1813 2024-05-08 11:24:55.872443 therix-0.1.7/therix/docs/docs/introduction/installation.md
--rw-r--r--   0        0        0      166 2024-05-03 05:53:02.649919 therix-0.1.7/therix/docs/docs/observability/_category_.json
--rw-r--r--   0        0        0       66 2024-05-03 05:53:02.649997 therix-0.1.7/therix/docs/docs/observability/index.md
--rw-r--r--   0        0        0      158 2024-05-03 05:53:02.650150 therix-0.1.7/therix/docs/docs/squad/_category_.json
--rw-r--r--   0        0        0       50 2024-05-03 05:53:02.650236 therix-0.1.7/therix/docs/docs/squad/index.md
--rw-r--r--   0        0        0      171 2024-05-03 05:53:02.650401 therix-0.1.7/therix/docs/docs/usage/_category_.json
--rw-r--r--   0        0        0       76 2024-05-03 05:53:02.650498 therix-0.1.7/therix/docs/docs/usage/index.md
--rw-r--r--   0        0        0     3717 2024-05-13 10:00:13.303378 therix-0.1.7/therix/docs/docs/use-cases/Keyword Search.md
--rw-r--r--   0        0        0      183 2024-05-03 05:53:02.650644 therix-0.1.7/therix/docs/docs/use-cases/_category_.json
--rw-r--r--   0        0        0       64 2024-05-03 05:53:02.650837 therix-0.1.7/therix/docs/docs/use-cases/faq.md
--rw-r--r--   0        0        0     3579 2024-05-13 10:00:13.303497 therix-0.1.7/therix/docs/docs/use-cases/pii_filer.md
--rw-r--r--   0        0        0     4861 2024-05-14 09:23:25.314499 therix-0.1.7/therix/docs/docs/use-cases/summarizer.md
--rw-r--r--   0        0        0     3888 2024-05-03 05:53:02.652039 therix-0.1.7/therix/docs/docusaurus.config.js
--rw-r--r--   0        0        0      133 2024-05-13 10:00:13.303753 therix-0.1.7/therix/docs/firebase.json
--rw-r--r--   0        0        0   574450 2024-05-03 05:53:02.654343 therix-0.1.7/therix/docs/package-lock.json
--rw-r--r--   0        0        0     1140 2024-05-03 05:53:02.654731 therix-0.1.7/therix/docs/package.json
--rw-r--r--   0        0        0      779 2024-04-16 12:12:31.287120 therix-0.1.7/therix/docs/sidebars.js
--rw-r--r--   0        0        0     1721 2024-04-16 12:12:31.287531 therix-0.1.7/therix/docs/src/components/HomepageFeatures/index.js
--rw-r--r--   0        0        0      181 2024-05-03 05:53:02.654898 therix-0.1.7/therix/docs/src/components/HomepageFeatures/styles.module.css
--rw-r--r--   0        0        0     2282 2024-05-03 05:53:02.655058 therix-0.1.7/therix/docs/src/css/custom.css
--rw-r--r--   0        0        0      365 2024-04-16 12:12:31.288118 therix-0.1.7/therix/docs/src/pages/index.module.css
--rw-r--r--   0        0        0      118 2024-04-16 12:12:31.288266 therix-0.1.7/therix/docs/src/pages/markdown-page.md
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.288338 therix-0.1.7/therix/docs/static/.nojekyll
--rw-r--r--   0        0        0    21038 2024-04-16 12:12:31.288709 therix-0.1.7/therix/docs/static/img/coditas.png
--rw-r--r--   0        0        0     5277 2024-04-16 12:12:31.289101 therix-0.1.7/therix/docs/static/img/coditasLogo.svg
--rw-r--r--   0        0        0    55746 2024-04-16 12:12:31.289498 therix-0.1.7/therix/docs/static/img/docusaurus-social-card.jpg
--rw-r--r--   0        0        0     5142 2024-04-16 12:12:31.289848 therix-0.1.7/therix/docs/static/img/docusaurus.png
--rw-r--r--   0        0        0     3902 2024-05-03 05:53:02.655308 therix-0.1.7/therix/docs/static/img/favicon.ico
--rw-r--r--   0        0        0      553 2024-05-03 05:53:02.655524 therix-0.1.7/therix/docs/static/img/icon.svg
--rw-r--r--   0        0        0      996 2024-05-03 05:53:02.655671 therix-0.1.7/therix/docs/static/img/logo.png
--rw-r--r--   0        0        0      553 2024-05-03 05:53:02.655859 therix-0.1.7/therix/docs/static/img/logo.svg
--rw-r--r--   0        0        0     2713 2024-05-03 05:53:02.656025 therix-0.1.7/therix/docs/static/img/therix-logo.png
--rw-r--r--   0        0        0    31486 2024-04-16 12:12:31.290706 therix-0.1.7/therix/docs/static/img/undraw_docusaurus_mountain.svg
--rw-r--r--   0        0        0    36002 2024-04-16 12:12:31.290979 therix-0.1.7/therix/docs/static/img/undraw_docusaurus_react.svg
--rw-r--r--   0        0        0    11887 2024-04-16 12:12:31.291206 therix-0.1.7/therix/docs/static/img/undraw_docusaurus_tree.svg
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.291242 therix-0.1.7/therix/entities/__init__.py
--rw-r--r--   0        0        0     2572 2024-05-14 09:23:25.315163 therix-0.1.7/therix/entities/models.py
--rw-r--r--   0        0        0     2489 2024-05-13 10:00:13.304041 therix-0.1.7/therix/examples/cache_config_example.py
--rw-r--r--   0        0        0     2720 2024-05-13 10:00:13.304169 therix-0.1.7/therix/examples/keyword_search_examples.py
--rw-r--r--   0        0        0     2475 2024-05-14 09:52:11.737235 therix-0.1.7/therix/examples/main.py
--rw-r--r--   0        0        0     1839 2024-05-13 10:00:13.304440 therix-0.1.7/therix/examples/pii_filter_example.py
--rw-r--r--   0        0        0     6380 2024-05-14 09:23:25.315855 therix-0.1.7/therix/examples/summarizer_example.py
--rw-r--r--   0        0        0     6934 2024-05-14 09:52:11.737539 therix-0.1.7/therix/examples/system_prompt_example.py
--rw-r--r--   0        0        0    21547 2024-04-26 09:41:57.773928 therix-0.1.7/therix/pylintrc
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.291387 therix-0.1.7/therix/services/__init__.py
--rw-r--r--   0        0        0     7305 2024-05-14 09:23:25.316581 therix-0.1.7/therix/services/pipeline_service.py
--rw-r--r--   0        0        0     1434 2024-04-16 12:12:31.291740 therix-0.1.7/therix/services/web_crawling.py
--rw-r--r--   0        0        0     2077 2024-05-13 10:00:13.304865 therix-0.1.7/therix/tests/test_cache.py
--rw-r--r--   0        0        0      602 2024-05-08 11:24:55.874269 therix-0.1.7/therix/tests/test_pii_filter.py
--rw-r--r--   0        0        0     8197 2024-05-13 10:00:13.305133 therix-0.1.7/therix/tests/test_summarizer.py
--rw-r--r--   0        0        0     3304 2024-05-13 10:00:13.305224 therix-0.1.7/therix/utils/keyword_search.py
--rw-r--r--   0        0        0      812 2024-04-26 09:41:57.774428 therix-0.1.7/therix/utils/pii_filter.py
--rw-r--r--   0        0        0    11283 2024-05-14 09:23:25.316980 therix-0.1.7/therix/utils/rag.py
--rw-r--r--   0        0        0     4921 2024-05-14 09:23:25.317276 therix-0.1.7/therix/utils/summarizer.py
--rw-r--r--   0        0        0     2722 1970-01-01 00:00:00.000000 therix-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-20 09:19:32.105170 therix-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1218 2024-04-16 12:12:31.272029 therix-0.1.8/README.md
+-rw-r--r--   0        0        0     1202 2024-05-20 05:54:01.079924 therix-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.275037 therix-0.1.8/therix/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-26 09:41:57.771370 therix-0.1.8/therix/alembic/README
+-rw-r--r--   0        0        0     2912 2024-04-26 09:41:57.771506 therix-0.1.8/therix/alembic/env.py
+-rw-r--r--   0        0        0      635 2024-04-26 09:41:57.771730 therix-0.1.8/therix/alembic/script.py.mako
+-rw-r--r--   0        0        0     2619 2024-04-29 11:17:18.463236 therix-0.1.8/therix/alembic/versions/2024_04_26_0914-739c7981bdd8_added_config_type_for_cache_config.py
+-rw-r--r--   0        0        0     2131 2024-05-03 12:50:17.295513 therix-0.1.8/therix/alembic/versions/2024_04_26_1644-b8fe483b5a71_add_type_column_in_pipeline_table.py
+-rw-r--r--   0        0        0      880 2024-05-08 11:24:55.867083 therix-0.1.8/therix/alembic/versions/2024_05_06_1524-1e7f3dc15e9c_added_chat_history_fix.py
+-rw-r--r--   0        0        0     2614 2024-05-14 09:23:25.311332 therix-0.1.8/therix/alembic/versions/2024_05_13_1842-f5c4562bcd86_added_config_type_for_system_prompt.py
+-rw-r--r--   0        0        0     3092 2024-04-26 10:10:45.584242 therix-0.1.8/therix/alembic/versions/f5fb392e6b0a_initial_database_setup.py
+-rw-r--r--   0        0        0     3599 2024-04-26 09:41:57.771233 therix-0.1.8/therix/alembic.ini
+-rw-r--r--   0        0        0     2083 2024-04-16 12:12:31.275418 therix-0.1.8/therix/core/JSONLoader.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.275458 therix-0.1.8/therix/core/__init__.py
+-rw-r--r--   0        0        0     2737 2024-05-13 10:00:13.299373 therix-0.1.8/therix/core/cache.py
+-rw-r--r--   0        0        0     1399 2024-05-13 10:00:13.301278 therix-0.1.8/therix/core/chat_history/base_chat_history.py
+-rw-r--r--   0        0        0     1771 2024-05-20 05:38:26.419587 therix-0.1.8/therix/core/constants.py
+-rw-r--r--   0        0        0      854 2024-04-16 12:12:31.275897 therix-0.1.8/therix/core/data_sources.py
+-rw-r--r--   0        0        0     1854 2024-05-20 05:38:26.420061 therix-0.1.8/therix/core/embedding_models.py
+-rw-r--r--   0        0        0     2722 2024-05-20 05:38:26.420176 therix-0.1.8/therix/core/inference_models.py
+-rw-r--r--   0        0        0      317 2024-05-13 10:00:13.302010 therix-0.1.8/therix/core/output_parser.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.276202 therix-0.1.8/therix/core/output_source.py
+-rw-r--r--   0        0        0      251 2024-04-26 09:41:57.772340 therix-0.1.8/therix/core/pii_filter_config.py
+-rw-r--r--   0        0        0     6893 2024-05-20 05:38:26.420716 therix-0.1.8/therix/core/pipeline.py
+-rw-r--r--   0        0        0     1153 2024-04-16 12:12:31.276619 therix-0.1.8/therix/core/pipeline_component.py
+-rw-r--r--   0        0        0      238 2024-05-08 11:24:55.868662 therix-0.1.8/therix/core/response.py
+-rw-r--r--   0        0        0      594 2024-05-13 10:00:13.302774 therix-0.1.8/therix/core/summarizer_config.py
+-rw-r--r--   0        0        0       98 2024-05-13 10:00:13.302847 therix-0.1.8/therix/core/summarizer_output_model.py
+-rw-r--r--   0        0        0      328 2024-05-14 09:23:25.312543 therix-0.1.8/therix/core/system_prompt_config.py
+-rw-r--r--   0        0        0      299 2024-04-16 12:12:31.276847 therix-0.1.8/therix/core/trace.py
+-rw-r--r--   0        0        0        0 2024-04-23 08:07:48.247669 therix-0.1.8/therix/db/__init__.py
+-rw-r--r--   0        0        0     3757 2024-05-14 09:52:11.737008 therix-0.1.8/therix/db/db_manager.py
+-rw-r--r--   0        0        0      412 2024-04-26 09:41:57.773326 therix-0.1.8/therix/db/session.py
+-rw-r--r--   0        0        0        0 2024-04-26 09:41:57.773383 therix-0.1.8/therix/db/tests/__init__.py
+-rw-r--r--   0        0        0     1895 2024-04-26 09:41:57.773575 therix-0.1.8/therix/db/tests/test_db_manager.py
+-rw-r--r--   0        0        0      235 2024-05-03 05:53:02.647293 therix-0.1.8/therix/docs/.gitignore
+-rw-r--r--   0        0        0      768 2024-04-16 12:12:31.278162 therix-0.1.8/therix/docs/README.md
+-rw-r--r--   0        0        0       89 2024-04-16 12:12:31.278296 therix-0.1.8/therix/docs/babel.config.js
+-rw-r--r--   0        0        0      389 2024-04-16 12:12:31.278633 therix-0.1.8/therix/docs/blog/2019-05-28-first-blog-post.md
+-rw-r--r--   0        0        0     3116 2024-04-16 12:12:31.278892 therix-0.1.8/therix/docs/blog/2019-05-29-long-blog-post.md
+-rw-r--r--   0        0        0      439 2024-04-16 12:12:31.279136 therix-0.1.8/therix/docs/blog/2021-08-01-mdx-blog-post.mdx
+-rw-r--r--   0        0        0    96122 2024-04-16 12:12:31.280182 therix-0.1.8/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg
+-rw-r--r--   0        0        0      783 2024-04-16 12:12:31.280655 therix-0.1.8/therix/docs/blog/2021-08-26-welcome/index.md
+-rw-r--r--   0        0        0      447 2024-04-16 12:12:31.280914 therix-0.1.8/therix/docs/blog/authors.yml
+-rw-r--r--   0        0        0      162 2024-05-03 05:53:02.647798 therix-0.1.8/therix/docs/docs/LLM-Proxy/_category_.json
+-rw-r--r--   0        0        0       66 2024-05-03 05:53:02.647994 therix-0.1.8/therix/docs/docs/LLM-Proxy/index.md
+-rw-r--r--   0        0        0      168 2024-05-03 05:53:02.648275 therix-0.1.8/therix/docs/docs/core-components/_category_.json
+-rw-r--r--   0        0        0      182 2024-05-03 05:53:02.648495 therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/_category_.json
+-rw-r--r--   0        0        0     3533 2024-05-08 11:24:55.869158 therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/caching.md
+-rw-r--r--   0        0        0     1288 2024-05-08 11:24:55.869292 therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/data-sources.md
+-rw-r--r--   0        0        0     3959 2024-05-08 11:24:55.869587 therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/embedding-model.md
+-rw-r--r--   0        0        0     5428 2024-05-13 10:00:13.303279 therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/inference-model.md
+-rw-r--r--   0        0        0   101843 2024-05-08 11:24:55.870971 therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_dashboard.JPG
+-rw-r--r--   0        0        0    87594 2024-05-08 11:24:55.871966 therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_settings_dashboard.JPG
+-rw-r--r--   0        0        0     1474 2024-05-20 05:38:26.421148 therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/system-prompt.md
+-rw-r--r--   0        0        0     1835 2024-05-08 11:24:55.872168 therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/trace.md
+-rw-r--r--   0        0        0     1377 2024-05-08 11:24:55.868823 therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations.md
+-rw-r--r--   0        0        0       88 2024-05-03 05:53:02.649320 therix-0.1.8/therix/docs/docs/core-components/pipeline-templates.md
+-rw-r--r--   0        0        0     3488 2024-05-08 11:24:55.872304 therix-0.1.8/therix/docs/docs/core-components/pipeline.md
+-rw-r--r--   0        0        0      182 2024-05-03 05:53:02.649540 therix-0.1.8/therix/docs/docs/introduction/_category_.json
+-rw-r--r--   0        0        0     1266 2024-05-03 05:53:02.649620 therix-0.1.8/therix/docs/docs/introduction/getting-started.md
+-rw-r--r--   0        0        0      701 2024-05-03 05:53:02.649715 therix-0.1.8/therix/docs/docs/introduction/index.md
+-rw-r--r--   0        0        0     1813 2024-05-08 11:24:55.872443 therix-0.1.8/therix/docs/docs/introduction/installation.md
+-rw-r--r--   0        0        0      166 2024-05-03 05:53:02.649919 therix-0.1.8/therix/docs/docs/observability/_category_.json
+-rw-r--r--   0        0        0       66 2024-05-03 05:53:02.649997 therix-0.1.8/therix/docs/docs/observability/index.md
+-rw-r--r--   0        0        0      158 2024-05-03 05:53:02.650150 therix-0.1.8/therix/docs/docs/squad/_category_.json
+-rw-r--r--   0        0        0       50 2024-05-03 05:53:02.650236 therix-0.1.8/therix/docs/docs/squad/index.md
+-rw-r--r--   0        0        0      171 2024-05-03 05:53:02.650401 therix-0.1.8/therix/docs/docs/usage/_category_.json
+-rw-r--r--   0        0        0       76 2024-05-03 05:53:02.650498 therix-0.1.8/therix/docs/docs/usage/index.md
+-rw-r--r--   0        0        0     3717 2024-05-13 10:00:13.303378 therix-0.1.8/therix/docs/docs/use-cases/Keyword Search.md
+-rw-r--r--   0        0        0      183 2024-05-03 05:53:02.650644 therix-0.1.8/therix/docs/docs/use-cases/_category_.json
+-rw-r--r--   0        0        0       64 2024-05-03 05:53:02.650837 therix-0.1.8/therix/docs/docs/use-cases/faq.md
+-rw-r--r--   0        0        0     3579 2024-05-13 10:00:13.303497 therix-0.1.8/therix/docs/docs/use-cases/pii_filer.md
+-rw-r--r--   0        0        0     4861 2024-05-14 09:23:25.314499 therix-0.1.8/therix/docs/docs/use-cases/summarizer.md
+-rw-r--r--   0        0        0     3888 2024-05-03 05:53:02.652039 therix-0.1.8/therix/docs/docusaurus.config.js
+-rw-r--r--   0        0        0      133 2024-05-13 10:00:13.303753 therix-0.1.8/therix/docs/firebase.json
+-rw-r--r--   0        0        0   574450 2024-05-03 05:53:02.654343 therix-0.1.8/therix/docs/package-lock.json
+-rw-r--r--   0        0        0     1140 2024-05-03 05:53:02.654731 therix-0.1.8/therix/docs/package.json
+-rw-r--r--   0        0        0      779 2024-04-16 12:12:31.287120 therix-0.1.8/therix/docs/sidebars.js
+-rw-r--r--   0        0        0     1721 2024-04-16 12:12:31.287531 therix-0.1.8/therix/docs/src/components/HomepageFeatures/index.js
+-rw-r--r--   0        0        0      181 2024-05-03 05:53:02.654898 therix-0.1.8/therix/docs/src/components/HomepageFeatures/styles.module.css
+-rw-r--r--   0        0        0     2282 2024-05-03 05:53:02.655058 therix-0.1.8/therix/docs/src/css/custom.css
+-rw-r--r--   0        0        0      365 2024-04-16 12:12:31.288118 therix-0.1.8/therix/docs/src/pages/index.module.css
+-rw-r--r--   0        0        0      118 2024-04-16 12:12:31.288266 therix-0.1.8/therix/docs/src/pages/markdown-page.md
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.288338 therix-0.1.8/therix/docs/static/.nojekyll
+-rw-r--r--   0        0        0    21038 2024-04-16 12:12:31.288709 therix-0.1.8/therix/docs/static/img/coditas.png
+-rw-r--r--   0        0        0     5277 2024-04-16 12:12:31.289101 therix-0.1.8/therix/docs/static/img/coditasLogo.svg
+-rw-r--r--   0        0        0    55746 2024-04-16 12:12:31.289498 therix-0.1.8/therix/docs/static/img/docusaurus-social-card.jpg
+-rw-r--r--   0        0        0     5142 2024-04-16 12:12:31.289848 therix-0.1.8/therix/docs/static/img/docusaurus.png
+-rw-r--r--   0        0        0     3902 2024-05-03 05:53:02.655308 therix-0.1.8/therix/docs/static/img/favicon.ico
+-rw-r--r--   0        0        0      553 2024-05-03 05:53:02.655524 therix-0.1.8/therix/docs/static/img/icon.svg
+-rw-r--r--   0        0        0      996 2024-05-03 05:53:02.655671 therix-0.1.8/therix/docs/static/img/logo.png
+-rw-r--r--   0        0        0      553 2024-05-03 05:53:02.655859 therix-0.1.8/therix/docs/static/img/logo.svg
+-rw-r--r--   0        0        0     2713 2024-05-03 05:53:02.656025 therix-0.1.8/therix/docs/static/img/therix-logo.png
+-rw-r--r--   0        0        0    31486 2024-04-16 12:12:31.290706 therix-0.1.8/therix/docs/static/img/undraw_docusaurus_mountain.svg
+-rw-r--r--   0        0        0    36002 2024-04-16 12:12:31.290979 therix-0.1.8/therix/docs/static/img/undraw_docusaurus_react.svg
+-rw-r--r--   0        0        0    11887 2024-04-16 12:12:31.291206 therix-0.1.8/therix/docs/static/img/undraw_docusaurus_tree.svg
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.291242 therix-0.1.8/therix/entities/__init__.py
+-rw-r--r--   0        0        0     2571 2024-05-20 05:38:26.421434 therix-0.1.8/therix/entities/models.py
+-rw-r--r--   0        0        0     2480 2024-05-20 05:38:26.421562 therix-0.1.8/therix/examples/cache_config_example.py
+-rw-r--r--   0        0        0     1294 2024-05-20 05:38:26.421625 therix-0.1.8/therix/examples/gemini.rag.py
+-rw-r--r--   0        0        0     2748 2024-05-20 05:38:26.421736 therix-0.1.8/therix/examples/keyword_search_examples.py
+-rw-r--r--   0        0        0     2475 2024-05-14 09:52:11.737235 therix-0.1.8/therix/examples/main.py
+-rw-r--r--   0        0        0     2099 2024-05-20 05:38:26.421832 therix-0.1.8/therix/examples/pii_filter_example.py
+-rw-r--r--   0        0        0     6384 2024-05-20 05:38:26.422087 therix-0.1.8/therix/examples/summarizer_example.py
+-rw-r--r--   0        0        0     6934 2024-05-14 09:52:11.737539 therix-0.1.8/therix/examples/system_prompt_example.py
+-rw-r--r--   0        0        0    21547 2024-04-26 09:41:57.773928 therix-0.1.8/therix/pylintrc
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.291387 therix-0.1.8/therix/services/__init__.py
+-rw-r--r--   0        0        0     7603 2024-05-20 05:38:26.422335 therix-0.1.8/therix/services/pipeline_service.py
+-rw-r--r--   0        0        0     1434 2024-04-16 12:12:31.291740 therix-0.1.8/therix/services/web_crawling.py
+-rw-r--r--   0        0        0     2077 2024-05-13 10:00:13.304865 therix-0.1.8/therix/tests/test_cache.py
+-rw-r--r--   0        0        0      602 2024-05-08 11:24:55.874269 therix-0.1.8/therix/tests/test_pii_filter.py
+-rw-r--r--   0        0        0     8197 2024-05-13 10:00:13.305133 therix-0.1.8/therix/tests/test_summarizer.py
+-rw-r--r--   0        0        0     3591 2024-05-20 05:38:26.422456 therix-0.1.8/therix/utils/keyword_search.py
+-rw-r--r--   0        0        0      812 2024-04-26 09:41:57.774428 therix-0.1.8/therix/utils/pii_filter.py
+-rw-r--r--   0        0        0    13454 2024-05-20 05:38:26.422650 therix-0.1.8/therix/utils/rag.py
+-rw-r--r--   0        0        0     5140 2024-05-20 05:38:26.422883 therix-0.1.8/therix/utils/summarizer.py
+-rw-r--r--   0        0        0     2988 1970-01-01 00:00:00.000000 therix-0.1.8/PKG-INFO
```

### Comparing `therix-0.1.7/LICENSE` & `therix-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/README.md` & `therix-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/pyproject.toml` & `therix-0.1.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "therix"
-version = "0.1.7"
+version = "0.1.8"
 description = "Therix is the SDK for langchain based applications."
 authors = ["Ajinath"]
 license = "MIT"
 readme = "README.md"
 include = ["alembic/**/*", "alembic.ini"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 wheel = "^0.43.0"
 alembic = "1.13.1"
 psycopg2-binary = "2.9.9"
 sqlalchemy = "2.0.28"
 pgvector = "0.2.5"
-langchain = "0.1.13"
+langchain = "^0.1.20"
 langchain-openai = "0.1.1"
 tiktoken = "0.6.0"
 pypdf = "4.1.0"
 langfuse = "2.21.1"
 alembic-postgresql-enum = "1.1.2"
 greenlet = "^3.0.3"
 youtube-transcript-api = "^0.6.2"
@@ -30,14 +30,20 @@
 langchain-groq = "^0.1.0"
 boto3 = "^1.34.81"
 pylint = "^3.1.0"
 coverage = "^7.4.4"
 pytest-cov = "^5.0.0"
 langchain-postgres = "^0.0.3"
 transformers = "^4.40.2"
+langchain-google-genai = "^1.0.3"
+langchain-experimental = "^0.0.58"
+faker = "^25.1.0"
+poetry-dotenv-plugin = "^0.2.0"
+presidio-anonymizer = "^2.2.354"
+
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^7.0.0"
 pytest = "^8.1.1"
 pytest-mock = "^3.14.0"
 
 [build-system]
```

### Comparing `therix-0.1.7/therix/alembic/env.py` & `therix-0.1.8/therix/alembic/env.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/alembic/script.py.mako` & `therix-0.1.8/therix/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/alembic/versions/2024_04_26_0914-739c7981bdd8_added_config_type_for_cache_config.py` & `therix-0.1.8/therix/alembic/versions/2024_04_26_0914-739c7981bdd8_added_config_type_for_cache_config.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/alembic/versions/2024_04_26_1644-b8fe483b5a71_add_type_column_in_pipeline_table.py` & `therix-0.1.8/therix/alembic/versions/2024_04_26_1644-b8fe483b5a71_add_type_column_in_pipeline_table.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/alembic/versions/2024_05_06_1524-1e7f3dc15e9c_added_chat_history_fix.py` & `therix-0.1.8/therix/alembic/versions/2024_05_06_1524-1e7f3dc15e9c_added_chat_history_fix.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/alembic/versions/2024_05_13_1842-f5c4562bcd86_added_config_type_for_system_prompt.py` & `therix-0.1.8/therix/alembic/versions/2024_05_13_1842-f5c4562bcd86_added_config_type_for_system_prompt.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/alembic/versions/f5fb392e6b0a_initial_database_setup.py` & `therix-0.1.8/therix/alembic/versions/f5fb392e6b0a_initial_database_setup.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/alembic.ini` & `therix-0.1.8/therix/alembic.ini`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/core/JSONLoader.py` & `therix-0.1.8/therix/core/JSONLoader.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/core/cache.py` & `therix-0.1.8/therix/core/cache.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/core/chat_history/base_chat_history.py` & `therix-0.1.8/therix/core/chat_history/base_chat_history.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/core/constants.py` & `therix-0.1.8/therix/core/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     OPENAI_TEXT_EMBEDDING_3_LARGE = 'text-embedding-3-large'
     OPENAI_TEXT_EMBEDDING_3_SMALL = 'text-embedding-3-small'
     AZURE_TEXT_ADA='text-embedding-ada-002'
     AZURE_TEXT_EMBEDDING_3_LARGE = 'text-embedding-3-large'
     AZURE_TEXT_EMBEDDING_3_SMALL = 'text-embedding-3-small'
     BEDROCK_TITAN_EMBEDDING='amazon.titan-embed-text-v1'
     BEDROCK_TITAN_MULTIMODAL_EMBEDDING='amazon.titan-embed-image-v1'
+    GEMINI_EMBEDDING='models/embedding-001'
 
 class InferenceModelMaster:
     OPENAI_GPT_4_TURBO_PREVIEW = 'gpt-4-turbo-preview'
     OPENAI_GPT_4 = 'gpt-4'
     OPENAI_GPT_3_5_TURBO = 'gpt-3.5-turbo'
     OPENAI_GPT_3_5_TURBO_INSTRUCT = 'gpt-3.5-turbo-instruct'
     AZURE_GPT_4_TURBO_PREVIEW = 'gpt-4-turbo-preview'
@@ -28,14 +29,16 @@
     AZURE_GPT_3_5_TURBO = 'gpt-3.5-turbo'
     AZURE_GPT_3_5_TURBO_INSTRUCT = 'gpt-3.5-turbo-instruct'
     GROQ_LLM_MIXTRAL_8_7_B='mixtral-8x7b-32768'
     GROQ_LLM_LLAMA3_70B= 'llama3-70b-8192'
     GROQ_LLM_GEMMA7B= 'gemma-7b-it'
     BEDROCK_TEXT_EXPRES_V1='amazon.titan-text-express-v1'
     BEDROCK_TEXT_LITE_G1='amazon.titan-text-lite-v1'
+    GOOGLE_GEMINI_PRO='gemini-pro'
+    GOOGLE_GEMINI_1_5_PRO='gemini-1.5-pro'
 
 class OutputSourceMaster:
     S3 = "S3"
     LOCAL = "LOCAL"
     DATABASE = "DATABASE"
```

### Comparing `therix-0.1.7/therix/core/data_sources.py` & `therix-0.1.8/therix/core/data_sources.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/core/embedding_models.py` & `therix-0.1.8/therix/core/embedding_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,7 +46,14 @@
 
 
 class BedrockTitanMultiModalEmbedding(EmbeddingModel):
     def __init__(self, **kwargs):
         super().__init__(
             name=EmbeddingModelMaster.BEDROCK_TITAN_MULTIMODAL_EMBEDDING, **kwargs
         )
+
+
+class GeminiAIEmbeddings(EmbeddingModel):
+    def __init__(self, **kwargs):
+        super().__init__(
+            name=EmbeddingModelMaster.GEMINI_EMBEDDING, **kwargs
+        )
```

### Comparing `therix-0.1.7/therix/core/inference_models.py` & `therix-0.1.8/therix/core/inference_models.py`

 * *Files 10% similar despite different names*

```diff
@@ -66,7 +66,16 @@
             name=InferenceModelMaster.BEDROCK_TEXT_EXPRES_V1, config=config
         )
 
 
 class BedrockLiteG1(InferenceModel):
     def __init__(self, config: dict):
         super().__init__(name=InferenceModelMaster.BEDROCK_TEXT_LITE_G1, config=config)
+        
+class GeminiPro(InferenceModel):
+    def __init__(self, config: dict):
+        super().__init__(name=InferenceModelMaster.GOOGLE_GEMINI_PRO, config=config)
+        
+        
+class Gemini_1_5_PRO(InferenceModel):
+    def __init__(self, config: dict):
+        super().__init__(name=InferenceModelMaster.GOOGLE_GEMINI_1_5_PRO, config=config)
```

### Comparing `therix-0.1.7/therix/core/pipeline.py` & `therix-0.1.8/therix/core/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
             pipeline_type = self.pipeline_service.get_pipeline(self.pipeline_data.id).type.value
 
             if pipeline_type == PipelineTypeMaster.RAG.value:
                 if add_cache:
                     cached_response = therix_cache.lookup(question, inference_model[0].name, self.pipeline_data.id)
                 if cached_response:
-                    return ModelResponse(cached_response, session_id).create_response()
+                    return ModelResponse(cached_response.response, session_id).create_response()
                 if (keyword_search_params and question == None):
                     keyword_search_params['pipeline_id'] = self.pipeline_data.id
                     keyword_search_params['trace_details'] = trace_details
                     answer = self.pipeline_service.search_keywords(keyword_search_params)
                 else:
                     if(pipeline_system_prompt):
                         answer = self.pipeline_service.invoke_pipeline(
```

### Comparing `therix-0.1.7/therix/core/pipeline_component.py` & `therix-0.1.8/therix/core/pipeline_component.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/core/summarizer_config.py` & `therix-0.1.8/therix/core/summarizer_config.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/db/db_manager.py` & `therix-0.1.8/therix/db/db_manager.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/db/tests/test_db_manager.py` & `therix-0.1.8/therix/db/tests/test_db_manager.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/README.md` & `therix-0.1.8/therix/docs/README.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/blog/2019-05-29-long-blog-post.md` & `therix-0.1.8/therix/docs/blog/2019-05-29-long-blog-post.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg` & `therix-0.1.8/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/blog/2021-08-26-welcome/index.md` & `therix-0.1.8/therix/docs/blog/2021-08-26-welcome/index.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/docs/core-components/pipeline-configurations/caching.md` & `therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/caching.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/docs/core-components/pipeline-configurations/data-sources.md` & `therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/data-sources.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/docs/core-components/pipeline-configurations/embedding-model.md` & `therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/embedding-model.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/docs/core-components/pipeline-configurations/inference-model.md` & `therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/inference-model.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_dashboard.JPG` & `therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_dashboard.JPG`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_settings_dashboard.JPG` & `therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_settings_dashboard.JPG`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/docs/core-components/pipeline-configurations/system-prompt.md` & `therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/system-prompt.md`

 * *Files 12% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 You can add system-prompt to your pipeline by doing a `.add` to your existing configurations.
 ```python
 .add(SystemPromptConfig(config={"system_prompt" : sys_prompt}))
 ```
 
 # Example
 ```python
+from therix.core.system_prompt_config import SystemPromptConfig
+
 pipeline = Pipeline(name="Summarizer Pipeline")
     (pipeline
     .add(SystemPromptConfig(config={"system_prompt" : sys_prompt}))
     .add(// Any other configuration you want to add)
     .save())
 
     pipeline.publish()
```

### Comparing `therix-0.1.7/therix/docs/docs/core-components/pipeline-configurations/trace.md` & `therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations/trace.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/docs/core-components/pipeline-configurations.md` & `therix-0.1.8/therix/docs/docs/core-components/pipeline-configurations.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/docs/core-components/pipeline.md` & `therix-0.1.8/therix/docs/docs/core-components/pipeline.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/docs/introduction/getting-started.md` & `therix-0.1.8/therix/docs/docs/introduction/getting-started.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/docs/introduction/index.md` & `therix-0.1.8/therix/docs/docs/introduction/index.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/docs/introduction/installation.md` & `therix-0.1.8/therix/docs/docs/introduction/installation.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/docs/use-cases/Keyword Search.md` & `therix-0.1.8/therix/docs/docs/use-cases/Keyword Search.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/docs/use-cases/pii_filer.md` & `therix-0.1.8/therix/docs/docs/use-cases/pii_filer.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/docs/use-cases/summarizer.md` & `therix-0.1.8/therix/docs/docs/use-cases/summarizer.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/docusaurus.config.js` & `therix-0.1.8/therix/docs/docusaurus.config.js`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/package-lock.json` & `therix-0.1.8/therix/docs/package-lock.json`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/package.json` & `therix-0.1.8/therix/docs/package.json`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/sidebars.js` & `therix-0.1.8/therix/docs/sidebars.js`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/src/components/HomepageFeatures/index.js` & `therix-0.1.8/therix/docs/src/components/HomepageFeatures/index.js`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/src/css/custom.css` & `therix-0.1.8/therix/docs/src/css/custom.css`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/static/img/coditas.png` & `therix-0.1.8/therix/docs/static/img/coditas.png`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/static/img/coditasLogo.svg` & `therix-0.1.8/therix/docs/static/img/coditasLogo.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/static/img/docusaurus-social-card.jpg` & `therix-0.1.8/therix/docs/static/img/docusaurus-social-card.jpg`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/static/img/docusaurus.png` & `therix-0.1.8/therix/docs/static/img/docusaurus.png`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/static/img/favicon.ico` & `therix-0.1.8/therix/docs/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/static/img/icon.svg` & `therix-0.1.8/therix/docs/static/img/icon.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/static/img/logo.png` & `therix-0.1.8/therix/docs/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/static/img/logo.svg` & `therix-0.1.8/therix/docs/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/static/img/therix-logo.png` & `therix-0.1.8/therix/docs/static/img/therix-logo.png`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/static/img/undraw_docusaurus_mountain.svg` & `therix-0.1.8/therix/docs/static/img/undraw_docusaurus_mountain.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/static/img/undraw_docusaurus_react.svg` & `therix-0.1.8/therix/docs/static/img/undraw_docusaurus_react.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/docs/static/img/undraw_docusaurus_tree.svg` & `therix-0.1.8/therix/docs/static/img/undraw_docusaurus_tree.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/entities/models.py` & `therix-0.1.8/therix/entities/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     INPUT_SOURCE = "INPUT_SOURCE"
     EMBEDDING_MODEL = "EMBEDDING_MODEL"
     INFERENCE_MODEL = "INFERENCE_MODEL"
     OUTPUT_SOURCE = "OUTPUT_SOURCE"
     TRACE_DETAILS = "TRACE_DETAILS"
     PII_FILTER = "PII_FILTER"
     SUMMARIZER = "SUMMARIZER"
-    CACHE_CONFIG = "CACHE_CONFIG",
+    CACHE_CONFIG = "CACHE_CONFIG"
     SYSTEM_PROMPT = 'SYSTEM_PROMPT'
 
 
 class Pipeline(Base):
     __tablename__ = "pipelines"
 
     id = Column(
```

### Comparing `therix-0.1.7/therix/examples/cache_config_example.py` & `therix-0.1.8/therix/examples/cache_config_example.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,23 +55,23 @@
                                 "bedrock_aws_secret_access_key" : ""        ,
                                 "bedrock_aws_session_token" : "",
                                 "bedrock_region_name" : "us-east-1"}))
     .add(GroqMixtral87bInferenceModel(config={'groq_api_key': GROQ_API_KEY}))
     .add(Trace(config={
         'secret_key': 'sk-lf-e62aa7ce-c4c8-4c77-ad7d-9d76dfd96db1',
         'public_key': 'pk-lf-282ad728-c1d6-4247-b6cd-8022198591a9',
-        'identifier': 'my own pipeline'
+        'identifier': 'cache_pipeline'
     }))
     .add(CacheConfig(config={}))
     .save())
 
     pipeline.publish()
     pipeline.preprocess_data()
     print(pipeline.id)
-    ans = pipeline.invoke("What are some use cases of RAT?")
+    ans = pipeline.invoke("Explain ablation study?")
 
     print(ans)
 
 
     end_time = time.process_time()
```

### Comparing `therix-0.1.7/therix/examples/keyword_search_examples.py` & `therix-0.1.8/therix/examples/keyword_search_examples.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,19 +21,19 @@
     ans = pipeline.invoke(question, session_id)
     print(ans)
 else:
     pipeline = Pipeline(name="My New Published Pipeline")
     (pipeline
     .add(PDFDataSource(config={'files': ['./test-data/file.pdf' , './test-data/rat.pdf']}))
     .add(AzureOpenAIEmbedding3LargeEmbeddingModel(config={"azure_deployment" : "", "azure_api_key" : "" , "azure_endpoint" : "" , "openai_api_version" :  ""}))
-    .add(AzureOpenAIGPT4InferenceModel(config={"azure_api_key" : "" , "openai_api_version" :  "", "azure_endpoint" : "" , "azure_deployment" : "" }))
+    .add(AzureOpenAIGPT4InferenceModel(config={"azure_api_key" : "" , "openai_api_version" :  "", "azure_endpoint" : "" , "azure_deployment" : "" , "temperature" : ""}))
     .add(Trace(config={
                     'secret_key': 'sk-lf-e62aa7ce-c4c8-4c77-ad7d-9d76dfd96db1',
                     'public_key': 'pk-lf-282ad728-c1d6-4247-b6cd-8022198591a9',
-                    'identifier': 'my own pipeline'
+                    'identifier': 'keyword_search_pipeline'
          }))
         .save()
         )
 
     pipeline.publish()
     embedding_created_response = pipeline.preprocess_data()
     print(pipeline.id)
```

### Comparing `therix-0.1.7/therix/examples/main.py` & `therix-0.1.8/therix/examples/main.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/examples/pii_filter_example.py` & `therix-0.1.8/therix/examples/pii_filter_example.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from therix.core.data_sources import PDFDataSource
-from therix.core.inference_models import GroqMixtral87bInferenceModel
+from therix.core.inference_models import BedrockLiteG1, BedrockTextExpressV1, GroqMixtral87bInferenceModel
 from therix.core.embedding_models import BedrockTitanEmbedding
 from therix.core.pii_filter_config import PIIFilterConfig
 from therix.core.pipeline import Pipeline
 import sys
 from therix.core.trace import Trace
 
 
@@ -22,26 +22,30 @@
     ans = pipeline.invoke(question)
     print(ans)
 else:
     pipeline = Pipeline(name="My New Published Pipeline")
     (pipeline
     .add(PDFDataSource(config={'files': ['../../test-data/Essay-on-Lata-Mangeshkar-final.pdf']}))
     .add(BedrockTitanEmbedding(config={ "bedrock_aws_access_key_id":"",
-                                            "bedrock_aws_secret_access_key" : "",
-                                            "bedrock_aws_session_token" : "",
-                                            "bedrock_region_name" : "us-east-1"
+                                        "bedrock_aws_secret_access_key" : "",
+                                        "bedrock_aws_session_token" : "",
+                                        "bedrock_region_name" : "us-east-1"
+                                            }))
+    .add(BedrockLiteG1(config={ "bedrock_aws_access_key_id":"",
+                                "bedrock_aws_secret_access_key" : "",
+                                "bedrock_aws_session_token" : "",
+                                "bedrock_region_name" : "us-east-1"
                                             }))
-    .add(GroqMixtral87bInferenceModel(config={"groq_api_key": 'your groq api key'}))
     .add(PIIFilterConfig(config={
         'entities': ['PERSON','PHONE_NUMBER','EMAIL_ADDRESS']
     }))
     .add(Trace(config={
-        'secret_key': 'sk-lf-e62aa7ce-c4c8-4c77-ad7d-9d76dfd96db1',
-        'public_key': 'pk-lf-282ad728-c1d6-4247-b6cd-8022198591a9',
-        'identifier': 'my own pipeline'
+        'secret_key': 'sk-lf-6fd11f23-6506-428c-9328-6a03cce5574b',
+        'public_key': 'pk-lf-d319ad68-34e1-45e5-b25c-c341e8f22462',
+        'identifier': 'pii_filter_pipeline'
     }))
     .save())
 
     pipeline.publish()
     pipeline.preprocess_data()
     print(pipeline.id)
     ans = pipeline.invoke("Whom is the data about? And what are their personal details?")
```

### Comparing `therix-0.1.7/therix/examples/summarizer_example.py` & `therix-0.1.8/therix/examples/summarizer_example.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,17 +98,17 @@
 else:
     pipeline = Pipeline(name="Summarizer Pipeline")
 
     (pipeline
     .add(GroqMixtral87bInferenceModel(config={"groq_api_key": "GROQ_API_KEY"}))
     .add(SummarizerConfig(SummarizerTypeMaster.EXTRACTIVE,TopicModel))
     .add(Trace(config={
-        'secret_key': 'sk-lf-e62aa7ce-c4c8-4c77-ad7d-9d76dfd96db1',
-        'public_key': 'pk-lf-282ad728-c1d6-4247-b6cd-8022198591a9',
-        'identifier': 'my own pipeline'
+        'secret_key': 'sk-lf-6fd11f23-6506-428c-9328-6a03cce5574b',
+        'public_key': 'pk-lf-d319ad68-34e1-45e5-b25c-c341e8f22462',
+        'identifier': 'summarizer_pipeline'
     }))
     .save())
 
     pipeline.publish()
     print(pipeline.id)
     ans = pipeline.invoke(text)
```

### Comparing `therix-0.1.7/therix/examples/system_prompt_example.py` & `therix-0.1.8/therix/examples/system_prompt_example.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/pylintrc` & `therix-0.1.8/therix/pylintrc`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/services/pipeline_service.py` & `therix-0.1.8/therix/services/pipeline_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,27 +81,35 @@
         )
         store = get_vectorstore(embedding_model[0], str(pipeline_id))
         retreiver = store.as_retriever()
 
         inference_model = self.get_pipeline_configuraitons_by_type(
             pipeline_id, "INFERENCE_MODEL"
         )
+        
+        pii_filter_config = self.get_pipeline_configuraitons_by_type(pipeline_id, ConfigType.PII_FILTER)
+        if len(pii_filter_config) != 0:
+            pii_filter_config = pii_filter_config[0]
+        else :
+            pii_filter_config = None
+                
         result = chat(
             question,
             retreiver,
             inference_model[0],
             embedding_model,
             session_id,
             pipeline_id,
             trace_details,
+            pii_filter_config,
             system_prompt
         )
-        pii_filter_config = self.get_pipeline_configuraitons_by_type(pipeline_id, ConfigType.PII_FILTER)
+        
         if pii_filter_config:
-            pii_filter_config = pii_filter_config[0].config
+            pii_filter_config = pii_filter_config.config
             entities = pii_filter_config['entities']
             return pii_filter(result,entities)
         else:
             return result
 
     def invoke_summarizer_pipeline(self, pipeline_id, text, trace_details = None, system_prompt=None):
         inference_model = self.get_pipeline_configuraitons_by_type(pipeline_id, ConfigType.INFERENCE_MODEL)
@@ -125,24 +133,26 @@
             "keywords": keyword_search_params.get("keywords"),
             "config_id": keyword_search_params.get("config_id"),
             "output_parser": keyword_search_params.get("output_parser"),
             "prompt" : keyword_search_params.get("prompt"),
             "pipeline_id" : keyword_search_params.get("pipeline_id"),
             "trace_details" : keyword_search_params.get("trace_details")
         }
+
         AZURE_OPENAI_API_KEY=infer_config.get("azure_api_key")
         AZURE_OPENAI_ENDPOINT=infer_config.get("azure_endpoint")
 
         embed_config=embedding_model.config
 
         llm = AzureChatOpenAI(
             deployment_name=keyword_search_params["infer_config"].get("azure_deployment"),
             azure_endpoint=keyword_search_params["infer_config"].get("azure_endpoint"),
             api_version=keyword_search_params["infer_config"].get("openai_api_version"),
-            api_key=keyword_search_params["infer_config"].get("azure_api_key")
+            api_key=keyword_search_params["infer_config"].get("azure_api_key"),
+            temperature=keyword_search_params["infer_config"].get("temperature") or 0.7
         )
 
         keyword_search_dict = {
             "pipeline_id" : keyword_search_params.get("pipeline_id"),
             "config_id" : keyword_search_params.get("config_id"),
             "keywords": keyword_search_params.get("keywords"),
             "output_parser": keyword_search_params.get("output_parser"),
```

### Comparing `therix-0.1.7/therix/services/web_crawling.py` & `therix-0.1.8/therix/services/web_crawling.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/tests/test_cache.py` & `therix-0.1.8/therix/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/tests/test_pii_filter.py` & `therix-0.1.8/therix/tests/test_pii_filter.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/tests/test_summarizer.py` & `therix-0.1.8/therix/tests/test_summarizer.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/utils/keyword_search.py` & `therix-0.1.8/therix/utils/keyword_search.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,14 @@
         if keyword_search_dict.get("trace_details") is not None:
             langfuse_handler = CallbackHandler(
             secret_key=keyword_search_dict.get("trace_details")["secret_key"],
             public_key=keyword_search_dict.get("trace_details")["public_key"],
             host=keyword_search_dict.get("trace_details")["host"],
             trace_name=keyword_search_dict.get("trace_details")["identifier"],
         )
-        chain_callbacks.append(langfuse_handler)
 
         store = get_vectorstore(self.embed_model , str(keyword_search_dict.get("pipeline_id")))
 
         if(type(keyword_search_dict.get("config_id")) is list):
             retriever=store.as_retriever(
             search_kwargs={"filter": {'configId': {'$in': keyword_search_dict.get('config_id')}}},
             )
@@ -71,12 +70,17 @@
                 ("system", prompt),
                 ("human",
                  "{BASIC_INSTRUCTIONS} {content} {keywords}")
             ]
         )
 
         chain = prompt | self.llmProvider | keyword_search_dict["output_parser"]
-
-        response_text = chain.invoke({"content": content, "keywords": keyword_search_dict["keywords"], "format_instructions": keyword_search_dict["output_parser"].get_format_instructions(), "BASIC_INSTRUCTIONS": BASIC_INSTRUCTIONS}, config={"callbacks": [langfuse_handler]})
+        if(keyword_search_dict.get("trace_details")):
+            response_text = chain.invoke({"content": content, "keywords": keyword_search_dict["keywords"], "format_instructions": keyword_search_dict["output_parser"].get_format_instructions(), "BASIC_INSTRUCTIONS": BASIC_INSTRUCTIONS}, config={"callbacks": [langfuse_handler]})
+        else: 
+            response_text = chain.invoke({"content": content, "keywords": keyword_search_dict["keywords"], "format_instructions": keyword_search_dict["output_parser"].get_format_instructions(), "BASIC_INSTRUCTIONS": BASIC_INSTRUCTIONS})
+        
+        
+        
         return response_text
```

### Comparing `therix-0.1.7/therix/utils/pii_filter.py` & `therix-0.1.8/therix/utils/pii_filter.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.7/therix/utils/rag.py` & `therix-0.1.8/therix/utils/rag.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json, uuid
 from operator import itemgetter
 from pathlib import Path
 from urllib import response
 from langchain.docstore.document import Document
 from langchain_community.document_loaders import TextLoader, PyPDFLoader
 from langchain_community.vectorstores.pgvector import PGVector
+from langchain_google_genai import ChatGoogleGenerativeAI, GoogleGenerativeAIEmbeddings
 from langchain_openai import OpenAIEmbeddings, ChatOpenAI
 from langchain_openai import AzureChatOpenAI
 from langchain_groq import ChatGroq
 from langchain_core.output_parsers import StrOutputParser
 from langchain_core.prompts import ChatPromptTemplate
 from langchain_community.document_loaders.youtube import YoutubeLoader
 from langchain_core.prompts import ChatPromptTemplate
@@ -32,14 +33,16 @@
 from langchain_core.runnables import RunnablePassthrough
 from langchain_core.output_parsers import StrOutputParser
 from langchain_core.messages import get_buffer_string
 from langchain_core.prompts import format_document
 from langchain_core.runnables import RunnableParallel
 from langchain_text_splitters import  RecursiveCharacterTextSplitter
 from operator import itemgetter
+from langchain_experimental.data_anonymizer import PresidioReversibleAnonymizer
+
 
 def sanitize_text(text):
     # Remove null characters (0x00) from the text
     sanitized_text = text.replace("\x00", "")
     return sanitized_text
 
 
@@ -99,17 +102,26 @@
 
         return BedrockEmbeddings(
             credentials_profile_name="bedrock-admin",
             client=bedrock_client,
             model_id=embedding_model_name,
             region_name=config["bedrock_region_name"],
         )
+        
+    elif(
+        embedding_model_name == EmbeddingModelMaster.GEMINI_EMBEDDING
+    ) and ("google_api_key" in config):
+        return GoogleGenerativeAIEmbeddings(
+            model=EmbeddingModelMaster.GEMINI_EMBEDDING,
+            google_api_key=config["google_api_key"],
+        )
     else:
         raise ValueError(f"Unknown embedding model: {embedding_model_name}")
-
+    
+    
 
 def get_inference_model(inference_model_name, config):
     if (
         inference_model_name == InferenceModelMaster.OPENAI_GPT_3_5_TURBO
         or inference_model_name == InferenceModelMaster.OPENAI_GPT_3_5_TURBO_INSTRUCT
         or inference_model_name == InferenceModelMaster.OPENAI_GPT_4
         or inference_model_name == InferenceModelMaster.OPENAI_GPT_4_TURBO_PREVIEW
@@ -148,14 +160,28 @@
         )
         return Bedrock(
             credentials_profile_name="bedrock-admin",
             model_id=inference_model_name,
             client=bedrock_client,
             region_name=config["bedrock_region_name"],
         )
+    
+    elif(
+        inference_model_name == InferenceModelMaster.GOOGLE_GEMINI_PRO
+        or inference_model_name == InferenceModelMaster.GOOGLE_GEMINI_1_5_PRO
+    ) and ("google_api_key" in config):
+        return ChatGoogleGenerativeAI(
+            model=inference_model_name,
+            google_api_key=config["google_api_key"],
+            temperature=0.7, 
+            top_p=0.85,
+            metadata= {'language': 'en'}
+          
+
+        )
     else:
         raise ValueError(f"Unknown inference model: {inference_model_name}")
 
 
 def create_embeddings(data_sources, embedding_model, collection_name):
 
     store = get_vectorstore(embedding_model, collection_name)
@@ -198,17 +224,17 @@
     question,
     retriever,
     inference_model,
     embed_model,
     session_id,
     pipeline_id,
     trace_details=None,
+    pii_filter_config = None,
     system_prompt=None
 ):
-
     # print(trace_details)
     chain_callbacks = []
     if trace_details is not None:
         langfuse_handler = CallbackHandler(
             secret_key=trace_details["secret_key"],
             public_key=trace_details["public_key"],
             host=trace_details["host"],
@@ -223,55 +249,91 @@
         table_name="chat_history",
     )
     chat_history = history.messages
 
     if(system_prompt):
         template = system_prompt.config.get("system_prompt")
     else : 
-        template = """Answer the question based only on the following context and do not reply anything that is out of context, reply with "I am sorry, I cannot help you with that" and do not add any more message to it.
-        Context: 
-        {context}
+        template = """
+        Answer the question based only on the following context:
+
+{context}
 
-        Question: {question}
+Answer the question based on the above context: {question}
         """
     ANSWER_PROMPT = ChatPromptTemplate.from_template(template)
     _template = """Given the following conversation and a follow up question, rephrase the follow up question to be a standalone question, in its original language.
                     Chat History:
                     {chat_history}
                     Follow Up Input: {question}
                     Standalone question:"""
 
     CONDENSE_QUESTION_PROMPT = PromptTemplate.from_template(_template)
     DEFAULT_DOCUMENT_PROMPT = PromptTemplate.from_template(template="{page_content}")
-
-
-    def _combine_documents(
-        docs, document_prompt=DEFAULT_DOCUMENT_PROMPT, document_separator="\n\n"
-    ):
-        doc_strings = [format_document(doc, document_prompt) for doc in docs]
-        return document_separator.join(doc_strings)
-
+    
     model = get_inference_model(inference_model.name, inference_model.config)
-
-    _inputs = RunnableParallel(
+    
+    if pii_filter_config:
+        pii_filter_config = pii_filter_config.config
+        entities = pii_filter_config['entities']
+        anonymizer = PresidioReversibleAnonymizer(
+        analyzed_fields=entities,
+        faker_seed=42)
+
+        def _combine_documents(
+            docs, document_prompt=DEFAULT_DOCUMENT_PROMPT, document_separator="\n\n"
+        ):
+            doc_strings = [format_document(doc, document_prompt) for doc in docs]
+            return anonymizer.anonymize(document_separator.join(doc_strings))
+        
+        _inputs = RunnableParallel(
+        standalone_question=RunnablePassthrough.assign(
+            chat_history=lambda x: anonymizer.anonymize(get_buffer_string(x["chat_history"]))
+        )
+        | CONDENSE_QUESTION_PROMPT
+        | model
+        | StrOutputParser(),
+        )
+    else :
+        def _combine_documents(
+            docs, document_prompt=DEFAULT_DOCUMENT_PROMPT, document_separator="\n\n"
+        ):
+            doc_strings = [format_document(doc, document_prompt) for doc in docs]
+            return document_separator.join(doc_strings)
+            
+        _inputs = RunnableParallel(
         standalone_question=RunnablePassthrough.assign(
             chat_history=lambda x: get_buffer_string(x["chat_history"])
         )
         | CONDENSE_QUESTION_PROMPT
         | model
         | StrOutputParser(),
-    )
+        )
+    
     _context = {
         "context": itemgetter("standalone_question") | retriever | _combine_documents,
         "question": lambda x: x["standalone_question"],
     }
+        
     conversational_qa_chain = _inputs | _context | ANSWER_PROMPT | model
-    result = conversational_qa_chain.invoke(
-        {"question": question, "chat_history": chat_history},
-        config={"callbacks": [langfuse_handler]}
-    )
-    
-    response=json.loads(result.json())["content"]
+        
+    if(trace_details):
+        result = conversational_qa_chain.invoke(
+            {"question": question, "chat_history": chat_history},
+            config={"callbacks": [langfuse_handler]}
+        )
+    else:
+        result = conversational_qa_chain.invoke(
+            {"question": question, "chat_history": chat_history}
+        )
     
+    if inference_model.name == InferenceModelMaster.BEDROCK_TEXT_EXPRES_V1 or inference_model.name == InferenceModelMaster.BEDROCK_TEXT_LITE_G1 : 
+        response = f'{result}'
+    else :
+        response = json.loads(result.json())["content"]
+
+    if pii_filter_config:
+        response = anonymizer.deanonymize(response)
+
     history.add_message("user",question,pipeline_id,session_id)
     history.add_message("system",response,pipeline_id,session_id)
     return response
```

### Comparing `therix-0.1.7/therix/utils/summarizer.py` & `therix-0.1.8/therix/utils/summarizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,11 +122,18 @@
             partial_variables={"response_schema_json": pydantic_prompt},
         )
 
 
     
     if summarization_type == SummarizerTypeMaster.EXTRACTIVE.value:
         chain = prompt | llm | parser
-        return json.dumps(chain.invoke({"context": summary},config={"callbacks": [langfuse_handler]}))
+        if(trace_details):
+            return json.dumps(chain.invoke({"context": summary},config={"callbacks": [langfuse_handler]}))
+        else:
+            return json.dumps(chain.invoke({"context": summary}))
+
     else:
         chain = prompt | llm
-        return  chain.invoke({"context": summary}, config={"callbacks": [langfuse_handler]}).content
+        if(trace_details):
+            return  chain.invoke({"context": summary}, config={"callbacks": [langfuse_handler]}).content
+        else:
+            return  chain.invoke({"context": summary}).content
```

### Comparing `therix-0.1.7/PKG-INFO` & `therix-0.1.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 Metadata-Version: 2.1
 Name: therix
-Version: 0.1.7
+Version: 0.1.8
 Summary: Therix is the SDK for langchain based applications.
 License: MIT
 Author: Ajinath
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: alembic (==1.13.1)
 Requires-Dist: alembic-postgresql-enum (==1.1.2)
 Requires-Dist: boto3 (>=1.34.81,<2.0.0)
 Requires-Dist: bs4 (>=0.0.2,<0.0.3)
 Requires-Dist: coverage (>=7.4.4,<8.0.0)
+Requires-Dist: faker (>=25.1.0,<26.0.0)
 Requires-Dist: greenlet (>=3.0.3,<4.0.0)
-Requires-Dist: langchain (==0.1.13)
+Requires-Dist: langchain (>=0.1.20,<0.2.0)
+Requires-Dist: langchain-experimental (>=0.0.58,<0.0.59)
+Requires-Dist: langchain-google-genai (>=1.0.3,<2.0.0)
 Requires-Dist: langchain-groq (>=0.1.0,<0.2.0)
 Requires-Dist: langchain-openai (==0.1.1)
 Requires-Dist: langchain-postgres (>=0.0.3,<0.0.4)
 Requires-Dist: langfuse (==2.21.1)
 Requires-Dist: pgvector (==0.2.5)
+Requires-Dist: poetry-dotenv-plugin (>=0.2.0,<0.3.0)
 Requires-Dist: presidio-analyzer (>=2.2.354,<3.0.0)
+Requires-Dist: presidio-anonymizer (>=2.2.354,<3.0.0)
 Requires-Dist: psycopg2-binary (==2.9.9)
 Requires-Dist: psycopg[binary,pool] (>=3.1.18,<4.0.0)
 Requires-Dist: pylint (>=3.1.0,<4.0.0)
 Requires-Dist: pypdf (==4.1.0)
 Requires-Dist: pytest-cov (>=5.0.0,<6.0.0)
 Requires-Dist: pytube (>=15.0.0,<16.0.0)
 Requires-Dist: selenium (>=4.19.0,<5.0.0)
```

