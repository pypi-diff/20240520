# Comparing `tmp/pr-agent-0.2.1.tar.gz` & `tmp/pr_agent-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pr-agent-0.2.1.tar", last modified: Sat Mar 23 14:24:48 2024, max compression
+gzip compressed data, was "pr_agent-0.2.2.tar", last modified: Mon May 20 06:29:57 2024, max compression
```

## Comparing `pr-agent-0.2.1.tar` & `pr_agent-0.2.2.tar`

### file list

```diff
@@ -1,104 +1,105 @@
-drwxr-xr-x   0 talrid     (501) staff       (20)        0 2024-03-23 14:24:48.524184 pr-agent-0.2.1/
--rw-r--r--   0 talrid     (501) staff       (20)    11344 2023-07-06 05:03:34.000000 pr-agent-0.2.1/LICENSE
--rw-r--r--   0 talrid     (501) staff       (20)       75 2024-03-22 19:36:21.000000 pr-agent-0.2.1/MANIFEST.in
--rw-r--r--   0 talrid     (501) staff       (20)    33333 2024-03-23 14:24:48.523917 pr-agent-0.2.1/PKG-INFO
--rw-r--r--   0 talrid     (501) staff       (20)    18853 2024-03-23 09:16:10.000000 pr-agent-0.2.1/README.md
-drwxr-xr-x   0 talrid     (501) staff       (20)        0 2024-03-23 14:24:48.502404 pr-agent-0.2.1/pr_agent/
--rw-r--r--   0 talrid     (501) staff       (20)        1 2023-07-06 05:03:34.000000 pr-agent-0.2.1/pr_agent/__init__.py
-drwxr-xr-x   0 talrid     (501) staff       (20)        0 2024-03-23 14:24:48.503507 pr-agent-0.2.1/pr_agent/agent/
--rw-r--r--   0 talrid     (501) staff       (20)        0 2023-07-06 05:03:34.000000 pr-agent-0.2.1/pr_agent/agent/__init__.py
--rw-r--r--   0 talrid     (501) staff       (20)     3798 2024-02-28 09:09:48.000000 pr-agent-0.2.1/pr_agent/agent/pr_agent.py
-drwxr-xr-x   0 talrid     (501) staff       (20)        0 2024-03-23 14:24:48.506093 pr-agent-0.2.1/pr_agent/algo/
--rw-r--r--   0 talrid     (501) staff       (20)     1257 2024-03-19 07:30:45.000000 pr-agent-0.2.1/pr_agent/algo/__init__.py
-drwxr-xr-x   0 talrid     (501) staff       (20)        0 2024-03-23 14:24:48.507432 pr-agent-0.2.1/pr_agent/algo/ai_handlers/
--rw-r--r--   0 talrid     (501) staff       (20)      888 2024-03-16 11:41:40.000000 pr-agent-0.2.1/pr_agent/algo/ai_handlers/base_ai_handler.py
--rw-r--r--   0 talrid     (501) staff       (20)     2849 2024-01-07 17:45:34.000000 pr-agent-0.2.1/pr_agent/algo/ai_handlers/langchain_ai_handler.py
--rw-r--r--   0 talrid     (501) staff       (20)     6980 2024-03-19 07:30:45.000000 pr-agent-0.2.1/pr_agent/algo/ai_handlers/litellm_ai_handler.py
--rw-r--r--   0 talrid     (501) staff       (20)     2959 2024-02-18 08:57:40.000000 pr-agent-0.2.1/pr_agent/algo/ai_handlers/openai_ai_handler.py
--rw-r--r--   0 talrid     (501) staff       (20)     1145 2023-11-26 08:39:52.000000 pr-agent-0.2.1/pr_agent/algo/file_filter.py
--rw-r--r--   0 talrid     (501) staff       (20)    11353 2024-02-18 06:09:21.000000 pr-agent-0.2.1/pr_agent/algo/git_patch_processing.py
--rw-r--r--   0 talrid     (501) staff       (20)     2910 2023-11-26 08:39:52.000000 pr-agent-0.2.1/pr_agent/algo/language_handler.py
--rw-r--r--   0 talrid     (501) staff       (20)    17647 2024-02-25 08:59:02.000000 pr-agent-0.2.1/pr_agent/algo/pr_processing.py
--rw-r--r--   0 talrid     (501) staff       (20)     2566 2023-09-14 04:43:17.000000 pr-agent-0.2.1/pr_agent/algo/token_handler.py
--rw-r--r--   0 talrid     (501) staff       (20)      419 2024-02-06 05:37:21.000000 pr-agent-0.2.1/pr_agent/algo/types.py
--rw-r--r--   0 talrid     (501) staff       (20)    27515 2024-03-19 07:30:35.000000 pr-agent-0.2.1/pr_agent/algo/utils.py
--rw-r--r--   0 talrid     (501) staff       (20)     2894 2024-03-23 14:14:31.000000 pr-agent-0.2.1/pr_agent/cli.py
--rw-r--r--   0 talrid     (501) staff       (20)      790 2024-03-23 14:18:11.000000 pr-agent-0.2.1/pr_agent/cli_pip.py
--rw-r--r--   0 talrid     (501) staff       (20)     2131 2024-02-18 06:09:21.000000 pr-agent-0.2.1/pr_agent/config_loader.py
-drwxr-xr-x   0 talrid     (501) staff       (20)        0 2024-03-23 14:24:48.510382 pr-agent-0.2.1/pr_agent/git_providers/
--rw-r--r--   0 talrid     (501) staff       (20)     1293 2023-11-26 08:39:52.000000 pr-agent-0.2.1/pr_agent/git_providers/__init__.py
--rw-r--r--   0 talrid     (501) staff       (20)    22866 2024-03-17 07:00:04.000000 pr-agent-0.2.1/pr_agent/git_providers/azuredevops_provider.py
--rw-r--r--   0 talrid     (501) staff       (20)    16472 2024-03-17 07:00:04.000000 pr-agent-0.2.1/pr_agent/git_providers/bitbucket_provider.py
--rw-r--r--   0 talrid     (501) staff       (20)    13906 2024-03-17 07:00:04.000000 pr-agent-0.2.1/pr_agent/git_providers/bitbucket_server_provider.py
--rw-r--r--   0 talrid     (501) staff       (20)    12545 2023-09-14 04:43:17.000000 pr-agent-0.2.1/pr_agent/git_providers/codecommit_client.py
--rw-r--r--   0 talrid     (501) staff       (20)    19326 2024-03-17 07:00:04.000000 pr-agent-0.2.1/pr_agent/git_providers/codecommit_provider.py
--rw-r--r--   0 talrid     (501) staff       (20)    12789 2024-03-17 07:00:04.000000 pr-agent-0.2.1/pr_agent/git_providers/gerrit_provider.py
--rw-r--r--   0 talrid     (501) staff       (20)    11182 2024-03-19 07:30:35.000000 pr-agent-0.2.1/pr_agent/git_providers/git_provider.py
--rw-r--r--   0 talrid     (501) staff       (20)    34209 2024-03-19 07:30:35.000000 pr-agent-0.2.1/pr_agent/git_providers/github_provider.py
--rw-r--r--   0 talrid     (501) staff       (20)    21964 2024-03-17 07:00:04.000000 pr-agent-0.2.1/pr_agent/git_providers/gitlab_provider.py
--rw-r--r--   0 talrid     (501) staff       (20)     8023 2024-03-17 07:00:04.000000 pr-agent-0.2.1/pr_agent/git_providers/local_git_provider.py
--rw-r--r--   0 talrid     (501) staff       (20)     2030 2024-02-25 08:59:02.000000 pr-agent-0.2.1/pr_agent/git_providers/utils.py
-drwxr-xr-x   0 talrid     (501) staff       (20)        0 2024-03-23 14:24:48.511159 pr-agent-0.2.1/pr_agent/identity_providers/
--rw-r--r--   0 talrid     (501) staff       (20)      509 2024-02-28 09:09:48.000000 pr-agent-0.2.1/pr_agent/identity_providers/__init__.py
--rw-r--r--   0 talrid     (501) staff       (20)      329 2024-02-28 09:09:48.000000 pr-agent-0.2.1/pr_agent/identity_providers/default_identity_provider.py
--rw-r--r--   0 talrid     (501) staff       (20)      374 2024-02-28 09:09:48.000000 pr-agent-0.2.1/pr_agent/identity_providers/identity_provider.py
-drwxr-xr-x   0 talrid     (501) staff       (20)        0 2024-03-23 14:24:48.511862 pr-agent-0.2.1/pr_agent/log/
--rw-r--r--   0 talrid     (501) staff       (20)     1700 2024-03-16 11:42:46.000000 pr-agent-0.2.1/pr_agent/log/__init__.py
-drwxr-xr-x   0 talrid     (501) staff       (20)        0 2024-03-23 14:24:48.512823 pr-agent-0.2.1/pr_agent/secret_providers/
--rw-r--r--   0 talrid     (501) staff       (20)      652 2024-02-06 15:38:46.000000 pr-agent-0.2.1/pr_agent/secret_providers/__init__.py
--rw-r--r--   0 talrid     (501) staff       (20)     1442 2023-10-26 08:44:30.000000 pr-agent-0.2.1/pr_agent/secret_providers/google_cloud_storage_secret_provider.py
--rw-r--r--   0 talrid     (501) staff       (20)      249 2023-09-05 05:03:53.000000 pr-agent-0.2.1/pr_agent/secret_providers/secret_provider.py
-drwxr-xr-x   0 talrid     (501) staff       (20)        0 2024-03-23 14:24:48.516255 pr-agent-0.2.1/pr_agent/servers/
--rw-r--r--   0 talrid     (501) staff       (20)        0 2024-03-22 19:36:21.000000 pr-agent-0.2.1/pr_agent/servers/__init__.py
--rw-r--r--   0 talrid     (501) staff       (20)     6110 2024-03-17 07:00:04.000000 pr-agent-0.2.1/pr_agent/servers/azuredevops_server_webhook.py
--rw-r--r--   0 talrid     (501) staff       (20)     9586 2024-03-17 07:00:04.000000 pr-agent-0.2.1/pr_agent/servers/bitbucket_app.py
--rw-r--r--   0 talrid     (501) staff       (20)     2645 2023-12-25 08:34:10.000000 pr-agent-0.2.1/pr_agent/servers/bitbucket_server_webhook.py
--rw-r--r--   0 talrid     (501) staff       (20)     1861 2023-12-14 06:43:56.000000 pr-agent-0.2.1/pr_agent/servers/gerrit_server.py
--rw-r--r--   0 talrid     (501) staff       (20)     6249 2024-02-18 06:09:21.000000 pr-agent-0.2.1/pr_agent/servers/github_action_runner.py
--rw-r--r--   0 talrid     (501) staff       (20)    16806 2024-03-22 19:36:45.000000 pr-agent-0.2.1/pr_agent/servers/github_app.py
--rw-r--r--   0 talrid     (501) staff       (20)     5417 2024-03-17 07:00:04.000000 pr-agent-0.2.1/pr_agent/servers/github_polling.py
--rw-r--r--   0 talrid     (501) staff       (20)     6448 2024-03-17 07:00:04.000000 pr-agent-0.2.1/pr_agent/servers/gitlab_webhook.py
--rw-r--r--   0 talrid     (501) staff       (20)    18105 2024-03-19 07:30:35.000000 pr-agent-0.2.1/pr_agent/servers/help.py
--rw-r--r--   0 talrid     (501) staff       (20)      430 2023-11-26 05:37:01.000000 pr-agent-0.2.1/pr_agent/servers/serverless.py
--rw-r--r--   0 talrid     (501) staff       (20)     3085 2023-10-29 16:07:06.000000 pr-agent-0.2.1/pr_agent/servers/utils.py
-drwxr-xr-x   0 talrid     (501) staff       (20)        0 2024-03-23 14:24:48.519414 pr-agent-0.2.1/pr_agent/settings/
--rw-r--r--   0 talrid     (501) staff       (20)     3347 2024-02-18 06:09:21.000000 pr-agent-0.2.1/pr_agent/settings/.secrets_template.toml
--rw-r--r--   0 talrid     (501) staff       (20)     6850 2024-03-22 19:36:45.000000 pr-agent-0.2.1/pr_agent/settings/configuration.toml
--rw-r--r--   0 talrid     (501) staff       (20)      605 2023-12-14 06:12:31.000000 pr-agent-0.2.1/pr_agent/settings/custom_labels.toml
--rw-r--r--   0 talrid     (501) staff       (20)      303 2023-11-23 07:11:16.000000 pr-agent-0.2.1/pr_agent/settings/ignore.toml
--rw-r--r--   0 talrid     (501) staff       (20)    13640 2023-10-26 08:44:30.000000 pr-agent-0.2.1/pr_agent/settings/language_extensions.toml
--rw-r--r--   0 talrid     (501) staff       (20)     3274 2024-01-30 07:30:51.000000 pr-agent-0.2.1/pr_agent/settings/pr_add_docs.toml
--rw-r--r--   0 talrid     (501) staff       (20)     4717 2024-03-05 15:12:59.000000 pr-agent-0.2.1/pr_agent/settings/pr_code_suggestions_prompts.toml
--rw-r--r--   0 talrid     (501) staff       (20)     1802 2023-12-25 08:34:10.000000 pr-agent-0.2.1/pr_agent/settings/pr_custom_labels.toml
--rw-r--r--   0 talrid     (501) staff       (20)     4165 2024-02-09 10:47:00.000000 pr-agent-0.2.1/pr_agent/settings/pr_description_prompts.toml
--rw-r--r--   0 talrid     (501) staff       (20)     1244 2023-12-05 14:47:29.000000 pr-agent-0.2.1/pr_agent/settings/pr_information_from_user_prompts.toml
--rw-r--r--   0 talrid     (501) staff       (20)     1437 2024-02-18 06:09:21.000000 pr-agent-0.2.1/pr_agent/settings/pr_line_questions_prompts.toml
--rw-r--r--   0 talrid     (501) staff       (20)     1030 2024-01-21 07:35:44.000000 pr-agent-0.2.1/pr_agent/settings/pr_questions_prompts.toml
--rw-r--r--   0 talrid     (501) staff       (20)     7085 2024-03-19 07:30:35.000000 pr-agent-0.2.1/pr_agent/settings/pr_reviewer_prompts.toml
--rw-r--r--   0 talrid     (501) staff       (20)     1389 2023-12-05 14:47:29.000000 pr-agent-0.2.1/pr_agent/settings/pr_sort_code_suggestions_prompts.toml
--rw-r--r--   0 talrid     (501) staff       (20)     1321 2023-12-05 14:47:29.000000 pr-agent-0.2.1/pr_agent/settings/pr_update_changelog_prompts.toml
-drwxr-xr-x   0 talrid     (501) staff       (20)        0 2024-03-23 14:24:48.522875 pr-agent-0.2.1/pr_agent/tools/
--rw-r--r--   0 talrid     (501) staff       (20)        0 2023-07-06 05:03:34.000000 pr-agent-0.2.1/pr_agent/tools/__init__.py
--rw-r--r--   0 talrid     (501) staff       (20)     8913 2024-03-18 05:57:48.000000 pr-agent-0.2.1/pr_agent/tools/pr_add_docs.py
--rw-r--r--   0 talrid     (501) staff       (20)    24043 2024-03-20 06:36:09.000000 pr-agent-0.2.1/pr_agent/tools/pr_code_suggestions.py
--rw-r--r--   0 talrid     (501) staff       (20)     2106 2024-01-07 17:45:34.000000 pr-agent-0.2.1/pr_agent/tools/pr_config.py
--rw-r--r--   0 talrid     (501) staff       (20)    22810 2024-03-18 05:57:48.000000 pr-agent-0.2.1/pr_agent/tools/pr_description.py
--rw-r--r--   0 talrid     (501) staff       (20)     7080 2024-03-18 05:57:48.000000 pr-agent-0.2.1/pr_agent/tools/pr_generate_labels.py
--rw-r--r--   0 talrid     (501) staff       (20)     6809 2024-03-17 07:00:04.000000 pr-agent-0.2.1/pr_agent/tools/pr_help_message.py
--rw-r--r--   0 talrid     (501) staff       (20)     4008 2024-03-18 05:57:48.000000 pr-agent-0.2.1/pr_agent/tools/pr_information_from_user.py
--rw-r--r--   0 talrid     (501) staff       (20)     5414 2024-03-18 05:57:48.000000 pr-agent-0.2.1/pr_agent/tools/pr_line_questions.py
--rw-r--r--   0 talrid     (501) staff       (20)     4545 2024-03-23 07:53:30.000000 pr-agent-0.2.1/pr_agent/tools/pr_questions.py
--rw-r--r--   0 talrid     (501) staff       (20)    21183 2024-03-19 07:30:35.000000 pr-agent-0.2.1/pr_agent/tools/pr_reviewer.py
--rw-r--r--   0 talrid     (501) staff       (20)    21810 2024-03-23 07:29:13.000000 pr-agent-0.2.1/pr_agent/tools/pr_similar_issue.py
--rw-r--r--   0 talrid     (501) staff       (20)     7528 2024-03-18 05:57:48.000000 pr-agent-0.2.1/pr_agent/tools/pr_update_changelog.py
-drwxr-xr-x   0 talrid     (501) staff       (20)        0 2024-03-23 14:24:48.523455 pr-agent-0.2.1/pr_agent.egg-info/
--rw-r--r--   0 talrid     (501) staff       (20)    33333 2024-03-23 14:24:48.000000 pr-agent-0.2.1/pr_agent.egg-info/PKG-INFO
--rw-r--r--   0 talrid     (501) staff       (20)     3169 2024-03-23 14:24:48.000000 pr-agent-0.2.1/pr_agent.egg-info/SOURCES.txt
--rw-r--r--   0 talrid     (501) staff       (20)        1 2024-03-23 14:24:48.000000 pr-agent-0.2.1/pr_agent.egg-info/dependency_links.txt
--rw-r--r--   0 talrid     (501) staff       (20)       46 2024-03-23 14:24:48.000000 pr-agent-0.2.1/pr_agent.egg-info/entry_points.txt
--rw-r--r--   0 talrid     (501) staff       (20)      454 2024-03-23 14:24:48.000000 pr-agent-0.2.1/pr_agent.egg-info/requires.txt
--rw-r--r--   0 talrid     (501) staff       (20)        9 2024-03-23 14:24:48.000000 pr-agent-0.2.1/pr_agent.egg-info/top_level.txt
--rw-r--r--   0 talrid     (501) staff       (20)     1873 2024-03-23 14:16:07.000000 pr-agent-0.2.1/pyproject.toml
--rw-r--r--   0 talrid     (501) staff       (20)      715 2024-03-22 19:41:45.000000 pr-agent-0.2.1/requirements.txt
--rw-r--r--   0 talrid     (501) staff       (20)       38 2024-03-23 14:24:48.524227 pr-agent-0.2.1/setup.cfg
--rw-r--r--   0 talrid     (501) staff       (20)      152 2023-07-28 06:53:35.000000 pr-agent-0.2.1/setup.py
+drwxr-xr-x   0 talrid     (501) staff       (20)        0 2024-05-20 06:29:57.087640 pr_agent-0.2.2/
+-rw-r--r--   0 talrid     (501) staff       (20)    11344 2023-07-06 05:03:34.000000 pr_agent-0.2.2/LICENSE
+-rw-r--r--   0 talrid     (501) staff       (20)       75 2024-03-25 06:36:13.000000 pr_agent-0.2.2/MANIFEST.in
+-rw-r--r--   0 talrid     (501) staff       (20)    34611 2024-05-20 06:29:57.087350 pr_agent-0.2.2/PKG-INFO
+-rw-r--r--   0 talrid     (501) staff       (20)    20131 2024-05-20 06:28:36.000000 pr_agent-0.2.2/README.md
+drwxr-xr-x   0 talrid     (501) staff       (20)        0 2024-05-20 06:29:57.061275 pr_agent-0.2.2/pr_agent/
+-rw-r--r--   0 talrid     (501) staff       (20)        1 2023-07-06 05:03:34.000000 pr_agent-0.2.2/pr_agent/__init__.py
+drwxr-xr-x   0 talrid     (501) staff       (20)        0 2024-05-20 06:29:57.062487 pr_agent-0.2.2/pr_agent/agent/
+-rw-r--r--   0 talrid     (501) staff       (20)        0 2023-07-06 05:03:34.000000 pr_agent-0.2.2/pr_agent/agent/__init__.py
+-rw-r--r--   0 talrid     (501) staff       (20)     3924 2024-04-10 11:20:30.000000 pr_agent-0.2.2/pr_agent/agent/pr_agent.py
+drwxr-xr-x   0 talrid     (501) staff       (20)        0 2024-05-20 06:29:57.065023 pr_agent-0.2.2/pr_agent/algo/
+-rw-r--r--   0 talrid     (501) staff       (20)     1789 2024-05-18 09:27:54.000000 pr_agent-0.2.2/pr_agent/algo/__init__.py
+drwxr-xr-x   0 talrid     (501) staff       (20)        0 2024-05-20 06:29:57.066169 pr_agent-0.2.2/pr_agent/algo/ai_handlers/
+-rw-r--r--   0 talrid     (501) staff       (20)      910 2024-04-17 05:50:25.000000 pr_agent-0.2.2/pr_agent/algo/ai_handlers/base_ai_handler.py
+-rw-r--r--   0 talrid     (501) staff       (20)     2849 2024-01-07 17:45:34.000000 pr_agent-0.2.2/pr_agent/algo/ai_handlers/langchain_ai_handler.py
+-rw-r--r--   0 talrid     (501) staff       (20)     8169 2024-04-24 05:36:43.000000 pr_agent-0.2.2/pr_agent/algo/ai_handlers/litellm_ai_handler.py
+-rw-r--r--   0 talrid     (501) staff       (20)     2959 2024-02-18 08:57:40.000000 pr_agent-0.2.2/pr_agent/algo/ai_handlers/openai_ai_handler.py
+-rw-r--r--   0 talrid     (501) staff       (20)     1145 2023-11-26 08:39:52.000000 pr_agent-0.2.2/pr_agent/algo/file_filter.py
+-rw-r--r--   0 talrid     (501) staff       (20)    11353 2024-02-18 06:09:21.000000 pr_agent-0.2.2/pr_agent/algo/git_patch_processing.py
+-rw-r--r--   0 talrid     (501) staff       (20)     2910 2023-11-26 08:39:52.000000 pr_agent-0.2.2/pr_agent/algo/language_handler.py
+-rw-r--r--   0 talrid     (501) staff       (20)    18914 2024-04-12 17:28:51.000000 pr_agent-0.2.2/pr_agent/algo/pr_processing.py
+-rw-r--r--   0 talrid     (501) staff       (20)     3138 2024-04-07 05:53:13.000000 pr_agent-0.2.2/pr_agent/algo/token_handler.py
+-rw-r--r--   0 talrid     (501) staff       (20)      419 2024-02-06 05:37:21.000000 pr_agent-0.2.2/pr_agent/algo/types.py
+-rw-r--r--   0 talrid     (501) staff       (20)    29240 2024-05-20 06:28:36.000000 pr_agent-0.2.2/pr_agent/algo/utils.py
+-rw-r--r--   0 talrid     (501) staff       (20)     2902 2024-03-25 09:42:03.000000 pr_agent-0.2.2/pr_agent/cli.py
+-rw-r--r--   0 talrid     (501) staff       (20)      790 2024-04-08 11:48:44.000000 pr_agent-0.2.2/pr_agent/cli_pip.py
+-rw-r--r--   0 talrid     (501) staff       (20)     2192 2024-05-18 09:27:54.000000 pr_agent-0.2.2/pr_agent/config_loader.py
+drwxr-xr-x   0 talrid     (501) staff       (20)        0 2024-05-20 06:29:57.072766 pr_agent-0.2.2/pr_agent/git_providers/
+-rw-r--r--   0 talrid     (501) staff       (20)     1293 2023-11-26 08:39:52.000000 pr_agent-0.2.2/pr_agent/git_providers/__init__.py
+-rw-r--r--   0 talrid     (501) staff       (20)    24330 2024-05-18 09:27:54.000000 pr_agent-0.2.2/pr_agent/git_providers/azuredevops_provider.py
+-rw-r--r--   0 talrid     (501) staff       (20)    16472 2024-03-17 07:00:04.000000 pr_agent-0.2.2/pr_agent/git_providers/bitbucket_provider.py
+-rw-r--r--   0 talrid     (501) staff       (20)    13906 2024-03-17 07:00:04.000000 pr_agent-0.2.2/pr_agent/git_providers/bitbucket_server_provider.py
+-rw-r--r--   0 talrid     (501) staff       (20)    12545 2023-09-14 04:43:17.000000 pr_agent-0.2.2/pr_agent/git_providers/codecommit_client.py
+-rw-r--r--   0 talrid     (501) staff       (20)    19382 2024-04-12 16:39:48.000000 pr_agent-0.2.2/pr_agent/git_providers/codecommit_provider.py
+-rw-r--r--   0 talrid     (501) staff       (20)    12789 2024-03-17 07:00:04.000000 pr_agent-0.2.2/pr_agent/git_providers/gerrit_provider.py
+-rw-r--r--   0 talrid     (501) staff       (20)    11190 2024-05-08 05:53:19.000000 pr_agent-0.2.2/pr_agent/git_providers/git_provider.py
+-rw-r--r--   0 talrid     (501) staff       (20)    33199 2024-05-13 15:02:48.000000 pr_agent-0.2.2/pr_agent/git_providers/github_provider.py
+-rw-r--r--   0 talrid     (501) staff       (20)    21964 2024-03-17 07:00:04.000000 pr_agent-0.2.2/pr_agent/git_providers/gitlab_provider.py
+-rw-r--r--   0 talrid     (501) staff       (20)     8023 2024-03-17 07:00:04.000000 pr_agent-0.2.2/pr_agent/git_providers/local_git_provider.py
+-rw-r--r--   0 talrid     (501) staff       (20)     2030 2024-02-25 08:59:02.000000 pr_agent-0.2.2/pr_agent/git_providers/utils.py
+drwxr-xr-x   0 talrid     (501) staff       (20)        0 2024-05-20 06:29:57.073661 pr_agent-0.2.2/pr_agent/identity_providers/
+-rw-r--r--   0 talrid     (501) staff       (20)      509 2024-02-28 09:09:48.000000 pr_agent-0.2.2/pr_agent/identity_providers/__init__.py
+-rw-r--r--   0 talrid     (501) staff       (20)      329 2024-02-28 09:09:48.000000 pr_agent-0.2.2/pr_agent/identity_providers/default_identity_provider.py
+-rw-r--r--   0 talrid     (501) staff       (20)      374 2024-02-28 09:09:48.000000 pr_agent-0.2.2/pr_agent/identity_providers/identity_provider.py
+drwxr-xr-x   0 talrid     (501) staff       (20)        0 2024-05-20 06:29:57.073889 pr_agent-0.2.2/pr_agent/log/
+-rw-r--r--   0 talrid     (501) staff       (20)     1700 2024-03-16 11:42:46.000000 pr_agent-0.2.2/pr_agent/log/__init__.py
+drwxr-xr-x   0 talrid     (501) staff       (20)        0 2024-05-20 06:29:57.075259 pr_agent-0.2.2/pr_agent/secret_providers/
+-rw-r--r--   0 talrid     (501) staff       (20)      652 2024-02-06 15:38:46.000000 pr_agent-0.2.2/pr_agent/secret_providers/__init__.py
+-rw-r--r--   0 talrid     (501) staff       (20)     1442 2023-10-26 08:44:30.000000 pr_agent-0.2.2/pr_agent/secret_providers/google_cloud_storage_secret_provider.py
+-rw-r--r--   0 talrid     (501) staff       (20)      249 2023-09-05 05:03:53.000000 pr_agent-0.2.2/pr_agent/secret_providers/secret_provider.py
+drwxr-xr-x   0 talrid     (501) staff       (20)        0 2024-05-20 06:29:57.078765 pr_agent-0.2.2/pr_agent/servers/
+-rw-r--r--   0 talrid     (501) staff       (20)        0 2024-03-25 06:36:13.000000 pr_agent-0.2.2/pr_agent/servers/__init__.py
+-rw-r--r--   0 talrid     (501) staff       (20)     6110 2024-04-18 05:33:27.000000 pr_agent-0.2.2/pr_agent/servers/azuredevops_server_webhook.py
+-rw-r--r--   0 talrid     (501) staff       (20)     9586 2024-03-17 07:00:04.000000 pr_agent-0.2.2/pr_agent/servers/bitbucket_app.py
+-rw-r--r--   0 talrid     (501) staff       (20)     2645 2023-12-25 08:34:10.000000 pr_agent-0.2.2/pr_agent/servers/bitbucket_server_webhook.py
+-rw-r--r--   0 talrid     (501) staff       (20)     1861 2023-12-14 06:43:56.000000 pr_agent-0.2.2/pr_agent/servers/gerrit_server.py
+-rw-r--r--   0 talrid     (501) staff       (20)     6548 2024-04-12 16:39:48.000000 pr_agent-0.2.2/pr_agent/servers/github_action_runner.py
+-rw-r--r--   0 talrid     (501) staff       (20)    17232 2024-04-24 05:36:43.000000 pr_agent-0.2.2/pr_agent/servers/github_app.py
+-rw-r--r--   0 talrid     (501) staff       (20)     5417 2024-03-17 07:00:04.000000 pr_agent-0.2.2/pr_agent/servers/github_polling.py
+-rw-r--r--   0 talrid     (501) staff       (20)     6448 2024-03-17 07:00:04.000000 pr_agent-0.2.2/pr_agent/servers/gitlab_webhook.py
+-rw-r--r--   0 talrid     (501) staff       (20)    10722 2024-05-16 18:47:56.000000 pr_agent-0.2.2/pr_agent/servers/help.py
+-rw-r--r--   0 talrid     (501) staff       (20)      430 2023-11-26 05:37:01.000000 pr_agent-0.2.2/pr_agent/servers/serverless.py
+-rw-r--r--   0 talrid     (501) staff       (20)     3085 2023-10-29 16:07:06.000000 pr_agent-0.2.2/pr_agent/servers/utils.py
+drwxr-xr-x   0 talrid     (501) staff       (20)        0 2024-05-20 06:29:57.083403 pr_agent-0.2.2/pr_agent/settings/
+-rw-r--r--   0 talrid     (501) staff       (20)     3412 2024-04-24 05:36:43.000000 pr_agent-0.2.2/pr_agent/settings/.secrets_template.toml
+-rw-r--r--   0 talrid     (501) staff       (20)     7098 2024-05-20 06:28:36.000000 pr_agent-0.2.2/pr_agent/settings/configuration.toml
+-rw-r--r--   0 talrid     (501) staff       (20)      605 2023-12-14 06:12:31.000000 pr_agent-0.2.2/pr_agent/settings/custom_labels.toml
+-rw-r--r--   0 talrid     (501) staff       (20)      303 2023-11-23 07:11:16.000000 pr_agent-0.2.2/pr_agent/settings/ignore.toml
+-rw-r--r--   0 talrid     (501) staff       (20)    13640 2023-10-26 08:44:30.000000 pr_agent-0.2.2/pr_agent/settings/language_extensions.toml
+-rw-r--r--   0 talrid     (501) staff       (20)     3274 2024-01-30 07:30:51.000000 pr_agent-0.2.2/pr_agent/settings/pr_add_docs.toml
+-rw-r--r--   0 talrid     (501) staff       (20)     5098 2024-05-18 09:27:54.000000 pr_agent-0.2.2/pr_agent/settings/pr_code_suggestions_prompts.toml
+-rw-r--r--   0 talrid     (501) staff       (20)     4202 2024-05-18 09:27:54.000000 pr_agent-0.2.2/pr_agent/settings/pr_code_suggestions_reflect_prompts.toml
+-rw-r--r--   0 talrid     (501) staff       (20)     1802 2023-12-25 08:34:10.000000 pr_agent-0.2.2/pr_agent/settings/pr_custom_labels.toml
+-rw-r--r--   0 talrid     (501) staff       (20)     4165 2024-02-09 10:47:00.000000 pr_agent-0.2.2/pr_agent/settings/pr_description_prompts.toml
+-rw-r--r--   0 talrid     (501) staff       (20)     1244 2023-12-05 14:47:29.000000 pr_agent-0.2.2/pr_agent/settings/pr_information_from_user_prompts.toml
+-rw-r--r--   0 talrid     (501) staff       (20)     1437 2024-02-18 06:09:21.000000 pr_agent-0.2.2/pr_agent/settings/pr_line_questions_prompts.toml
+-rw-r--r--   0 talrid     (501) staff       (20)     1030 2024-01-21 07:35:44.000000 pr_agent-0.2.2/pr_agent/settings/pr_questions_prompts.toml
+-rw-r--r--   0 talrid     (501) staff       (20)     7085 2024-04-08 06:10:44.000000 pr_agent-0.2.2/pr_agent/settings/pr_reviewer_prompts.toml
+-rw-r--r--   0 talrid     (501) staff       (20)     1389 2024-05-16 17:12:28.000000 pr_agent-0.2.2/pr_agent/settings/pr_sort_code_suggestions_prompts.toml
+-rw-r--r--   0 talrid     (501) staff       (20)     1321 2023-12-05 14:47:29.000000 pr_agent-0.2.2/pr_agent/settings/pr_update_changelog_prompts.toml
+drwxr-xr-x   0 talrid     (501) staff       (20)        0 2024-05-20 06:29:57.086564 pr_agent-0.2.2/pr_agent/tools/
+-rw-r--r--   0 talrid     (501) staff       (20)        0 2023-07-06 05:03:34.000000 pr_agent-0.2.2/pr_agent/tools/__init__.py
+-rw-r--r--   0 talrid     (501) staff       (20)     8913 2024-03-18 05:57:48.000000 pr_agent-0.2.2/pr_agent/tools/pr_add_docs.py
+-rw-r--r--   0 talrid     (501) staff       (20)    31123 2024-05-20 06:28:36.000000 pr_agent-0.2.2/pr_agent/tools/pr_code_suggestions.py
+-rw-r--r--   0 talrid     (501) staff       (20)     2106 2024-01-07 17:45:34.000000 pr_agent-0.2.2/pr_agent/tools/pr_config.py
+-rw-r--r--   0 talrid     (501) staff       (20)    23839 2024-05-20 06:28:36.000000 pr_agent-0.2.2/pr_agent/tools/pr_description.py
+-rw-r--r--   0 talrid     (501) staff       (20)     7080 2024-03-18 05:57:48.000000 pr_agent-0.2.2/pr_agent/tools/pr_generate_labels.py
+-rw-r--r--   0 talrid     (501) staff       (20)     7307 2024-05-18 09:27:54.000000 pr_agent-0.2.2/pr_agent/tools/pr_help_message.py
+-rw-r--r--   0 talrid     (501) staff       (20)     4008 2024-03-18 05:57:48.000000 pr_agent-0.2.2/pr_agent/tools/pr_information_from_user.py
+-rw-r--r--   0 talrid     (501) staff       (20)     5414 2024-05-19 09:21:30.000000 pr_agent-0.2.2/pr_agent/tools/pr_line_questions.py
+-rw-r--r--   0 talrid     (501) staff       (20)     5868 2024-05-20 06:28:36.000000 pr_agent-0.2.2/pr_agent/tools/pr_questions.py
+-rw-r--r--   0 talrid     (501) staff       (20)    21567 2024-05-20 06:28:36.000000 pr_agent-0.2.2/pr_agent/tools/pr_reviewer.py
+-rw-r--r--   0 talrid     (501) staff       (20)    21810 2024-03-25 06:36:13.000000 pr_agent-0.2.2/pr_agent/tools/pr_similar_issue.py
+-rw-r--r--   0 talrid     (501) staff       (20)     7807 2024-05-20 06:28:36.000000 pr_agent-0.2.2/pr_agent/tools/pr_update_changelog.py
+drwxr-xr-x   0 talrid     (501) staff       (20)        0 2024-05-20 06:29:57.086947 pr_agent-0.2.2/pr_agent.egg-info/
+-rw-r--r--   0 talrid     (501) staff       (20)    34611 2024-05-20 06:29:57.000000 pr_agent-0.2.2/pr_agent.egg-info/PKG-INFO
+-rw-r--r--   0 talrid     (501) staff       (20)     3228 2024-05-20 06:29:57.000000 pr_agent-0.2.2/pr_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 talrid     (501) staff       (20)        1 2024-05-20 06:29:57.000000 pr_agent-0.2.2/pr_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 talrid     (501) staff       (20)       46 2024-05-20 06:29:57.000000 pr_agent-0.2.2/pr_agent.egg-info/entry_points.txt
+-rw-r--r--   0 talrid     (501) staff       (20)      454 2024-05-20 06:29:57.000000 pr_agent-0.2.2/pr_agent.egg-info/requires.txt
+-rw-r--r--   0 talrid     (501) staff       (20)        9 2024-05-20 06:29:57.000000 pr_agent-0.2.2/pr_agent.egg-info/top_level.txt
+-rw-r--r--   0 talrid     (501) staff       (20)     1873 2024-05-20 06:28:36.000000 pr_agent-0.2.2/pyproject.toml
+-rw-r--r--   0 talrid     (501) staff       (20)      715 2024-05-18 09:27:54.000000 pr_agent-0.2.2/requirements.txt
+-rw-r--r--   0 talrid     (501) staff       (20)       38 2024-05-20 06:29:57.087717 pr_agent-0.2.2/setup.cfg
+-rw-r--r--   0 talrid     (501) staff       (20)      152 2023-07-28 06:53:35.000000 pr_agent-0.2.2/setup.py
```

### Comparing `pr-agent-0.2.1/LICENSE` & `pr_agent-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/PKG-INFO` & `pr_agent-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr-agent
-Version: 0.2.1
+Version: 0.2.2
 Summary: CodiumAI PR-Agent aims to help efficiently review and handle pull requests, by providing AI feedbacks and suggestions.
 Author-email: CodiumAI <tal.r@codium.ai>
 Maintainer-email: Tal Ridnik <tal.r@codium.ai>, Ori Kotek <ori.k@codium.ai>, Hussam Lawen <hussam.l@codium.ai>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -231,15 +231,15 @@
 Requires-Dist: openai==1.13.3
 Requires-Dist: pytest==7.4.0
 Requires-Dist: PyGithub==1.59.*
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: python-gitlab==3.15.0
 Requires-Dist: retry==0.9.2
 Requires-Dist: starlette-context==0.3.6
-Requires-Dist: tiktoken==0.5.2
+Requires-Dist: tiktoken==0.7.0
 Requires-Dist: ujson==5.8.0
 Requires-Dist: uvicorn==0.22.0
 Requires-Dist: tenacity==8.2.3
 
 <div align="center">
 
 <div align="center">
@@ -248,111 +248,108 @@
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://codium.ai/images/pr_agent/logo-dark.png" width="330">
   <source media="(prefers-color-scheme: light)" srcset="https://codium.ai/images/pr_agent/logo-light.png" width="330">
   <img src="https://codium.ai/images/pr_agent/logo-light.png" alt="logo" width="330">
 
 </picture>
 <br/>
-Making pull requests less painful with an AI agent
+CodiumAI PR-Agent aims to help efficiently review and handle pull requests, by providing AI feedbacks and suggestions
 </div>
 
 [![GitHub license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/Codium-ai/pr-agent/blob/main/LICENSE)
+[![Static Badge](https://img.shields.io/badge/Chrome-Extension-violet)](https://chromewebstore.google.com/detail/pr-agent-chrome-extension/ephlnjeghhogofkifjloamocljapahnl)
 [![Discord](https://badgen.net/badge/icon/discord?icon=discord&label&color=purple)](https://discord.com/channels/1057273017547378788/1126104260430528613)
 [![Twitter](https://img.shields.io/twitter/follow/codiumai)](https://twitter.com/codiumai)
     <a href="https://github.com/Codium-ai/pr-agent/commits/main">
     <img alt="GitHub" src="https://img.shields.io/github/last-commit/Codium-ai/pr-agent/main?style=for-the-badge" height="20">
     </a>
 </div>
 
+### [Documentation](https://pr-agent-docs.codium.ai/)
+- See the [Installation Guide](https://pr-agent-docs.codium.ai/installation/) for instructions on installing PR-Agent on different platforms.
+
+- See the [Usage Guide](https://pr-agent-docs.codium.ai/usage-guide/) for instructions on running PR-Agent tools via different interfaces, such as CLI, PR Comments, or by automatically triggering them when a new PR is opened.
+
+- See the [Tools Guide](https://pr-agent-docs.codium.ai/tools/) for a detailed description of the different tools, and the available configurations for each tool.
+
+
 ## Table of Contents
 - [News and Updates](#news-and-updates)
 - [Overview](#overview)
 - [Example results](#example-results)
 - [Try it now](#try-it-now)
-- [Installation](#installation)
 - [PR-Agent Pro 💎](#pr-agent-pro-)
 - [How it works](#how-it-works)
 - [Why use PR-Agent?](#why-use-pr-agent)
   
 ## News and Updates
 
-### March 24, 2024
-PR-Agent is now available for easy installation via [pip](https://pr-agent-docs.codium.ai/installation/locally/#using-pip-package).
-
-### March 17, 2024
-- A new feature is now available for the review tool: [`require_can_be_split_review`](https://pr-agent-docs.codium.ai/tools/review/#enabledisable-features). 
-If set to true, the tool will add a section that checks if the PR contains several themes, and can be split into smaller PRs.
+### May 19, 2024
+GPT-4o is now the default fast model ("Turbo"). This model will be used for all commands except `review` and `improve`, which will still use "GPT-4-2024-04-09", since they are harder and would still benefit from the larger model.
 
-<kbd><img src="https://codium.ai/images/pr_agent/multiple_pr_themes.png" width="512"></kbd>
+### May 12, 2024
+Inspired by [AlphaCodium](https://github.com/Codium-ai/AlphaCodium) flow engineering scheme, PR-Agent now performs **self-reflection** on the code suggestions it provides,
+enabling to remove invalid suggestions, and score the valid ones. The suggestions will be presented sorted by their score, enabling to focus on the most important ones first.
 
-### March 10, 2024
-- A new [knowledge-base website](https://pr-agent-docs.codium.ai/) for PR-Agent is now available. It includes detailed information about the different tools, usage guides and more, in an accessible and organized format.
+You can also choose to automatically remove suggestions below a certain importance score threshold, by setting the `pr_code_suggestions.suggestions_score_threshold` [configuration](https://pr-agent-docs.codium.ai/tools/improve/#configuration-options).
 
-### March 8, 2024
+<kbd><img src="https://codium.ai/images/pr_agent/self_reflection1.png" width="512"></kbd>
 
-- A new tool, [Find Similar Code](https://pr-agent-docs.codium.ai/tools/similar_code/) 💎 is now available. 
-<br>This tool retrieves the most similar code components from inside the organization's codebase, or from open-source code:
+<kbd><img src="https://codium.ai/images/pr_agent/self_reflection2.png" width="512"></kbd>
 
-<kbd><a href="https://codium.ai/images/pr_agent/similar_code.mp4"><img src="https://codium.ai/images/pr_agent/similar_code_global2.png" width="512"></a></kbd>
 
-(click on the image to see an instructional video)
+### May 2, 2024
+Check out the new [PR-Agent Chrome Extension](https://chromewebstore.google.com/detail/pr-agent-chrome-extension/ephlnjeghhogofkifjloamocljapahnl) 🚀🚀🚀
 
-### Feb 29, 2024
-- You can now use the repo's [wiki page](https://pr-agent-docs.codium.ai/usage-guide/configuration_options/) to set configurations for PR-Agent 💎
+This toolbar integrates seamlessly with your GitHub environment, allowing you to access PR-Agent tools [directly from the GitHub interface](https://www.youtube.com/watch?v=gT5tli7X4H4).
+You can also easily export your chosen configuration, and use it for the automatic commands.
 
-<kbd><img src="https://codium.ai/images/pr_agent/wiki_configuration.png" width="512"></kbd>
+<kbd><img src="https://codium.ai/images/pr_agent/toolbar1.png" width="512"></kbd>
 
+<kbd><img src="https://codium.ai/images/pr_agent/toolbar2.png" width="512"></kbd>
 
 ## Overview
 <div style="text-align:left;">
 
-CodiumAI PR-Agent aims to help efficiently review and handle pull requests, by providing AI feedbacks and suggestions
-
-- See the [Installation Guide](https://pr-agent-docs.codium.ai/installation/) for instructions on installing and running the tool on different git platforms.
-
-- See the [Usage Guide](https://pr-agent-docs.codium.ai/usage-guide/) for instructions on running the PR-Agent commands via different interfaces, including _CLI_, _online usage_, or by _automatically triggering_ them when a new PR is opened.
-
-- See the [Tools Guide](https://pr-agent-docs.codium.ai/tools/) for a detailed description of the different tools.
-
 Supported commands per platform:
 
-|       |                                                                                                                   | GitHub             | Gitlab             | Bitbucket          | Azure DevOps       |
-|-------|-------------------------------------------------------------------------------------------------------------------|:--------------------:|:--------------------:|:--------------------:|:--------------------:|
-| TOOLS | Review                                                                                                            | ✅ | ✅ | ✅ | ✅ |
-|       | ⮑ Incremental                                                                                                     | ✅ |                    |                    |                    |
+|       |                                                                                                         | GitHub             | Gitlab             | Bitbucket          | Azure DevOps       |
+|-------|---------------------------------------------------------------------------------------------------------|:--------------------:|:--------------------:|:--------------------:|:--------------------:|
+| TOOLS | Review                                                                                                  | ✅ | ✅ | ✅ | ✅ |
+|       | ⮑ Incremental                                                                                           | ✅ |                    |                    |                    |
 |       | ⮑ [SOC2 Compliance](https://pr-agent-docs.codium.ai/tools/review/#soc2-ticket-compliance) 💎            | ✅ | ✅ | ✅ | ✅ |
-|       | Describe                                                                                                          | ✅ | ✅ | ✅ | ✅ |
+|       | Describe                                                                                                | ✅ | ✅ | ✅ | ✅ |
 |       | ⮑ [Inline File Summary](https://pr-agent-docs.codium.ai/tools/describe#inline-file-summary) 💎          | ✅ |                    |                    |                    |
-|       | Improve                                                                                                           | ✅ | ✅ | ✅ | ✅ |
-|       | ⮑ Extended                                                                                                        | ✅ | ✅ | ✅ | ✅ |
-|       | Ask                                                                                                               | ✅ | ✅ | ✅ | ✅ |
+|       | Improve                                                                                                 | ✅ | ✅ | ✅ | ✅ |
+|       | ⮑ Extended                                                                                              | ✅ | ✅ | ✅ | ✅ |
+|       | Ask                                                                                                     | ✅ | ✅ | ✅ | ✅ |
 |       | ⮑ [Ask on code lines](https://pr-agent-docs.codium.ai/tools/ask#ask-lines)                              | ✅ | ✅ |                    |                    |
-|       | [Custom Suggestions](https://pr-agent-docs.codium.ai/tools/custom_suggestions/) 💎                      | ✅ | ✅ | ✅ | ✅ |
+|       | [Custom Prompt](https://pr-agent-docs.codium.ai/tools/custom_prompt/) 💎                                | ✅ | ✅ | ✅ | ✅ |
 |       | [Test](https://pr-agent-docs.codium.ai/tools/test/) 💎                                                  | ✅ | ✅ |                    | ✅ |
-|       | Reflect and Review                                                                                                | ✅ | ✅ | ✅ | ✅ |
-|       | Update CHANGELOG.md                                                                                               | ✅ | ✅ | ✅ | ✅ |
-|       | Find Similar Issue                                                                                                | ✅ |                    |                    |                    |
+|       | Reflect and Review                                                                                      | ✅ | ✅ | ✅ | ✅ |
+|       | Update CHANGELOG.md                                                                                     | ✅ | ✅ | ✅ | ✅ |
+|       | Find Similar Issue                                                                                      | ✅ |                    |                    |                    |
 |       | [Add PR Documentation](https://pr-agent-docs.codium.ai/tools/documentation/) 💎                         | ✅ | ✅ |                   | ✅ |
 |       | [Custom Labels](https://pr-agent-docs.codium.ai/tools/custom_labels/) 💎                                | ✅ | ✅ |                    | ✅ |
 |       | [Analyze](https://pr-agent-docs.codium.ai/tools/analyze/) 💎                                            | ✅ | ✅ |                    | ✅ |
 |       | [CI Feedback](https://pr-agent-docs.codium.ai/tools/ci_feedback/) 💎                                    | ✅ |                    |                    |                    |
 |       | [Similar Code](https://pr-agent-docs.codium.ai/tools/similar_code/) 💎                                  | ✅ |                    |                    |                    |
-|       |                                                                                                                   |                    |                    |                    |                    |
-| USAGE | CLI                                                                                                               | ✅ | ✅ | ✅ | ✅ |
-|       | App / webhook                                                                                                     | ✅ | ✅ | ✅ | ✅ |
-|       | Tagging bot                                                                                                       | ✅ |                    |                    |                    |
-|       | Actions                                                                                                           | ✅ |                    | ✅ |                    |
-|       |                                                                                                                   |                    |                    |                    |                    |
-| CORE  | PR compression                                                                                                    | ✅ | ✅ | ✅ | ✅ |
-|       | Repo language prioritization                                                                                      | ✅ | ✅ | ✅ | ✅ |
-|       | Adaptive and token-aware file patch fitting                                                                       | ✅ | ✅ | ✅ | ✅ |
-|       | Multiple models support                                                                                           | ✅ | ✅ | ✅ | ✅ |
+|       |                                                                                                         |                    |                    |                    |                    |
+| USAGE | CLI                                                                                                     | ✅ | ✅ | ✅ | ✅ |
+|       | App / webhook                                                                                           | ✅ | ✅ | ✅ | ✅ |
+|       | Tagging bot                                                                                             | ✅ |                    |                    |                    |
+|       | Actions                                                                                                 | ✅ |                    | ✅ |                    |
+|       |                                                                                                         |                    |                    |                    |                    |
+| CORE  | PR compression                                                                                          | ✅ | ✅ | ✅ | ✅ |
+|       | Repo language prioritization                                                                            | ✅ | ✅ | ✅ | ✅ |
+|       | Adaptive and token-aware file patch fitting                                                             | ✅ | ✅ | ✅ | ✅ |
+|       | Multiple models support                                                                                 | ✅ | ✅ | ✅ | ✅ |
 |       | [Static code analysis](https://pr-agent-docs.codium.ai/core-abilities/#static-code-analysis) 💎         | ✅ | ✅ | ✅ | ✅ |
 |       | [Global and wiki configurations](https://pr-agent-docs.codium.ai/usage-guide/configuration_options/) 💎 | ✅ | ✅ | ✅ | ✅ |
-|       | [PR interactive actions](https://www.codium.ai/images/pr_agent/pr-actions.mp4) 💎                                 | ✅ |                    |                    |                    |
+|       | [PR interactive actions](https://www.codium.ai/images/pr_agent/pr-actions.mp4) 💎                       | ✅ |                    |                    |                    |
 - 💎 means this feature is available only in [PR-Agent Pro](https://www.codium.ai/pricing/)
 
 [//]: # (- Support for additional git providers is described in [here]&#40;./docs/Full_environments.md&#41;)
 ___
 
 ‣ **Auto Description ([`/describe`](https://pr-agent-docs.codium.ai/tools/describe/))**: Automatically generating PR description - title, type, summary, code walkthrough and labels.
 \
@@ -368,21 +365,21 @@
 \
 ‣ **Add Documentation 💎  ([`/add_docs`](https://pr-agent-docs.codium.ai/tools/documentation/))**: Generates documentation to methods/functions/classes that changed in the PR.
 \
 ‣ **Generate Custom Labels 💎 ([`/generate_labels`](https://pr-agent-docs.codium.ai/tools/custom_labels/))**: Generates custom labels for the PR, based on specific guidelines defined by the user.
 \
 ‣ **Analyze 💎 ([`/analyze`](https://pr-agent-docs.codium.ai/tools/analyze/))**: Identify code components that changed in the PR, and enables to interactively generate tests, docs, and code suggestions for each component.
 \
-‣ **Custom Suggestions 💎 ([`/custom_suggestions`](https://pr-agent-docs.codium.ai/tools/custom_suggestions/))**: Automatically generates custom suggestions for improving the PR code, based on specific guidelines defined by the user.
+‣ **Custom Prompt 💎 ([`/custom_prompt`](https://pr-agent-docs.codium.ai/tools/custom_prompt/))**: Automatically generates custom suggestions for improving the PR code, based on specific guidelines defined by the user.
 \
 ‣ **Generate Tests 💎 ([`/test component_name`](https://pr-agent-docs.codium.ai/tools/test/))**: Generates unit tests for a selected component, based on the PR code changes.
 \
 ‣ **CI Feedback 💎 ([`/checks ci_job`](https://pr-agent-docs.codium.ai/tools/ci_feedback/))**: Automatically generates feedback and analysis for a failed CI job.
 \
-‣ **Similar Code 💎 ([`/find_similar_component`](https://pr-agent-docs.codium.ai/tools/similar_code//))**: Retrieves the most similar code components from inside the organization's codebase, or from open-source code.
+‣ **Similar Code 💎 ([`/find_similar_component`](https://pr-agent-docs.codium.ai/tools/similar_code/))**: Retrieves the most similar code components from inside the organization's codebase, or from open-source code.
 ___
 
 ## Example results
 </div>
 <h4><a href="https://github.com/Codium-ai/pr-agent/pull/530">/describe</a></h4>
 <div align="center">
 <p float="center">
@@ -473,40 +470,55 @@
 
 
 To set up your own PR-Agent, see the [Installation](https://pr-agent-docs.codium.ai/installation/) section below.
 Note that when you set your own PR-Agent or use CodiumAI hosted PR-Agent, there is no need to mention `@CodiumAI-Agent ...`. Instead, directly start with the command, e.g., `/ask ...`.
 
 ---
 
-## Installation
-To use your own version of PR-Agent, you first need to acquire two tokens:
+[//]: # (## Installation)
+
+[//]: # (To use your own version of PR-Agent, you first need to acquire two tokens:)
+
+[//]: # ()
+[//]: # (1. An OpenAI key from [here]&#40;https://platform.openai.com/&#41;, with access to GPT-4.)
 
-1. An OpenAI key from [here](https://platform.openai.com/), with access to GPT-4.
-2. A GitHub personal access token (classic) with the repo scope.
+[//]: # (2. A GitHub personal access token &#40;classic&#41; with the repo scope.)
 
-There are several ways to use PR-Agent:
+[//]: # ()
+[//]: # (There are several ways to use PR-Agent:)
 
-**Locally**
-- [Using pip package](https://pr-agent-docs.codium.ai/installation/locally/#using-pip-package)
-- [Using Docker image](https://pr-agent-docs.codium.ai/installation/locally/#using-docker-image)
-- [Run from source](https://pr-agent-docs.codium.ai/installation/locally/#run-from-source)
+[//]: # ()
+[//]: # (**Locally**)
 
-**GitHub specific methods**
-- [Run as a GitHub Action](https://pr-agent-docs.codium.ai/installation/github/#run-as-a-github-action)
-- [Run as a GitHub App](https://pr-agent-docs.codium.ai/installation/github/#run-as-a-github-app)
+[//]: # (- [Using pip package]&#40;https://pr-agent-docs.codium.ai/installation/locally/#using-pip-package&#41;)
 
-**GitLab specific methods**
-- [Run a GitLab webhook server](https://pr-agent-docs.codium.ai/installation/gitlab/)
+[//]: # (- [Using Docker image]&#40;https://pr-agent-docs.codium.ai/installation/locally/#using-docker-image&#41;)
 
-**BitBucket specific methods**
-- [Run as a Bitbucket Pipeline](https://pr-agent-docs.codium.ai/installation/bitbucket/)
+[//]: # (- [Run from source]&#40;https://pr-agent-docs.codium.ai/installation/locally/#run-from-source&#41;)
+
+[//]: # ()
+[//]: # (**GitHub specific methods**)
+
+[//]: # (- [Run as a GitHub Action]&#40;https://pr-agent-docs.codium.ai/installation/github/#run-as-a-github-action&#41;)
+
+[//]: # (- [Run as a GitHub App]&#40;https://pr-agent-docs.codium.ai/installation/github/#run-as-a-github-app&#41;)
+
+[//]: # ()
+[//]: # (**GitLab specific methods**)
+
+[//]: # (- [Run a GitLab webhook server]&#40;https://pr-agent-docs.codium.ai/installation/gitlab/&#41;)
+
+[//]: # ()
+[//]: # (**BitBucket specific methods**)
+
+[//]: # (- [Run as a Bitbucket Pipeline]&#40;https://pr-agent-docs.codium.ai/installation/bitbucket/&#41;)
 
 ## PR-Agent Pro 💎
 [PR-Agent Pro](https://www.codium.ai/pricing/) is a hosted version of PR-Agent, provided by CodiumAI. It is available for a monthly fee, and provides the following benefits:
-1. **Fully managed** - We take care of everything for you - hosting, models, regular updates, and more. Installation is as simple as signing up and adding the PR-Agent app to your GitHub\BitBucket repo.
+1. **Fully managed** - We take care of everything for you - hosting, models, regular updates, and more. Installation is as simple as signing up and adding the PR-Agent app to your GitHub\GitLab\BitBucket repo.
 2. **Improved privacy** - No data will be stored or used to train models. PR-Agent Pro will employ zero data retention, and will use an OpenAI account with zero data retention.
 3. **Improved support** - PR-Agent Pro users will receive priority support, and will be able to request new features and capabilities.
 4. **Extra features** -In addition to the benefits listed above, PR-Agent Pro will emphasize more customization, and the usage of static code analysis, in addition to LLM logic, to improve results. 
 See [here](https://pr-agent-docs.codium.ai/#pr-agent-pro) for a list of features available in PR-Agent Pro.
 
 
 
@@ -528,19 +540,30 @@
 - Our [PR Compression strategy](https://pr-agent-docs.codium.ai/core-abilities/#pr-compression-strategy)  is a core ability that enables to effectively tackle both short and long PRs.
 - Our JSON prompting strategy enables to have **modular, customizable tools**. For example, the '/review' tool categories can be controlled via the [configuration](pr_agent/settings/configuration.toml) file. Adding additional categories is easy and accessible.
 - We support **multiple git providers** (GitHub, Gitlab, Bitbucket), **multiple ways** to use the tool (CLI, GitHub Action, GitHub App, Docker, ...), and **multiple models** (GPT-4, GPT-3.5, Anthropic, Cohere, Llama2).
 
 
 ## Data privacy
 
-If you host PR-Agent with your OpenAI API key, it is between you and OpenAI. You can read their API data privacy policy here:
+### Self-hosted PR-Agent
+
+- If you host PR-Agent with your OpenAI API key, it is between you and OpenAI. You can read their API data privacy policy here:
 https://openai.com/enterprise-privacy
 
-When using PR-Agent Pro 💎, hosted by CodiumAI, we will not store any of your data, nor will we use it for training.
-You will also benefit from an OpenAI account with zero data retention.
+### CodiumAI-hosted PR-Agent Pro 💎
+
+- When using PR-Agent Pro 💎, hosted by CodiumAI, we will not store any of your data, nor will we use it for training. You will also benefit from an OpenAI account with zero data retention.
+
+- For certain clients, CodiumAI-hosted PR-Agent Pro will use CodiumAI’s proprietary models — if this is the case, you will be notified.
+
+- No passive collection of Code and Pull Requests’ data — PR-Agent will be active only when you invoke it, and it will then extract and analyze only data relevant to the executed command and queried pull request.
+
+### PR-Agent Chrome extension
+
+- The [PR-Agent Chrome extension](https://chromewebstore.google.com/detail/pr-agent-chrome-extension/ephlnjeghhogofkifjloamocljapahnl) serves solely to modify the visual appearance of a GitHub PR screen. It does not transmit any user's repo or pull request code. Code is only sent for processing when a user submits a GitHub comment that activates a PR-Agent tool, in accordance with the standard privacy policy of PR-Agent.
 
 ## Links
 
 [![Join our Discord community](https://raw.githubusercontent.com/Codium-ai/codiumai-vscode-release/main/media/docs/Joincommunity.png)](https://discord.gg/kG35uSHDBc)
 
 - Discord community: https://discord.gg/kG35uSHDBc
 - CodiumAI site: https://codium.ai
```

### Comparing `pr-agent-0.2.1/README.md` & `pr_agent-0.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,111 +6,108 @@
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://codium.ai/images/pr_agent/logo-dark.png" width="330">
   <source media="(prefers-color-scheme: light)" srcset="https://codium.ai/images/pr_agent/logo-light.png" width="330">
   <img src="https://codium.ai/images/pr_agent/logo-light.png" alt="logo" width="330">
 
 </picture>
 <br/>
-Making pull requests less painful with an AI agent
+CodiumAI PR-Agent aims to help efficiently review and handle pull requests, by providing AI feedbacks and suggestions
 </div>
 
 [![GitHub license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/Codium-ai/pr-agent/blob/main/LICENSE)
+[![Static Badge](https://img.shields.io/badge/Chrome-Extension-violet)](https://chromewebstore.google.com/detail/pr-agent-chrome-extension/ephlnjeghhogofkifjloamocljapahnl)
 [![Discord](https://badgen.net/badge/icon/discord?icon=discord&label&color=purple)](https://discord.com/channels/1057273017547378788/1126104260430528613)
 [![Twitter](https://img.shields.io/twitter/follow/codiumai)](https://twitter.com/codiumai)
     <a href="https://github.com/Codium-ai/pr-agent/commits/main">
     <img alt="GitHub" src="https://img.shields.io/github/last-commit/Codium-ai/pr-agent/main?style=for-the-badge" height="20">
     </a>
 </div>
 
+### [Documentation](https://pr-agent-docs.codium.ai/)
+- See the [Installation Guide](https://pr-agent-docs.codium.ai/installation/) for instructions on installing PR-Agent on different platforms.
+
+- See the [Usage Guide](https://pr-agent-docs.codium.ai/usage-guide/) for instructions on running PR-Agent tools via different interfaces, such as CLI, PR Comments, or by automatically triggering them when a new PR is opened.
+
+- See the [Tools Guide](https://pr-agent-docs.codium.ai/tools/) for a detailed description of the different tools, and the available configurations for each tool.
+
+
 ## Table of Contents
 - [News and Updates](#news-and-updates)
 - [Overview](#overview)
 - [Example results](#example-results)
 - [Try it now](#try-it-now)
-- [Installation](#installation)
 - [PR-Agent Pro 💎](#pr-agent-pro-)
 - [How it works](#how-it-works)
 - [Why use PR-Agent?](#why-use-pr-agent)
   
 ## News and Updates
 
-### March 24, 2024
-PR-Agent is now available for easy installation via [pip](https://pr-agent-docs.codium.ai/installation/locally/#using-pip-package).
-
-### March 17, 2024
-- A new feature is now available for the review tool: [`require_can_be_split_review`](https://pr-agent-docs.codium.ai/tools/review/#enabledisable-features). 
-If set to true, the tool will add a section that checks if the PR contains several themes, and can be split into smaller PRs.
+### May 19, 2024
+GPT-4o is now the default fast model ("Turbo"). This model will be used for all commands except `review` and `improve`, which will still use "GPT-4-2024-04-09", since they are harder and would still benefit from the larger model.
 
-<kbd><img src="https://codium.ai/images/pr_agent/multiple_pr_themes.png" width="512"></kbd>
+### May 12, 2024
+Inspired by [AlphaCodium](https://github.com/Codium-ai/AlphaCodium) flow engineering scheme, PR-Agent now performs **self-reflection** on the code suggestions it provides,
+enabling to remove invalid suggestions, and score the valid ones. The suggestions will be presented sorted by their score, enabling to focus on the most important ones first.
 
-### March 10, 2024
-- A new [knowledge-base website](https://pr-agent-docs.codium.ai/) for PR-Agent is now available. It includes detailed information about the different tools, usage guides and more, in an accessible and organized format.
+You can also choose to automatically remove suggestions below a certain importance score threshold, by setting the `pr_code_suggestions.suggestions_score_threshold` [configuration](https://pr-agent-docs.codium.ai/tools/improve/#configuration-options).
 
-### March 8, 2024
+<kbd><img src="https://codium.ai/images/pr_agent/self_reflection1.png" width="512"></kbd>
 
-- A new tool, [Find Similar Code](https://pr-agent-docs.codium.ai/tools/similar_code/) 💎 is now available. 
-<br>This tool retrieves the most similar code components from inside the organization's codebase, or from open-source code:
+<kbd><img src="https://codium.ai/images/pr_agent/self_reflection2.png" width="512"></kbd>
 
-<kbd><a href="https://codium.ai/images/pr_agent/similar_code.mp4"><img src="https://codium.ai/images/pr_agent/similar_code_global2.png" width="512"></a></kbd>
 
-(click on the image to see an instructional video)
+### May 2, 2024
+Check out the new [PR-Agent Chrome Extension](https://chromewebstore.google.com/detail/pr-agent-chrome-extension/ephlnjeghhogofkifjloamocljapahnl) 🚀🚀🚀
 
-### Feb 29, 2024
-- You can now use the repo's [wiki page](https://pr-agent-docs.codium.ai/usage-guide/configuration_options/) to set configurations for PR-Agent 💎
+This toolbar integrates seamlessly with your GitHub environment, allowing you to access PR-Agent tools [directly from the GitHub interface](https://www.youtube.com/watch?v=gT5tli7X4H4).
+You can also easily export your chosen configuration, and use it for the automatic commands.
 
-<kbd><img src="https://codium.ai/images/pr_agent/wiki_configuration.png" width="512"></kbd>
+<kbd><img src="https://codium.ai/images/pr_agent/toolbar1.png" width="512"></kbd>
 
+<kbd><img src="https://codium.ai/images/pr_agent/toolbar2.png" width="512"></kbd>
 
 ## Overview
 <div style="text-align:left;">
 
-CodiumAI PR-Agent aims to help efficiently review and handle pull requests, by providing AI feedbacks and suggestions
-
-- See the [Installation Guide](https://pr-agent-docs.codium.ai/installation/) for instructions on installing and running the tool on different git platforms.
-
-- See the [Usage Guide](https://pr-agent-docs.codium.ai/usage-guide/) for instructions on running the PR-Agent commands via different interfaces, including _CLI_, _online usage_, or by _automatically triggering_ them when a new PR is opened.
-
-- See the [Tools Guide](https://pr-agent-docs.codium.ai/tools/) for a detailed description of the different tools.
-
 Supported commands per platform:
 
-|       |                                                                                                                   | GitHub             | Gitlab             | Bitbucket          | Azure DevOps       |
-|-------|-------------------------------------------------------------------------------------------------------------------|:--------------------:|:--------------------:|:--------------------:|:--------------------:|
-| TOOLS | Review                                                                                                            | ✅ | ✅ | ✅ | ✅ |
-|       | ⮑ Incremental                                                                                                     | ✅ |                    |                    |                    |
+|       |                                                                                                         | GitHub             | Gitlab             | Bitbucket          | Azure DevOps       |
+|-------|---------------------------------------------------------------------------------------------------------|:--------------------:|:--------------------:|:--------------------:|:--------------------:|
+| TOOLS | Review                                                                                                  | ✅ | ✅ | ✅ | ✅ |
+|       | ⮑ Incremental                                                                                           | ✅ |                    |                    |                    |
 |       | ⮑ [SOC2 Compliance](https://pr-agent-docs.codium.ai/tools/review/#soc2-ticket-compliance) 💎            | ✅ | ✅ | ✅ | ✅ |
-|       | Describe                                                                                                          | ✅ | ✅ | ✅ | ✅ |
+|       | Describe                                                                                                | ✅ | ✅ | ✅ | ✅ |
 |       | ⮑ [Inline File Summary](https://pr-agent-docs.codium.ai/tools/describe#inline-file-summary) 💎          | ✅ |                    |                    |                    |
-|       | Improve                                                                                                           | ✅ | ✅ | ✅ | ✅ |
-|       | ⮑ Extended                                                                                                        | ✅ | ✅ | ✅ | ✅ |
-|       | Ask                                                                                                               | ✅ | ✅ | ✅ | ✅ |
+|       | Improve                                                                                                 | ✅ | ✅ | ✅ | ✅ |
+|       | ⮑ Extended                                                                                              | ✅ | ✅ | ✅ | ✅ |
+|       | Ask                                                                                                     | ✅ | ✅ | ✅ | ✅ |
 |       | ⮑ [Ask on code lines](https://pr-agent-docs.codium.ai/tools/ask#ask-lines)                              | ✅ | ✅ |                    |                    |
-|       | [Custom Suggestions](https://pr-agent-docs.codium.ai/tools/custom_suggestions/) 💎                      | ✅ | ✅ | ✅ | ✅ |
+|       | [Custom Prompt](https://pr-agent-docs.codium.ai/tools/custom_prompt/) 💎                                | ✅ | ✅ | ✅ | ✅ |
 |       | [Test](https://pr-agent-docs.codium.ai/tools/test/) 💎                                                  | ✅ | ✅ |                    | ✅ |
-|       | Reflect and Review                                                                                                | ✅ | ✅ | ✅ | ✅ |
-|       | Update CHANGELOG.md                                                                                               | ✅ | ✅ | ✅ | ✅ |
-|       | Find Similar Issue                                                                                                | ✅ |                    |                    |                    |
+|       | Reflect and Review                                                                                      | ✅ | ✅ | ✅ | ✅ |
+|       | Update CHANGELOG.md                                                                                     | ✅ | ✅ | ✅ | ✅ |
+|       | Find Similar Issue                                                                                      | ✅ |                    |                    |                    |
 |       | [Add PR Documentation](https://pr-agent-docs.codium.ai/tools/documentation/) 💎                         | ✅ | ✅ |                   | ✅ |
 |       | [Custom Labels](https://pr-agent-docs.codium.ai/tools/custom_labels/) 💎                                | ✅ | ✅ |                    | ✅ |
 |       | [Analyze](https://pr-agent-docs.codium.ai/tools/analyze/) 💎                                            | ✅ | ✅ |                    | ✅ |
 |       | [CI Feedback](https://pr-agent-docs.codium.ai/tools/ci_feedback/) 💎                                    | ✅ |                    |                    |                    |
 |       | [Similar Code](https://pr-agent-docs.codium.ai/tools/similar_code/) 💎                                  | ✅ |                    |                    |                    |
-|       |                                                                                                                   |                    |                    |                    |                    |
-| USAGE | CLI                                                                                                               | ✅ | ✅ | ✅ | ✅ |
-|       | App / webhook                                                                                                     | ✅ | ✅ | ✅ | ✅ |
-|       | Tagging bot                                                                                                       | ✅ |                    |                    |                    |
-|       | Actions                                                                                                           | ✅ |                    | ✅ |                    |
-|       |                                                                                                                   |                    |                    |                    |                    |
-| CORE  | PR compression                                                                                                    | ✅ | ✅ | ✅ | ✅ |
-|       | Repo language prioritization                                                                                      | ✅ | ✅ | ✅ | ✅ |
-|       | Adaptive and token-aware file patch fitting                                                                       | ✅ | ✅ | ✅ | ✅ |
-|       | Multiple models support                                                                                           | ✅ | ✅ | ✅ | ✅ |
+|       |                                                                                                         |                    |                    |                    |                    |
+| USAGE | CLI                                                                                                     | ✅ | ✅ | ✅ | ✅ |
+|       | App / webhook                                                                                           | ✅ | ✅ | ✅ | ✅ |
+|       | Tagging bot                                                                                             | ✅ |                    |                    |                    |
+|       | Actions                                                                                                 | ✅ |                    | ✅ |                    |
+|       |                                                                                                         |                    |                    |                    |                    |
+| CORE  | PR compression                                                                                          | ✅ | ✅ | ✅ | ✅ |
+|       | Repo language prioritization                                                                            | ✅ | ✅ | ✅ | ✅ |
+|       | Adaptive and token-aware file patch fitting                                                             | ✅ | ✅ | ✅ | ✅ |
+|       | Multiple models support                                                                                 | ✅ | ✅ | ✅ | ✅ |
 |       | [Static code analysis](https://pr-agent-docs.codium.ai/core-abilities/#static-code-analysis) 💎         | ✅ | ✅ | ✅ | ✅ |
 |       | [Global and wiki configurations](https://pr-agent-docs.codium.ai/usage-guide/configuration_options/) 💎 | ✅ | ✅ | ✅ | ✅ |
-|       | [PR interactive actions](https://www.codium.ai/images/pr_agent/pr-actions.mp4) 💎                                 | ✅ |                    |                    |                    |
+|       | [PR interactive actions](https://www.codium.ai/images/pr_agent/pr-actions.mp4) 💎                       | ✅ |                    |                    |                    |
 - 💎 means this feature is available only in [PR-Agent Pro](https://www.codium.ai/pricing/)
 
 [//]: # (- Support for additional git providers is described in [here]&#40;./docs/Full_environments.md&#41;)
 ___
 
 ‣ **Auto Description ([`/describe`](https://pr-agent-docs.codium.ai/tools/describe/))**: Automatically generating PR description - title, type, summary, code walkthrough and labels.
 \
@@ -126,21 +123,21 @@
 \
 ‣ **Add Documentation 💎  ([`/add_docs`](https://pr-agent-docs.codium.ai/tools/documentation/))**: Generates documentation to methods/functions/classes that changed in the PR.
 \
 ‣ **Generate Custom Labels 💎 ([`/generate_labels`](https://pr-agent-docs.codium.ai/tools/custom_labels/))**: Generates custom labels for the PR, based on specific guidelines defined by the user.
 \
 ‣ **Analyze 💎 ([`/analyze`](https://pr-agent-docs.codium.ai/tools/analyze/))**: Identify code components that changed in the PR, and enables to interactively generate tests, docs, and code suggestions for each component.
 \
-‣ **Custom Suggestions 💎 ([`/custom_suggestions`](https://pr-agent-docs.codium.ai/tools/custom_suggestions/))**: Automatically generates custom suggestions for improving the PR code, based on specific guidelines defined by the user.
+‣ **Custom Prompt 💎 ([`/custom_prompt`](https://pr-agent-docs.codium.ai/tools/custom_prompt/))**: Automatically generates custom suggestions for improving the PR code, based on specific guidelines defined by the user.
 \
 ‣ **Generate Tests 💎 ([`/test component_name`](https://pr-agent-docs.codium.ai/tools/test/))**: Generates unit tests for a selected component, based on the PR code changes.
 \
 ‣ **CI Feedback 💎 ([`/checks ci_job`](https://pr-agent-docs.codium.ai/tools/ci_feedback/))**: Automatically generates feedback and analysis for a failed CI job.
 \
-‣ **Similar Code 💎 ([`/find_similar_component`](https://pr-agent-docs.codium.ai/tools/similar_code//))**: Retrieves the most similar code components from inside the organization's codebase, or from open-source code.
+‣ **Similar Code 💎 ([`/find_similar_component`](https://pr-agent-docs.codium.ai/tools/similar_code/))**: Retrieves the most similar code components from inside the organization's codebase, or from open-source code.
 ___
 
 ## Example results
 </div>
 <h4><a href="https://github.com/Codium-ai/pr-agent/pull/530">/describe</a></h4>
 <div align="center">
 <p float="center">
@@ -231,40 +228,55 @@
 
 
 To set up your own PR-Agent, see the [Installation](https://pr-agent-docs.codium.ai/installation/) section below.
 Note that when you set your own PR-Agent or use CodiumAI hosted PR-Agent, there is no need to mention `@CodiumAI-Agent ...`. Instead, directly start with the command, e.g., `/ask ...`.
 
 ---
 
-## Installation
-To use your own version of PR-Agent, you first need to acquire two tokens:
+[//]: # (## Installation)
+
+[//]: # (To use your own version of PR-Agent, you first need to acquire two tokens:)
+
+[//]: # ()
+[//]: # (1. An OpenAI key from [here]&#40;https://platform.openai.com/&#41;, with access to GPT-4.)
 
-1. An OpenAI key from [here](https://platform.openai.com/), with access to GPT-4.
-2. A GitHub personal access token (classic) with the repo scope.
+[//]: # (2. A GitHub personal access token &#40;classic&#41; with the repo scope.)
 
-There are several ways to use PR-Agent:
+[//]: # ()
+[//]: # (There are several ways to use PR-Agent:)
 
-**Locally**
-- [Using pip package](https://pr-agent-docs.codium.ai/installation/locally/#using-pip-package)
-- [Using Docker image](https://pr-agent-docs.codium.ai/installation/locally/#using-docker-image)
-- [Run from source](https://pr-agent-docs.codium.ai/installation/locally/#run-from-source)
+[//]: # ()
+[//]: # (**Locally**)
 
-**GitHub specific methods**
-- [Run as a GitHub Action](https://pr-agent-docs.codium.ai/installation/github/#run-as-a-github-action)
-- [Run as a GitHub App](https://pr-agent-docs.codium.ai/installation/github/#run-as-a-github-app)
+[//]: # (- [Using pip package]&#40;https://pr-agent-docs.codium.ai/installation/locally/#using-pip-package&#41;)
 
-**GitLab specific methods**
-- [Run a GitLab webhook server](https://pr-agent-docs.codium.ai/installation/gitlab/)
+[//]: # (- [Using Docker image]&#40;https://pr-agent-docs.codium.ai/installation/locally/#using-docker-image&#41;)
 
-**BitBucket specific methods**
-- [Run as a Bitbucket Pipeline](https://pr-agent-docs.codium.ai/installation/bitbucket/)
+[//]: # (- [Run from source]&#40;https://pr-agent-docs.codium.ai/installation/locally/#run-from-source&#41;)
+
+[//]: # ()
+[//]: # (**GitHub specific methods**)
+
+[//]: # (- [Run as a GitHub Action]&#40;https://pr-agent-docs.codium.ai/installation/github/#run-as-a-github-action&#41;)
+
+[//]: # (- [Run as a GitHub App]&#40;https://pr-agent-docs.codium.ai/installation/github/#run-as-a-github-app&#41;)
+
+[//]: # ()
+[//]: # (**GitLab specific methods**)
+
+[//]: # (- [Run a GitLab webhook server]&#40;https://pr-agent-docs.codium.ai/installation/gitlab/&#41;)
+
+[//]: # ()
+[//]: # (**BitBucket specific methods**)
+
+[//]: # (- [Run as a Bitbucket Pipeline]&#40;https://pr-agent-docs.codium.ai/installation/bitbucket/&#41;)
 
 ## PR-Agent Pro 💎
 [PR-Agent Pro](https://www.codium.ai/pricing/) is a hosted version of PR-Agent, provided by CodiumAI. It is available for a monthly fee, and provides the following benefits:
-1. **Fully managed** - We take care of everything for you - hosting, models, regular updates, and more. Installation is as simple as signing up and adding the PR-Agent app to your GitHub\BitBucket repo.
+1. **Fully managed** - We take care of everything for you - hosting, models, regular updates, and more. Installation is as simple as signing up and adding the PR-Agent app to your GitHub\GitLab\BitBucket repo.
 2. **Improved privacy** - No data will be stored or used to train models. PR-Agent Pro will employ zero data retention, and will use an OpenAI account with zero data retention.
 3. **Improved support** - PR-Agent Pro users will receive priority support, and will be able to request new features and capabilities.
 4. **Extra features** -In addition to the benefits listed above, PR-Agent Pro will emphasize more customization, and the usage of static code analysis, in addition to LLM logic, to improve results. 
 See [here](https://pr-agent-docs.codium.ai/#pr-agent-pro) for a list of features available in PR-Agent Pro.
 
 
 
@@ -286,19 +298,30 @@
 - Our [PR Compression strategy](https://pr-agent-docs.codium.ai/core-abilities/#pr-compression-strategy)  is a core ability that enables to effectively tackle both short and long PRs.
 - Our JSON prompting strategy enables to have **modular, customizable tools**. For example, the '/review' tool categories can be controlled via the [configuration](pr_agent/settings/configuration.toml) file. Adding additional categories is easy and accessible.
 - We support **multiple git providers** (GitHub, Gitlab, Bitbucket), **multiple ways** to use the tool (CLI, GitHub Action, GitHub App, Docker, ...), and **multiple models** (GPT-4, GPT-3.5, Anthropic, Cohere, Llama2).
 
 
 ## Data privacy
 
-If you host PR-Agent with your OpenAI API key, it is between you and OpenAI. You can read their API data privacy policy here:
+### Self-hosted PR-Agent
+
+- If you host PR-Agent with your OpenAI API key, it is between you and OpenAI. You can read their API data privacy policy here:
 https://openai.com/enterprise-privacy
 
-When using PR-Agent Pro 💎, hosted by CodiumAI, we will not store any of your data, nor will we use it for training.
-You will also benefit from an OpenAI account with zero data retention.
+### CodiumAI-hosted PR-Agent Pro 💎
+
+- When using PR-Agent Pro 💎, hosted by CodiumAI, we will not store any of your data, nor will we use it for training. You will also benefit from an OpenAI account with zero data retention.
+
+- For certain clients, CodiumAI-hosted PR-Agent Pro will use CodiumAI’s proprietary models — if this is the case, you will be notified.
+
+- No passive collection of Code and Pull Requests’ data — PR-Agent will be active only when you invoke it, and it will then extract and analyze only data relevant to the executed command and queried pull request.
+
+### PR-Agent Chrome extension
+
+- The [PR-Agent Chrome extension](https://chromewebstore.google.com/detail/pr-agent-chrome-extension/ephlnjeghhogofkifjloamocljapahnl) serves solely to modify the visual appearance of a GitHub PR screen. It does not transmit any user's repo or pull request code. Code is only sent for processing when a user submits a GitHub comment that activates a PR-Agent tool, in accordance with the standard privacy policy of PR-Agent.
 
 ## Links
 
 [![Join our Discord community](https://raw.githubusercontent.com/Codium-ai/codiumai-vscode-release/main/media/docs/Joincommunity.png)](https://discord.gg/kG35uSHDBc)
 
 - Discord community: https://discord.gg/kG35uSHDBc
 - CodiumAI site: https://codium.ai
```

#### html2text {}

```diff
@@ -1,113 +1,117 @@
                                     [logo]
-              Making pull requests less painful with an AI agent
- [![GitHub license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)]
-(https://github.com/Codium-ai/pr-agent/blob/main/LICENSE) [![Discord](https://
-   badgen.net/badge/icon/discord?icon=discord&label&color=purple)](https://
-   discord.com/channels/1057273017547378788/1126104260430528613) [![Twitter]
-(https://img.shields.io/twitter/follow/codiumai)](https://twitter.com/codiumai)
-                                   _[_G_i_t_H_u_b_]
-## Table of Contents - [News and Updates](#news-and-updates) - [Overview]
-(#overview) - [Example results](#example-results) - [Try it now](#try-it-now) -
-[Installation](#installation) - [PR-Agent Pro ð](#pr-agent-pro-) - [How it
-works](#how-it-works) - [Why use PR-Agent?](#why-use-pr-agent) ## News and
-Updates ### March 24, 2024 PR-Agent is now available for easy installation via
-[pip](https://pr-agent-docs.codium.ai/installation/locally/#using-pip-package).
-### March 17, 2024 - A new feature is now available for the review tool:
-[`require_can_be_split_review`](https://pr-agent-docs.codium.ai/tools/review/
-#enabledisable-features). If set to true, the tool will add a section that
-checks if the PR contains several themes, and can be split into smaller PRs.
-[https://codium.ai/images/pr_agent/multiple_pr_themes.png]### March 10, 2024 -
-A new [knowledge-base website](https://pr-agent-docs.codium.ai/) for PR-Agent
-is now available. It includes detailed information about the different tools,
-usage guides and more, in an accessible and organized format. ### March 8, 2024
-- A new tool, [Find Similar Code](https://pr-agent-docs.codium.ai/tools/
-similar_code/) ð is now available.
-This tool retrieves the most similar code components from inside the
-organization's codebase, or from open-source code: _[_h_t_t_p_s_:_/_/_c_o_d_i_u_m_._a_i_/_i_m_a_g_e_s_/
-_p_r___a_g_e_n_t_/_s_i_m_i_l_a_r___c_o_d_e___g_l_o_b_a_l_2_._p_n_g_](click on the image to see an instructional
-video) ### Feb 29, 2024 - You can now use the repo's [wiki page](https://pr-
-agent-docs.codium.ai/usage-guide/configuration_options/) to set configurations
-for PR-Agent ð [https://codium.ai/images/pr_agent/wiki_configuration.png]##
-Overview
 CodiumAI PR-Agent aims to help efficiently review and handle pull requests, by
-providing AI feedbacks and suggestions - See the [Installation Guide](https://
-pr-agent-docs.codium.ai/installation/) for instructions on installing and
-running the tool on different git platforms. - See the [Usage Guide](https://
-pr-agent-docs.codium.ai/usage-guide/) for instructions on running the PR-Agent
-commands via different interfaces, including _CLI_, _online usage_, or by
-_automatically triggering_ them when a new PR is opened. - See the [Tools
-Guide](https://pr-agent-docs.codium.ai/tools/) for a detailed description of
-the different tools. Supported commands per platform: | | | GitHub | Gitlab |
-Bitbucket | Azure DevOps | |-------|-------------------------------------------
-------------------------------------------------------------------------|:-----
----------------:|:--------------------:|:--------------------:|:---------------
------:| | TOOLS | Review | â | â | â | â | | | â® Incremental | â |
-| | | | | â® [SOC2 Compliance](https://pr-agent-docs.codium.ai/tools/review/
-#soc2-ticket-compliance) ð | â | â | â | â | | | Describe | â |
-â | â | â | | | â® [Inline File Summary](https://pr-agent-
-docs.codium.ai/tools/describe#inline-file-summary) ð | â | | | | | |
-Improve | â | â | â | â | | | â® Extended | â | â | â | â | |
-| Ask | â | â | â | â | | | â® [Ask on code lines](https://pr-agent-
-docs.codium.ai/tools/ask#ask-lines) | â | â | | | | | [Custom Suggestions]
-(https://pr-agent-docs.codium.ai/tools/custom_suggestions/) ð | â | â |
-â | â | | | [Test](https://pr-agent-docs.codium.ai/tools/test/) ð | â
-| â | | â | | | Reflect and Review | â | â | â | â | | | Update
-CHANGELOG.md | â | â | â | â | | | Find Similar Issue | â | | | | | |
-[Add PR Documentation](https://pr-agent-docs.codium.ai/tools/documentation/
-) ð | â | â | | â | | | [Custom Labels](https://pr-agent-
-docs.codium.ai/tools/custom_labels/) ð | â | â | | â | | | [Analyze]
-(https://pr-agent-docs.codium.ai/tools/analyze/) ð | â | â | | â | | |
-[CI Feedback](https://pr-agent-docs.codium.ai/tools/ci_feedback/) ð | â |
-| | | | | [Similar Code](https://pr-agent-docs.codium.ai/tools/similar_code/
-) ð | â | | | | | | | | | | | | USAGE | CLI | â | â | â | â | | |
-App / webhook | â | â | â | â | | | Tagging bot | â | | | | | |
-Actions | â | | â | | | | | | | | | | CORE | PR compression | â | â |
-â | â | | | Repo language prioritization | â | â | â | â | | |
-Adaptive and token-aware file patch fitting | â | â | â | â | | |
-Multiple models support | â | â | â | â | | | [Static code analysis]
-(https://pr-agent-docs.codium.ai/core-abilities/#static-code-analysis) ð |
-â | â | â | â | | | [Global and wiki configurations](https://pr-agent-
-docs.codium.ai/usage-guide/configuration_options/) ð | â | â | â | â
-| | | [PR interactive actions](https://www.codium.ai/images/pr_agent/pr-
-actions.mp4) ð | â | | | | - ð means this feature is available only in
-[PR-Agent Pro](https://www.codium.ai/pricing/) [//]: # (- Support for
-additional git providers is described in [here](./docs/Full_environments.md))
-___ â£ **Auto Description ([`/describe`](https://pr-agent-docs.codium.ai/
-tools/describe/))**: Automatically generating PR description - title, type,
-summary, code walkthrough and labels. \ â£ **Auto Review ([`/review`](https://
-pr-agent-docs.codium.ai/tools/review/))**: Adjustable feedback about the PR,
-possible issues, security concerns, review effort and more. \ â£ **Code
-Suggestions ([`/improve`](https://pr-agent-docs.codium.ai/tools/improve/))**:
-Code suggestions for improving the PR. \ â£ **Question Answering ([`/ask ...`]
+                    providing AI feedbacks and suggestions
+ [![GitHub license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)]
+  (https://github.com/Codium-ai/pr-agent/blob/main/LICENSE) [![Static Badge]
+       (https://img.shields.io/badge/Chrome-Extension-violet)](https://
+          chromewebstore.google.com/detail/pr-agent-chrome-extension/
+ ephlnjeghhogofkifjloamocljapahnl) [![Discord](https://badgen.net/badge/icon/
+    discord?icon=discord&label&color=purple)](https://discord.com/channels/
+ 1057273017547378788/1126104260430528613) [![Twitter](https://img.shields.io/
+        twitter/follow/codiumai)](https://twitter.com/codiumai)_[_G_i_t_H_u_b_]
+### [Documentation](https://pr-agent-docs.codium.ai/) - See the [Installation
+Guide](https://pr-agent-docs.codium.ai/installation/) for instructions on
+installing PR-Agent on different platforms. - See the [Usage Guide](https://pr-
+agent-docs.codium.ai/usage-guide/) for instructions on running PR-Agent tools
+via different interfaces, such as CLI, PR Comments, or by automatically
+triggering them when a new PR is opened. - See the [Tools Guide](https://pr-
+agent-docs.codium.ai/tools/) for a detailed description of the different tools,
+and the available configurations for each tool. ## Table of Contents - [News
+and Updates](#news-and-updates) - [Overview](#overview) - [Example results]
+(#example-results) - [Try it now](#try-it-now) - [PR-Agent Pro ð](#pr-agent-
+pro-) - [How it works](#how-it-works) - [Why use PR-Agent?](#why-use-pr-agent)
+## News and Updates ### May 19, 2024 GPT-4o is now the default fast model
+("Turbo"). This model will be used for all commands except `review` and
+`improve`, which will still use "GPT-4-2024-04-09", since they are harder and
+would still benefit from the larger model. ### May 12, 2024 Inspired by
+[AlphaCodium](https://github.com/Codium-ai/AlphaCodium) flow engineering
+scheme, PR-Agent now performs **self-reflection** on the code suggestions it
+provides, enabling to remove invalid suggestions, and score the valid ones. The
+suggestions will be presented sorted by their score, enabling to focus on the
+most important ones first. You can also choose to automatically remove
+suggestions below a certain importance score threshold, by setting the
+`pr_code_suggestions.suggestions_score_threshold` [configuration](https://pr-
+agent-docs.codium.ai/tools/improve/#configuration-options). [https://codium.ai/
+images/pr_agent/self_reflection1.png][https://codium.ai/images/pr_agent/
+self_reflection2.png]### May 2, 2024 Check out the new [PR-Agent Chrome
+Extension](https://chromewebstore.google.com/detail/pr-agent-chrome-extension/
+ephlnjeghhogofkifjloamocljapahnl) ððð This toolbar integrates
+seamlessly with your GitHub environment, allowing you to access PR-Agent tools
+[directly from the GitHub interface](https://www.youtube.com/
+watch?v=gT5tli7X4H4). You can also easily export your chosen configuration, and
+use it for the automatic commands. [https://codium.ai/images/pr_agent/
+toolbar1.png][https://codium.ai/images/pr_agent/toolbar2.png]## Overview
+Supported commands per platform: | | | GitHub | Gitlab | Bitbucket | Azure
+DevOps | |-------|-------------------------------------------------------------
+--------------------------------------------|:--------------------:|:----------
+----------:|:--------------------:|:--------------------:| | TOOLS | Review |
+â | â | â | â | | | â® Incremental | â | | | | | | â® [SOC2
+Compliance](https://pr-agent-docs.codium.ai/tools/review/#soc2-ticket-
+compliance) ð | â | â | â | â | | | Describe | â | â | â | â
+| | | â® [Inline File Summary](https://pr-agent-docs.codium.ai/tools/
+describe#inline-file-summary) ð | â | | | | | | Improve | â | â | â
+| â | | | â® Extended | â | â | â | â | | | Ask | â | â | â |
+â | | | â® [Ask on code lines](https://pr-agent-docs.codium.ai/tools/
+ask#ask-lines) | â | â | | | | | [Custom Prompt](https://pr-agent-
+docs.codium.ai/tools/custom_prompt/) ð | â | â | â | â | | | [Test]
+(https://pr-agent-docs.codium.ai/tools/test/) ð | â | â | | â | | |
+Reflect and Review | â | â | â | â | | | Update CHANGELOG.md | â |
+â | â | â | | | Find Similar Issue | â | | | | | | [Add PR
+Documentation](https://pr-agent-docs.codium.ai/tools/documentation/) ð | â
+| â | | â | | | [Custom Labels](https://pr-agent-docs.codium.ai/tools/
+custom_labels/) ð | â | â | | â | | | [Analyze](https://pr-agent-
+docs.codium.ai/tools/analyze/) ð | â | â | | â | | | [CI Feedback]
+(https://pr-agent-docs.codium.ai/tools/ci_feedback/) ð | â | | | | | |
+[Similar Code](https://pr-agent-docs.codium.ai/tools/similar_code/) ð | â
+| | | | | | | | | | | | USAGE | CLI | â | â | â | â | | | App / webhook
+| â | â | â | â | | | Tagging bot | â | | | | | | Actions | â | |
+â | | | | | | | | | | CORE | PR compression | â | â | â | â | | |
+Repo language prioritization | â | â | â | â | | | Adaptive and token-
+aware file patch fitting | â | â | â | â | | | Multiple models support
+| â | â | â | â | | | [Static code analysis](https://pr-agent-
+docs.codium.ai/core-abilities/#static-code-analysis) ð | â | â | â |
+â | | | [Global and wiki configurations](https://pr-agent-docs.codium.ai/
+usage-guide/configuration_options/) ð | â | â | â | â | | | [PR
+interactive actions](https://www.codium.ai/images/pr_agent/pr-actions.mp4) ð
+| â | | | | - ð means this feature is available only in [PR-Agent Pro]
+(https://www.codium.ai/pricing/) [//]: # (- Support for additional git
+providers is described in [here](./docs/Full_environments.md)) ___ â£ **Auto
+Description ([`/describe`](https://pr-agent-docs.codium.ai/tools/describe/))**:
+Automatically generating PR description - title, type, summary, code
+walkthrough and labels. \ â£ **Auto Review ([`/review`](https://pr-agent-
+docs.codium.ai/tools/review/))**: Adjustable feedback about the PR, possible
+issues, security concerns, review effort and more. \ â£ **Code Suggestions (
+[`/improve`](https://pr-agent-docs.codium.ai/tools/improve/))**: Code
+suggestions for improving the PR. \ â£ **Question Answering ([`/ask ...`]
 (https://pr-agent-docs.codium.ai/tools/ask/))**: Answering free-text questions
 about the PR. \ â£ **Update Changelog ([`/update_changelog`](https://pr-agent-
 docs.codium.ai/tools/update_changelog/))**: Automatically updating the
 CHANGELOG.md file with the PR changes. \ â£ **Find Similar Issue ([`/
 similar_issue`](https://pr-agent-docs.codium.ai/tools/similar_issues/))**:
 Automatically retrieves and presents similar issues. \ â£ **Add Documentation
 ð ([`/add_docs`](https://pr-agent-docs.codium.ai/tools/documentation/))**:
 Generates documentation to methods/functions/classes that changed in the PR. \
 â£ **Generate Custom Labels ð ([`/generate_labels`](https://pr-agent-
 docs.codium.ai/tools/custom_labels/))**: Generates custom labels for the PR,
 based on specific guidelines defined by the user. \ â£ **Analyze ð ([`/
 analyze`](https://pr-agent-docs.codium.ai/tools/analyze/))**: Identify code
 components that changed in the PR, and enables to interactively generate tests,
-docs, and code suggestions for each component. \ â£ **Custom Suggestions ð
-([`/custom_suggestions`](https://pr-agent-docs.codium.ai/tools/
-custom_suggestions/))**: Automatically generates custom suggestions for
-improving the PR code, based on specific guidelines defined by the user. \ â£
-**Generate Tests ð ([`/test component_name`](https://pr-agent-
-docs.codium.ai/tools/test/))**: Generates unit tests for a selected component,
-based on the PR code changes. \ â£ **CI Feedback ð ([`/checks ci_job`]
-(https://pr-agent-docs.codium.ai/tools/ci_feedback/))**: Automatically
-generates feedback and analysis for a failed CI job. \ â£ **Similar Code ð
-([`/find_similar_component`](https://pr-agent-docs.codium.ai/tools/
-similar_code//))**: Retrieves the most similar code components from inside the
-organization's codebase, or from open-source code. ___ ## Example results
+docs, and code suggestions for each component. \ â£ **Custom Prompt ð ([`/
+custom_prompt`](https://pr-agent-docs.codium.ai/tools/custom_prompt/))**:
+Automatically generates custom suggestions for improving the PR code, based on
+specific guidelines defined by the user. \ â£ **Generate Tests ð ([`/test
+component_name`](https://pr-agent-docs.codium.ai/tools/test/))**: Generates
+unit tests for a selected component, based on the PR code changes. \ â£ **CI
+Feedback ð ([`/checks ci_job`](https://pr-agent-docs.codium.ai/tools/
+ci_feedback/))**: Automatically generates feedback and analysis for a failed CI
+job. \ â£ **Similar Code ð ([`/find_similar_component`](https://pr-agent-
+docs.codium.ai/tools/similar_code/))**: Retrieves the most similar code
+components from inside the organization's codebase, or from open-source code.
+___ ## Example results
 ****** _//_dd_ee_ss_cc_rr_ii_bb_ee ******
       [https://www.codium.ai/images/pr_agent/describe_new_short_main.png]
 ===============================================================================
 ****** _//_rr_ee_vv_ii_ee_ww ******
        [https://www.codium.ai/images/pr_agent/review_new_short_main.png]
 ===============================================================================
 ****** _//_ii_mm_pp_rr_oo_vv_ee ******
@@ -140,64 +144,78 @@
 PR comment. The agent will generate a response based on your command. For
 example, add a comment to any pull request with the following text: ```
 @CodiumAI-Agent /review ``` and the agent will respond with a review of your PR
 ![Review generation process](https://www.codium.ai/images/demo-2.gif) To set up
 your own PR-Agent, see the [Installation](https://pr-agent-docs.codium.ai/
 installation/) section below. Note that when you set your own PR-Agent or use
 CodiumAI hosted PR-Agent, there is no need to mention `@CodiumAI-Agent ...`.
-Instead, directly start with the command, e.g., `/ask ...`. --- ## Installation
-To use your own version of PR-Agent, you first need to acquire two tokens: 1.
-An OpenAI key from [here](https://platform.openai.com/), with access to GPT-4.
-2. A GitHub personal access token (classic) with the repo scope. There are
-several ways to use PR-Agent: **Locally** - [Using pip package](https://pr-
-agent-docs.codium.ai/installation/locally/#using-pip-package) - [Using Docker
-image](https://pr-agent-docs.codium.ai/installation/locally/#using-docker-
-image) - [Run from source](https://pr-agent-docs.codium.ai/installation/
-locally/#run-from-source) **GitHub specific methods** - [Run as a GitHub
+Instead, directly start with the command, e.g., `/ask ...`. --- [//]: # (##
+Installation) [//]: # (To use your own version of PR-Agent, you first need to
+acquire two tokens:) [//]: # () [//]: # (1. An OpenAI key from [here](https://
+platform.openai.com/), with access to GPT-4.) [//]: # (2. A GitHub personal
+access token (classic) with the repo scope.) [//]: # () [//]: # (There are
+several ways to use PR-Agent:) [//]: # () [//]: # (**Locally**) [//]: # (-
+[Using pip package](https://pr-agent-docs.codium.ai/installation/locally/
+#using-pip-package)) [//]: # (- [Using Docker image](https://pr-agent-
+docs.codium.ai/installation/locally/#using-docker-image)) [//]: # (- [Run from
+source](https://pr-agent-docs.codium.ai/installation/locally/#run-from-source))
+[//]: # () [//]: # (**GitHub specific methods**) [//]: # (- [Run as a GitHub
 Action](https://pr-agent-docs.codium.ai/installation/github/#run-as-a-github-
-action) - [Run as a GitHub App](https://pr-agent-docs.codium.ai/installation/
-github/#run-as-a-github-app) **GitLab specific methods** - [Run a GitLab
-webhook server](https://pr-agent-docs.codium.ai/installation/gitlab/
-) **BitBucket specific methods** - [Run as a Bitbucket Pipeline](https://pr-
-agent-docs.codium.ai/installation/bitbucket/) ## PR-Agent Pro ð [PR-Agent
-Pro](https://www.codium.ai/pricing/) is a hosted version of PR-Agent, provided
-by CodiumAI. It is available for a monthly fee, and provides the following
+action)) [//]: # (- [Run as a GitHub App](https://pr-agent-docs.codium.ai/
+installation/github/#run-as-a-github-app)) [//]: # () [//]: # (**GitLab
+specific methods**) [//]: # (- [Run a GitLab webhook server](https://pr-agent-
+docs.codium.ai/installation/gitlab/)) [//]: # () [//]: # (**BitBucket specific
+methods**) [//]: # (- [Run as a Bitbucket Pipeline](https://pr-agent-
+docs.codium.ai/installation/bitbucket/)) ## PR-Agent Pro ð [PR-Agent Pro]
+(https://www.codium.ai/pricing/) is a hosted version of PR-Agent, provided by
+CodiumAI. It is available for a monthly fee, and provides the following
 benefits: 1. **Fully managed** - We take care of everything for you - hosting,
 models, regular updates, and more. Installation is as simple as signing up and
-adding the PR-Agent app to your GitHub\BitBucket repo. 2. **Improved privacy**
-- No data will be stored or used to train models. PR-Agent Pro will employ zero
-data retention, and will use an OpenAI account with zero data retention. 3.
-**Improved support** - PR-Agent Pro users will receive priority support, and
-will be able to request new features and capabilities. 4. **Extra features** -
-In addition to the benefits listed above, PR-Agent Pro will emphasize more
-customization, and the usage of static code analysis, in addition to LLM logic,
-to improve results. See [here](https://pr-agent-docs.codium.ai/#pr-agent-pro)
-for a list of features available in PR-Agent Pro. ## How it works The following
-diagram illustrates PR-Agent tools and their flow: ![PR-Agent Tools](https://
-codium.ai/images/pr_agent/diagram-v0.9.png) Check out the [PR Compression
+adding the PR-Agent app to your GitHub\GitLab\BitBucket repo. 2. **Improved
+privacy** - No data will be stored or used to train models. PR-Agent Pro will
+employ zero data retention, and will use an OpenAI account with zero data
+retention. 3. **Improved support** - PR-Agent Pro users will receive priority
+support, and will be able to request new features and capabilities. 4. **Extra
+features** -In addition to the benefits listed above, PR-Agent Pro will
+emphasize more customization, and the usage of static code analysis, in
+addition to LLM logic, to improve results. See [here](https://pr-agent-
+docs.codium.ai/#pr-agent-pro) for a list of features available in PR-Agent Pro.
+## How it works The following diagram illustrates PR-Agent tools and their
+flow: ![PR-Agent Tools](https://codium.ai/images/pr_agent/diagram-v0.9.png)
+Check out the [PR Compression strategy](https://pr-agent-docs.codium.ai/core-
+abilities/#pr-compression-strategy) page for more details on how we convert a
+code diff to a manageable LLM prompt ## Why use PR-Agent? A reasonable question
+that can be asked is: `"Why use PR-Agent? What makes it stand out from existing
+tools?"` Here are some advantages of PR-Agent: - We emphasize **real-life
+practical usage**. Each tool (review, improve, ask, ...) has a single GPT-
+4 call, no more. We feel that this is critical for realistic team usage -
+obtaining an answer quickly (~30 seconds) and affordably. - Our [PR Compression
 strategy](https://pr-agent-docs.codium.ai/core-abilities/#pr-compression-
-strategy) page for more details on how we convert a code diff to a manageable
-LLM prompt ## Why use PR-Agent? A reasonable question that can be asked is:
-`"Why use PR-Agent? What makes it stand out from existing tools?"` Here are
-some advantages of PR-Agent: - We emphasize **real-life practical usage**. Each
-tool (review, improve, ask, ...) has a single GPT-4 call, no more. We feel that
-this is critical for realistic team usage - obtaining an answer quickly (~30
-seconds) and affordably. - Our [PR Compression strategy](https://pr-agent-
-docs.codium.ai/core-abilities/#pr-compression-strategy) is a core ability that
-enables to effectively tackle both short and long PRs. - Our JSON prompting
-strategy enables to have **modular, customizable tools**. For example, the '/
-review' tool categories can be controlled via the [configuration](pr_agent/
-settings/configuration.toml) file. Adding additional categories is easy and
-accessible. - We support **multiple git providers** (GitHub, Gitlab,
-Bitbucket), **multiple ways** to use the tool (CLI, GitHub Action, GitHub App,
-Docker, ...), and **multiple models** (GPT-4, GPT-3.5, Anthropic, Cohere,
-Llama2). ## Data privacy If you host PR-Agent with your OpenAI API key, it is
-between you and OpenAI. You can read their API data privacy policy here: https:
-//openai.com/enterprise-privacy When using PR-Agent Pro ð, hosted by
+strategy) is a core ability that enables to effectively tackle both short and
+long PRs. - Our JSON prompting strategy enables to have **modular, customizable
+tools**. For example, the '/review' tool categories can be controlled via the
+[configuration](pr_agent/settings/configuration.toml) file. Adding additional
+categories is easy and accessible. - We support **multiple git providers**
+(GitHub, Gitlab, Bitbucket), **multiple ways** to use the tool (CLI, GitHub
+Action, GitHub App, Docker, ...), and **multiple models** (GPT-4, GPT-3.5,
+Anthropic, Cohere, Llama2). ## Data privacy ### Self-hosted PR-Agent - If you
+host PR-Agent with your OpenAI API key, it is between you and OpenAI. You can
+read their API data privacy policy here: https://openai.com/enterprise-privacy
+### CodiumAI-hosted PR-Agent Pro ð - When using PR-Agent Pro ð, hosted by
 CodiumAI, we will not store any of your data, nor will we use it for training.
-You will also benefit from an OpenAI account with zero data retention. ## Links
-[![Join our Discord community](https://raw.githubusercontent.com/Codium-ai/
-codiumai-vscode-release/main/media/docs/Joincommunity.png)](https://discord.gg/
-kG35uSHDBc) - Discord community: https://discord.gg/kG35uSHDBc - CodiumAI site:
-https://codium.ai - Blog: https://www.codium.ai/blog/ - Troubleshooting: https:
-//www.codium.ai/blog/technical-faq-and-troubleshooting/ - Support:
-support@codium.ai
+You will also benefit from an OpenAI account with zero data retention. - For
+certain clients, CodiumAI-hosted PR-Agent Pro will use CodiumAIâs proprietary
+models â if this is the case, you will be notified. - No passive collection
+of Code and Pull Requestsâ data â PR-Agent will be active only when you
+invoke it, and it will then extract and analyze only data relevant to the
+executed command and queried pull request. ### PR-Agent Chrome extension - The
+[PR-Agent Chrome extension](https://chromewebstore.google.com/detail/pr-agent-
+chrome-extension/ephlnjeghhogofkifjloamocljapahnl) serves solely to modify the
+visual appearance of a GitHub PR screen. It does not transmit any user's repo
+or pull request code. Code is only sent for processing when a user submits a
+GitHub comment that activates a PR-Agent tool, in accordance with the standard
+privacy policy of PR-Agent. ## Links [![Join our Discord community](https://
+raw.githubusercontent.com/Codium-ai/codiumai-vscode-release/main/media/docs/
+Joincommunity.png)](https://discord.gg/kG35uSHDBc) - Discord community: https:/
+/discord.gg/kG35uSHDBc - CodiumAI site: https://codium.ai - Blog: https://
+www.codium.ai/blog/ - Troubleshooting: https://www.codium.ai/blog/technical-
+faq-and-troubleshooting/ - Support: support@codium.ai
```

### Comparing `pr-agent-0.2.1/pr_agent/agent/pr_agent.py` & `pr_agent-0.2.2/pr_agent/agent/pr_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,17 @@
                 for arg in args:
                     if forbidden_arg in arg:
                         get_logger().error(f"CLI argument for param '{forbidden_arg}' is forbidden. Use instead a configuration file.")
                         return False
         args = update_settings_from_args(args)
 
         action = action.lstrip("/").lower()
+        if action not in command2class:
+            get_logger().debug(f"Unknown command: {action}")
+            return False
         with get_logger().contextualize(command=action):
             get_logger().info("PR-Agent request handler started", analytics=True)
             if action == "reflect_and_review":
                 get_settings().pr_reviewer.ask_and_reflect = True
             if action == "answer":
                 if notify:
                     notify()
```

### Comparing `pr-agent-0.2.1/pr_agent/algo/__init__.py` & `pr_agent-0.2.2/pr_agent/algo/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 MAX_TOKENS = {
     'text-embedding-ada-002': 8000,
-    'gpt-3.5-turbo': 4000,
+    'gpt-3.5-turbo': 16000,
+    'gpt-3.5-turbo-0125': 16000,
     'gpt-3.5-turbo-0613': 4000,
-    'gpt-3.5-turbo-0301': 4000,
+    'gpt-3.5-turbo-1106': 16000,
     'gpt-3.5-turbo-16k': 16000,
     'gpt-3.5-turbo-16k-0613': 16000,
     'gpt-4': 8000,
     'gpt-4-0613': 8000,
     'gpt-4-32k': 32000,
     'gpt-4-1106-preview': 128000, # 128K, but may be limited by config.max_model_tokens
     'gpt-4-0125-preview': 128000,  # 128K, but may be limited by config.max_model_tokens
+    'gpt-4o': 128000,  # 128K, but may be limited by config.max_model_tokens
+    'gpt-4o-2024-05-13': 128000,  # 128K, but may be limited by config.max_model_tokens
+    'gpt-4-turbo-preview': 128000,  # 128K, but may be limited by config.max_model_tokens
+    'gpt-4-turbo-2024-04-09': 128000,  # 128K, but may be limited by config.max_model_tokens
+    'gpt-4-turbo': 128000,  # 128K, but may be limited by config.max_model_tokens
     'claude-instant-1': 100000,
     'claude-2': 100000,
     'command-nightly': 4096,
     'replicate/llama-2-70b-chat:2c1608e18606fad2812020dc541930f2d0495ce32eee50074220b87300bc16e1': 4096,
     'meta-llama/Llama-2-7b-chat-hf': 4096,
     'vertex_ai/codechat-bison': 6144,
     'vertex_ai/codechat-bison-32k': 32000,
@@ -24,8 +30,10 @@
     'anthropic.claude-v2': 100000,
     'anthropic/claude-3-opus-20240229': 100000,
     'bedrock/anthropic.claude-instant-v1': 100000,
     'bedrock/anthropic.claude-v2': 100000,
     'bedrock/anthropic.claude-v2:1': 100000,
     'bedrock/anthropic.claude-3-sonnet-20240229-v1:0': 100000,
     'bedrock/anthropic.claude-3-haiku-20240307-v1:0': 100000,
+    'groq/llama3-8b-8192': 8192,
+    'groq/llama3-70b-8192': 8192,
 }
```

### Comparing `pr-agent-0.2.1/pr_agent/algo/ai_handlers/base_ai_handler.py` & `pr_agent-0.2.2/pr_agent/algo/ai_handlers/base_ai_handler.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     @property
     @abstractmethod
     def deployment_id(self):
         pass
 
     @abstractmethod   
-    async def chat_completion(self, model: str, system: str, user: str, temperature: float = 0.2):
+    async def chat_completion(self, model: str, system: str, user: str, temperature: float = 0.2, img_path: str = None):
         """
         This method should be implemented to return a chat completion from the AI model.
         Args:
             model (str): the name of the model to use for the chat completion
             system (str): the system message string to use for the chat completion
             user (str): the user message string to use for the chat completion
             temperature (float): the temperature to use for the chat completion
```

### Comparing `pr-agent-0.2.1/pr_agent/algo/ai_handlers/langchain_ai_handler.py` & `pr_agent-0.2.2/pr_agent/algo/ai_handlers/langchain_ai_handler.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/algo/ai_handlers/litellm_ai_handler.py` & `pr_agent-0.2.2/pr_agent/algo/ai_handlers/litellm_ai_handler.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-
+import requests
 import boto3
 import litellm
 import openai
 from litellm import acompletion
 from tenacity import retry, retry_if_exception_type, stop_after_attempt
 from pr_agent.algo.ai_handlers.base_ai_handler import BaseAiHandler
 from pr_agent.config_loader import get_settings
@@ -48,23 +48,26 @@
             litellm.api_version = get_settings().openai.api_version
         if get_settings().get("OPENAI.API_BASE", None):
             litellm.api_base = get_settings().openai.api_base
         if get_settings().get("ANTHROPIC.KEY", None):
             litellm.anthropic_key = get_settings().anthropic.key
         if get_settings().get("COHERE.KEY", None):
             litellm.cohere_key = get_settings().cohere.key
-        if get_settings().get("REPLICATE.KEY", None):
-            litellm.replicate_key = get_settings().replicate.key
+        if get_settings().get("GROQ.KEY", None):
+            litellm.api_key = get_settings().groq.key
         if get_settings().get("REPLICATE.KEY", None):
             litellm.replicate_key = get_settings().replicate.key
         if get_settings().get("HUGGINGFACE.KEY", None):
             litellm.huggingface_key = get_settings().huggingface.key
         if get_settings().get("HUGGINGFACE.API_BASE", None) and 'huggingface' in get_settings().config.model:
             litellm.api_base = get_settings().huggingface.api_base
             self.api_base = get_settings().huggingface.api_base
+        if get_settings().get("OLLAMA.API_BASE", None) :
+            litellm.api_base = get_settings().ollama.api_base
+            self.api_base = get_settings().ollama.api_base
         if get_settings().get("HUGGINGFACE.REPITITION_PENALTY", None):
             self.repetition_penalty = float(get_settings().huggingface.repetition_penalty)
         if get_settings().get("VERTEXAI.VERTEX_PROJECT", None):
             litellm.vertex_project = get_settings().vertexai.vertex_project
             litellm.vertex_location = get_settings().get(
                 "VERTEXAI.VERTEX_LOCATION", None
             )
@@ -95,21 +98,35 @@
         """
         return get_settings().get("OPENAI.DEPLOYMENT_ID", None)
 
     @retry(
         retry=retry_if_exception_type((openai.APIError, openai.APIConnectionError, openai.Timeout)), # No retry on RateLimitError
         stop=stop_after_attempt(OPENAI_RETRIES)
     )
-    async def chat_completion(self, model: str, system: str, user: str, temperature: float = 0.2):
+    async def chat_completion(self, model: str, system: str, user: str, temperature: float = 0.2, img_path: str = None):
         try:
             resp, finish_reason = None, None
             deployment_id = self.deployment_id
             if self.azure:
                 model = 'azure/' + model
             messages = [{"role": "system", "content": system}, {"role": "user", "content": user}]
+            if img_path:
+                try:
+                    # check if the image link is alive
+                    r = requests.head(img_path, allow_redirects=True)
+                    if r.status_code == 404:
+                        error_msg = f"The image link is not [alive](img_path).\nPlease repost the original image as a comment, and send the question again with 'quote reply' (see [instructions](https://pr-agent-docs.codium.ai/tools/ask/#ask-on-images-using-the-pr-code-as-context))."
+                        get_logger().error(error_msg)
+                        return f"{error_msg}", "error"
+                except Exception as e:
+                    get_logger().error(f"Error fetching image: {img_path}", e)
+                    return f"Error fetching image: {img_path}", "error"
+                messages[1]["content"] = [{"type": "text", "text": messages[1]["content"]},
+                                          {"type": "image_url", "image_url": {"url": img_path}}]
+
             kwargs = {
                 "model": model,
                 "deployment_id": deployment_id,
                 "messages": messages,
                 "temperature": temperature,
                 "force_timeout": get_settings().config.ai_timeout,
                 "api_base" : self.api_base,
@@ -146,8 +163,8 @@
             response_log = self.prepare_logs(response, system, user, resp, finish_reason)
             get_logger().debug("Full_response", artifact=response_log)
 
             # for CLI debugging
             if get_settings().config.verbosity_level >= 2:
                 get_logger().info(f"\nAI response:\n{resp}")
 
-        return resp, finish_reason
+        return resp, finish_reason
```

### Comparing `pr-agent-0.2.1/pr_agent/algo/ai_handlers/openai_ai_handler.py` & `pr_agent-0.2.2/pr_agent/algo/ai_handlers/openai_ai_handler.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/algo/file_filter.py` & `pr_agent-0.2.2/pr_agent/algo/file_filter.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/algo/git_patch_processing.py` & `pr_agent-0.2.2/pr_agent/algo/git_patch_processing.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/algo/language_handler.py` & `pr_agent-0.2.2/pr_agent/algo/language_handler.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/algo/pr_processing.py` & `pr_agent-0.2.2/pr_agent/algo/pr_processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from github import RateLimitExceededException
 
 from pr_agent.algo.git_patch_processing import convert_to_hunks_with_lines_numbers, extend_patch, handle_patch_deletions
 from pr_agent.algo.language_handler import sort_files_by_main_languages
 from pr_agent.algo.file_filter import filter_ignored
 from pr_agent.algo.token_handler import TokenHandler
-from pr_agent.algo.utils import get_max_tokens, ModelType
+from pr_agent.algo.utils import get_max_tokens, clip_tokens, ModelType
 from pr_agent.config_loader import get_settings
 from pr_agent.git_providers.git_provider import GitProvider
 from pr_agent.algo.types import EDIT_TYPE, FilePatchInfo
 from pr_agent.log import get_logger
 
 DELETED_FILES_ = "Deleted files:\n"
 
@@ -83,30 +83,42 @@
         get_logger().info(f"Tokens: {total_tokens}, total tokens under limit: {get_max_tokens(model)}, "
                           f"returning full diff.")
         return "\n".join(patches_extended)
 
     # if we are over the limit, start pruning
     get_logger().info(f"Tokens: {total_tokens}, total tokens over limit: {get_max_tokens(model)}, "
                       f"pruning diff.")
-    patches_compressed, modified_file_names, deleted_file_names, added_file_names = \
+    patches_compressed, modified_file_names, deleted_file_names, added_file_names, total_tokens_new = \
         pr_generate_compressed_diff(pr_languages, token_handler, model, add_line_numbers_to_hunks)
 
+    # Insert additional information about added, modified, and deleted files if there is enough space
+    max_tokens = get_max_tokens(model) - OUTPUT_BUFFER_TOKENS_HARD_THRESHOLD
+    curr_token = total_tokens_new  # == token_handler.count_tokens(final_diff)+token_handler.prompt_tokens
     final_diff = "\n".join(patches_compressed)
-    if added_file_names:
+    delta_tokens = 10
+    if added_file_names and (max_tokens - curr_token) > delta_tokens:
         added_list_str = ADDED_FILES_ + "\n".join(added_file_names)
-        final_diff = final_diff + "\n\n" + added_list_str
-    if modified_file_names:
+        added_list_str = clip_tokens(added_list_str, max_tokens - curr_token)
+        if added_list_str:
+            final_diff = final_diff + "\n\n" + added_list_str
+            curr_token += token_handler.count_tokens(added_list_str) + 2
+    if modified_file_names and (max_tokens - curr_token) > delta_tokens:
         modified_list_str = MORE_MODIFIED_FILES_ + "\n".join(modified_file_names)
-        final_diff = final_diff + "\n\n" + modified_list_str
-    if deleted_file_names:
+        modified_list_str = clip_tokens(modified_list_str, max_tokens - curr_token)
+        if modified_list_str:
+            final_diff = final_diff + "\n\n" + modified_list_str
+            curr_token += token_handler.count_tokens(modified_list_str) + 2
+    if deleted_file_names and (max_tokens - curr_token) > delta_tokens:
         deleted_list_str = DELETED_FILES_ + "\n".join(deleted_file_names)
-        final_diff = final_diff + "\n\n" + deleted_list_str
+        deleted_list_str = clip_tokens(deleted_list_str, max_tokens - curr_token)
+        if deleted_list_str:
+            final_diff = final_diff + "\n\n" + deleted_list_str
     try:
         get_logger().debug(f"After pruning, added_list_str: {added_list_str}, modified_list_str: {modified_list_str}, "
-                          f"deleted_list_str: {deleted_list_str}")
+                           f"deleted_list_str: {deleted_list_str}")
     except Exception as e:
         pass
     return final_diff
 
 
 def pr_generate_extended_diff(pr_languages: list,
                               token_handler: TokenHandler,
@@ -145,15 +157,15 @@
             patches_extended_tokens.append(patch_tokens)
             patches_extended.append(full_extended_patch)
 
     return patches_extended, total_tokens, patches_extended_tokens
 
 
 def pr_generate_compressed_diff(top_langs: list, token_handler: TokenHandler, model: str,
-                                convert_hunks_to_line_numbers: bool) -> Tuple[list, list, list, list]:
+                                convert_hunks_to_line_numbers: bool) -> Tuple[list, list, list, list, int]:
     """
     Generate a compressed diff string for a pull request, using diff minimization techniques to reduce the number of
     tokens used.
     Args:
         top_langs (list): A list of dictionaries representing the languages used in the pull request and their
         corresponding files.
         token_handler (TokenHandler): An object of the TokenHandler class used for handling tokens in the context of the
@@ -191,18 +203,19 @@
         if not patch:
             continue
 
         # removing delete-only hunks
         patch = handle_patch_deletions(patch, original_file_content_str,
                                        new_file_content_str, file.filename, file.edit_type)
         if patch is None:
-            if not deleted_files_list:
-                total_tokens += token_handler.count_tokens(DELETED_FILES_)
-            deleted_files_list.append(file.filename)
-            total_tokens += token_handler.count_tokens(file.filename) + 1
+            # if not deleted_files_list:
+            #     total_tokens += token_handler.count_tokens(DELETED_FILES_)
+            if file.filename not in deleted_files_list:
+                deleted_files_list.append(file.filename)
+            # total_tokens += token_handler.count_tokens(file.filename) + 1
             continue
 
         if convert_hunks_to_line_numbers:
             patch = convert_to_hunks_with_lines_numbers(patch, file)
 
         new_patch_tokens = token_handler.count_tokens(patch)
 
@@ -215,35 +228,38 @@
         if total_tokens + new_patch_tokens > get_max_tokens(model) - OUTPUT_BUFFER_TOKENS_SOFT_THRESHOLD:
             # Current logic is to skip the patch if it's too large
             # TODO: Option for alternative logic to remove hunks from the patch to reduce the number of tokens
             #  until we meet the requirements
             if get_settings().config.verbosity_level >= 2:
                 get_logger().warning(f"Patch too large, minimizing it, {file.filename}")
             if file.edit_type == EDIT_TYPE.ADDED:
-                if not added_files_list:
-                    total_tokens += token_handler.count_tokens(ADDED_FILES_)
-                added_files_list.append(file.filename)
+                # if not added_files_list:
+                #     total_tokens += token_handler.count_tokens(ADDED_FILES_)
+                if file.filename not in added_files_list:
+                    added_files_list.append(file.filename)
+                # total_tokens += token_handler.count_tokens(file.filename) + 1
             else:
-                if not modified_files_list:
-                    total_tokens += token_handler.count_tokens(MORE_MODIFIED_FILES_)
-                modified_files_list.append(file.filename)
-                total_tokens += token_handler.count_tokens(file.filename) + 1
+                # if not modified_files_list:
+                #     total_tokens += token_handler.count_tokens(MORE_MODIFIED_FILES_)
+                if file.filename not in modified_files_list:
+                    modified_files_list.append(file.filename)
+                # total_tokens += token_handler.count_tokens(file.filename) + 1
             continue
 
         if patch:
             if not convert_hunks_to_line_numbers:
                 patch_final = f"\n\n## file: '{file.filename.strip()}\n\n{patch.strip()}\n'"
             else:
                 patch_final = "\n\n" + patch.strip()
             patches.append(patch_final)
             total_tokens += token_handler.count_tokens(patch_final)
             if get_settings().config.verbosity_level >= 2:
                 get_logger().info(f"Tokens: {total_tokens}, last filename: {file.filename}")
 
-    return patches, modified_files_list, deleted_files_list, added_files_list
+    return patches, modified_files_list, deleted_files_list, added_files_list, total_tokens
 
 
 async def retry_with_fallback_models(f: Callable, model_type: ModelType = ModelType.REGULAR):
     all_models = _get_all_models(model_type)
     all_deployments = _get_all_deployments(all_models)
     # try each (model, deployment_id) pair until one is successful, otherwise raise exception
     for i, (model, deployment_id) in enumerate(zip(all_models, all_deployments)):
@@ -378,8 +394,8 @@
                 get_logger().info(f"Tokens: {total_tokens}, last filename: {file.filename}")
 
     # Add the last chunk
     if patches:
         final_diff = "\n".join(patches)
         final_diff_list.append(final_diff)
 
-    return final_diff_list
+    return final_diff_list
```

### Comparing `pr-agent-0.2.1/pr_agent/algo/token_handler.py` & `pr_agent-0.2.2/pr_agent/algo/token_handler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,29 @@
 from jinja2 import Environment, StrictUndefined
 from tiktoken import encoding_for_model, get_encoding
-
 from pr_agent.config_loader import get_settings
+from threading import Lock
+
 
+class TokenEncoder:
+    _encoder_instance = None
+    _model = None
+    _lock = Lock()  # Create a lock object
+
+    @classmethod
+    def get_token_encoder(cls):
+        model = get_settings().config.model
+        if cls._encoder_instance is None or model != cls._model:  # Check without acquiring the lock for performance
+            with cls._lock:  # Lock acquisition to ensure thread safety
+                if cls._encoder_instance is None or model != cls._model:
+                    cls._model = model
+                    cls._encoder_instance = encoding_for_model(cls._model) if "gpt" in cls._model else get_encoding(
+                        "cl100k_base")
+        return cls._encoder_instance
 
-def get_token_encoder():
-    return encoding_for_model(get_settings().config.model) if "gpt" in get_settings().config.model else get_encoding(
-        "cl100k_base")
 
 class TokenHandler:
     """
     A class for handling tokens in the context of a pull request.
 
     Attributes:
     - encoder: An object of the encoding_for_model class from the tiktoken module. Used to encode strings and count the
@@ -27,15 +40,15 @@
 
         Args:
         - pr: The pull request object.
         - vars: A dictionary of variables.
         - system: The system string.
         - user: The user string.
         """
-        self.encoder = get_token_encoder()
+        self.encoder = TokenEncoder.get_token_encoder()
         if pr is not None:
             self.prompt_tokens = self._get_system_user_tokens(pr, self.encoder, vars, system, user)
 
     def _get_system_user_tokens(self, pr, encoder, vars: dict, system, user):
         """
         Calculates the number of tokens in the system and user strings.
```

### Comparing `pr-agent-0.2.1/pr_agent/algo/utils.py` & `pr_agent-0.2.2/pr_agent/algo/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from __future__ import annotations
 
 import difflib
 import json
+import os
 import re
 import textwrap
 from datetime import datetime
 from enum import Enum
 from typing import Any, List, Tuple
 
 import yaml
 from starlette_context import context
 
 from pr_agent.algo import MAX_TOKENS
-from pr_agent.algo.token_handler import get_token_encoder
+from pr_agent.algo.token_handler import TokenEncoder
 from pr_agent.config_loader import get_settings, global_settings
 from pr_agent.algo.types import FilePatchInfo
 from pr_agent.log import get_logger
 
 class ModelType(str, Enum):
     REGULAR = "regular"
     TURBO = "turbo"
@@ -63,32 +64,32 @@
 def convert_to_markdown(output_data: dict, gfm_supported: bool = True, incremental_review=None) -> str:
     """
     Convert a dictionary of data into markdown format.
     Args:
         output_data (dict): A dictionary containing data to be converted to markdown format.
     Returns:
         str: The markdown formatted text generated from the input dictionary.
-    """    
+    """
 
     emojis = {
         "Can be split": "🔀",
-        "Possible issues": "🔍",
+        "Possible issues": "⚡",
         "Score": "🏅",
         "Relevant tests": "🧪",
         "Focused PR": "✨",
         "Security concerns": "🔒",
         "Insights from user's answers": "📝",
         "Code feedback": "🤖",
         "Estimated effort to review [1-5]": "⏱️",
     }
     markdown_text = ""
     if not incremental_review:
-        markdown_text += f"## PR Review\n\n"
+        markdown_text += f"## PR Review 🔍\n\n"
     else:
-        markdown_text += f"## Incremental PR Review\n\n"
+        markdown_text += f"## Incremental PR Review 🔍 \n\n"
         markdown_text += f"⏮️ Review for commits since previous PR-Agent review {incremental_review}.\n\n"
     if gfm_supported:
         markdown_text += "<table>\n<tr>\n"
         # markdown_text += """<td> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Feedback&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</td> <td></td></tr>"""
 
     if not output_data or not output_data.get('review', {}):
         return ""
@@ -351,15 +352,15 @@
         >>> convert_str_to_datetime('Mon, 01 Jan 2022 12:00:00 UTC')
         datetime.datetime(2022, 1, 1, 12, 0, 0)
     """
     datetime_format = '%a, %d %b %Y %H:%M:%S %Z'
     return datetime.strptime(date_str, datetime_format)
 
 
-def load_large_diff(filename, new_file_content_str: str, original_file_content_str: str) -> str:
+def load_large_diff(filename, new_file_content_str: str, original_file_content_str: str, show_warning: bool = True) -> str:
     """
     Generate a patch for a modified file by comparing the original content of the file with the new content provided as
     input.
 
     Args:
         new_file_content_str: The new content of the file as a string.
         original_file_content_str: The original content of the file as a string.
@@ -370,15 +371,15 @@
     Raises:
         None.
     """
     patch = ""
     try:
         diff = difflib.unified_diff(original_file_content_str.splitlines(keepends=True),
                                     new_file_content_str.splitlines(keepends=True))
-        if get_settings().config.verbosity_level >= 2:
+        if get_settings().config.verbosity_level >= 2 and show_warning:
             get_logger().warning(f"File was modified, but no patch was found. Manually creating patch: {filename}.")
         patch = ''.join(diff)
     except Exception:
         pass
     return patch
 
 
@@ -562,24 +563,24 @@
     Returns:
         str: The clipped string.
     """
     if not text:
         return text
 
     try:
-        encoder = get_token_encoder()
+        encoder = TokenEncoder.get_token_encoder()
         num_input_tokens = len(encoder.encode(text))
         if num_input_tokens <= max_tokens:
             return text
         num_chars = len(text)
         chars_per_token = num_chars / num_input_tokens
         num_output_chars = int(chars_per_token * max_tokens)
         clipped_text = text[:num_output_chars]
         if add_three_dots:
-            clipped_text += "...(truncated)"
+            clipped_text += "\n...(truncated)"
         return clipped_text
     except Exception as e:
         get_logger().warning(f"Failed to clip tokens: {e}")
         return text
 
 def replace_code_tags(text):
     """
@@ -657,7 +658,42 @@
                         if no_plus_line in line and line[0] != '-':
                             # The model might add a '+' to the beginning of the relevant_line_in_file even if originally
                             # it's a context line
                             position = i
                             absolute_position = start2 + delta - 1
                             break
     return position, absolute_position
+
+def github_action_output(output_data: dict, key_name: str):
+    try:
+        if not get_settings().get('github_action_config.enable_output', False):
+            return
+        
+        key_data = output_data.get(key_name, {})
+        with open(os.environ['GITHUB_OUTPUT'], 'a') as fh:
+            print(f"{key_name}={json.dumps(key_data, indent=None, ensure_ascii=False)}", file=fh)
+    except Exception as e:
+        get_logger().error(f"Failed to write to GitHub Action output: {e}")
+    return
+
+
+def show_relevant_configurations(relevant_section: str) -> str:
+    forbidden_keys = ['ai_disclaimer', 'ai_disclaimer_title', 'ANALYTICS_FOLDER', 'secret_provider',
+                      'trial_prefix_message', 'no_eligible_message', 'identity_provider', 'ALLOWED_REPOS','APP_NAME']
+
+    markdown_text = ""
+    markdown_text += "\n<hr>\n<details> <summary><strong>🛠️ Relevant configurations:</strong></summary> \n\n"
+    markdown_text +="<br>These are the relevant [configurations](https://github.com/Codium-ai/pr-agent/blob/main/pr_agent/settings/configuration.toml) for this tool:\n\n"
+    markdown_text += f"**[config**]\n```yaml\n\n"
+    for key, value in get_settings().config.items():
+        if key in forbidden_keys:
+            continue
+        markdown_text += f"{key}: {value}\n"
+    markdown_text += "\n```\n"
+    markdown_text += f"\n**[{relevant_section}]**\n```yaml\n\n"
+    for key, value in get_settings().get(relevant_section, {}).items():
+        if key in forbidden_keys:
+            continue
+        markdown_text += f"{key}: {value}\n"
+    markdown_text += "\n```"
+    markdown_text += "\n</details>\n"
+    return markdown_text
```

### Comparing `pr-agent-0.2.1/pr_agent/cli.py` & `pr_agent-0.2.2/pr_agent/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,16 @@
     parser.add_argument('--issue_url', type=str, help='The URL of the Issue to review', default=None)
     parser.add_argument('command', type=str, help='The', choices=commands, default='review')
     parser.add_argument('rest', nargs=argparse.REMAINDER, default=[])
     return parser
 
 def run_command(pr_url, command):
     # Preparing the command
-    run_command = f"--pr_url={pr_url} {command.lstrip('/')}"
-    args = set_parser().parse_args(run_command.split())
+    run_command_str = f"--pr_url={pr_url} {command.lstrip('/')}"
+    args = set_parser().parse_args(run_command_str.split())
 
     # Run the command. Feedback will appear in GitHub PR comments
     run(args=args)
 
 def run(inargs=None, args=None):
     parser = set_parser()
     if not args:
```

### Comparing `pr-agent-0.2.1/pr_agent/cli_pip.py` & `pr_agent-0.2.2/pr_agent/cli_pip.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/config_loader.py` & `pr_agent-0.2.2/pr_agent/config_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         "settings/ignore.toml",
         "settings/language_extensions.toml",
         "settings/pr_reviewer_prompts.toml",
         "settings/pr_questions_prompts.toml",
         "settings/pr_line_questions_prompts.toml",
         "settings/pr_description_prompts.toml",
         "settings/pr_code_suggestions_prompts.toml",
+        "settings/pr_code_suggestions_reflect_prompts.toml",
         "settings/pr_sort_code_suggestions_prompts.toml",
         "settings/pr_information_from_user_prompts.toml",
         "settings/pr_update_changelog_prompts.toml",
         "settings/pr_custom_labels.toml",
         "settings/pr_add_docs.toml",
         "settings_prod/.secrets.toml",
         "settings/custom_labels.toml"
```

### Comparing `pr-agent-0.2.1/pr_agent/git_providers/__init__.py` & `pr_agent-0.2.2/pr_agent/git_providers/__init__.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/git_providers/azuredevops_provider.py` & `pr_agent-0.2.2/pr_agent/git_providers/azuredevops_provider.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     from azure.identity import DefaultAzureCredential
     # noinspection PyUnresolvedReferences
     from azure.devops.v7_1.git.models import (
         Comment,
         CommentThread,
         GitVersionDescriptor,
         GitPullRequest,
+        GitPullRequestIterationChanges,
     )
 except ImportError:
     AZURE_DEVOPS_AVAILABLE = False
 
 
 class AzureDevopsProvider(GitProvider):
 
@@ -226,37 +227,66 @@
 
             if self.diff_files:
                 return self.diff_files
 
             base_sha = self.pr.last_merge_target_commit
             head_sha = self.pr.last_merge_source_commit
 
-            commits = self.azure_devops_client.get_pull_request_commits(
-                project=self.workspace_slug,
+            # Get PR iterations
+            iterations = self.azure_devops_client.get_pull_request_iterations(
                 repository_id=self.repo_slug,
                 pull_request_id=self.pr_num,
+                project=self.workspace_slug
             )
+            changes = None
+            if iterations:
+                iteration_id = iterations[-1].id  # Get the last iteration (most recent changes)
 
+                # Get changes for the iteration
+                changes = self.azure_devops_client.get_pull_request_iteration_changes(
+                    repository_id=self.repo_slug,
+                    pull_request_id=self.pr_num,
+                    iteration_id=iteration_id,
+                    project=self.workspace_slug
+                )
             diff_files = []
             diffs = []
             diff_types = {}
-
-            for c in commits:
-                changes_obj = self.azure_devops_client.get_changes(
-                    project=self.workspace_slug,
-                    repository_id=self.repo_slug,
-                    commit_id=c.commit_id,
-                )
-                for i in changes_obj.changes:
-                    if i["item"]["gitObjectType"] == "tree":
-                        continue
-                    diffs.append(i["item"]["path"])
-                    diff_types[i["item"]["path"]] = i["changeType"]
-
-            diffs = list(set(diffs))
+            if changes:
+                for change in changes.change_entries:
+                    item = change.additional_properties.get('item', {})
+                    path = item.get('path', None)
+                    if path:
+                        diffs.append(path)
+                        diff_types[path] = change.additional_properties.get('changeType', 'Unknown')
+
+            # wrong implementation - gets all the files that were changed in any commit in the PR
+            # commits = self.azure_devops_client.get_pull_request_commits(
+            #     project=self.workspace_slug,
+            #     repository_id=self.repo_slug,
+            #     pull_request_id=self.pr_num,
+            # )
+            #
+            # diff_files = []
+            # diffs = []
+            # diff_types = {}
+
+            # for c in commits:
+            #     changes_obj = self.azure_devops_client.get_changes(
+            #         project=self.workspace_slug,
+            #         repository_id=self.repo_slug,
+            #         commit_id=c.commit_id,
+            #     )
+            #     for i in changes_obj.changes:
+            #         if i["item"]["gitObjectType"] == "tree":
+            #             continue
+            #         diffs.append(i["item"]["path"])
+            #         diff_types[i["item"]["path"]] = i["changeType"]
+            #
+            # diffs = list(set(diffs))
 
             for file in diffs:
                 if not is_valid_file(file):
                     continue
 
                 version = GitVersionDescriptor(
                     version=head_sha.commit_id, version_type="commit"
@@ -269,20 +299,21 @@
                         version_descriptor=version,
                         download=False,
                         include_content=True,
                     )
 
                     new_file_content_str = new_file_content_str.content
                 except Exception as error:
-                    get_logger().error(
-                        "Failed to retrieve new file content of %s at version %s. Error: %s",
-                        file,
-                        version,
-                        str(error),
-                    )
+                    get_logger().error(f"Failed to retrieve new file content of {file} at version {version}. Error: {str(error)}")
+                    # get_logger().error(
+                    #     "Failed to retrieve new file content of %s at version %s. Error: %s",
+                    #     file,
+                    #     version,
+                    #     str(error),
+                    # )
                     new_file_content_str = ""
 
                 edit_type = EDIT_TYPE.MODIFIED
                 if diff_types[file] == "add":
                     edit_type = EDIT_TYPE.ADDED
                 elif diff_types[file] == "delete":
                     edit_type = EDIT_TYPE.DELETED
@@ -299,25 +330,20 @@
                         project=self.workspace_slug,
                         version_descriptor=version,
                         download=False,
                         include_content=True,
                     )
                     original_file_content_str = original_file_content_str.content
                 except Exception as error:
-                    get_logger().error(
-                        "Failed to retrieve original file content of %s at version %s. Error: %s",
-                        file,
-                        version,
-                        str(error),
-                    )
+                    get_logger().error(f"Failed to retrieve original file content of {file} at version {version}. Error: {str(error)}")
                     original_file_content_str = ""
 
                 patch = load_large_diff(
-                    file, new_file_content_str, original_file_content_str
-                )
+                    file, new_file_content_str, original_file_content_str, show_warning=False
+                ).rstrip()
 
                 diff_files.append(
                     FilePatchInfo(
                         original_file_content_str,
                         new_file_content_str,
                         patch=patch,
                         filename=file,
```

### Comparing `pr-agent-0.2.1/pr_agent/git_providers/bitbucket_provider.py` & `pr_agent-0.2.2/pr_agent/git_providers/bitbucket_provider.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/git_providers/bitbucket_server_provider.py` & `pr_agent-0.2.2/pr_agent/git_providers/bitbucket_server_provider.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/git_providers/codecommit_client.py` & `pr_agent-0.2.2/pr_agent/git_providers/codecommit_client.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/git_providers/codecommit_provider.py` & `pr_agent-0.2.2/pr_agent/git_providers/codecommit_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from pr_agent.git_providers.codecommit_client import CodeCommitClient
 from pr_agent.algo.types import EDIT_TYPE, FilePatchInfo
 from ..algo.utils import load_large_diff
 from .git_provider import GitProvider
 from ..config_loader import get_settings
 from ..log import get_logger
-
+from pr_agent.algo.language_handler import is_valid_file
 
 class PullRequestCCMimic:
     """
     This class mimics the PullRequest class from the PyGithub library for the CodeCommitProvider.
     """
 
     def __init__(self, title: str, diff_files: List[FilePatchInfo]):
```

### Comparing `pr-agent-0.2.1/pr_agent/git_providers/gerrit_provider.py` & `pr_agent-0.2.2/pr_agent/git_providers/gerrit_provider.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/git_providers/git_provider.py` & `pr_agent-0.2.2/pr_agent/git_providers/git_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         # if the existing description wasn't generated by the pr-agent, just return it as-is
         if not self._is_generated_by_pr_agent(description_lowercase):
             get_logger().info(f"Existing description was not generated by the pr-agent")
             return description
 
         # if the existing description was generated by the pr-agent, but it doesn't contain a user description,
         # return nothing (empty string) because it means there is no user description
-        user_description_header = "## **user description**"
+        user_description_header = "### **user description**"
         if user_description_header not in description_lowercase:
             get_logger().info(f"Existing description was generated by the pr-agent, but it doesn't contain a user description")
             return ""
 
         # otherwise, extract the original user description from the existing pr-agent description and return it
         # user_description_start_position = description_lowercase.find(user_description_header) + len(user_description_header)
         # return description[user_description_start_position:].split("\n", 1)[-1].strip()
@@ -98,16 +98,16 @@
 
         get_logger().info(f"Extracted user description from existing description",
                           description=original_user_description)
         self.user_description = original_user_description
         return original_user_description
 
     def _possible_headers(self):
-        return ("## **user description**", "## **pr type**", "## **pr description**", "## **pr labels**", "## **type**", "## **description**",
-                "## **labels**", "### 🤖 generated by pr agent")
+        return ("### **user description**", "### **pr type**", "### **pr description**", "### **pr labels**", "### **type**", "### **description**",
+                "### **labels**", "### 🤖 generated by pr agent")
 
     def _is_generated_by_pr_agent(self, description_lowercase: str) -> bool:
         possible_headers = self._possible_headers()
         return any(description_lowercase.startswith(header) for header in possible_headers)
 
     @abstractmethod
     def get_repo_settings(self):
```

### Comparing `pr-agent-0.2.1/pr_agent/git_providers/github_provider.py` & `pr_agent-0.2.2/pr_agent/git_providers/github_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -741,26 +741,8 @@
                 return True
             return False
         except Exception as e:
             get_logger().exception(f"Failed to auto-approve, error: {e}")
             return False
 
     def calc_pr_statistics(self, pull_request_data: dict):
-        try:
-            out = {}
-            from datetime import datetime
-            created_at = pull_request_data['created_at']
-            closed_at = pull_request_data['closed_at']
-            closed_at_datetime = datetime.strptime(closed_at, "%Y-%m-%dT%H:%M:%SZ")
-            created_at_datetime = datetime.strptime(created_at, "%Y-%m-%dT%H:%M:%SZ")
-            difference = closed_at_datetime - created_at_datetime
-            out['hours'] = difference.total_seconds() / 3600
-            out['commits'] = pull_request_data['commits']
-            out['comments'] = pull_request_data['comments']
-            out['review_comments'] = pull_request_data['review_comments']
-            out['changed_files'] = pull_request_data['changed_files']
-            out['additions'] = pull_request_data['additions']
-            out['deletions'] = pull_request_data['deletions']
-        except Exception as e:
-            get_logger().exception(f"Failed to calculate PR statistics, error: {e}")
-            return {}
-        return out
+        return {}
```

### Comparing `pr-agent-0.2.1/pr_agent/git_providers/gitlab_provider.py` & `pr_agent-0.2.2/pr_agent/git_providers/gitlab_provider.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/git_providers/local_git_provider.py` & `pr_agent-0.2.2/pr_agent/git_providers/local_git_provider.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/git_providers/utils.py` & `pr_agent-0.2.2/pr_agent/git_providers/utils.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/log/__init__.py` & `pr_agent-0.2.2/pr_agent/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/secret_providers/__init__.py` & `pr_agent-0.2.2/pr_agent/secret_providers/__init__.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/secret_providers/google_cloud_storage_secret_provider.py` & `pr_agent-0.2.2/pr_agent/secret_providers/google_cloud_storage_secret_provider.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/servers/azuredevops_server_webhook.py` & `pr_agent-0.2.2/pr_agent/servers/azuredevops_server_webhook.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/servers/bitbucket_app.py` & `pr_agent-0.2.2/pr_agent/servers/bitbucket_app.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/servers/bitbucket_server_webhook.py` & `pr_agent-0.2.2/pr_agent/servers/bitbucket_server_webhook.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/servers/gerrit_server.py` & `pr_agent-0.2.2/pr_agent/servers/gerrit_server.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/servers/github_action_runner.py` & `pr_agent-0.2.2/pr_agent/servers/github_action_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,27 +42,30 @@
     # Check if required environment variables are set
     if not GITHUB_EVENT_NAME:
         print("GITHUB_EVENT_NAME not set")
         return
     if not GITHUB_EVENT_PATH:
         print("GITHUB_EVENT_PATH not set")
         return
-    if not OPENAI_KEY:
-        print("OPENAI_KEY not set")
-        return
     if not GITHUB_TOKEN:
         print("GITHUB_TOKEN not set")
         return
 
     # Set the environment variables in the settings
-    get_settings().set("OPENAI.KEY", OPENAI_KEY)
+    if OPENAI_KEY:
+        get_settings().set("OPENAI.KEY", OPENAI_KEY)
+    else:
+        # Might not be set if the user is using models not from OpenAI
+        print("OPENAI_KEY not set")
     if OPENAI_ORG:
         get_settings().set("OPENAI.ORG", OPENAI_ORG)
     get_settings().set("GITHUB.USER_TOKEN", GITHUB_TOKEN)
     get_settings().set("GITHUB.DEPLOYMENT_TYPE", "user")
+    enable_output = get_setting_or_env("GITHUB_ACTION_CONFIG.ENABLE_OUTPUT", True)
+    get_settings().set("GITHUB_ACTION_CONFIG.ENABLE_OUTPUT", enable_output)
 
     # Load the event payload
     try:
         with open(GITHUB_EVENT_PATH, 'r') as f:
             event_payload = json.load(f)
     except json.decoder.JSONDecodeError as e:
         print(f"Failed to parse JSON: {e}")
@@ -97,14 +100,16 @@
                 # invoke by default all three tools
                 if auto_describe is None or is_true(auto_describe):
                     await PRDescription(pr_url).run()
                 if auto_review is None or is_true(auto_review):
                     await PRReviewer(pr_url).run()
                 if auto_improve is None or is_true(auto_improve):
                     await PRCodeSuggestions(pr_url).run()
+        else:
+            get_logger().info(f"Skipping action: {action}")
 
     # Handle issue comment event
     elif GITHUB_EVENT_NAME == "issue_comment" or GITHUB_EVENT_NAME == "pull_request_review_comment":
         action = event_payload.get("action")
         if action in ["created", "edited"]:
             comment_body = event_payload.get("comment", {}).get("body")
             try:
```

### Comparing `pr-agent-0.2.1/pr_agent/servers/github_app.py` & `pr_agent-0.2.2/pr_agent/servers/github_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,16 +82,21 @@
                                 action: str,
                                 log_context: Dict[str, Any],
                                 agent: PRAgent):
     if "comment" not in body:
         return {}
     comment_body = body.get("comment", {}).get("body")
     if comment_body and isinstance(comment_body, str) and not comment_body.lstrip().startswith("/"):
-        get_logger().info("Ignoring comment not starting with /")
-        return {}
+        if '/ask' in comment_body and comment_body.strip().startswith('> ![image]'):
+            comment_body_split = comment_body.split('/ask')
+            comment_body = '/ask' + comment_body_split[1] +' \n' +comment_body_split[0].strip().lstrip('>')
+            get_logger().info(f"Reformatting comment_body so command is at the beginning: {comment_body}")
+        else:
+            get_logger().info("Ignoring comment not starting with /")
+            return {}
     disable_eyes = False
     if "issue" in body and "pull_request" in body["issue"] and "url" in body["issue"]["pull_request"]:
         api_url = body["issue"]["pull_request"]["url"]
     elif "comment" in body and "pull_request_url" in body["comment"]:
         api_url = body["comment"]["pull_request_url"]
         try:
             if ('/ask' in comment_body and
@@ -114,38 +119,32 @@
         else:
             get_logger().info(f"User {sender=} is not eligible to process comment on PR {api_url=}")
 
 async def handle_new_pr_opened(body: Dict[str, Any],
                                event: str,
                                sender: str,
                                sender_id: str,
-                               sender_type: str,
                                action: str,
                                log_context: Dict[str, Any],
                                agent: PRAgent):
-    # logic to ignore PRs opened by bot
-    if get_settings().get("GITHUB_APP.IGNORE_BOT_PR", False) and sender_type == "Bot":
-        get_logger().info(f"Ignoring PR from '{sender=}' due to github_app.ignore_bot_pr setting")
-        return {}
-
     title = body.get("pull_request", {}).get("title", "")
 
     # logic to ignore PRs with specific titles (e.g. "[Auto] ...")
     ignore_pr_title_re = get_settings().get("GITHUB_APP.IGNORE_PR_TITLE", [])
     if not isinstance(ignore_pr_title_re, list):
         ignore_pr_title_re = [ignore_pr_title_re]
     if ignore_pr_title_re and any(re.search(regex, title) for regex in ignore_pr_title_re):
         get_logger().info(f"Ignoring PR with title '{title}' due to github_app.ignore_pr_title setting")
         return {}
 
     pull_request, api_url = _check_pull_request_event(action, body, log_context)
     if not (pull_request and api_url):
         get_logger().info(f"Invalid PR event: {action=} {api_url=}")
         return {}
-    if action in get_settings().github_app.handle_pr_actions:  # ['opened', 'reopened', 'ready_for_review', 'review_requested']
+    if action in get_settings().github_app.handle_pr_actions:  # ['opened', 'reopened', 'ready_for_review']
         if get_identity_provider().verify_eligibility("github", sender_id, api_url) is not Eligibility.NOT_ELIGIBLE:
             await _perform_auto_commands_github("pr_commands", agent, body, api_url, log_context)
         else:
             get_logger().info(f"User {sender=} is not eligible to process PR {api_url=}")
 
 async def handle_push_trigger_for_new_commits(body: Dict[str, Any],
                         event: str,
@@ -233,18 +232,19 @@
     sender_type = ""
     try:
         sender = body.get("sender", {}).get("login")
         sender_id = body.get("sender", {}).get("id")
         sender_type = body.get("sender", {}).get("type")
         repo = body.get("repository", {}).get("full_name", "")
         git_org = body.get("organization", {}).get("login", "")
+        installation_id = body.get("installation", {}).get("id", "")
         app_name = get_settings().get("CONFIG.APP_NAME", "Unknown")
         log_context = {"action": action, "event": event, "sender": sender, "server_type": "github_app",
                        "request_id": uuid.uuid4().hex, "build_number": build_number, "app_name": app_name,
-                       "repo": repo, "git_org": git_org}
+                       "repo": repo, "git_org": git_org, "installation_id": installation_id}
     except Exception as e:
         get_logger().error("Failed to get log context", e)
         log_context = {}
     return log_context, sender, sender_id, sender_type
 
 
 async def handle_request(body: Dict[str, Any], event: str):
@@ -257,22 +257,28 @@
     """
     action = body.get("action") # "created", "opened", "reopened", "ready_for_review", "review_requested", "synchronize"
     if not action:
         return {}
     agent = PRAgent()
     log_context, sender, sender_id, sender_type = get_log_context(body, event, action, build_number)
 
+    # logic to ignore PRs opened by bot
+    if get_settings().get("GITHUB_APP.IGNORE_BOT_PR", False) and sender_type == "Bot":
+        if 'pr-agent' not in sender:
+            get_logger().info(f"Ignoring PR from '{sender=}' because it is a bot")
+        return {}
+
     # handle comments on PRs
     if action == 'created':
         get_logger().debug(f'Request body', artifact=body, event=event)
         await handle_comments_on_pr(body, event, sender, sender_id, action, log_context, agent)
     # handle new PRs
     elif event == 'pull_request' and action != 'synchronize' and action != 'closed':
         get_logger().debug(f'Request body', artifact=body, event=event)
-        await handle_new_pr_opened(body, event, sender, sender_id, sender_type, action, log_context, agent)
+        await handle_new_pr_opened(body, event, sender, sender_id, action, log_context, agent)
     # handle pull_request event with synchronize action - "push trigger" for new commits
     elif event == 'pull_request' and action == 'synchronize':
         get_logger().debug(f'Request body', artifact=body, event=event)
         await handle_push_trigger_for_new_commits(body, event, sender, sender_id, action, log_context, agent)
     elif event == 'pull_request' and action == 'closed':
         if get_settings().get("CONFIG.ANALYTICS_FOLDER", ""):
             handle_closed_pr(body, event, action, log_context)
```

### Comparing `pr-agent-0.2.1/pr_agent/servers/github_polling.py` & `pr_agent-0.2.2/pr_agent/servers/github_polling.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/servers/gitlab_webhook.py` & `pr_agent-0.2.2/pr_agent/servers/gitlab_webhook.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/servers/utils.py` & `pr_agent-0.2.2/pr_agent/servers/utils.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/settings/.secrets_template.toml` & `pr_agent-0.2.2/pr_agent/settings/.secrets_template.toml`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 
 [cohere]
 key = "" # Optional, uncomment if you want to use Cohere. Acquire through https://dashboard.cohere.ai/
 
 [replicate]
 key = "" # Optional, uncomment if you want to use Replicate. Acquire through https://replicate.com/
 
+[groq]
+key = "" # Acquire through https://console.groq.com/keys
+
 [huggingface]
 key = "" # Optional, uncomment if you want to use Huggingface Inference API. Acquire through https://huggingface.co/docs/api-inference/quicktour
 api_base = "" # the base url for your huggingface inference endpoint 
 
 [ollama]
 api_base = "" # the base url for your local Llama 2, Code Llama, and other models inference endpoint. Acquire through https://ollama.ai/
```

### Comparing `pr-agent-0.2.1/pr_agent/settings/configuration.toml` & `pr_agent-0.2.2/pr_agent/settings/configuration.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [config]
-model="gpt-4" # "gpt-4-0125-preview"
-model_turbo="gpt-4-0125-preview"
-fallback_models=["gpt-3.5-turbo-16k"]
+model="gpt-4-turbo-2024-04-09"
+model_turbo="gpt-4o"
+fallback_models=["gpt-4-0125-preview"]
 git_provider="github"
 publish_output=true
 publish_output_progress=true
 verbosity_level=0 # 0,1,2
 use_extra_bad_extensions=false
 use_wiki_settings_file=true
 use_repo_settings_file=true
@@ -15,14 +15,15 @@
 max_commits_tokens = 500
 max_model_tokens = 32000 # Limits the maximum number of tokens that can be used by any model, regardless of the model's default capabilities.
 patch_extra_lines = 1
 secret_provider="google_cloud_storage"
 cli_mode=false
 ai_disclaimer_title=""  # Pro feature, title for a collapsible disclaimer to AI outputs
 ai_disclaimer=""  # Pro feature, full text for the AI disclaimer
+output_relevant_configurations=false
 
 [pr_reviewer] # /review #
 # enable/disable features
 require_score_review=false
 require_tests_review=true
 require_estimate_effort_to_review=true
 require_can_be_split_review=false
@@ -40,56 +41,61 @@
 # review labels
 enable_review_labels_security=true
 enable_review_labels_effort=true
 # specific configurations for incremental review (/review -i)
 require_all_thresholds_for_incremental_review=false
 minimal_commits_for_incremental_review=0
 minimal_minutes_for_incremental_review=0
-enable_help_text=true # Determines whether to include help text in the PR review. Enabled by default.
+enable_help_text=false # Determines whether to include help text in the PR review. Enabled by default.
 # auto approval
 enable_auto_approval=false
 maximal_review_effort=5
 
 
 [pr_description] # /describe #
 publish_labels=true
-publish_description_as_comment=false
 add_original_user_description=true
-keep_original_user_title=true
+generate_ai_title=false
 use_bullet_points=true
 extra_instructions = ""
 enable_pr_type=true
 final_update_message = true
 enable_help_text=false
 enable_help_comment=true
+# describe as comment
+publish_description_as_comment=false
+publish_description_as_comment_persistent=true
 ## changes walkthrough section
 enable_semantic_files_types=true
 collapsible_file_list='adaptive' # true, false, 'adaptive'
 inline_file_summary=false # false, true, 'table'
 # markers
 use_description_markers=false
 include_generated_by_header=true
 
 #custom_labels = ['Bug fix', 'Tests', 'Bug fix with tests', 'Enhancement', 'Documentation', 'Other']
 
 [pr_questions] # /ask #
-enable_help_text=true
+enable_help_text=false
 
 
 [pr_code_suggestions] # /improve #
 max_context_tokens=8000
 num_code_suggestions=4
-summarize = true
+commitable_code_suggestions = false
 extra_instructions = ""
 rank_suggestions = false
-enable_help_text=true
+enable_help_text=false
 persistent_comment=false
+# suggestions scoring
+self_reflect_on_suggestions=true
+suggestions_score_threshold=0 # [0-10]. highly recommend not to set this value above 8, since above it may clip highly relevant suggestions
 # params for '/improve --extended' mode
 auto_extended_mode=true
-num_code_suggestions_per_chunk=5
+num_code_suggestions_per_chunk=4
 max_number_of_calls = 3
 parallel_calls = true
 rank_extended_suggestions = false
 final_clip_factor = 0.8
 
 [pr_add_docs] # /add_docs #
 extra_instructions = ""
@@ -104,16 +110,21 @@
 [pr_test] # /test #
 extra_instructions = ""
 testing_framework = "" # specify the testing framework you want to use
 num_tests=3            # number of tests to generate. max 5.
 avoid_mocks=true       # if true, the generated tests will prefer to use real objects instead of mocks
 file = ""              # in case there are several components with the same name, you can specify the relevant file
 class_name = ""        # in case there are several methods with the same name in the same file, you can specify the relevant class name
-enable_help_text=true
+enable_help_text=false
 
+[pr_improve_component] # /improve_component #
+num_code_suggestions=4
+extra_instructions = ""
+file = ""              # in case there are several components with the same name, you can specify the relevant file
+class_name = ""
 
 [checks] # /checks (pro feature) #
 enable_auto_checks_feedback=true
 excluded_checks_list=["lint"] # list of checks to exclude, for example: ["check1", "check2"]
 persistent_comment=true
 enable_help_text=true
 
@@ -129,51 +140,52 @@
 publish_inline_comments_fallback_with_verification = true
 try_fix_invalid_inline_comments = true
 
 [github_action_config]
 # auto_review = true    # set as env var in .github/workflows/pr-agent.yaml
 # auto_describe = true  # set as env var in .github/workflows/pr-agent.yaml
 # auto_improve = true   # set as env var in .github/workflows/pr-agent.yaml
+# enable_output = true   # set as env var in .github/workflows/pr-agent.yaml
 
 [github_app]
 # these toggles allows running the github app from custom deployments
 override_deployment_type = true
 # settings for "pull_request" event
 handle_pr_actions = ['opened', 'reopened', 'ready_for_review']
 pr_commands = [
-    "/describe --pr_description.add_original_user_description=true --pr_description.keep_original_user_title=true",
+    "/describe",
     "/review --pr_reviewer.num_code_suggestions=0",
-    "/improve --pr_code_suggestions.summarize=true",
+    "/improve",
 ]
 # settings for "pull_request" event with "synchronize" action - used to detect and handle push triggers for new commits
 handle_push_trigger = false
 push_trigger_ignore_bot_commits = true
 push_trigger_ignore_merge_commits = true
 push_trigger_wait_for_initial_review = true
 push_trigger_pending_tasks_backlog = true
 push_trigger_pending_tasks_ttl = 300
 push_commands = [
-    "/describe --pr_description.add_original_user_description=true --pr_description.keep_original_user_title=true",
+    "/describe",
     "/review --pr_reviewer.num_code_suggestions=0",
 ]
 ignore_pr_title = []
-ignore_bot_pr = false
+ignore_bot_pr = true
 
 [gitlab]
 url = "https://gitlab.com" # URL to the gitlab service
 pr_commands = [
-    "/describe --pr_description.add_original_user_description=true --pr_description.keep_original_user_title=true",
+    "/describe",
     "/review --pr_reviewer.num_code_suggestions=0",
-    "/improve --pr_code_suggestions.summarize=true",
+    "/improve",
 ]
 
 [bitbucket_app]
 pr_commands = [
     "/review --pr_reviewer.num_code_suggestions=0",
-    "/improve --pr_code_suggestions.summarize=false",
+    "/improve --pr_code_suggestions.commitable_code_suggestions=true",
 ]
 
 
 [local]
 # LocalGitProvider settings - uncomment to use paths other than default
 # description_path= "path/to/description.md"
 # review_path= "path/to/review.md"
```

### Comparing `pr-agent-0.2.1/pr_agent/settings/custom_labels.toml` & `pr_agent-0.2.2/pr_agent/settings/custom_labels.toml`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/settings/language_extensions.toml` & `pr_agent-0.2.2/pr_agent/settings/language_extensions.toml`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/settings/pr_add_docs.toml` & `pr_agent-0.2.2/pr_agent/settings/pr_add_docs.toml`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/settings/pr_code_suggestions_prompts.toml` & `pr_agent-0.2.2/pr_agent/settings/pr_code_suggestions_prompts.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [pr_code_suggestions_prompt]
-system="""You are PR-Reviewer, a language model that specializes in suggesting code improvements for a Pull Request (PR).
-Your task is to provide meaningful and actionable code suggestions, to improve the new code presented in a PR diff (lines starting with '+').
+system="""You are PR-Reviewer, a language model that specializes in suggesting ways to improve for a Pull Request (PR) code.
+Your task is to provide meaningful and actionable code suggestions, to improve the new code presented in a PR diff.
 
-Example for the PR Diff format:
+
+The format we will use to present the PR code diff:
 ======
 ## file: 'src/file1.py'
 
 @@ ... @@ def func1():
 __new hunk__
 12  code line1 that remained unchanged in the PR
 13 +new hunk code line2 added in the PR
@@ -22,53 +23,52 @@
 __old hunk__
 ...
 
 
 ## file: 'src/file2.py'
 ...
 ======
+- In this format, we separated each hunk of code to '__new hunk__' and '__old hunk__' sections. The '__new hunk__' section contains the new code of the chunk, and the '__old hunk__' section contains the old code that was removed.
+- Code lines are prefixed symbols ('+', '-', ' '). The '+' symbol indicates new code added in the PR, the '-' symbol indicates code removed in the PR, and the ' ' symbol indicates unchanged code.
+- We also added line numbers for the '__new hunk__' sections, to help you refer to the code lines in your suggestions. These line numbers are not part of the actual code, and are only used for reference.
 
 
-Specific instructions:
+Specific instructions for generating code suggestions:
 - Provide up to {{ num_code_suggestions }} code suggestions. The suggestions should be diverse and insightful.
-- The suggestions should refer only to code from the '__new hunk__' sections, and focus on new lines of code (lines starting with '+').
-- Prioritize suggestions that address major problems, issues and bugs in the PR code. As a second priority, suggestions should focus on enhancement, best practice, performance, maintainability, and other aspects.
+- The suggestions should focus on ways to improve the new code in the PR, meaning focusing on lines from '__new hunk__' sections, starting with '+'. Use the '__old hunk__' sections to understand the context of the code changes.
+- Prioritize suggestions that address possible issues, major problems, and bugs in the PR code.
 - Don't suggest to add docstring, type hints, or comments, or to remove unused imports.
 - Suggestions should not repeat code already present in the '__new hunk__' sections.
-- Provide the exact line numbers range (inclusive) for each suggestion.
+- Provide the exact line numbers range (inclusive) for each suggestion. Use the line numbers from the '__new hunk__' sections.
 - When quoting variables or names from the code, use backticks (`) instead of single quote (').
+- Take into account that you are reviewing a PR code diff, and that the entire codebase is not available for you as context. Hence, avoid suggestions that might conflict with unseen parts of the codebase.
 
 
 {%- if extra_instructions %}
 
 
-Extra instructions from the user:
+Extra instructions from the user, that should be taken into account with high priority:
 ======
 {{ extra_instructions }}
 ======
 {%- endif %}
 
 
 The output must be a YAML object equivalent to type $PRCodeSuggestions, according to the following Pydantic definitions:
 =====
 class CodeSuggestion(BaseModel):
     relevant_file: str = Field(description="the relevant file full path")
     language: str = Field(description="the code language of the relevant file")
     suggestion_content: str = Field(description="an actionable suggestion for meaningfully improving the new code introduced in the PR")
-{%- if summarize_mode %}
-    existing_code: str = Field(description="a short code snippet from a '__new hunk__' section to illustrate the relevant existing code. Don't show the line numbers.")
-    improved_code: str = Field(description="a short code snippet to illustrate the improved code, after applying the suggestion.")
-    one_sentence_summary:str = Field(description="a short summary of the suggestion action, in a single sentence. Focus on the 'what'. Be general, and avoid method or variable names.")
-{%- else %}
-    existing_code: str = Field(description="a code snippet, demonstrating the relevant code lines from a '__new hunk__' section. It must be contiguous, correctly formatted and indented, and without line numbers")
-    improved_code: str = Field(description="a new code snippet, that can be used to replace the relevant lines in '__new hunk__' code. Replacement suggestions should be complete, correctly formatted and indented, and without line numbers")
-{%- endif %}
+    existing_code: str = Field(description="a short code snippet, demonstrating the relevant code lines from a '__new hunk__' section. It must be without line numbers. Use abbreviations if needed")
+    improved_code: str = Field(description="a new code snippet, that can be used to replace the relevant 'existing_code' lines in '__new hunk__' code after applying the suggestion")
+    one_sentence_summary: str = Field(description="a short summary of the suggestion action, in a single sentence. Focus on the 'what'. Be general, and avoid method or variable names.")
     relevant_lines_start: int = Field(description="The relevant line number, from a '__new hunk__' section, where the suggestion starts (inclusive). Should be derived from the hunk line numbers, and correspond to the 'existing code' snippet above")
     relevant_lines_end: int = Field(description="The relevant line number, from a '__new hunk__' section, where the suggestion ends (inclusive). Should be derived from the hunk line numbers, and correspond to the 'existing code' snippet above")
-    label: str = Field(description="a single label for the suggestion, to help the user understand the suggestion type. For example: 'security', 'bug', 'performance', 'enhancement', 'possible issue', 'best practice', 'maintainability', etc. Other labels are also allowed")
+    label: str = Field(description="a single label for the suggestion, to help the user understand the suggestion type. For example: 'security', 'possible bug', 'possible issue', 'performance', 'enhancement', 'best practice', 'maintainability', etc. Other labels are also allowed")
 
 class PRCodeSuggestions(BaseModel):
     code_suggestions: List[CodeSuggestion]
 =====
 
 
 Example output:
@@ -76,31 +76,22 @@
 code_suggestions:
 - relevant_file: |
     src/file1.py
   language: |
     python
   suggestion_content: |
     ...
-{%- if summarize_mode %}
   existing_code: |
     ...
   improved_code: |
     ...
   one_sentence_summary: |
     ...
   relevant_lines_start: 12
   relevant_lines_end: 13
-{%- else %}
-  existing_code: |
-    ...
-  relevant_lines_start: 12
-  relevant_lines_end: 13
-  improved_code: |
-    ...
-{%- endif %}
   label: |
     ...
 ```
 
 
 Each YAML output MUST be after a newline, indented, with block scalar indicator ('|').
 """
```

### Comparing `pr-agent-0.2.1/pr_agent/settings/pr_custom_labels.toml` & `pr_agent-0.2.2/pr_agent/settings/pr_custom_labels.toml`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/settings/pr_description_prompts.toml` & `pr_agent-0.2.2/pr_agent/settings/pr_description_prompts.toml`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/settings/pr_information_from_user_prompts.toml` & `pr_agent-0.2.2/pr_agent/settings/pr_information_from_user_prompts.toml`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/settings/pr_line_questions_prompts.toml` & `pr_agent-0.2.2/pr_agent/settings/pr_line_questions_prompts.toml`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/settings/pr_questions_prompts.toml` & `pr_agent-0.2.2/pr_agent/settings/pr_questions_prompts.toml`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/settings/pr_reviewer_prompts.toml` & `pr_agent-0.2.2/pr_agent/settings/pr_reviewer_prompts.toml`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/settings/pr_sort_code_suggestions_prompts.toml` & `pr_agent-0.2.2/pr_agent/settings/pr_sort_code_suggestions_prompts.toml`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/settings/pr_update_changelog_prompts.toml` & `pr_agent-0.2.2/pr_agent/settings/pr_update_changelog_prompts.toml`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/tools/pr_add_docs.py` & `pr_agent-0.2.2/pr_agent/tools/pr_add_docs.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/tools/pr_code_suggestions.py` & `pr_agent-0.2.2/pr_agent/tools/pr_code_suggestions.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Dict, List
 from jinja2 import Environment, StrictUndefined
 
 from pr_agent.algo.ai_handlers.base_ai_handler import BaseAiHandler
 from pr_agent.algo.ai_handlers.litellm_ai_handler import LiteLLMAIHandler
 from pr_agent.algo.pr_processing import get_pr_diff, get_pr_multi_diffs, retry_with_fallback_models
 from pr_agent.algo.token_handler import TokenHandler
-from pr_agent.algo.utils import load_yaml, replace_code_tags, ModelType
+from pr_agent.algo.utils import load_yaml, replace_code_tags, ModelType, show_relevant_configurations
 from pr_agent.config_loader import get_settings
 from pr_agent.git_providers import get_git_provider
 from pr_agent.git_providers.git_provider import get_main_pr_language
 from pr_agent.log import get_logger
 from pr_agent.servers.help import HelpMessage
 from pr_agent.tools.pr_description import insert_br_after_x_chars
 import difflib
@@ -53,15 +53,14 @@
         self.vars = {
             "title": self.git_provider.pr.title,
             "branch": self.git_provider.get_pr_branch(),
             "description": self.git_provider.get_pr_description(),
             "language": self.main_language,
             "diff": "",  # empty diff for initial calculation
             "num_code_suggestions": num_code_suggestions,
-            "summarize_mode": get_settings().pr_code_suggestions.summarize,
             "extra_instructions": get_settings().pr_code_suggestions.extra_instructions,
             "commit_messages_str": self.git_provider.get_commit_messages(),
         }
         self.token_handler = TokenHandler(self.git_provider.pr,
                                           self.vars,
                                           get_settings().pr_code_suggestions_prompt.system,
                                           get_settings().pr_code_suggestions_prompt.user)
@@ -72,59 +71,65 @@
 
     async def run(self):
         try:
             get_logger().info('Generating code suggestions for PR...')
             relevant_configs = {'pr_code_suggestions': dict(get_settings().pr_code_suggestions),
                                 'config': dict(get_settings().config)}
             get_logger().debug("Relevant configs", artifacts=relevant_configs)
-            if get_settings().config.publish_output:
+            if get_settings().config.publish_output and get_settings().config.publish_output_progress:
                 if self.git_provider.is_supported("gfm_markdown"):
                     self.progress_response = self.git_provider.publish_comment(self.progress)
                 else:
                     self.git_provider.publish_comment("Preparing suggestions...", is_temporary=True)
 
             if not self.is_extended:
-                await retry_with_fallback_models(self._prepare_prediction, ModelType.TURBO)
-                data = self._prepare_pr_code_suggestions()
+                data = await retry_with_fallback_models(self._prepare_prediction)
             else:
-                data = await retry_with_fallback_models(self._prepare_prediction_extended, ModelType.TURBO)
+                data = await retry_with_fallback_models(self._prepare_prediction_extended)
+            if not data:
+                data = {"code_suggestions": []}
 
-            if (not data) or (not 'code_suggestions' in data) or (not data['code_suggestions']):
+            if data is None or 'code_suggestions' not in data or not data['code_suggestions']:
                 get_logger().error('No code suggestions found for PR.')
-                pr_body = "## PR Code Suggestions\n\nNo code suggestions found for PR."
+                pr_body = "## PR Code Suggestions ✨\n\nNo code suggestions found for PR."
                 get_logger().debug(f"PR output", artifact=pr_body)
                 if self.progress_response:
                     self.git_provider.edit_comment(self.progress_response, body=pr_body)
                 else:
                     self.git_provider.publish_comment(pr_body)
                 return
 
             if (not self.is_extended and get_settings().pr_code_suggestions.rank_suggestions) or \
                     (self.is_extended and get_settings().pr_code_suggestions.rank_extended_suggestions):
                 get_logger().info('Ranking Suggestions...')
                 data['code_suggestions'] = await self.rank_suggestions(data['code_suggestions'])
 
             if get_settings().config.publish_output:
                 self.git_provider.remove_initial_comment()
-                if get_settings().pr_code_suggestions.summarize and self.git_provider.is_supported("gfm_markdown"):
+                if ((not get_settings().pr_code_suggestions.commitable_code_suggestions) and
+                        self.git_provider.is_supported("gfm_markdown")):
 
                     # generate summarized suggestions
                     pr_body = self.generate_summarized_suggestions(data)
                     get_logger().debug(f"PR output", artifact=pr_body)
 
                     # add usage guide
                     if get_settings().pr_code_suggestions.enable_help_text:
-                        pr_body += "<hr>\n\n<details> <summary><strong>✨ Improve tool usage guide:</strong></summary><hr> \n\n"
+                        pr_body += "<hr>\n\n<details> <summary><strong>💡 Tool usage guide:</strong></summary><hr> \n\n"
                         pr_body += HelpMessage.get_improve_usage_guide()
                         pr_body += "\n</details>\n"
 
+                    # Output the relevant configurations if enabled
+                    if get_settings().get('config', {}).get('output_relevant_configurations', False):
+                        pr_body += show_relevant_configurations(relevant_section='pr_code_suggestions')
+
                     if get_settings().pr_code_suggestions.persistent_comment:
                         final_update_message = False
                         self.git_provider.publish_persistent_comment(pr_body,
-                                                                     initial_header="## PR Code Suggestions",
+                                                                     initial_header="## PR Code Suggestions ✨",
                                                                      update_header=True,
                                                                      name="suggestions",
                                                                      final_update_message=final_update_message, )
                         if self.progress_response:
                             self.progress_response.delete()
                     else:
 
@@ -144,80 +149,121 @@
             else:
                 try:
                     self.git_provider.remove_initial_comment()
                     self.git_provider.publish_comment(f"Failed to generate code suggestions for PR")
                 except Exception as e:
                     pass
 
-    async def _prepare_prediction(self, model: str):
+    async def _prepare_prediction(self, model: str) -> dict:
         self.patches_diff = get_pr_diff(self.git_provider,
                                         self.token_handler,
                                         model,
                                         add_line_numbers_to_hunks=True,
                                         disable_extra_lines=True)
 
         if self.patches_diff:
             get_logger().debug(f"PR diff", artifact=self.patches_diff)
             self.prediction = await self._get_prediction(model, self.patches_diff)
         else:
             get_logger().error(f"Error getting PR diff")
             self.prediction = None
 
-    async def _get_prediction(self, model: str, patches_diff: str):
+        data = self.prediction
+        return data
+
+    async def _get_prediction(self, model: str, patches_diff: str) -> dict:
         variables = copy.deepcopy(self.vars)
         variables["diff"] = patches_diff  # update diff
         environment = Environment(undefined=StrictUndefined)
         system_prompt = environment.from_string(get_settings().pr_code_suggestions_prompt.system).render(variables)
         user_prompt = environment.from_string(get_settings().pr_code_suggestions_prompt.user).render(variables)
         response, finish_reason = await self.ai_handler.chat_completion(model=model, temperature=0.2,
                                                                         system=system_prompt, user=user_prompt)
 
-        return response
+        # load suggestions from the AI response
+        data = self._prepare_pr_code_suggestions(response)
+
+        # self-reflect on suggestions
+        if get_settings().pr_code_suggestions.self_reflect_on_suggestions:
+            model = get_settings().config.model_turbo # use turbo model for self-reflection, since it is an easier task
+            response_reflect = await self.self_reflect_on_suggestions(data["code_suggestions"], patches_diff, model=model)
+            if response_reflect:
+                response_reflect_yaml = load_yaml(response_reflect)
+                code_suggestions_feedback = response_reflect_yaml["code_suggestions"]
+                if len(code_suggestions_feedback) == len(data["code_suggestions"]):
+                    for i, suggestion in enumerate(data["code_suggestions"]):
+                        try:
+                            suggestion["score"] = code_suggestions_feedback[i]["suggestion_score"]
+                            suggestion["score_why"] = code_suggestions_feedback[i]["why"]
+                        except Exception as e: #
+                            get_logger().error(f"Error processing suggestion score {i}",
+                                               artifact={"suggestion": suggestion,
+                                                         "code_suggestions_feedback": code_suggestions_feedback[i]})
+                            suggestion["score"] = 7
+                            suggestion["score_why"] = ""
+            else:
+                # get_logger().error(f"Could not self-reflect on suggestions. using default score 7")
+                for i, suggestion in enumerate(data["code_suggestions"]):
+                    suggestion["score"] = 7
+                    suggestion["score_why"] = ""
+
+        return data
 
     @staticmethod
     def _truncate_if_needed(suggestion):
         max_code_suggestion_length = get_settings().get("PR_CODE_SUGGESTIONS.MAX_CODE_SUGGESTION_LENGTH", 0)
         suggestion_truncation_message = get_settings().get("PR_CODE_SUGGESTIONS.SUGGESTION_TRUNCATION_MESSAGE", "")
         if max_code_suggestion_length > 0:
             if len(suggestion['improved_code']) > max_code_suggestion_length:
                 suggestion['improved_code'] = suggestion['improved_code'][:max_code_suggestion_length]
                 suggestion['improved_code'] += f"\n{suggestion_truncation_message}"
                 get_logger().info(f"Truncated suggestion from {len(suggestion['improved_code'])} "
                                       f"characters to {max_code_suggestion_length} characters")
         return suggestion
 
-    def _prepare_pr_code_suggestions(self) -> Dict:
-        review = self.prediction.strip()
-        data = load_yaml(review,
+    def _prepare_pr_code_suggestions(self, predictions: str) -> Dict:
+        data = load_yaml(predictions.strip(),
                          keys_fix_yaml=["relevant_file", "suggestion_content", "existing_code", "improved_code"])
         if isinstance(data, list):
             data = {'code_suggestions': data}
 
-        # remove invalid suggestions
+        # remove or edit invalid suggestions
         suggestion_list = []
         one_sentence_summary_list = []
         for i, suggestion in enumerate(data['code_suggestions']):
-            if get_settings().pr_code_suggestions.summarize:
-                if not suggestion or 'one_sentence_summary' not in suggestion or 'label' not in suggestion or 'relevant_file' not in suggestion:
+            try:
+                if (not suggestion or 'one_sentence_summary' not in suggestion or
+                        'label' not in suggestion or 'relevant_file' not in suggestion):
                     get_logger().debug(f"Skipping suggestion {i + 1}, because it is invalid: {suggestion}")
                     continue
 
                 if suggestion['one_sentence_summary'] in one_sentence_summary_list:
                     get_logger().debug(f"Skipping suggestion {i + 1}, because it is a duplicate: {suggestion}")
                     continue
 
-            if ('existing_code' in suggestion) and ('improved_code' in suggestion) and (
-                    suggestion['existing_code'] != suggestion['improved_code']):
-                suggestion = self._truncate_if_needed(suggestion)
-                if get_settings().pr_code_suggestions.summarize:
+                if 'const' in suggestion['suggestion_content'] and 'instead' in suggestion['suggestion_content'] and 'let' in suggestion['suggestion_content']:
+                    get_logger().debug(f"Skipping suggestion {i + 1}, because it uses 'const instead let': {suggestion}")
+                    continue
+
+                if ('existing_code' in suggestion) and ('improved_code' in suggestion):
+                    if suggestion['existing_code'] == suggestion['improved_code']:
+                        get_logger().debug(
+                            f"edited improved suggestion {i + 1}, because equal to existing code: {suggestion['existing_code']}")
+                        if get_settings().pr_code_suggestions.commitable_code_suggestions:
+                            suggestion['improved_code'] = "" # we need 'existing_code' to locate the code in the PR
+                        else:
+                            suggestion['existing_code'] = ""
+                    suggestion = self._truncate_if_needed(suggestion)
                     one_sentence_summary_list.append(suggestion['one_sentence_summary'])
-                suggestion_list.append(suggestion)
-            else:
-                get_logger().debug(
-                    f"Skipping suggestion {i + 1}, because existing code is equal to improved code {suggestion['existing_code']}")
+                    suggestion_list.append(suggestion)
+                else:
+                    get_logger().info(
+                        f"Skipping suggestion {i + 1}, because it does not contain 'existing_code' or 'improved_code': {suggestion}")
+            except Exception as e:
+                get_logger().error(f"Error processing suggestion {i + 1}: {suggestion}, error: {e}")
         data['code_suggestions'] = suggestion_list
 
         return data
 
     def push_inline_code_suggestions(self, data):
         code_suggestions = []
 
@@ -236,15 +282,18 @@
                 content = d['suggestion_content'].rstrip()
                 new_code_snippet = d['improved_code'].rstrip()
                 label = d['label'].strip()
 
                 if new_code_snippet:
                     new_code_snippet = self.dedent_code(relevant_file, relevant_lines_start, new_code_snippet)
 
-                body = f"**Suggestion:** {content} [{label}]\n```suggestion\n" + new_code_snippet + "\n```"
+                if d.get('score'):
+                    body = f"**Suggestion:** {content} [{label}, importance: {d.get('score')}]\n```suggestion\n" + new_code_snippet + "\n```"
+                else:
+                    body = f"**Suggestion:** {content} [{label}]\n```suggestion\n" + new_code_snippet + "\n```"
                 code_suggestions.append({'body': body, 'relevant_file': relevant_file,
                                              'relevant_lines_start': relevant_lines_start,
                                              'relevant_lines_end': relevant_lines_end})
             except Exception:
                 get_logger().info(f"Could not parse suggestion: {d}")
 
         is_successful = self.git_provider.publish_code_suggestions(code_suggestions)
@@ -285,35 +334,46 @@
             return True
         return False
 
     async def _prepare_prediction_extended(self, model: str) -> dict:
         self.patches_diff_list = get_pr_multi_diffs(self.git_provider, self.token_handler, model,
                                                     max_calls=get_settings().pr_code_suggestions.max_number_of_calls)
         if self.patches_diff_list:
-            get_logger().debug(f"PR diff", artifact=self.patches_diff_list)
+            get_logger().info(f"Number of PR chunk calls: {len(self.patches_diff_list)}")
+            get_logger().debug(f"PR diff:", artifact=self.patches_diff_list)
 
             # parallelize calls to AI:
             if get_settings().pr_code_suggestions.parallel_calls:
                 prediction_list = await asyncio.gather(
                     *[self._get_prediction(model, patches_diff) for patches_diff in self.patches_diff_list])
                 self.prediction_list = prediction_list
             else:
                 prediction_list = []
                 for i, patches_diff in enumerate(self.patches_diff_list):
                     prediction = await self._get_prediction(model, patches_diff)
                     prediction_list.append(prediction)
 
-            data = {}
-            for prediction in prediction_list:
-                self.prediction = prediction
-                data_per_chunk = self._prepare_pr_code_suggestions()
-                if "code_suggestions" in data:
-                    data["code_suggestions"].extend(data_per_chunk["code_suggestions"])
-                else:
-                    data.update(data_per_chunk)
+            data = {"code_suggestions": []}
+            for j, predictions in enumerate(prediction_list):  # each call adds an element to the list
+                if "code_suggestions" in predictions:
+                    score_threshold = max(1, get_settings().pr_code_suggestions.suggestions_score_threshold)
+                    for i, prediction in enumerate(predictions["code_suggestions"]):
+                        try:
+                            if get_settings().pr_code_suggestions.self_reflect_on_suggestions:
+                                score = int(prediction["score"])
+                                if score >= score_threshold:
+                                    data["code_suggestions"].append(prediction)
+                                else:
+                                    get_logger().info(
+                                        f"Removing suggestions {i} from call {j}, because score is {score}, and score_threshold is {score_threshold}",
+                                        artifact=prediction)
+                            else:
+                                data["code_suggestions"].append(prediction)
+                        except Exception as e:
+                            get_logger().error(f"Error getting PR diff for suggestion {i} in call {j}, error: {e}")
             self.data = data
         else:
             get_logger().error(f"Error getting PR diff")
             self.data = data = None
         return data
 
     async def rank_suggestions(self, data: List) -> List:
@@ -371,57 +431,72 @@
                 get_logger().info(f"Could not sort suggestions, error: {e}")
             data_sorted = suggestion_list
 
         return data_sorted
 
     def generate_summarized_suggestions(self, data: Dict) -> str:
         try:
-            pr_body = "## PR Code Suggestions\n\n"
+            pr_body = "## PR Code Suggestions ✨\n\n"
 
             if len(data.get('code_suggestions', [])) == 0:
                 pr_body += "No suggestions found to improve this PR."
                 return pr_body
 
             language_extension_map_org = get_settings().language_extension_map_org
             extension_to_language = {}
             for language, extensions in language_extension_map_org.items():
                 for ext in extensions:
                     extension_to_language[ext] = language
 
-            pr_body = "## PR Code Suggestions\n\n"
+            pr_body = "## PR Code Suggestions ✨\n\n"
 
             pr_body += "<table>"
-            header = f"Suggestions"
-            delta = 76
+            header = f"Suggestion"
+            delta = 66
             header += "&nbsp; " * delta
-            pr_body += f"""<thead><tr><td>Category</td><td align=left>{header}</td></tr></thead>"""
+            if get_settings().pr_code_suggestions.self_reflect_on_suggestions:
+                pr_body += f"""<thead><tr><td>Category</td><td align=left>{header}</td><td align=center>Score</td></tr>"""
+            else:
+                pr_body += f"""<thead><tr><td>Category</td><td align=left>{header}</td></tr>"""
             pr_body += """<tbody>"""
             suggestions_labels = dict()
             # add all suggestions related to each label
             for suggestion in data['code_suggestions']:
                 label = suggestion['label'].strip().strip("'").strip('"')
                 if label not in suggestions_labels:
                     suggestions_labels[label] = []
                 suggestions_labels[label].append(suggestion)
 
+            # sort suggestions_labels by the suggestion with the highest score
+            if get_settings().pr_code_suggestions.self_reflect_on_suggestions:
+                suggestions_labels = dict(sorted(suggestions_labels.items(), key=lambda x: max([s['score'] for s in x[1]]), reverse=True))
+                # sort the suggestions inside each label group by score
+                for label, suggestions in suggestions_labels.items():
+                    suggestions_labels[label] = sorted(suggestions, key=lambda x: x['score'], reverse=True)
+
+
             for label, suggestions in suggestions_labels.items():
                 num_suggestions=len(suggestions)
                 pr_body += f"""<tr><td rowspan={num_suggestions}><strong>{label.capitalize()}</strong></td>\n"""
                 for i, suggestion in enumerate(suggestions):
 
                     relevant_file = suggestion['relevant_file'].strip()
                     relevant_lines_start = int(suggestion['relevant_lines_start'])
                     relevant_lines_end = int(suggestion['relevant_lines_end'])
                     range_str = ""
                     if relevant_lines_start == relevant_lines_end:
                         range_str = f"[{relevant_lines_start}]"
                     else:
                         range_str = f"[{relevant_lines_start}-{relevant_lines_end}]"
-                    code_snippet_link = self.git_provider.get_line_link(relevant_file, relevant_lines_start,
-                                                                        relevant_lines_end)
+
+                    try:
+                        code_snippet_link = self.git_provider.get_line_link(relevant_file, relevant_lines_start,
+                                                                            relevant_lines_end)
+                    except:
+                        code_snippet_link = ""
                     # add html table for each suggestion
 
                     suggestion_content = suggestion['suggestion_content'].rstrip().rstrip()
 
                     suggestion_content = insert_br_after_x_chars(suggestion_content, 90)
                     # pr_body += f"<tr><td><details><summary>{suggestion_content}</summary>"
                     existing_code = suggestion['existing_code'].rstrip()+"\n"
@@ -434,31 +509,66 @@
 
                     example_code = ""
                     example_code += f"```diff\n{patch}\n```\n"
                     if i==0:
                         pr_body += f"""<td>\n\n"""
                     else:
                         pr_body += f"""<tr><td>\n\n"""
-                    suggestion_summary = suggestion['one_sentence_summary'].strip()
+                    suggestion_summary = suggestion['one_sentence_summary'].strip().rstrip('.')
                     if '`' in suggestion_summary:
                         suggestion_summary = replace_code_tags(suggestion_summary)
-                    # suggestion_summary = suggestion_summary + max((77-len(suggestion_summary)), 0)*"&nbsp;"
-                    pr_body += f"""\n\n<details><summary>{suggestion_summary}</summary>\n\n___\n\n"""
 
+                    pr_body += f"""\n\n<details><summary>{suggestion_summary}</summary>\n\n___\n\n"""
                     pr_body += f"""
 **{suggestion_content}**
     
 [{relevant_file} {range_str}]({code_snippet_link})
 
 {example_code}                   
 """
+                    if get_settings().pr_code_suggestions.self_reflect_on_suggestions:
+                        pr_body +=f"\n\n<details><summary><b>Suggestion importance[1-10]: {suggestion['score']}</b></summary>\n\n"
+                        pr_body += f"Why: {suggestion['score_why']}\n\n"
+                        pr_body += f"</details>"
+
                     pr_body += f"</details>"
+
+                    # # add another column for 'score'
+                    if get_settings().pr_code_suggestions.self_reflect_on_suggestions:
+                        pr_body += f"</td><td align=center>{suggestion['score']}\n\n"
+
                     pr_body += f"</td></tr>"
 
 
                 # pr_body += "</details>"
                 # pr_body += """</td></tr>"""
             pr_body += """</tr></tbody></table>"""
             return pr_body
         except Exception as e:
             get_logger().info(f"Failed to publish summarized code suggestions, error: {e}")
             return ""
+
+    async def self_reflect_on_suggestions(self, suggestion_list: List, patches_diff: str, model: str) -> str:
+        if not suggestion_list:
+            return ""
+
+        try:
+            suggestion_str = ""
+            for i, suggestion in enumerate(suggestion_list):
+                suggestion_str += f"suggestion {i + 1}: " + str(suggestion) + '\n\n'
+
+            variables = {'suggestion_list': suggestion_list,
+                         'suggestion_str': suggestion_str,
+                         "diff": patches_diff,
+                         'num_code_suggestions': len(suggestion_list)}
+            environment = Environment(undefined=StrictUndefined)
+            system_prompt_reflect = environment.from_string(get_settings().pr_code_suggestions_reflect_prompt.system).render(
+                variables)
+            user_prompt_reflect = environment.from_string(get_settings().pr_code_suggestions_reflect_prompt.user).render(variables)
+            with get_logger().contextualize(command="self_reflect_on_suggestions"):
+                response_reflect, finish_reason_reflect = await self.ai_handler.chat_completion(model=model,
+                                                                                system=system_prompt_reflect,
+                                                                                user=user_prompt_reflect)
+        except Exception as e:
+            get_logger().info(f"Could not reflect on suggestions, error: {e}")
+            return ""
+        return response_reflect
```

### Comparing `pr-agent-0.2.1/pr_agent/tools/pr_config.py` & `pr_agent-0.2.2/pr_agent/tools/pr_config.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/tools/pr_description.py` & `pr_agent-0.2.2/pr_agent/tools/pr_description.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from jinja2 import Environment, StrictUndefined
 
 from pr_agent.algo.ai_handlers.base_ai_handler import BaseAiHandler
 from pr_agent.algo.ai_handlers.litellm_ai_handler import LiteLLMAIHandler
 from pr_agent.algo.pr_processing import get_pr_diff, retry_with_fallback_models
 from pr_agent.algo.token_handler import TokenHandler
-from pr_agent.algo.utils import load_yaml, set_custom_labels, get_user_labels, ModelType
+from pr_agent.algo.utils import load_yaml, set_custom_labels, get_user_labels, ModelType, show_relevant_configurations
 from pr_agent.config_loader import get_settings
 from pr_agent.git_providers import get_git_provider
 from pr_agent.git_providers.git_provider import get_main_pr_language
 from pr_agent.log import get_logger
 from pr_agent.servers.help import HelpMessage
 
 
@@ -78,15 +78,15 @@
             get_logger().info(f"Generating a PR description for pr_id: {self.pr_id}")
             relevant_configs = {'pr_description': dict(get_settings().pr_description),
                                 'config': dict(get_settings().config)}
             get_logger().debug("Relevant configs", artifacts=relevant_configs)
             if get_settings().config.publish_output:
                 self.git_provider.publish_comment("Preparing PR description...", is_temporary=True)
 
-            await retry_with_fallback_models(self._prepare_prediction, ModelType.TURBO) # turbo model because larger context
+            await retry_with_fallback_models(self._prepare_prediction, ModelType.TURBO)
 
             if self.prediction:
                 self._prepare_data()
             else:
                 get_logger().error(f"Error getting AI prediction {self.pr_id}")
                 self.git_provider.remove_initial_comment()
                 return None
@@ -109,17 +109,21 @@
 
             # Add help text if gfm_markdown is supported
             if self.git_provider.is_supported("gfm_markdown") and get_settings().pr_description.enable_help_text:
                 pr_body += "<hr>\n\n<details> <summary><strong>✨ Describe tool usage guide:</strong></summary><hr> \n\n"
                 pr_body += HelpMessage.get_describe_usage_guide()
                 pr_body += "\n</details>\n"
             elif get_settings().pr_description.enable_help_comment:
-                pr_body += "\n\n___\n\n> ✨ **PR-Agent usage**:"
+                pr_body += "\n\n___\n\n> 💡 **PR-Agent usage**:"
                 pr_body += "\n>Comment `/help` on the PR to get a list of all available PR-Agent tools and their descriptions\n\n"
 
+            # Output the relevant configurations if enabled
+            if get_settings().get('config', {}).get('output_relevant_configurations', False):
+                pr_body += show_relevant_configurations(relevant_section='pr_description')
+
             if get_settings().config.publish_output:
                 # publish labels
                 if get_settings().pr_description.publish_labels and self.git_provider.is_supported("get_labels"):
                     original_labels = self.git_provider.get_pr_labels(update=True)
                     get_logger().debug(f"original labels", artifact=original_labels)
                     user_labels = get_user_labels(original_labels)
                     new_labels = pr_labels + user_labels
@@ -128,15 +132,22 @@
                         self.git_provider.publish_labels(new_labels)
                     else:
                         get_logger().debug(f"Labels are the same, not updating")
 
                 # publish description
                 if get_settings().pr_description.publish_description_as_comment:
                     full_markdown_description = f"## Title\n\n{pr_title}\n\n___\n{pr_body}"
-                    self.git_provider.publish_comment(full_markdown_description)
+                    if get_settings().pr_description.publish_description_as_comment_persistent:
+                        self.git_provider.publish_persistent_comment(full_markdown_description,
+                                                                     initial_header="## Title",
+                                                                     update_header=True,
+                                                                     name="describe",
+                                                                     final_update_message=False, )
+                    else:
+                        self.git_provider.publish_comment(full_markdown_description)
                 else:
                     self.git_provider.publish_description(pr_title, pr_body)
 
                     # publish final update message
                     if (get_settings().pr_description.final_update_message):
                         latest_commit_url = self.git_provider.get_latest_commit_url()
                         if latest_commit_url:
@@ -290,15 +301,15 @@
             self.data.pop('type')
         for key, value in self.data.items():
             markdown_text += f"## **{key}**\n\n"
             markdown_text += f"{value}\n\n"
 
         # Remove the 'PR Title' key from the dictionary
         ai_title = self.data.pop('title', self.vars["title"])
-        if get_settings().pr_description.keep_original_user_title:
+        if (not get_settings().pr_description.generate_ai_title):
             # Assign the original PR title to the 'title' variable
             title = self.vars["title"]
         else:
             # Assign the value of the 'PR Title' key to 'title' variable
             title = ai_title
 
         # Iterate over the remaining dictionary items and append the key and value to 'pr_body' in a markdown format,
@@ -306,27 +317,31 @@
         pr_body, changes_walkthrough = "", ""
         pr_file_changes = []
         for idx, (key, value) in enumerate(self.data.items()):
             if key == 'pr_files':
                 value = self.file_label_dict
             else:
                 key_publish = key.rstrip(':').replace("_", " ").capitalize()
-                pr_body += f"## **{key_publish}**\n"
+                if key_publish== "Type":
+                    key_publish = "PR Type"
+                # elif key_publish == "Description":
+                #     key_publish = "PR Description"
+                pr_body += f"### **{key_publish}**\n"
             if 'walkthrough' in key.lower():
                 if self.git_provider.is_supported("gfm_markdown"):
                     pr_body += "<details> <summary>files:</summary>\n\n"
                 for file in value:
                     filename = file['filename'].replace("'", "`")
                     description = file['changes_in_file']
                     pr_body += f'- `{filename}`: {description}\n'
                 if self.git_provider.is_supported("gfm_markdown"):
                     pr_body += "</details>\n"
             elif 'pr_files' in key.lower():
                 changes_walkthrough, pr_file_changes = self.process_pr_files_prediction(changes_walkthrough, value)
-                changes_walkthrough = f"## **Changes walkthrough**\n{changes_walkthrough}"
+                changes_walkthrough = f"### **Changes walkthrough** 📝\n{changes_walkthrough}"
             else:
                 # if the value is a list, join its items by comma
                 if isinstance(value, list):
                     value = ', '.join(v for v in value)
                 pr_body += f"{value}\n"
             if idx < len(self.data) - 1:
                 pr_body += "\n\n___\n\n"
```

### Comparing `pr-agent-0.2.1/pr_agent/tools/pr_generate_labels.py` & `pr_agent-0.2.2/pr_agent/tools/pr_generate_labels.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/tools/pr_help_message.py` & `pr_agent-0.2.2/pr_agent/tools/pr_help_message.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,86 +14,93 @@
                     "The `Help` tool requires gfm markdown, which is not supported by your code platform.")
                 return
 
             get_logger().info('Getting PR Help Message...')
             relevant_configs = {'pr_help': dict(get_settings().pr_help),
                                 'config': dict(get_settings().config)}
             get_logger().debug("Relevant configs", artifacts=relevant_configs)
-            pr_comment = "## PR Agent Walkthrough\n\n"
-            pr_comment += "🤖 Welcome to the PR Agent, an AI-powered tool for automated pull request analysis, feedback, suggestions and more."""
+            pr_comment = "## PR Agent Walkthrough 🤖\n\n"
+            pr_comment += "Welcome to the PR Agent, an AI-powered tool for automated pull request analysis, feedback, suggestions and more."""
             pr_comment += "\n\nHere is a list of tools you can use to interact with the PR Agent:\n"
             base_path = "https://pr-agent-docs.codium.ai/tools"
 
             tool_names = []
             tool_names.append(f"[DESCRIBE]({base_path}/describe/)")
             tool_names.append(f"[REVIEW]({base_path}/review/)")
             tool_names.append(f"[IMPROVE]({base_path}/improve/)")
-            tool_names.append(f"[ANALYZE]({base_path}/analyze/) 💎")
             tool_names.append(f"[UPDATE CHANGELOG]({base_path}/update_changelog/)")
-            tool_names.append(f"[ADD DOCUMENTATION]({base_path}/documentation/) 💎")
-            tool_names.append(f"[ASK]({base_path}/ask/)")
-            tool_names.append(f"[GENERATE CUSTOM LABELS]({base_path}/custom_labels/)")
+            tool_names.append(f"[ADD DOCS]({base_path}/documentation/) 💎")
             tool_names.append(f"[TEST]({base_path}/test/) 💎")
+            tool_names.append(f"[IMPROVE COMPONENT]({base_path}/improve_component/) 💎")
+            tool_names.append(f"[ANALYZE]({base_path}/analyze/) 💎")
+            tool_names.append(f"[ASK]({base_path}/ask/)")
+            tool_names.append(f"[GENERATE CUSTOM LABELS]({base_path}/custom_labels/) 💎")
             tool_names.append(f"[CI FEEDBACK]({base_path}/ci_feedback/) 💎")
-            tool_names.append(f"[CUSTOM SUGGESTIONS]({base_path}/custom_suggestions/) 💎")
+            tool_names.append(f"[CUSTOM PROMPT]({base_path}/custom_prompt/) 💎")
             tool_names.append(f"[SIMILAR ISSUE]({base_path}/similar_issues/)")
 
             descriptions = []
             descriptions.append("Generates PR description - title, type, summary, code walkthrough and labels")
             descriptions.append("Adjustable feedback about the PR, possible issues, security concerns, review effort and more")
-            descriptions.append("Code suggestions for improving the PR.")
-            descriptions.append("Identifies code components that changed in the PR, and enables to interactively generate tests, docs, and code suggestions for each component.")
-            descriptions.append("Automatically updates the changelog.")
-            descriptions.append("Generates documentation to methods/functions/classes that changed in the PR.")
-            descriptions.append("Answering free-text questions about the PR.")
+            descriptions.append("Code suggestions for improving the PR")
+            descriptions.append("Automatically updates the changelog")
+            descriptions.append("Generates documentation to methods/functions/classes that changed in the PR")
+            descriptions.append("Generates unit tests for a specific component, based on the PR code change")
+            descriptions.append("Code suggestions for a specific component that changed in the PR")
+            descriptions.append("Identifies code components that changed in the PR, and enables to interactively generate tests, docs, and code suggestions for each component")
+            descriptions.append("Answering free-text questions about the PR")
             descriptions.append("Generates custom labels for the PR, based on specific guidelines defined by the user")
-            descriptions.append("Generates unit tests for a specific component, based on the PR code change.")
-            descriptions.append("Generates feedback and analysis for a failed CI job.")
-            descriptions.append("Generates custom suggestions for improving the PR code, based on specific guidelines defined by the user.")
-            descriptions.append("Automatically retrieves and presents similar issues.")
+            descriptions.append("Generates feedback and analysis for a failed CI job")
+            descriptions.append("Generates custom suggestions for improving the PR code, derived only from a specific guidelines prompt defined by the user")
+            descriptions.append("Automatically retrieves and presents similar issues")
 
             commands  =[]
             commands.append("`/describe`")
             commands.append("`/review`")
             commands.append("`/improve`")
-            commands.append("`/analyze`")
             commands.append("`/update_changelog`")
             commands.append("`/add_docs`")
+            commands.append("`/test`")
+            commands.append("`/improve_component`")
+            commands.append("`/analyze`")
             commands.append("`/ask`")
             commands.append("`/generate_labels`")
-            commands.append("`/test`")
             commands.append("`/checks`")
-            commands.append("`/custom_suggestions`")
+            commands.append("`/custom_prompt`")
             commands.append("`/similar_issue`")
 
             checkbox_list = []
             checkbox_list.append(" - [ ] Run <!-- /describe -->")
             checkbox_list.append(" - [ ] Run <!-- /review -->")
             checkbox_list.append(" - [ ] Run <!-- /improve -->")
-            checkbox_list.append(" - [ ] Run <!-- /analyze -->")
             checkbox_list.append(" - [ ] Run <!-- /update_changelog -->")
             checkbox_list.append(" - [ ] Run <!-- /add_docs -->")
+            checkbox_list.append(" - [ ] Run <!-- /test -->")
+            checkbox_list.append(" - [ ] Run <!-- /improve_component -->")
+            checkbox_list.append(" - [ ] Run <!-- /analyze -->")
+            checkbox_list.append("[*]")
+            checkbox_list.append("[*]")
             checkbox_list.append("[*]")
             checkbox_list.append("[*]")
             checkbox_list.append("[*]")
             checkbox_list.append("[*]")
             checkbox_list.append("[*]")
             checkbox_list.append("[*]")
 
-            if isinstance(self.git_provider, GithubProvider):
-                pr_comment += f"<table><tr align='center'><th align='center'>Tool</th><th align='center'>Description</th><th align='center'>Invoke Interactively :gem:</th></tr>"
+            if isinstance(self.git_provider, GithubProvider) and not get_settings().config.get('disable_checkboxes', False):
+                pr_comment += f"<table><tr align='left'><th align='left'>Tool</th><th align='left'>Description</th><th align='left'>Trigger Interactively :gem:</th></tr>"
                 for i in range(len(tool_names)):
-                    pr_comment += f"\n<tr><td align='center'>\n\n<strong>{tool_names[i]}</strong></td>\n<td>{descriptions[i]}</td>\n<td>\n\n{checkbox_list[i]}\n</td></tr>"
+                    pr_comment += f"\n<tr><td align='left'>\n\n<strong>{tool_names[i]}</strong></td>\n<td>{descriptions[i]}</td>\n<td>\n\n{checkbox_list[i]}\n</td></tr>"
                 pr_comment += "</table>\n\n"
                 pr_comment += f"""\n\n(1) Note that each tool be [triggered automatically](https://github.com/Codium-ai/pr-agent/blob/main/Usage.md#github-app-automatic-tools-for-pr-actions) when a new PR is opened, or called manually by [commenting on a PR](https://github.com/Codium-ai/pr-agent/blob/main/Usage.md#online-usage)."""
                 pr_comment += f"""\n\n(2) Tools marked with [*] require additional parameters to be passed. For example, to invoke the `/ask` tool, you need to comment on a PR: `/ask "<question content>"`. See the relevant documentation for each tool for more details."""
             else:
-                pr_comment += f"<table><tr align='center'><th align='center'>Tool</th><th align='left'>Command</th><th align='left'>Description</th></tr>"
+                pr_comment += f"<table><tr align='left'><th align='left'>Tool</th><th align='left'>Command</th><th align='left'>Description</th></tr>"
                 for i in range(len(tool_names)):
-                    pr_comment += f"\n<tr><td align='center'>\n\n<strong>{tool_names[i]}</strong></td><td>{commands[i]}</td><td>{descriptions[i]}</td></tr>"
+                    pr_comment += f"\n<tr><td align='left'>\n\n<strong>{tool_names[i]}</strong></td><td>{commands[i]}</td><td>{descriptions[i]}</td></tr>"
                 pr_comment += "</table>\n\n"
                 pr_comment += f"""\n\nNote that each tool be [invoked automatically](https://pr-agent-docs.codium.ai/usage-guide/automations_and_usage/) when a new PR is opened, or called manually by [commenting on a PR](https://pr-agent-docs.codium.ai/usage-guide/automations_and_usage/#online-usage)."""
             if get_settings().config.publish_output:
                 self.git_provider.publish_comment(pr_comment)
         except Exception as e:
             get_logger().error(f"Error while running PRHelpMessage: {e}")
         return ""
```

### Comparing `pr-agent-0.2.1/pr_agent/tools/pr_information_from_user.py` & `pr_agent-0.2.2/pr_agent/tools/pr_information_from_user.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/tools/pr_line_questions.py` & `pr_agent-0.2.2/pr_agent/tools/pr_line_questions.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/tools/pr_questions.py` & `pr_agent-0.2.2/pr_agent/tools/pr_questions.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from jinja2 import Environment, StrictUndefined
 
 from pr_agent.algo.ai_handlers.base_ai_handler import BaseAiHandler
 from pr_agent.algo.ai_handlers.litellm_ai_handler import LiteLLMAIHandler
 from pr_agent.algo.pr_processing import get_pr_diff, retry_with_fallback_models
 from pr_agent.algo.token_handler import TokenHandler
+from pr_agent.algo.utils import ModelType
 from pr_agent.config_loader import get_settings
 from pr_agent.git_providers import get_git_provider
 from pr_agent.git_providers.git_provider import get_main_pr_language
 from pr_agent.log import get_logger
 from pr_agent.servers.help import HelpMessage
 
 
@@ -52,29 +53,48 @@
     async def run(self):
         get_logger().info(f'Answering a PR question about the PR {self.pr_url} ')
         relevant_configs = {'pr_questions': dict(get_settings().pr_questions),
                             'config': dict(get_settings().config)}
         get_logger().debug("Relevant configs", artifacts=relevant_configs)
         if get_settings().config.publish_output:
             self.git_provider.publish_comment("Preparing answer...", is_temporary=True)
-        await retry_with_fallback_models(self._prepare_prediction)
+
+        # identify image
+        img_path = self.idenfity_image_in_comment()
+        if img_path:
+            get_logger().debug(f"Image path identified", artifact=img_path)
+
+        await retry_with_fallback_models(self._prepare_prediction, model_type=ModelType.TURBO)
 
         pr_comment = self._prepare_pr_answer()
         get_logger().debug(f"PR output", artifact=pr_comment)
 
         if self.git_provider.is_supported("gfm_markdown") and get_settings().pr_questions.enable_help_text:
-            pr_comment += "<hr>\n\n<details> <summary><strong>✨ Ask tool usage guide:</strong></summary><hr> \n\n"
+            pr_comment += "<hr>\n\n<details> <summary><strong>💡 Tool usage guide:</strong></summary><hr> \n\n"
             pr_comment += HelpMessage.get_ask_usage_guide()
             pr_comment += "\n</details>\n"
 
         if get_settings().config.publish_output:
             self.git_provider.publish_comment(pr_comment)
             self.git_provider.remove_initial_comment()
         return ""
 
+    def idenfity_image_in_comment(self):
+        img_path = ''
+        if '![image]' in self.question_str:
+            # assuming structure:
+            # /ask question ...  > ![image](img_path)
+            img_path = self.question_str.split('![image]')[1].strip().strip('()')
+            self.vars['img_path'] = img_path
+        elif 'https://' in self.question_str and ('.png' in self.question_str or 'jpg' in self.question_str): # direct image link
+            # include https:// in the image path
+            img_path = 'https://' + self.question_str.split('https://')[1]
+            self.vars['img_path'] = img_path
+        return img_path
+
     async def _prepare_prediction(self, model: str):
         self.patches_diff = get_pr_diff(self.git_provider, self.token_handler, model)
         if self.patches_diff:
             get_logger().debug(f"PR diff", artifact=self.patches_diff)
             self.prediction = await self._get_prediction(model)
         else:
             get_logger().error(f"Error getting PR diff")
@@ -82,15 +102,21 @@
 
     async def _get_prediction(self, model: str):
         variables = copy.deepcopy(self.vars)
         variables["diff"] = self.patches_diff  # update diff
         environment = Environment(undefined=StrictUndefined)
         system_prompt = environment.from_string(get_settings().pr_questions_prompt.system).render(variables)
         user_prompt = environment.from_string(get_settings().pr_questions_prompt.user).render(variables)
-        response, finish_reason = await self.ai_handler.chat_completion(model=model, temperature=0.2,
-                                                                        system=system_prompt, user=user_prompt)
+        if 'img_path' in variables:
+            img_path = self.vars['img_path']
+            response, finish_reason = await self.ai_handler.chat_completion(model=model, temperature=0.2,
+                                                                            system=system_prompt, user=user_prompt,
+                                                                            img_path=img_path)
+        else:
+            response, finish_reason = await self.ai_handler.chat_completion(model=model, temperature=0.2,
+                                                                            system=system_prompt, user=user_prompt)
         return response
 
     def _prepare_pr_answer(self) -> str:
-        answer_str = f"Question: {self.question_str}\n\n"
-        answer_str += f"Answer:\n{self.prediction.strip()}\n\n"
+        answer_str = f"### **Ask**❓\n{self.question_str}\n\n"
+        answer_str += f"### **Answer:**\n{self.prediction.strip()}\n\n"
         return answer_str
```

### Comparing `pr-agent-0.2.1/pr_agent/tools/pr_reviewer.py` & `pr_agent-0.2.2/pr_agent/tools/pr_reviewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from functools import partial
 from typing import List, Tuple
 from jinja2 import Environment, StrictUndefined
 from pr_agent.algo.ai_handlers.base_ai_handler import BaseAiHandler
 from pr_agent.algo.ai_handlers.litellm_ai_handler import LiteLLMAIHandler
 from pr_agent.algo.pr_processing import get_pr_diff, retry_with_fallback_models
 from pr_agent.algo.token_handler import TokenHandler
-from pr_agent.algo.utils import convert_to_markdown, load_yaml, ModelType
+from pr_agent.algo.utils import convert_to_markdown, github_action_output, load_yaml, ModelType, \
+    show_relevant_configurations
 from pr_agent.config_loader import get_settings
 from pr_agent.git_providers import get_git_provider
 from pr_agent.git_providers.git_provider import IncrementalPR, get_main_pr_language
 from pr_agent.log import get_logger
 from pr_agent.servers.help import HelpMessage
 
 
@@ -120,28 +121,28 @@
                     self.git_provider.publish_comment(f"Incremental Review Skipped\n"
                                     f"No files were changed since the [previous PR Review]({previous_review_url})")
                 return None
 
             if get_settings().config.publish_output:
                 self.git_provider.publish_comment("Preparing review...", is_temporary=True)
 
-            await retry_with_fallback_models(self._prepare_prediction, model_type=ModelType.TURBO)
+            await retry_with_fallback_models(self._prepare_prediction)
             if not self.prediction:
                 self.git_provider.remove_initial_comment()
                 return None
 
             pr_review = self._prepare_pr_review()
             get_logger().debug(f"PR output", artifact=pr_review)
 
             if get_settings().config.publish_output:
                 # publish the review
                 if get_settings().pr_reviewer.persistent_comment and not self.incremental.is_incremental:
                     final_update_message = get_settings().pr_reviewer.final_update_message
                     self.git_provider.publish_persistent_comment(pr_review,
-                                                                 initial_header="## PR Review",
+                                                                 initial_header="## PR Review 🔍",
                                                                  update_header=True,
                                                                  final_update_message=final_update_message, )
                 else:
                     self.git_provider.publish_comment(pr_review)
 
                 self.git_provider.remove_initial_comment()
                 if get_settings().pr_reviewer.inline_code_comments:
@@ -188,14 +189,15 @@
         """
         Prepare the PR review by processing the AI prediction and generating a markdown-formatted text that summarizes
         the feedback.
         """
         data = load_yaml(self.prediction.strip(),
                          keys_fix_yaml=["estimated_effort_to_review_[1-5]:", "security_concerns:", "possible_issues:",
                                         "relevant_file:", "relevant_line:", "suggestion:"])
+        github_action_output(data, 'review')
 
         if 'code_feedback' in data:
             code_feedback = data['code_feedback']
 
             # Filter out code suggestions that can be submitted as inline comments
             if get_settings().pr_reviewer.inline_code_comments:
                 del data['code_feedback']
@@ -229,18 +231,22 @@
             incremental_review_markdown_text = f"Starting from commit {last_commit_url}"
 
         markdown_text = convert_to_markdown(data, self.git_provider.is_supported("gfm_markdown"),
                                             incremental_review_markdown_text)
 
         # Add help text if gfm_markdown is supported
         if self.git_provider.is_supported("gfm_markdown") and get_settings().pr_reviewer.enable_help_text:
-            markdown_text += "<hr>\n\n<details> <summary><strong>✨ Review tool usage guide:</strong></summary><hr> \n\n"
+            markdown_text += "<hr>\n\n<details> <summary><strong>💡 Tool usage guide:</strong></summary><hr> \n\n"
             markdown_text += HelpMessage.get_review_usage_guide()
             markdown_text += "\n</details>\n"
 
+        # Output the relevant configurations if enabled
+        if get_settings().get('config', {}).get('output_relevant_configurations', False):
+            markdown_text += show_relevant_configurations(relevant_section='pr_reviewer')
+
         # Add custom labels from the review prediction (effort, security)
         self.set_review_labels(data)
 
         if markdown_text == None or len(markdown_text) == 0:
             markdown_text = ""
 
         return markdown_text
@@ -353,14 +359,17 @@
                 f"\n* Number of new commits = {num_new_commits} (threshold is {num_commits_threshold})"
                 f"\n* Last seen commit date = {last_seen_commit_date} (threshold is {recent_commits_threshold})"
             )
             return False
         return True
 
     def set_review_labels(self, data):
+        if not get_settings().config.publish_output:
+            return
+
         if (get_settings().pr_reviewer.enable_review_labels_security or
                 get_settings().pr_reviewer.enable_review_labels_effort):
             try:
                 review_labels = []
                 if get_settings().pr_reviewer.enable_review_labels_effort:
                     estimated_effort = data['review']['estimated_effort_to_review_[1-5]']
                     estimated_effort_number = int(estimated_effort.split(',')[0])
```

### Comparing `pr-agent-0.2.1/pr_agent/tools/pr_similar_issue.py` & `pr_agent-0.2.2/pr_agent/tools/pr_similar_issue.py`

 * *Files identical despite different names*

### Comparing `pr-agent-0.2.1/pr_agent/tools/pr_update_changelog.py` & `pr_agent-0.2.2/pr_agent/tools/pr_update_changelog.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from time import sleep
 from typing import Tuple
 from jinja2 import Environment, StrictUndefined
 from pr_agent.algo.ai_handlers.base_ai_handler import BaseAiHandler
 from pr_agent.algo.ai_handlers.litellm_ai_handler import LiteLLMAIHandler
 from pr_agent.algo.pr_processing import get_pr_diff, retry_with_fallback_models
 from pr_agent.algo.token_handler import TokenHandler
-from pr_agent.algo.utils import ModelType
+from pr_agent.algo.utils import ModelType, show_relevant_configurations
 from pr_agent.config_loader import get_settings
 from pr_agent.git_providers import get_git_provider, GithubProvider
 from pr_agent.git_providers.git_provider import get_main_pr_language
 from pr_agent.log import get_logger
 
 CHANGELOG_LINES = 50
 
@@ -70,22 +70,27 @@
 
         if get_settings().config.publish_output:
             self.git_provider.publish_comment("Preparing changelog updates...", is_temporary=True)
 
         await retry_with_fallback_models(self._prepare_prediction, model_type=ModelType.TURBO)
 
         new_file_content, answer = self._prepare_changelog_update()
+
+        # Output the relevant configurations if enabled
+        if get_settings().get('config', {}).get('output_relevant_configurations', False):
+            answer += show_relevant_configurations(relevant_section='pr_update_changelog')
+
         get_logger().debug(f"PR output", artifact=answer)
 
         if get_settings().config.publish_output:
             self.git_provider.remove_initial_comment()
             if self.commit_changelog:
                 self._push_changelog_update(new_file_content, answer)
             else:
-                self.git_provider.publish_comment(f"**Changelog updates:**\n\n{answer}")
+                self.git_provider.publish_comment(f"**Changelog updates:** 🔄\n\n{answer}")
 
     async def _prepare_prediction(self, model: str):
         self.patches_diff = get_pr_diff(self.git_provider, self.token_handler, model)
         if self.patches_diff:
             get_logger().debug(f"PR diff", artifact=self.patches_diff)
             self.prediction = await self._get_prediction(model)
         else:
@@ -137,15 +142,15 @@
                     path="CHANGELOG.md",
                     line=max(2, len(answer.splitlines())),
                     start_line=1,
                 )
                 self.git_provider.pr.create_review(commit=last_commit_id, comments=[d])
         except Exception:
             # we can't create a review for some reason, let's just publish a comment
-            self.git_provider.publish_comment(f"**Changelog updates:**\n\n{answer}")
+            self.git_provider.publish_comment(f"**Changelog updates: 🔄**\n\n{answer}")
 
     def _get_default_changelog(self):
         example_changelog = \
 """
 Example:
 ## <current_date>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pr-agent-0.2.1/pr_agent.egg-info/PKG-INFO` & `pr_agent-0.2.2/pr_agent.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr-agent
-Version: 0.2.1
+Version: 0.2.2
 Summary: CodiumAI PR-Agent aims to help efficiently review and handle pull requests, by providing AI feedbacks and suggestions.
 Author-email: CodiumAI <tal.r@codium.ai>
 Maintainer-email: Tal Ridnik <tal.r@codium.ai>, Ori Kotek <ori.k@codium.ai>, Hussam Lawen <hussam.l@codium.ai>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -231,15 +231,15 @@
 Requires-Dist: openai==1.13.3
 Requires-Dist: pytest==7.4.0
 Requires-Dist: PyGithub==1.59.*
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: python-gitlab==3.15.0
 Requires-Dist: retry==0.9.2
 Requires-Dist: starlette-context==0.3.6
-Requires-Dist: tiktoken==0.5.2
+Requires-Dist: tiktoken==0.7.0
 Requires-Dist: ujson==5.8.0
 Requires-Dist: uvicorn==0.22.0
 Requires-Dist: tenacity==8.2.3
 
 <div align="center">
 
 <div align="center">
@@ -248,111 +248,108 @@
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://codium.ai/images/pr_agent/logo-dark.png" width="330">
   <source media="(prefers-color-scheme: light)" srcset="https://codium.ai/images/pr_agent/logo-light.png" width="330">
   <img src="https://codium.ai/images/pr_agent/logo-light.png" alt="logo" width="330">
 
 </picture>
 <br/>
-Making pull requests less painful with an AI agent
+CodiumAI PR-Agent aims to help efficiently review and handle pull requests, by providing AI feedbacks and suggestions
 </div>
 
 [![GitHub license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/Codium-ai/pr-agent/blob/main/LICENSE)
+[![Static Badge](https://img.shields.io/badge/Chrome-Extension-violet)](https://chromewebstore.google.com/detail/pr-agent-chrome-extension/ephlnjeghhogofkifjloamocljapahnl)
 [![Discord](https://badgen.net/badge/icon/discord?icon=discord&label&color=purple)](https://discord.com/channels/1057273017547378788/1126104260430528613)
 [![Twitter](https://img.shields.io/twitter/follow/codiumai)](https://twitter.com/codiumai)
     <a href="https://github.com/Codium-ai/pr-agent/commits/main">
     <img alt="GitHub" src="https://img.shields.io/github/last-commit/Codium-ai/pr-agent/main?style=for-the-badge" height="20">
     </a>
 </div>
 
+### [Documentation](https://pr-agent-docs.codium.ai/)
+- See the [Installation Guide](https://pr-agent-docs.codium.ai/installation/) for instructions on installing PR-Agent on different platforms.
+
+- See the [Usage Guide](https://pr-agent-docs.codium.ai/usage-guide/) for instructions on running PR-Agent tools via different interfaces, such as CLI, PR Comments, or by automatically triggering them when a new PR is opened.
+
+- See the [Tools Guide](https://pr-agent-docs.codium.ai/tools/) for a detailed description of the different tools, and the available configurations for each tool.
+
+
 ## Table of Contents
 - [News and Updates](#news-and-updates)
 - [Overview](#overview)
 - [Example results](#example-results)
 - [Try it now](#try-it-now)
-- [Installation](#installation)
 - [PR-Agent Pro 💎](#pr-agent-pro-)
 - [How it works](#how-it-works)
 - [Why use PR-Agent?](#why-use-pr-agent)
   
 ## News and Updates
 
-### March 24, 2024
-PR-Agent is now available for easy installation via [pip](https://pr-agent-docs.codium.ai/installation/locally/#using-pip-package).
-
-### March 17, 2024
-- A new feature is now available for the review tool: [`require_can_be_split_review`](https://pr-agent-docs.codium.ai/tools/review/#enabledisable-features). 
-If set to true, the tool will add a section that checks if the PR contains several themes, and can be split into smaller PRs.
+### May 19, 2024
+GPT-4o is now the default fast model ("Turbo"). This model will be used for all commands except `review` and `improve`, which will still use "GPT-4-2024-04-09", since they are harder and would still benefit from the larger model.
 
-<kbd><img src="https://codium.ai/images/pr_agent/multiple_pr_themes.png" width="512"></kbd>
+### May 12, 2024
+Inspired by [AlphaCodium](https://github.com/Codium-ai/AlphaCodium) flow engineering scheme, PR-Agent now performs **self-reflection** on the code suggestions it provides,
+enabling to remove invalid suggestions, and score the valid ones. The suggestions will be presented sorted by their score, enabling to focus on the most important ones first.
 
-### March 10, 2024
-- A new [knowledge-base website](https://pr-agent-docs.codium.ai/) for PR-Agent is now available. It includes detailed information about the different tools, usage guides and more, in an accessible and organized format.
+You can also choose to automatically remove suggestions below a certain importance score threshold, by setting the `pr_code_suggestions.suggestions_score_threshold` [configuration](https://pr-agent-docs.codium.ai/tools/improve/#configuration-options).
 
-### March 8, 2024
+<kbd><img src="https://codium.ai/images/pr_agent/self_reflection1.png" width="512"></kbd>
 
-- A new tool, [Find Similar Code](https://pr-agent-docs.codium.ai/tools/similar_code/) 💎 is now available. 
-<br>This tool retrieves the most similar code components from inside the organization's codebase, or from open-source code:
+<kbd><img src="https://codium.ai/images/pr_agent/self_reflection2.png" width="512"></kbd>
 
-<kbd><a href="https://codium.ai/images/pr_agent/similar_code.mp4"><img src="https://codium.ai/images/pr_agent/similar_code_global2.png" width="512"></a></kbd>
 
-(click on the image to see an instructional video)
+### May 2, 2024
+Check out the new [PR-Agent Chrome Extension](https://chromewebstore.google.com/detail/pr-agent-chrome-extension/ephlnjeghhogofkifjloamocljapahnl) 🚀🚀🚀
 
-### Feb 29, 2024
-- You can now use the repo's [wiki page](https://pr-agent-docs.codium.ai/usage-guide/configuration_options/) to set configurations for PR-Agent 💎
+This toolbar integrates seamlessly with your GitHub environment, allowing you to access PR-Agent tools [directly from the GitHub interface](https://www.youtube.com/watch?v=gT5tli7X4H4).
+You can also easily export your chosen configuration, and use it for the automatic commands.
 
-<kbd><img src="https://codium.ai/images/pr_agent/wiki_configuration.png" width="512"></kbd>
+<kbd><img src="https://codium.ai/images/pr_agent/toolbar1.png" width="512"></kbd>
 
+<kbd><img src="https://codium.ai/images/pr_agent/toolbar2.png" width="512"></kbd>
 
 ## Overview
 <div style="text-align:left;">
 
-CodiumAI PR-Agent aims to help efficiently review and handle pull requests, by providing AI feedbacks and suggestions
-
-- See the [Installation Guide](https://pr-agent-docs.codium.ai/installation/) for instructions on installing and running the tool on different git platforms.
-
-- See the [Usage Guide](https://pr-agent-docs.codium.ai/usage-guide/) for instructions on running the PR-Agent commands via different interfaces, including _CLI_, _online usage_, or by _automatically triggering_ them when a new PR is opened.
-
-- See the [Tools Guide](https://pr-agent-docs.codium.ai/tools/) for a detailed description of the different tools.
-
 Supported commands per platform:
 
-|       |                                                                                                                   | GitHub             | Gitlab             | Bitbucket          | Azure DevOps       |
-|-------|-------------------------------------------------------------------------------------------------------------------|:--------------------:|:--------------------:|:--------------------:|:--------------------:|
-| TOOLS | Review                                                                                                            | ✅ | ✅ | ✅ | ✅ |
-|       | ⮑ Incremental                                                                                                     | ✅ |                    |                    |                    |
+|       |                                                                                                         | GitHub             | Gitlab             | Bitbucket          | Azure DevOps       |
+|-------|---------------------------------------------------------------------------------------------------------|:--------------------:|:--------------------:|:--------------------:|:--------------------:|
+| TOOLS | Review                                                                                                  | ✅ | ✅ | ✅ | ✅ |
+|       | ⮑ Incremental                                                                                           | ✅ |                    |                    |                    |
 |       | ⮑ [SOC2 Compliance](https://pr-agent-docs.codium.ai/tools/review/#soc2-ticket-compliance) 💎            | ✅ | ✅ | ✅ | ✅ |
-|       | Describe                                                                                                          | ✅ | ✅ | ✅ | ✅ |
+|       | Describe                                                                                                | ✅ | ✅ | ✅ | ✅ |
 |       | ⮑ [Inline File Summary](https://pr-agent-docs.codium.ai/tools/describe#inline-file-summary) 💎          | ✅ |                    |                    |                    |
-|       | Improve                                                                                                           | ✅ | ✅ | ✅ | ✅ |
-|       | ⮑ Extended                                                                                                        | ✅ | ✅ | ✅ | ✅ |
-|       | Ask                                                                                                               | ✅ | ✅ | ✅ | ✅ |
+|       | Improve                                                                                                 | ✅ | ✅ | ✅ | ✅ |
+|       | ⮑ Extended                                                                                              | ✅ | ✅ | ✅ | ✅ |
+|       | Ask                                                                                                     | ✅ | ✅ | ✅ | ✅ |
 |       | ⮑ [Ask on code lines](https://pr-agent-docs.codium.ai/tools/ask#ask-lines)                              | ✅ | ✅ |                    |                    |
-|       | [Custom Suggestions](https://pr-agent-docs.codium.ai/tools/custom_suggestions/) 💎                      | ✅ | ✅ | ✅ | ✅ |
+|       | [Custom Prompt](https://pr-agent-docs.codium.ai/tools/custom_prompt/) 💎                                | ✅ | ✅ | ✅ | ✅ |
 |       | [Test](https://pr-agent-docs.codium.ai/tools/test/) 💎                                                  | ✅ | ✅ |                    | ✅ |
-|       | Reflect and Review                                                                                                | ✅ | ✅ | ✅ | ✅ |
-|       | Update CHANGELOG.md                                                                                               | ✅ | ✅ | ✅ | ✅ |
-|       | Find Similar Issue                                                                                                | ✅ |                    |                    |                    |
+|       | Reflect and Review                                                                                      | ✅ | ✅ | ✅ | ✅ |
+|       | Update CHANGELOG.md                                                                                     | ✅ | ✅ | ✅ | ✅ |
+|       | Find Similar Issue                                                                                      | ✅ |                    |                    |                    |
 |       | [Add PR Documentation](https://pr-agent-docs.codium.ai/tools/documentation/) 💎                         | ✅ | ✅ |                   | ✅ |
 |       | [Custom Labels](https://pr-agent-docs.codium.ai/tools/custom_labels/) 💎                                | ✅ | ✅ |                    | ✅ |
 |       | [Analyze](https://pr-agent-docs.codium.ai/tools/analyze/) 💎                                            | ✅ | ✅ |                    | ✅ |
 |       | [CI Feedback](https://pr-agent-docs.codium.ai/tools/ci_feedback/) 💎                                    | ✅ |                    |                    |                    |
 |       | [Similar Code](https://pr-agent-docs.codium.ai/tools/similar_code/) 💎                                  | ✅ |                    |                    |                    |
-|       |                                                                                                                   |                    |                    |                    |                    |
-| USAGE | CLI                                                                                                               | ✅ | ✅ | ✅ | ✅ |
-|       | App / webhook                                                                                                     | ✅ | ✅ | ✅ | ✅ |
-|       | Tagging bot                                                                                                       | ✅ |                    |                    |                    |
-|       | Actions                                                                                                           | ✅ |                    | ✅ |                    |
-|       |                                                                                                                   |                    |                    |                    |                    |
-| CORE  | PR compression                                                                                                    | ✅ | ✅ | ✅ | ✅ |
-|       | Repo language prioritization                                                                                      | ✅ | ✅ | ✅ | ✅ |
-|       | Adaptive and token-aware file patch fitting                                                                       | ✅ | ✅ | ✅ | ✅ |
-|       | Multiple models support                                                                                           | ✅ | ✅ | ✅ | ✅ |
+|       |                                                                                                         |                    |                    |                    |                    |
+| USAGE | CLI                                                                                                     | ✅ | ✅ | ✅ | ✅ |
+|       | App / webhook                                                                                           | ✅ | ✅ | ✅ | ✅ |
+|       | Tagging bot                                                                                             | ✅ |                    |                    |                    |
+|       | Actions                                                                                                 | ✅ |                    | ✅ |                    |
+|       |                                                                                                         |                    |                    |                    |                    |
+| CORE  | PR compression                                                                                          | ✅ | ✅ | ✅ | ✅ |
+|       | Repo language prioritization                                                                            | ✅ | ✅ | ✅ | ✅ |
+|       | Adaptive and token-aware file patch fitting                                                             | ✅ | ✅ | ✅ | ✅ |
+|       | Multiple models support                                                                                 | ✅ | ✅ | ✅ | ✅ |
 |       | [Static code analysis](https://pr-agent-docs.codium.ai/core-abilities/#static-code-analysis) 💎         | ✅ | ✅ | ✅ | ✅ |
 |       | [Global and wiki configurations](https://pr-agent-docs.codium.ai/usage-guide/configuration_options/) 💎 | ✅ | ✅ | ✅ | ✅ |
-|       | [PR interactive actions](https://www.codium.ai/images/pr_agent/pr-actions.mp4) 💎                                 | ✅ |                    |                    |                    |
+|       | [PR interactive actions](https://www.codium.ai/images/pr_agent/pr-actions.mp4) 💎                       | ✅ |                    |                    |                    |
 - 💎 means this feature is available only in [PR-Agent Pro](https://www.codium.ai/pricing/)
 
 [//]: # (- Support for additional git providers is described in [here]&#40;./docs/Full_environments.md&#41;)
 ___
 
 ‣ **Auto Description ([`/describe`](https://pr-agent-docs.codium.ai/tools/describe/))**: Automatically generating PR description - title, type, summary, code walkthrough and labels.
 \
@@ -368,21 +365,21 @@
 \
 ‣ **Add Documentation 💎  ([`/add_docs`](https://pr-agent-docs.codium.ai/tools/documentation/))**: Generates documentation to methods/functions/classes that changed in the PR.
 \
 ‣ **Generate Custom Labels 💎 ([`/generate_labels`](https://pr-agent-docs.codium.ai/tools/custom_labels/))**: Generates custom labels for the PR, based on specific guidelines defined by the user.
 \
 ‣ **Analyze 💎 ([`/analyze`](https://pr-agent-docs.codium.ai/tools/analyze/))**: Identify code components that changed in the PR, and enables to interactively generate tests, docs, and code suggestions for each component.
 \
-‣ **Custom Suggestions 💎 ([`/custom_suggestions`](https://pr-agent-docs.codium.ai/tools/custom_suggestions/))**: Automatically generates custom suggestions for improving the PR code, based on specific guidelines defined by the user.
+‣ **Custom Prompt 💎 ([`/custom_prompt`](https://pr-agent-docs.codium.ai/tools/custom_prompt/))**: Automatically generates custom suggestions for improving the PR code, based on specific guidelines defined by the user.
 \
 ‣ **Generate Tests 💎 ([`/test component_name`](https://pr-agent-docs.codium.ai/tools/test/))**: Generates unit tests for a selected component, based on the PR code changes.
 \
 ‣ **CI Feedback 💎 ([`/checks ci_job`](https://pr-agent-docs.codium.ai/tools/ci_feedback/))**: Automatically generates feedback and analysis for a failed CI job.
 \
-‣ **Similar Code 💎 ([`/find_similar_component`](https://pr-agent-docs.codium.ai/tools/similar_code//))**: Retrieves the most similar code components from inside the organization's codebase, or from open-source code.
+‣ **Similar Code 💎 ([`/find_similar_component`](https://pr-agent-docs.codium.ai/tools/similar_code/))**: Retrieves the most similar code components from inside the organization's codebase, or from open-source code.
 ___
 
 ## Example results
 </div>
 <h4><a href="https://github.com/Codium-ai/pr-agent/pull/530">/describe</a></h4>
 <div align="center">
 <p float="center">
@@ -473,40 +470,55 @@
 
 
 To set up your own PR-Agent, see the [Installation](https://pr-agent-docs.codium.ai/installation/) section below.
 Note that when you set your own PR-Agent or use CodiumAI hosted PR-Agent, there is no need to mention `@CodiumAI-Agent ...`. Instead, directly start with the command, e.g., `/ask ...`.
 
 ---
 
-## Installation
-To use your own version of PR-Agent, you first need to acquire two tokens:
+[//]: # (## Installation)
+
+[//]: # (To use your own version of PR-Agent, you first need to acquire two tokens:)
+
+[//]: # ()
+[//]: # (1. An OpenAI key from [here]&#40;https://platform.openai.com/&#41;, with access to GPT-4.)
 
-1. An OpenAI key from [here](https://platform.openai.com/), with access to GPT-4.
-2. A GitHub personal access token (classic) with the repo scope.
+[//]: # (2. A GitHub personal access token &#40;classic&#41; with the repo scope.)
 
-There are several ways to use PR-Agent:
+[//]: # ()
+[//]: # (There are several ways to use PR-Agent:)
 
-**Locally**
-- [Using pip package](https://pr-agent-docs.codium.ai/installation/locally/#using-pip-package)
-- [Using Docker image](https://pr-agent-docs.codium.ai/installation/locally/#using-docker-image)
-- [Run from source](https://pr-agent-docs.codium.ai/installation/locally/#run-from-source)
+[//]: # ()
+[//]: # (**Locally**)
 
-**GitHub specific methods**
-- [Run as a GitHub Action](https://pr-agent-docs.codium.ai/installation/github/#run-as-a-github-action)
-- [Run as a GitHub App](https://pr-agent-docs.codium.ai/installation/github/#run-as-a-github-app)
+[//]: # (- [Using pip package]&#40;https://pr-agent-docs.codium.ai/installation/locally/#using-pip-package&#41;)
 
-**GitLab specific methods**
-- [Run a GitLab webhook server](https://pr-agent-docs.codium.ai/installation/gitlab/)
+[//]: # (- [Using Docker image]&#40;https://pr-agent-docs.codium.ai/installation/locally/#using-docker-image&#41;)
 
-**BitBucket specific methods**
-- [Run as a Bitbucket Pipeline](https://pr-agent-docs.codium.ai/installation/bitbucket/)
+[//]: # (- [Run from source]&#40;https://pr-agent-docs.codium.ai/installation/locally/#run-from-source&#41;)
+
+[//]: # ()
+[//]: # (**GitHub specific methods**)
+
+[//]: # (- [Run as a GitHub Action]&#40;https://pr-agent-docs.codium.ai/installation/github/#run-as-a-github-action&#41;)
+
+[//]: # (- [Run as a GitHub App]&#40;https://pr-agent-docs.codium.ai/installation/github/#run-as-a-github-app&#41;)
+
+[//]: # ()
+[//]: # (**GitLab specific methods**)
+
+[//]: # (- [Run a GitLab webhook server]&#40;https://pr-agent-docs.codium.ai/installation/gitlab/&#41;)
+
+[//]: # ()
+[//]: # (**BitBucket specific methods**)
+
+[//]: # (- [Run as a Bitbucket Pipeline]&#40;https://pr-agent-docs.codium.ai/installation/bitbucket/&#41;)
 
 ## PR-Agent Pro 💎
 [PR-Agent Pro](https://www.codium.ai/pricing/) is a hosted version of PR-Agent, provided by CodiumAI. It is available for a monthly fee, and provides the following benefits:
-1. **Fully managed** - We take care of everything for you - hosting, models, regular updates, and more. Installation is as simple as signing up and adding the PR-Agent app to your GitHub\BitBucket repo.
+1. **Fully managed** - We take care of everything for you - hosting, models, regular updates, and more. Installation is as simple as signing up and adding the PR-Agent app to your GitHub\GitLab\BitBucket repo.
 2. **Improved privacy** - No data will be stored or used to train models. PR-Agent Pro will employ zero data retention, and will use an OpenAI account with zero data retention.
 3. **Improved support** - PR-Agent Pro users will receive priority support, and will be able to request new features and capabilities.
 4. **Extra features** -In addition to the benefits listed above, PR-Agent Pro will emphasize more customization, and the usage of static code analysis, in addition to LLM logic, to improve results. 
 See [here](https://pr-agent-docs.codium.ai/#pr-agent-pro) for a list of features available in PR-Agent Pro.
 
 
 
@@ -528,19 +540,30 @@
 - Our [PR Compression strategy](https://pr-agent-docs.codium.ai/core-abilities/#pr-compression-strategy)  is a core ability that enables to effectively tackle both short and long PRs.
 - Our JSON prompting strategy enables to have **modular, customizable tools**. For example, the '/review' tool categories can be controlled via the [configuration](pr_agent/settings/configuration.toml) file. Adding additional categories is easy and accessible.
 - We support **multiple git providers** (GitHub, Gitlab, Bitbucket), **multiple ways** to use the tool (CLI, GitHub Action, GitHub App, Docker, ...), and **multiple models** (GPT-4, GPT-3.5, Anthropic, Cohere, Llama2).
 
 
 ## Data privacy
 
-If you host PR-Agent with your OpenAI API key, it is between you and OpenAI. You can read their API data privacy policy here:
+### Self-hosted PR-Agent
+
+- If you host PR-Agent with your OpenAI API key, it is between you and OpenAI. You can read their API data privacy policy here:
 https://openai.com/enterprise-privacy
 
-When using PR-Agent Pro 💎, hosted by CodiumAI, we will not store any of your data, nor will we use it for training.
-You will also benefit from an OpenAI account with zero data retention.
+### CodiumAI-hosted PR-Agent Pro 💎
+
+- When using PR-Agent Pro 💎, hosted by CodiumAI, we will not store any of your data, nor will we use it for training. You will also benefit from an OpenAI account with zero data retention.
+
+- For certain clients, CodiumAI-hosted PR-Agent Pro will use CodiumAI’s proprietary models — if this is the case, you will be notified.
+
+- No passive collection of Code and Pull Requests’ data — PR-Agent will be active only when you invoke it, and it will then extract and analyze only data relevant to the executed command and queried pull request.
+
+### PR-Agent Chrome extension
+
+- The [PR-Agent Chrome extension](https://chromewebstore.google.com/detail/pr-agent-chrome-extension/ephlnjeghhogofkifjloamocljapahnl) serves solely to modify the visual appearance of a GitHub PR screen. It does not transmit any user's repo or pull request code. Code is only sent for processing when a user submits a GitHub comment that activates a PR-Agent tool, in accordance with the standard privacy policy of PR-Agent.
 
 ## Links
 
 [![Join our Discord community](https://raw.githubusercontent.com/Codium-ai/codiumai-vscode-release/main/media/docs/Joincommunity.png)](https://discord.gg/kG35uSHDBc)
 
 - Discord community: https://discord.gg/kG35uSHDBc
 - CodiumAI site: https://codium.ai
```

### Comparing `pr-agent-0.2.1/pr_agent.egg-info/SOURCES.txt` & `pr_agent-0.2.2/pr_agent.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 pr_agent/settings/.secrets_template.toml
 pr_agent/settings/configuration.toml
 pr_agent/settings/custom_labels.toml
 pr_agent/settings/ignore.toml
 pr_agent/settings/language_extensions.toml
 pr_agent/settings/pr_add_docs.toml
 pr_agent/settings/pr_code_suggestions_prompts.toml
+pr_agent/settings/pr_code_suggestions_reflect_prompts.toml
 pr_agent/settings/pr_custom_labels.toml
 pr_agent/settings/pr_description_prompts.toml
 pr_agent/settings/pr_information_from_user_prompts.toml
 pr_agent/settings/pr_line_questions_prompts.toml
 pr_agent/settings/pr_questions_prompts.toml
 pr_agent/settings/pr_reviewer_prompts.toml
 pr_agent/settings/pr_sort_code_suggestions_prompts.toml
```

### Comparing `pr-agent-0.2.1/pyproject.toml` & `pr_agent-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pr-agent"
-version = "0.2.1"
+version = "0.2.2"
 
 authors = [{name= "CodiumAI", email = "tal.r@codium.ai"}]
 
 maintainers = [
   {name = "Tal Ridnik", email = "tal.r@codium.ai"},
   {name = "Ori Kotek", email = "ori.k@codium.ai"},
   {name = "Hussam Lawen", email = "hussam.l@codium.ai"},
```

### Comparing `pr-agent-0.2.1/requirements.txt` & `pr_agent-0.2.2/requirements.txt`

 * *Files 17% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 openai==1.13.3
 pytest==7.4.0
 PyGithub==1.59.*
 PyYAML==6.0.1
 python-gitlab==3.15.0
 retry==0.9.2
 starlette-context==0.3.6
-tiktoken==0.5.2
+tiktoken==0.7.0
 ujson==5.8.0
 uvicorn==0.22.0
 tenacity==8.2.3
 # Uncomment the following lines to enable the 'similar issue' tool
 # pinecone-client
 # pinecone-datasets @ git+https://github.com/mrT23/pinecone-datasets.git@main
 # lancedb==0.5.1
```

