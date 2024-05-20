# Comparing `tmp/contrast_agent-8.1.0.tar.gz` & `tmp/contrast_agent-8.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contrast_agent-8.1.0.tar", last modified: Tue May  7 15:59:08 2024, max compression
+gzip compressed data, was "contrast_agent-8.2.0.tar", last modified: Mon May 20 15:41:07 2024, max compression
```

## Comparing `contrast_agent-8.1.0.tar` & `contrast_agent-8.2.0.tar`

### file list

```diff
@@ -1,788 +1,788 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.642629 contrast_agent-8.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-07 15:59:08.642629 contrast_agent-8.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.510628 contrast_agent-8.1.0/hookspy/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/hookspy/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/hookspy/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.510628 contrast_agent-8.1.0/hookspy/ext/
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/hookspy/ext/hookspy.c
--rwxr-xr-x   0 runner    (1001) docker     (127)      952 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/hookspy/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.498628 contrast_agent-8.1.0/hookspy/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.514628 contrast_agent-8.1.0/hookspy/src/hookspy/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/hookspy/src/hookspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/hookspy/src/hookspy/autogen.py
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/hookspy/src/hookspy/body.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/hookspy/src/hookspy/signatures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/hookspy/src/hookspy/spy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 15:59:08.642629 contrast_agent-8.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.510628 contrast_agent-8.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.514628 contrast_agent-8.1.0/src/contrast/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.518628 contrast_agent-8.1.0/src/contrast/agent/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.518628 contrast_agent-8.1.0/src/contrast/agent/agent_lib/
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/agent_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13355 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/agent_lib/input_tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/agent_lib/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/agent_lib/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    16006 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/agent_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    10536 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.522628 contrast_agent-8.1.0/src/contrast/agent/assess/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/adjusted_span.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/apply_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/assess_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18900 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/contrast_event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.522628 contrast_agent-8.1.0/src/contrast/agent/assess/policy/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/deadzone_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/patches.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/preshift.py
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagation_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagation_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.526628 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/append_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/base_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/center_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/codecs_splat_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/db_write_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/encode_html_splat_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/format_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/join_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/json_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/keep_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/prepend_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/reductive_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/regex_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/replace_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/repr_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator_django.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/slice_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/splat_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/split_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/starlette_safe_path_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/stream_propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/tagger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/source_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    14175 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/source_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11245 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/string_propagation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.530628 contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/default_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/fromstring_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/openai_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/redos_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/ssrf_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/subprocess_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/preflight.py
--rw-r--r--   0 runner    (1001) docker     (127)    14431 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/properties.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.530628 contrast_agent-8.1.0/src/contrast/agent/assess/rules/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/base_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.534628 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/base_config_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/base_django_config_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/base_flask_config_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/django_httponly_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/django_secure_flag_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/django_session_age_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/falcon_secure_flag_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/flask_httponly_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/flask_secure_flag_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/flask_session_age_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/httponly_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/secure_flag_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/session_age_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/dataflow_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/non_dataflow_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.534628 contrast_agent-8.1.0/src/contrast/agent/assess/rules/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/providers/code_parser_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/providers/enable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/providers/hardcoded_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/providers/hardcoded_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/providers/hardcoded_value_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.538628 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/autocomplete_missing_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/base_body_only_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/base_header_only_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/base_response_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/cache_controls_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/clickjacking_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/csp_header_insecure_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/csp_header_missing_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/hsts_header_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/parameter_pollution_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/x_content_type_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/x_xss_protection_disabled_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/xss.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/static_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/trigger_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.538628 contrast_agent-8.1.0/src/contrast/agent/assess/rules/triggers/
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/triggers/httponly_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/triggers/secure_flag_missing_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/triggers/session_rewriting_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/triggers/session_timeout_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/rules/triggers/trigger_config_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/string_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/truncate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/assess/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/disable_reaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/exclusions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/heartbeat_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.538628 contrast_agent-8.1.0/src/contrast/agent/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/app_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)    14101 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/base_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/environ_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.538628 contrast_agent-8.1.0/src/contrast/agent/middlewares/response_wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/response_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/response_wrappers/aiohttp_response_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/response_wrappers/base_response_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.542628 contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/aiohttp_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/bottle_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/django_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/falcon_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/flask_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/pyramid_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/routes_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/starlette_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/patch_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.542628 contrast_agent-8.1.0/src/contrast/agent/policy/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/policy/applicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/policy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/policy/patch_location_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9673 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/policy/patch_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/policy/policy_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/policy/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/policy/rewriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/policy/trigger_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/policy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.542628 contrast_agent-8.1.0/src/contrast/agent/protect/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12667 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/input_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.542628 contrast_agent-8.1.0/src/contrast/agent/protect/policy/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.546628 contrast_agent-8.1.0/src/contrast/agent/protect/rule/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13381 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/base_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/bot_blocker_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/cmdi_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.546628 contrast_agent-8.1.0/src/contrast/agent/protect/rule/deserialization/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/deserialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/deserialization/custom_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/deserialization/pickle_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/deserialization/yaml_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/deserialization_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/http_method_tampering.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/malformed_header.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/mode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.546628 contrast_agent-8.1.0/src/contrast/agent/protect/rule/nosql_injection/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/nosql_injection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12710 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/nosql_injection/mongo_nosql_scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/nosqli_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/path_traversal_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/rules_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/sqli_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/ssrf_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/unsafe_file_upload_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/xss_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.550628 contrast_agent-8.1.0/src/contrast/agent/protect/rule/xxe/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/xxe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/xxe/entity_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/protect/rule/xxe_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/reaction_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/request_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/request_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/server_settings_poll.py
--rw-r--r--   0 runner    (1001) docker     (127)    24894 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/sys_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    12551 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/thread_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/agent/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.550628 contrast_agent-8.1.0/src/contrast/aiohttp/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/aiohttp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/aiohttp/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/aiohttp/sources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.550628 contrast_agent-8.1.0/src/contrast/api/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/api/architecture_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/api/attack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/api/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/api/library.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/api/route_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/api/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/api/trace_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/api/type_checked_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/api/user_input.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.550628 contrast_agent-8.1.0/src/contrast/applies/
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/applies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.550628 contrast_agent-8.1.0/src/contrast/applies/assess/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/applies/assess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/applies/assess/unsafe_code_execution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.550628 contrast_agent-8.1.0/src/contrast/applies/common/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/applies/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.550628 contrast_agent-8.1.0/src/contrast/applies/protect/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/applies/protect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/applies/sqli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.550628 contrast_agent-8.1.0/src/contrast/asgi/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/asgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/asgi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.554628 contrast_agent-8.1.0/src/contrast/assess_extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      167 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/build_funchook.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.554628 contrast_agent-8.1.0/src/contrast/assess_extensions/common/
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/common/cast.c
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/common/format.c
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/common/intern.c
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/common/logging.c
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/common/patches.c
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/common/propagate.c
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/common/repeat.c
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/common/repr.c
--rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/common/scope.c
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/common/streams.c
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/common/subscript.c
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/common/trace.c
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/cs_str.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.558628 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/.git
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/.gitmodules
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.558628 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/.travis/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/.travis/Dockerfile-alpine-test
--rwxr-xr-x   0 runner    (1001) docker     (127)      201 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/.travis/run-test.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)    19118 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/appveyor.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)       34 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/autogen.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)    44826 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/config.guess
--rwxr-xr-x   0 runner    (1001) docker     (127)    35454 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/config.sub
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/configure.ac
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.558628 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/.git
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/MANIFEST
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.558628 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/include/
--rw-r--r--   0 runner    (1001) docker     (127)    19536 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/include/distorm.h
--rw-r--r--   0 runner    (1001) docker     (127)    22674 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/include/mnemonics.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.502628 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.558628 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/linux/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/linux/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.558628 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/mac/
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/mac/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.562628 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/win32/
--rw-r--r--   0 runner    (1001) docker     (127)    12995 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj.filters
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/win32/distorm.sln
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.h
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.rc
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.566628 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/config.h
--rw-r--r--   0 runner    (1001) docker     (127)    25059 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.c
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.h
--rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/distorm.c
--rw-r--r--   0 runner    (1001) docker     (127)    24718 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.c
--rw-r--r--   0 runner    (1001) docker     (127)    17569 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.h
--rw-r--r--   0 runner    (1001) docker     (127)   209309 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/insts.c
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/insts.h
--rw-r--r--   0 runner    (1001) docker     (127)    24295 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/mnemonics.c
--rw-r--r--   0 runner    (1001) docker     (127)    45685 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/operands.c
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/operands.h
--rw-r--r--   0 runner    (1001) docker     (127)    12423 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.c
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.h
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.c
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.h
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.c
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.h
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-07 15:58:58.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/x86defs.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.566628 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/include/
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/include/funchook.h
--rwxr-xr-x   0 runner    (1001) docker     (127)    13998 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/install-sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.570628 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/__strerror.h
--rw-r--r--   0 runner    (1001) docker     (127)    13592 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook.c
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_internal.h
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_io.c
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_io.h
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_syscall.S
--rw-r--r--   0 runner    (1001) docker     (127)    16239 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_unix.c
--rw-r--r--   0 runner    (1001) docker     (127)    14804 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_windows.c
--rw-r--r--   0 runner    (1001) docker     (127)    20159 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_x86.c
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/os_func.c
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/os_func.h
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/os_func_unix.c
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/os_func_windows.c
--rw-r--r--   0 runner    (1001) docker     (127)    43872 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/printf_base.c
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/printf_base.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.570628 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/test/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/test/libfunchook_test.c
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/test/libfunchook_test2.c
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/test/suffix.list
--rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/test/test_main.c
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/test/x86_64_test.S
--rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/test/x86_test.S
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.570628 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/config.h
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook.sln
--rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj.filters
--rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj.filters
--rw-r--r--   0 runner    (1001) docker     (127)     8909 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj.filters
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-07 15:58:57.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook_test_exe.def
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.502628 contrast_agent-8.1.0/src/contrast/assess_extensions/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.502628 contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.574628 contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/assess/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/assess/intern.h
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/assess/logging.h
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/assess/patches.h
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/assess/propagate.h
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/assess/scope.h
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/assess/trace.h
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/assess/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.574628 contrast_agent-8.1.0/src/contrast/assess_extensions/py3/
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py3/patches.c
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py3/str_concat.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.574628 contrast_agent-8.1.0/src/contrast/assess_extensions/py310/
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py310/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py310/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py310/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py310/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py310/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py310/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.574628 contrast_agent-8.1.0/src/contrast/assess_extensions/py311/
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py311/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py311/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py311/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py311/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py311/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py311/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.578628 contrast_agent-8.1.0/src/contrast/assess_extensions/py312/
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py312/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py312/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py312/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py312/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py312/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py312/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.578628 contrast_agent-8.1.0/src/contrast/assess_extensions/py35/
--rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py35/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py35/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py35/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py35/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py35/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py35/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.578628 contrast_agent-8.1.0/src/contrast/assess_extensions/py36/
--rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py36/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py36/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py36/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py36/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py36/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py36/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.578628 contrast_agent-8.1.0/src/contrast/assess_extensions/py37/
--rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py37/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py37/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py37/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py37/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py37/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py37/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.582628 contrast_agent-8.1.0/src/contrast/assess_extensions/py38/
--rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py38/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)     9589 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py38/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py38/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py38/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py38/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py38/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.582628 contrast_agent-8.1.0/src/contrast/assess_extensions/py39/
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py39/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py39/bytes.c
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py39/bytesio.c
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py39/iobase.c
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py39/stringio.c
--rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/assess_extensions/py39/unicode.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.582628 contrast_agent-8.1.0/src/contrast/bottle/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/bottle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/bottle/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.586628 contrast_agent-8.1.0/src/contrast/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/configuration/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/configuration/agent_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/configuration/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/configuration/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/configuration/assess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/configuration/config_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/configuration/config_option.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/configuration/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/configuration/protect.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/configuration/root.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/configuration/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.586628 contrast_agent-8.1.0/src/contrast/django/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/django/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.586628 contrast_agent-8.1.0/src/contrast/django_asgi/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/django_asgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/django_asgi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.586628 contrast_agent-8.1.0/src/contrast/falcon/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/falcon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/falcon/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.586628 contrast_agent-8.1.0/src/contrast/falcon_asgi/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/falcon_asgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/falcon_asgi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.586628 contrast_agent-8.1.0/src/contrast/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/fastapi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.586628 contrast_agent-8.1.0/src/contrast/flask/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/flask/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.586628 contrast_agent-8.1.0/src/contrast/loader/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/loader/sitecustomize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.590628 contrast_agent-8.1.0/src/contrast/patches/
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/cgi_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/concurrent_futures_thread_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/cs_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/cs_str.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.590628 contrast_agent-8.1.0/src/contrast/patches/databases/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/databases/dbapi2.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/databases/mysql_connector_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/databases/psycopg2_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/databases/pymysql_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/databases/sqlalchemy_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/databases/sqlite3_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/encodings_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/exec_and_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.594628 contrast_agent-8.1.0/src/contrast/patches/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/frameworks/bottle_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/frameworks/django_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/frameworks/drf_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/frameworks/falcon_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     5401 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/frameworks/flask_and_quart_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/frameworks/pyramid_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6494 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/frameworks/starlette_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/genshi_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9370 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/import_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/lxml_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.594628 contrast_agent-8.1.0/src/contrast/patches/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/middleware/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/middleware/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/middleware/django.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/middleware/mod_wsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/pathlib_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/re_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/str_new.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/sys_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/threading_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/urllib_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/patches/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.594628 contrast_agent-8.1.0/src/contrast/policy/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/deadzones.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.598628 contrast_agent-8.1.0/src/contrast/policy/propagators/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/propagators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/propagators/codecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/propagators/encodings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/propagators/frameworks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/propagators/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/propagators/re.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/propagators/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/propagators/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.598628 contrast_agent-8.1.0/src/contrast/policy/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/sources/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/sources/cgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/sources/django.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/sources/falcon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/sources/flask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/sources/quart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/sources/webob.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.602628 contrast_agent-8.1.0/src/contrast/policy/triggers/
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/cmd_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/httponly.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/nosql_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/path_traversal.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/prompt_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/redos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/reflected_xss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/secure_flag_missing.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/session_rewriting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/session_timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/sql_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/ssrf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/trust_boundary_violation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/unsafe_code_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/untrusted_deserialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/unvalidated_redirect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/xpath_injection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/policy/triggers/xxe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.602628 contrast_agent-8.1.0/src/contrast/pyramid/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/pyramid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/pyramid/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.602628 contrast_agent-8.1.0/src/contrast/quart/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/quart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/quart/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.602628 contrast_agent-8.1.0/src/contrast/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/activity_masker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/reporting_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/request_audit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.606628 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/_traces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/agent_startup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/application_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/application_inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/application_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/base_ts_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/effective_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/library_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/observed_route.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/preflight.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/server_activity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.606628 contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/application_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/ng_application_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/ng_server_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/protect_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/server_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.606628 contrast_agent-8.1.0/src/contrast/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/scripts/fix_interpreter_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/scripts/propagator_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/scripts/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/scripts/validate_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.610628 contrast_agent-8.1.0/src/contrast/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.614628 contrast_agent-8.1.0/src/contrast/utils/assess/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/assess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/assess/duck_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.614628 contrast_agent-8.1.0/src/contrast/utils/assess/formatting/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/assess/formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/assess/formatting/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/assess/formatting/tokenize_cformat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/assess/formatting/tokenize_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     6671 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/assess/stream_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/assess/tag_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/assess/tracking_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/base64_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/configuration_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/context_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/deprecated_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/digest_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/environ.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.614628 contrast_agent-8.1.0/src/contrast/utils/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/exceptions/deprecation_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/exceptions/wrong_django_middleware_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/exceptions/wsgi_compliance_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/ignored_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.614628 contrast_agent-8.1.0/src/contrast/utils/library_reader/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/library_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/library_reader/library_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/library_reader/patched_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/library_reader/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/locale.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.614628 contrast_agent-8.1.0/src/contrast/utils/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/loggers/structlog.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/module_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/object_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9573 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/patch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/pattern_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/safe_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/stack_trace_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/stdlib_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/string_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 15:59:08.000000 contrast_agent-8.1.0/src/contrast/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.614628 contrast_agent-8.1.0/src/contrast/wsgi/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/wsgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast/wsgi/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.638629 contrast_agent-8.1.0/src/contrast_agent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    32206 2024-05-07 15:59:08.000000 contrast_agent-8.1.0/src/contrast_agent.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.614628 contrast_agent-8.1.0/src/contrast_rewriter/
--rw-r--r--   0 runner    (1001) docker     (127)    15340 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_rewriter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.618628 contrast_agent-8.1.0/src/contrast_vendor/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/.clang-format
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.618628 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    34323 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_functools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.618628 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/compat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/compat/py39.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/diagnose.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.618628 contrast_agent-8.1.0/src/contrast_vendor/isort/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.622628 contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/all.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py27.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py310.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py311.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py312.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py36.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py37.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py38.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py39.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.622628 contrast_agent-8.1.0/src/contrast_vendor/ported_cpython_code/
--rw-r--r--   0 runner    (1001) docker     (127)    12769 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ported_cpython_code/PYTHON_SOFTWARE_FOUNDATION_LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ported_cpython_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ported_cpython_code/import_functionality.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.510628 contrast_agent-8.1.0/src/contrast_vendor/ruamel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.630628 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/anchor.py
--rw-r--r--   0 runner    (1001) docker     (127)    37673 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/composer.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/configobjwalker.py
--rw-r--r--   0 runner    (1001) docker     (127)    70392 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/cyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/dumper.py
--rw-r--r--   0 runner    (1001) docker     (127)    67960 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/emitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8807 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    59457 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    36019 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    44497 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/representer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15209 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/scalarbool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/scalarfloat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/scalarint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/scalarstring.py
--rw-r--r--   0 runner    (1001) docker     (127)    87945 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.634628 contrast_agent-8.1.0/src/contrast_vendor/structlog/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/LICENSE-APACHE
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/LICENSE-MIT
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13882 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/_frames.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/_greenlets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/_log_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/_native.py
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/contextvars.py
--rw-r--r--   0 runner    (1001) docker     (127)    23428 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    27977 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/processors.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    37555 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/stdlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9206 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/threadlocal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/tracebacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/twisted.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/structlog/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/vendor-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.638629 contrast_agent-8.1.0/src/contrast_vendor/webob/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   210210 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/acceptparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/byterange.py
--rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/cachecontrol.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    32879 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/datetime_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/dec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/etag.py
--rw-r--r--   0 runner    (1001) docker     (127)    38268 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/exc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/license.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13961 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/multidict.py
--rw-r--r--   0 runner    (1001) docker     (127)    59159 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/request.py
--rw-r--r--   0 runner    (1001) docker     (127)    55423 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/static.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/webob/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.638629 contrast_agent-8.1.0/src/contrast_vendor/wrapt/
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/wrapt/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/wrapt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/wrapt/__wrapt__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/wrapt/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)    21333 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/wrapt/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/wrapt/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/wrapt/patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/wrapt/weakrefs.py
--rw-r--r--   0 runner    (1001) docker     (127)    27137 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/wrapt/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.638629 contrast_agent-8.1.0/src/contrast_vendor/zipp/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/zipp/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/zipp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:59:08.638629 contrast_agent-8.1.0/src/contrast_vendor/zipp/compat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/zipp/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/zipp/compat/py310.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-07 15:58:55.000000 contrast_agent-8.1.0/src/contrast_vendor/zipp/glob.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.623546 contrast_agent-8.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-20 15:41:07.623546 contrast_agent-8.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.495546 contrast_agent-8.2.0/hookspy/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/hookspy/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/hookspy/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.495546 contrast_agent-8.2.0/hookspy/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/hookspy/ext/hookspy.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)      952 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/hookspy/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.479546 contrast_agent-8.2.0/hookspy/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.495546 contrast_agent-8.2.0/hookspy/src/hookspy/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/hookspy/src/hookspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/hookspy/src/hookspy/autogen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/hookspy/src/hookspy/body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/hookspy/src/hookspy/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/hookspy/src/hookspy/spy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 15:41:07.623546 contrast_agent-8.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.491546 contrast_agent-8.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.495546 contrast_agent-8.2.0/src/contrast/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.499546 contrast_agent-8.2.0/src/contrast/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.503546 contrast_agent-8.2.0/src/contrast/agent/agent_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/agent_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13355 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/agent_lib/input_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/agent_lib/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/agent_lib/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16054 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/agent_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10536 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.503546 contrast_agent-8.2.0/src/contrast/agent/assess/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/adjusted_span.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/apply_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/assess_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18900 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/contrast_event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.507546 contrast_agent-8.2.0/src/contrast/agent/assess/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/deadzone_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/preshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagation_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagation_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.511546 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/append_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/base_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/center_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/codecs_splat_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/db_write_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/encode_html_splat_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/format_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/join_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/json_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/keep_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/prepend_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/reductive_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/regex_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/replace_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/repr_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator_django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/slice_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/splat_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/split_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/starlette_safe_path_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/stream_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/tagger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/source_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14175 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/source_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11245 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/string_propagation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.511546 contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/default_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/fromstring_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/openai_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/redos_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/ssrf_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/subprocess_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/preflight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14431 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.511546 contrast_agent-8.2.0/src/contrast/agent/assess/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/base_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.515546 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/base_config_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/base_django_config_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/base_flask_config_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/django_httponly_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/django_secure_flag_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/django_session_age_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/falcon_secure_flag_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/flask_httponly_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/flask_secure_flag_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/flask_session_age_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/httponly_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/secure_flag_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/session_age_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/dataflow_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/non_dataflow_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.515546 contrast_agent-8.2.0/src/contrast/agent/assess/rules/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/providers/code_parser_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/providers/enable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/providers/hardcoded_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/providers/hardcoded_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/providers/hardcoded_value_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.519546 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/autocomplete_missing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/base_body_only_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/base_header_only_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/base_response_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/cache_controls_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/clickjacking_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/csp_header_insecure_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/csp_header_missing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/hsts_header_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/parameter_pollution_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/x_content_type_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/x_xss_protection_disabled_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/xss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/static_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/trigger_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.519546 contrast_agent-8.2.0/src/contrast/agent/assess/rules/triggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/triggers/httponly_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/triggers/secure_flag_missing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/triggers/session_rewriting_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/triggers/session_timeout_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/rules/triggers/trigger_config_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/string_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/truncate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/assess/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/disable_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/exclusions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/heartbeat_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.523546 contrast_agent-8.2.0/src/contrast/agent/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/app_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14326 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/base_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/environ_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.523546 contrast_agent-8.2.0/src/contrast/agent/middlewares/response_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/response_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/response_wrappers/aiohttp_response_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/response_wrappers/base_response_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.523546 contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/aiohttp_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/bottle_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/django_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/falcon_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/flask_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/pyramid_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/routes_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/starlette_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/patch_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.527546 contrast_agent-8.2.0/src/contrast/agent/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/policy/applicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/policy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/policy/patch_location_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9673 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/policy/patch_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/policy/policy_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/policy/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/policy/rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/policy/trigger_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/policy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.527546 contrast_agent-8.2.0/src/contrast/agent/protect/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12667 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/input_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.527546 contrast_agent-8.2.0/src/contrast/agent/protect/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.527546 contrast_agent-8.2.0/src/contrast/agent/protect/rule/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13381 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/base_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/bot_blocker_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/cmdi_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.531546 contrast_agent-8.2.0/src/contrast/agent/protect/rule/deserialization/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/deserialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/deserialization/custom_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/deserialization/pickle_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/deserialization/yaml_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/deserialization_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/http_method_tampering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/malformed_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/mode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.531546 contrast_agent-8.2.0/src/contrast/agent/protect/rule/nosql_injection/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/nosql_injection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12710 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/nosql_injection/mongo_nosql_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/nosqli_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/path_traversal_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/rules_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/sqli_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/ssrf_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/unsafe_file_upload_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/xss_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.531546 contrast_agent-8.2.0/src/contrast/agent/protect/rule/xxe/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/xxe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/xxe/entity_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/protect/rule/xxe_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/reaction_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/request_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/request_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/server_settings_poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24894 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/sys_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12551 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/thread_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/agent/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.531546 contrast_agent-8.2.0/src/contrast/aiohttp/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/aiohttp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/aiohttp/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/aiohttp/sources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.531546 contrast_agent-8.2.0/src/contrast/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/api/architecture_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/api/attack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/api/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/api/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/api/route_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/api/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/api/trace_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/api/type_checked_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/api/user_input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.531546 contrast_agent-8.2.0/src/contrast/applies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/applies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.535546 contrast_agent-8.2.0/src/contrast/applies/assess/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/applies/assess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/applies/assess/unsafe_code_execution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.535546 contrast_agent-8.2.0/src/contrast/applies/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/applies/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.535546 contrast_agent-8.2.0/src/contrast/applies/protect/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/applies/protect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/applies/sqli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.535546 contrast_agent-8.2.0/src/contrast/asgi/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/asgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/asgi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.535546 contrast_agent-8.2.0/src/contrast/assess_extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      167 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/build_funchook.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.535546 contrast_agent-8.2.0/src/contrast/assess_extensions/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/common/cast.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/common/format.c
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/common/intern.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/common/logging.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/common/patches.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/common/propagate.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/common/repeat.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/common/repr.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/common/scope.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/common/streams.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/common/subscript.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/common/trace.c
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/cs_str.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.539546 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/.git
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/.gitmodules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.539546 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/.travis/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/.travis/Dockerfile-alpine-test
+-rwxr-xr-x   0 runner    (1001) docker     (127)      201 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/.travis/run-test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    19118 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/appveyor.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       34 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/autogen.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44826 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/config.guess
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35454 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/config.sub
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/configure.ac
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.543546 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/.git
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/MANIFEST
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.543546 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/include/
+-rw-r--r--   0 runner    (1001) docker     (127)    19536 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/include/distorm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22674 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/include/mnemonics.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.483546 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.543546 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/linux/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.543546 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/mac/
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/mac/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.543546 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/win32/
+-rw-r--r--   0 runner    (1001) docker     (127)    12995 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj.filters
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/win32/distorm.sln
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.547546 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/config.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25059 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/distorm.c
+-rw-r--r--   0 runner    (1001) docker     (127)    24718 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.c
+-rw-r--r--   0 runner    (1001) docker     (127)    17569 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.h
+-rw-r--r--   0 runner    (1001) docker     (127)   209309 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/insts.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/insts.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24295 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/mnemonics.c
+-rw-r--r--   0 runner    (1001) docker     (127)    45685 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/operands.c
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/operands.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12423 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.h
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-20 15:40:54.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/x86defs.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.547546 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/include/funchook.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13998 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/install-sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.551546 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/__strerror.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13592 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_internal.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_io.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_io.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_syscall.S
+-rw-r--r--   0 runner    (1001) docker     (127)    16239 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_unix.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14804 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_windows.c
+-rw-r--r--   0 runner    (1001) docker     (127)    20159 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_x86.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/os_func.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/os_func.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/os_func_unix.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/os_func_windows.c
+-rw-r--r--   0 runner    (1001) docker     (127)    43872 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/printf_base.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/printf_base.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.551546 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/test/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/test/libfunchook_test.c
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/test/libfunchook_test2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/test/suffix.list
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/test/test_main.c
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/test/x86_64_test.S
+-rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/test/x86_test.S
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.555546 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/config.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook.sln
+-rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj.filters
+-rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj.filters
+-rw-r--r--   0 runner    (1001) docker     (127)     8909 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj.filters
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-20 15:40:53.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook_test_exe.def
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.487546 contrast_agent-8.2.0/src/contrast/assess_extensions/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.487546 contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.555546 contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/assess/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/assess/intern.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/assess/logging.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/assess/patches.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/assess/propagate.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/assess/scope.h
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/assess/trace.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/assess/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.555546 contrast_agent-8.2.0/src/contrast/assess_extensions/py3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py3/patches.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py3/str_concat.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.555546 contrast_agent-8.2.0/src/contrast/assess_extensions/py310/
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py310/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py310/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py310/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py310/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py310/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py310/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.559546 contrast_agent-8.2.0/src/contrast/assess_extensions/py311/
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py311/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py311/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py311/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py311/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py311/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py311/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.559546 contrast_agent-8.2.0/src/contrast/assess_extensions/py312/
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py312/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py312/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py312/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py312/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py312/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py312/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.559546 contrast_agent-8.2.0/src/contrast/assess_extensions/py35/
+-rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py35/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py35/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py35/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py35/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py35/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py35/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.559546 contrast_agent-8.2.0/src/contrast/assess_extensions/py36/
+-rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py36/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py36/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py36/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py36/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py36/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py36/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.563546 contrast_agent-8.2.0/src/contrast/assess_extensions/py37/
+-rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py37/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py37/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py37/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py37/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py37/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py37/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.563546 contrast_agent-8.2.0/src/contrast/assess_extensions/py38/
+-rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py38/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9589 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py38/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py38/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py38/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py38/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py38/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.563546 contrast_agent-8.2.0/src/contrast/assess_extensions/py39/
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py39/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py39/bytes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py39/bytesio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py39/iobase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py39/stringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/assess_extensions/py39/unicode.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.563546 contrast_agent-8.2.0/src/contrast/bottle/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/bottle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/bottle/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.567546 contrast_agent-8.2.0/src/contrast/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/configuration/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/configuration/agent_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/configuration/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/configuration/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/configuration/assess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/configuration/config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/configuration/config_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/configuration/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/configuration/protect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/configuration/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/configuration/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.567546 contrast_agent-8.2.0/src/contrast/django/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/django/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.567546 contrast_agent-8.2.0/src/contrast/django_asgi/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/django_asgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/django_asgi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.567546 contrast_agent-8.2.0/src/contrast/falcon/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/falcon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/falcon/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.567546 contrast_agent-8.2.0/src/contrast/falcon_asgi/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/falcon_asgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/falcon_asgi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.567546 contrast_agent-8.2.0/src/contrast/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/fastapi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.567546 contrast_agent-8.2.0/src/contrast/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/flask/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.567546 contrast_agent-8.2.0/src/contrast/loader/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/loader/sitecustomize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.571546 contrast_agent-8.2.0/src/contrast/patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/cgi_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/concurrent_futures_thread_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/cs_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/cs_str.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.575546 contrast_agent-8.2.0/src/contrast/patches/databases/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/databases/dbapi2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/databases/mysql_connector_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/databases/psycopg2_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/databases/pymysql_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/databases/sqlalchemy_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/databases/sqlite3_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/encodings_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/exec_and_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.575546 contrast_agent-8.2.0/src/contrast/patches/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/frameworks/bottle_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/frameworks/django_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/frameworks/drf_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/frameworks/falcon_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/frameworks/flask_and_quart_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/frameworks/pyramid_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/frameworks/starlette_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/genshi_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9370 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/import_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/lxml_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.575546 contrast_agent-8.2.0/src/contrast/patches/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/middleware/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/middleware/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6613 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/middleware/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/middleware/mod_wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/pathlib_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/re_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/str_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/sys_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/threading_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/urllib_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/patches/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.575546 contrast_agent-8.2.0/src/contrast/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/deadzones.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.579546 contrast_agent-8.2.0/src/contrast/policy/propagators/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/propagators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/propagators/codecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/propagators/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/propagators/frameworks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/propagators/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/propagators/re.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/propagators/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/propagators/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.579546 contrast_agent-8.2.0/src/contrast/policy/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/sources/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/sources/cgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/sources/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/sources/falcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/sources/flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/sources/quart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/sources/webob.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.583546 contrast_agent-8.2.0/src/contrast/policy/triggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/cmd_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/httponly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/nosql_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/path_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/prompt_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/redos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/reflected_xss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/secure_flag_missing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/session_rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/session_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/sql_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/ssrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/trust_boundary_violation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/unsafe_code_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/untrusted_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/unvalidated_redirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/xpath_injection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/policy/triggers/xxe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.583546 contrast_agent-8.2.0/src/contrast/pyramid/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/pyramid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/pyramid/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.583546 contrast_agent-8.2.0/src/contrast/quart/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/quart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/quart/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.583546 contrast_agent-8.2.0/src/contrast/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/activity_masker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/reporting_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/request_audit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.587546 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/_traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/agent_startup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/application_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/application_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/application_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/base_ts_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/effective_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/library_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/observed_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/preflight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/server_activity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.587546 contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/application_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/ng_application_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/ng_server_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/protect_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/server_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.591546 contrast_agent-8.2.0/src/contrast/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/scripts/fix_interpreter_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/scripts/propagator_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/scripts/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/scripts/validate_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.595546 contrast_agent-8.2.0/src/contrast/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.595546 contrast_agent-8.2.0/src/contrast/utils/assess/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/assess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/assess/duck_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.595546 contrast_agent-8.2.0/src/contrast/utils/assess/formatting/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/assess/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/assess/formatting/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/assess/formatting/tokenize_cformat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/assess/formatting/tokenize_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6671 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/assess/stream_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/assess/tag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/assess/tracking_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/base64_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/configuration_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/context_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/deprecated_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/digest_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/environ.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.595546 contrast_agent-8.2.0/src/contrast/utils/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/exceptions/deprecation_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/exceptions/wrong_django_middleware_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/exceptions/wsgi_compliance_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/ignored_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.595546 contrast_agent-8.2.0/src/contrast/utils/library_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/library_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/library_reader/library_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/library_reader/patched_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/library_reader/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/locale.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.599546 contrast_agent-8.2.0/src/contrast/utils/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/loggers/structlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/module_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/object_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/patch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/pattern_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/safe_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/stack_trace_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/stdlib_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 15:41:07.000000 contrast_agent-8.2.0/src/contrast/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.599546 contrast_agent-8.2.0/src/contrast/wsgi/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/wsgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast/wsgi/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.623546 contrast_agent-8.2.0/src/contrast_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    32206 2024-05-20 15:41:07.000000 contrast_agent-8.2.0/src/contrast_agent.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.599546 contrast_agent-8.2.0/src/contrast_rewriter/
+-rw-r--r--   0 runner    (1001) docker     (127)    15340 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_rewriter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.599546 contrast_agent-8.2.0/src/contrast_vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.599546 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    34323 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_functools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.599546 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/compat/py39.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/diagnose.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.599546 contrast_agent-8.2.0/src/contrast_vendor/isort/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.603546 contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py27.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py311.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py312.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py36.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py37.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py39.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.603546 contrast_agent-8.2.0/src/contrast_vendor/ported_cpython_code/
+-rw-r--r--   0 runner    (1001) docker     (127)    12769 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ported_cpython_code/PYTHON_SOFTWARE_FOUNDATION_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ported_cpython_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ported_cpython_code/import_functionality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.491546 contrast_agent-8.2.0/src/contrast_vendor/ruamel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.611546 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/anchor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37673 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/configobjwalker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70392 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/cyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67960 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8807 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59457 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36019 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44497 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/representer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15209 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/scalarbool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/scalarfloat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/scalarint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/scalarstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87945 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.615546 contrast_agent-8.2.0/src/contrast_vendor/structlog/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/LICENSE-APACHE
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/LICENSE-MIT
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13882 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/_frames.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/_greenlets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/_log_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/_native.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/contextvars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23428 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27977 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    37555 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9206 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/threadlocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/tracebacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/twisted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/structlog/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/vendor-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.619546 contrast_agent-8.2.0/src/contrast_vendor/webob/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   210210 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/acceptparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/byterange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/cachecontrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32879 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/datetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/dec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/etag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38268 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/exc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/license.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13961 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/multidict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59159 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55423 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/webob/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.619546 contrast_agent-8.2.0/src/contrast_vendor/wrapt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/wrapt/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/wrapt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/wrapt/__wrapt__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/wrapt/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21333 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/wrapt/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/wrapt/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/wrapt/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/wrapt/weakrefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27137 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/wrapt/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.623546 contrast_agent-8.2.0/src/contrast_vendor/zipp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/zipp/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/zipp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:41:07.623546 contrast_agent-8.2.0/src/contrast_vendor/zipp/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/zipp/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/zipp/compat/py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-20 15:40:51.000000 contrast_agent-8.2.0/src/contrast_vendor/zipp/glob.py
```

### Comparing `contrast_agent-8.1.0/LICENSE.txt` & `contrast_agent-8.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/MANIFEST.in` & `contrast_agent-8.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/PKG-INFO` & `contrast_agent-8.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contrast-agent
-Version: 8.1.0
+Version: 8.2.0
 Summary: Contrast Security's agent for Python web frameworks
 Author-email: "Contrast Security, Inc." <python@contrastsecurity.com>
 License: Copyright: 2024 Contrast Security, Inc
         Contact: support@contrastsecurity.com
         License: Commercial
         
         NOTICE: This Software and the patented inventions embodied within may only be used as
@@ -24,15 +24,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: <3.13,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests<3,>=2.4.2
-Requires-Dist: contrast-agent-lib~=0.5.4
+Requires-Dist: contrast-agent-lib~=0.7.0
 
 # Contrast Python Agent
 
 
 The Contrast Python Agent provides interactive vulnerability discovery and
 runtime protection for web applications. The agent is a WSGI-, ASGI-, and
 framework-specific middleware that's compatible with the most popular web
```

### Comparing `contrast_agent-8.1.0/hookspy/README.md` & `contrast_agent-8.2.0/hookspy/README.md`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/hookspy/ext/hookspy.c` & `contrast_agent-8.2.0/hookspy/ext/hookspy.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/hookspy/setup.py` & `contrast_agent-8.2.0/hookspy/setup.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/hookspy/src/hookspy/autogen.py` & `contrast_agent-8.2.0/hookspy/src/hookspy/autogen.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/hookspy/src/hookspy/body.py` & `contrast_agent-8.2.0/hookspy/src/hookspy/body.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/hookspy/src/hookspy/signatures.py` & `contrast_agent-8.2.0/hookspy/src/hookspy/signatures.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/hookspy/src/hookspy/spy.py` & `contrast_agent-8.2.0/hookspy/src/hookspy/spy.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/pyproject.toml` & `contrast_agent-8.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,19 @@
     "Development Status :: 5 - Production/Stable",
     # Audience
     "Intended Audience :: Developers",
     # License; commercial
     # supported languages
     "Programming Language :: Python :: 3",
 ]
-dynamic = ["version", "dependencies"]
+dynamic = ["version"]
+dependencies = [
+    "requests>=2.4.2,<3",
+    "contrast-agent-lib~=0.7.0",
+]
 description = "Contrast Security's agent for Python web frameworks"
 keywords = ["security development"]
 license = { file = "LICENSE.txt" }
 requires-python = ">=3.8,<3.13"
 readme = "README.md"
 [project.urls]
 "Contrast" = "https://www.contrastsecurity.com"
@@ -119,10 +123,11 @@
   # turn off YAMLLoadWarning about unsafe yaml since we have to test for unsafe use
   "ignore:.*calling yaml.load.*as the default Loader is unsafe.*",
   # we still test these functions
   "ignore:.*'flask.helpers.safe_join' is deprecated.*",
   "ignore:.*'utils.escape' is deprecated.*",
   "ignore:.*unicode_internal codec has been deprecated.*",
   "ignore:.*'cgi' is deprecated.*",
+  "ignore::contrast.utils.exceptions.deprecation_warning.ContrastDeprecationWarning",
 ]
 asyncio_mode = "auto"
 addopts = "--ignore=tests/performance"
```

### Comparing `contrast_agent-8.1.0/setup.py` & `contrast_agent-8.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,14 @@
 from setuptools import Extension, setup
 from setuptools.command.build_ext import build_ext
 from setuptools.command.install_lib import install_lib
 
 root_dir = path.abspath(path.dirname(__file__))
 
 
-AGENT_LIB_REQUIREMENT = "~=0.5.4"
-
-
 def read(*parts):
     with open(path.join(root_dir, *parts), encoding="utf-8") as f:
         return f.read()
 
 
 def is_arm():
     machine = platform.machine()
@@ -157,14 +154,10 @@
         if funchook_temp is not None:
             dest_dir = path.join(self.install_dir, extension_path)
             self.copy_file(funchook_temp, dest_dir)
             rmtree(tempdir)
 
 
 setup(
-    install_requires=[
-        "requests>=2.4.2,<3",
-        f"contrast-agent-lib{AGENT_LIB_REQUIREMENT}",
-    ],
     cmdclass=dict(build_ext=ContrastBuildExt, install_lib=ContrastInstallLib),
     ext_modules=extensions,
 )
```

### Comparing `contrast_agent-8.1.0/src/contrast/__init__.py` & `contrast_agent-8.2.0/src/contrast/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/agent_lib/__init__.py` & `contrast_agent-8.2.0/src/contrast/agent/agent_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/agent_lib/input_tracing.py` & `contrast_agent-8.2.0/src/contrast/agent/agent_lib/input_tracing.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/agent_lib/main.py` & `contrast_agent-8.2.0/src/contrast/agent/agent_lib/main.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/agent_state.py` & `contrast_agent-8.2.0/src/contrast/agent/agent_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,14 @@
 
 NO_EXPLICIT_MIDDLEWARE_WARNING = f"""
 Explicit middleware configuration is generally no longer necessary when using
 the `contrast-python-run` command.
 {SHARED_WARNING_MESSAGE}
 """
 
-
 NO_SPECIFIC_MIDDLEWARE_WARNING = """
 Using framework-specific middleware is no longer recommended for {}.
 Use contrast.{}.ContrastMiddleware instead.
 """
 
 PROTECT_MISMATCH_MESSAGE = (
     "Protect enabled in local config but disabled in Contrast UI. It is running."
@@ -91,15 +90,15 @@
 class module(Namespace):
     init_lock: threading.Lock = threading.Lock()
     is_initialized = False
     id: Optional[int] = None
     settings: Optional[Settings] = None
     reporting_client: Optional[_ReportingClient] = None
     library_reader: Optional[LibraryReader] = None
-    routes: Dict[str, Route] = {}
+    discovered_routes: Dict[str, Route] = {}
     first_request: bool = True
 
     automatic_middleware: ContextVar = ContextVar("automatic_middleware", default=False)
 
     deprecated_middleware: Optional[Tuple[str, bool]] = None
 
     # NOTE: these field can be set prior to initialization
@@ -137,19 +136,20 @@
         installed_webserver=settings.server,
         cwd=AGENT_CURR_WORKING_DIR,
         executable=sys.executable,
         platform=platform_str,
         default_encoding=DEFAULT_ENCODING,
     )
 
-    # TODO: PYT-3116 uncomment with deprecation of py38
-    # if sys.version_info[:2] == (3, 8):
-    #     logger.warn(
-    #         "Support for Python 3.8 is deprecated and will be removed in a future release"
-    #     )
+    # py38: remove
+    if sys.version_info[:2] == (3, 8):
+        _log_and_warn(
+            "Contrast Security support for Python 3.8 is deprecated and will be removed"
+            " in October 2024"
+        )
 
 
 def _warn_for_misleading_config(settings: Settings):
     protect_option = settings.config.get("protect.enable")
     protect_enabled = protect_option.value()
     if protect_enabled and not protect_option.ui_value:
         logger.warning(PROTECT_MISMATCH_MESSAGE)
@@ -238,20 +238,20 @@
     return module.is_initialized
 
 
 def get_settings():
     return module.settings
 
 
-def get_routes() -> Dict[str, Route]:
-    return module.routes
+def get_discovered_routes() -> Dict[str, Route]:
+    return module.discovered_routes
 
 
-def update_routes(new_routes: Dict[str, Route]):
-    module.routes.update(new_routes)
+def update_discovered_routes(new_routes: Dict[str, Route]) -> None:
+    module.discovered_routes.update(new_routes)
 
 
 def is_first_request():
     return module.first_request
 
 
 def set_first_request(val: bool):
```

### Comparing `contrast_agent-8.1.0/src/contrast/agent/asgi.py` & `contrast_agent-8.2.0/src/contrast/agent/asgi.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/adjusted_span.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/adjusted_span.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/apply_trigger.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/apply_trigger.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/contrast_event.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/contrast_event.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/analysis.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/analysis.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/deadzone_node.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/deadzone_node.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/patches.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/patches.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/preshift.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/preshift.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagation_node.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagation_node.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagation_policy.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagation_policy.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/__init__.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/append_propagator.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/append_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/base_propagator.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/base_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/db_write_propagator.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/db_write_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/encode_html_splat_propagator.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/encode_html_splat_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/format_propagator.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/format_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/join_propagator.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/join_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/json_propagator.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/json_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/prepend_propagator.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/prepend_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/reductive_propagator.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/reductive_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/regex_propagator.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/regex_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/replace_propagator.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/replace_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/repr_propagator.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/repr_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator_django.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/safe_join_propagator_django.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/slice_propagator.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/slice_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/splat_propagator.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/splat_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/split_propagator.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/split_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/starlette_safe_path_propagator.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/starlette_safe_path_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/propagators/stream_propagator.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/propagators/stream_propagator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/source_node.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/source_node.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/source_policy.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/source_policy.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/string_propagation.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/string_propagation.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/default_action.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/default_action.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/fromstring_action.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/fromstring_action.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/openai_action.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/openai_action.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/redos_action.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/redos_action.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/ssrf_action.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/ssrf_action.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_actions/subprocess_action.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_actions/subprocess_action.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/policy/trigger_policy.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/policy/trigger_policy.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/preflight.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/preflight.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,24 +22,24 @@
            for path parameters. typically this involves a regex to abstract
            numeric or UUID path segments, but is not well defined. ideally,
            this case will phase out as route coverage expands, so the
            definition does not need to be consistent across agents so long
            as it is consistent within them.
         3. Raw uri
     """
-    route = context.current_route
+    route = context.observed_route
     if route is not None and route.signature:
         return route.signature
 
     normalized_uri = context.request.get_normalized_uri()
     return normalized_uri or context.request.path_qs
 
 
 def _get_verb_for_hash(context):
-    route = context.current_route
+    route = context.observed_route
     if route is not None and route.verb:
         return route.verb
 
     return context.request.method
 
 
 @fail_loudly("Failed to update preflight hashes")
```

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/properties.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/properties.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/base_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/base_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/base_config_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/base_config_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/base_django_config_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/base_django_config_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/base_flask_config_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/base_flask_config_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/falcon_secure_flag_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/falcon_secure_flag_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/secure_flag_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/secure_flag_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/config/session_age_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/config/session_age_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/dataflow_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/dataflow_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/non_dataflow_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/non_dataflow_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/providers/code_parser_mixin.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/providers/code_parser_mixin.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/providers/enable.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/providers/enable.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/providers/hardcoded_key.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/providers/hardcoded_key.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/providers/hardcoded_password.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/providers/hardcoded_password.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/providers/hardcoded_value_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/providers/hardcoded_value_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/analyze.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/analyze.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/autocomplete_missing_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/autocomplete_missing_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/base_body_only_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/base_body_only_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/base_header_only_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/base_header_only_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/base_response_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/base_response_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/cache_controls_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/cache_controls_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/clickjacking_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/clickjacking_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/csp_header_insecure_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/csp_header_insecure_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/csp_header_missing_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/csp_header_missing_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/hsts_header_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/hsts_header_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/parameter_pollution_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/parameter_pollution_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/x_content_type_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/x_content_type_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/x_xss_protection_disabled_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/x_xss_protection_disabled_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/response/xss.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/response/xss.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/static_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/static_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/trigger_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/trigger_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/triggers/httponly_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/triggers/httponly_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/triggers/secure_flag_missing_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/triggers/secure_flag_missing_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/triggers/session_rewriting_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/triggers/session_rewriting_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/triggers/session_timeout_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/triggers/session_timeout_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/rules/triggers/trigger_config_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/rules/triggers/trigger_config_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/sampling.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/sampling.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/string_tracker.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/string_tracker.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/tag.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/tag.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/truncate.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/truncate.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/assess/utils.py` & `contrast_agent-8.2.0/src/contrast/agent/assess/utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/disable_reaction.py` & `contrast_agent-8.2.0/src/contrast/agent/disable_reaction.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/events.py` & `contrast_agent-8.2.0/src/contrast/agent/events.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/exceptions.py` & `contrast_agent-8.2.0/src/contrast/agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/exclusions.py` & `contrast_agent-8.2.0/src/contrast/agent/exclusions.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/framework.py` & `contrast_agent-8.2.0/src/contrast/agent/framework.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/heartbeat_thread.py` & `contrast_agent-8.2.0/src/contrast/agent/heartbeat_thread.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/metrics.py` & `contrast_agent-8.2.0/src/contrast/agent/metrics.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/middlewares/app_finder.py` & `contrast_agent-8.2.0/src/contrast/agent/middlewares/app_finder.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/middlewares/base_middleware.py` & `contrast_agent-8.2.0/src/contrast/agent/middlewares/base_middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from contrast.agent.assess.rules.response.analyze import analyze_response_rules
 from contrast.agent.assess.preflight import update_preflight_hashes
 from contrast.agent.middlewares.route_coverage.routes_mixin import RoutesMixin
 from contrast.agent.middlewares.response_wrappers.base_response_wrapper import (
     BaseResponseWrapper,
 )
 from contrast.api.attack import ProtectResponse
+from contrast.reporting.activity_masker import ActivityMasker
 from contrast.utils.decorators import cached_property
 from contrast.utils.loggers.logger import (
     setup_basic_agent_logger,
 )
 from contrast.reporting import get_reporting_client
 from contrast.utils.decorators import fail_loudly, fail_quietly
 from contrast.utils import timer
@@ -222,35 +223,35 @@
         ]
 
         if (
             self.settings.is_assess_enabled()
             and context.findings is not None
             and len(context.findings) > 0
         ):
+            # Masking can be expensive for large requests, so we only do it if
+            # we're sending a message that requires masking, such as findings (here)
+            # or application activity (for Protect attack samples).
+            #
+            # In the future, we'd like to move masking to within Request.reportable_format .
+            ActivityMasker().mask_sensitive_data(context.request)
             messages.append(
                 teamserver_messages.Preflight(context.findings, context.request)
             )
 
         # Per the spec, we do not report an observed route if the route signature or URL is empty.
-        # Also, we don't report 404s. (SUP-5369)
+        # Also, we don't report on a subset of error response codes. (PYT-3306)
         if (
             self.settings.is_assess_enabled()
             and context.response is not None
-            and context.response.status_code != 404
+            and context.response.status_code not in (403, 404, 405, 501)
             and context.observed_route.signature
             and context.observed_route.url
         ):
             messages.append(teamserver_messages.ObservedRoute(context.observed_route))
 
-        # ApplicationUpdate message only sent at first request once we have routes
-        if agent_state.is_first_request() and self.settings.is_inventory_enabled():
-            messages.append(
-                teamserver_messages.ApplicationInventory(agent_state.get_routes())
-            )
-
         # Not every request will have a new dependency loaded, so we can skip sending empty messages.
         if context.observed_library_usage is not None:
             messages.append(context.observed_library_usage)
 
         return messages
 
     @fail_loudly("Failed to run prefilter.")
```

### Comparing `contrast_agent-8.1.0/src/contrast/agent/middlewares/environ_tracker.py` & `contrast_agent-8.2.0/src/contrast/agent/middlewares/environ_tracker.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/middlewares/response_wrappers/aiohttp_response_wrapper.py` & `contrast_agent-8.2.0/src/contrast/agent/middlewares/response_wrappers/aiohttp_response_wrapper.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/middlewares/response_wrappers/base_response_wrapper.py` & `contrast_agent-8.2.0/src/contrast/agent/middlewares/response_wrappers/base_response_wrapper.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/aiohttp_routes.py` & `contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/aiohttp_routes.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,10 +33,11 @@
             )
             method_type = resource.method
             key = build_key(route_id, method_type)
             routes[key] = Route(
                 verb=method_type,
                 url=get_normalized_uri(_route_attr),
                 route=route,
+                framework="AIOHTTP",
             )
 
     return routes
```

### Comparing `contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/bottle_routes.py` & `contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/bottle_routes.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,9 +25,10 @@
 
         for method_type in DEFAULT_ROUTE_METHODS:
             key = build_key(route_id, method_type)
             routes[key] = Route(
                 verb=method_type,
                 url=get_normalized_uri(str(rule.rule)),
                 route=route,
+                framework="Bottle",
             )
     return routes
```

### Comparing `contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/django_routes.py` & `contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/django_routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
+from typing import Dict
+
 import ast
 import textwrap
 import functools
 
 from collections import deque
 from copy import copy
 from importlib import import_module
@@ -125,19 +127,22 @@
     route = build_django_route(pattern_or_resolver, method_arg_names)
 
     route_id = str(id(pattern_or_resolver.callback))
 
     key = build_key(route_id, method_type)
 
     routes[key] = Route(
-        verb=method_type, url=create_url(pattern_or_resolver), route=route
+        verb=method_type,
+        url=create_url(pattern_or_resolver),
+        route=route,
+        framework="Django",
     )
 
 
-def create_routes(urlpatterns):
+def create_routes(urlpatterns) -> Dict[str, Route]:
     from django.urls.resolvers import (
         URLPattern as RegexURLPattern,
         URLResolver as RegexURLResolver,
     )
 
     routes = {}
 
@@ -152,41 +157,41 @@
         elif isinstance(url_pattern, RegexURLPattern):
             method_types, method_arg_names = get_method_info(url_pattern)
             for method_type in method_types:
                 create_one_route(routes, method_type, method_arg_names, url_pattern)
     return routes
 
 
-def create_django_routes():
+def create_django_routes() -> Dict[str, Route]:
     """
     Grabs all URL's from the root settings and searches for possible required_method decorators
 
     In Django there is no implicit declaration of GET or POST. Often times decorators are used to fix this.
 
     Returns a dict of key = id, value = api.Route.
     """
 
     from django.conf import settings
 
     if not settings.ROOT_URLCONF:
         logger.info("Application does not define settings.ROOT_URLCONF")
         logger.debug("Skipping enumeration of urlpatterns")
-        return None
+        return {}
 
     try:
         root_urlconf = import_module(settings.ROOT_URLCONF)
     except Exception as exception:
         logger.debug("Failed to import ROOT_URLCONF: %s", exception)
-        return None
+        return {}
 
     try:
         urlpatterns = root_urlconf.urlpatterns or []
     except Exception as exception:
         logger.debug("Failed to get urlpatterns: %s", exception)
-        return None
+        return {}
 
     url_patterns = copy(urlpatterns)
     return create_routes(url_patterns)
 
 
 def _function_loc(func):
     """Return the function's module and name"""
```

### Comparing `contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/falcon_routes.py` & `contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/falcon_routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
             route = build_falcon_route(view_func, endpoint_cls)
 
             route_id = build_key(str(id(view_func)), method)
             routes[route_id] = Route(
                 verb=method,
                 url=get_normalized_uri(str(path)),
                 route=route,
+                framework="Falcon",
             )
 
 
 def get_view_method(cls_instance, request_method):
     """
     Falcon defines views like this
     ```
```

### Comparing `contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/flask_routes.py` & `contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/flask_routes.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 
         for method_type in methods:
             key = build_key(route_id, method_type)
             routes[key] = Route(
                 verb=method_type,
                 url=get_normalized_uri(str(rule)),
                 route=route,
+                # Safety check to not directly echo classnames to TeamServer without validation
+                framework=("Quart" if type(app).__name__ == "Quart" else "Flask"),
             )
 
     return routes
 
 
 def get_view_func_for_request(request, app):
     """
```

### Comparing `contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/pyramid_routes.py` & `contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/pyramid_routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,17 @@
 
             methods = pyramid_route.predicates or DEFAULT_ROUTE_METHODS
 
             for method_type in methods:
                 key = build_key(route_id, method_type)
 
                 url = get_normalized_uri(pyramid_route.path)
-                routes[key] = Route(verb=method_type, url=url, route=route)
+                routes[key] = Route(
+                    verb=method_type, url=url, route=route, framework="Pyramid"
+                )
         else:
             logger.debug("Unable to add %s to route coverage.", pyramid_route.path)
 
     return routes
 
 
 def build_pyramid_route(pyramid_route_name, view_func):
```

### Comparing `contrast_agent-8.1.0/src/contrast/agent/middlewares/route_coverage/starlette_routes.py` & `contrast_agent-8.2.0/src/contrast/agent/middlewares/route_coverage/starlette_routes.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,10 +35,11 @@
 
         for method_type in methods:
             key = build_key(route_id, method_type)
             routes[key] = Route(
                 verb=method_type,
                 url=get_normalized_uri(str(app_route.name)),
                 route=route,
+                framework="Starlette",
             )
 
     return routes
```

### Comparing `contrast_agent-8.1.0/src/contrast/agent/patch_controller.py` & `contrast_agent-8.2.0/src/contrast/agent/patch_controller.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/policy/applicator.py` & `contrast_agent-8.2.0/src/contrast/agent/policy/applicator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/policy/constants.py` & `contrast_agent-8.2.0/src/contrast/agent/policy/constants.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/policy/patch_location_policy.py` & `contrast_agent-8.2.0/src/contrast/agent/policy/patch_location_policy.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/policy/patch_manager.py` & `contrast_agent-8.2.0/src/contrast/agent/policy/patch_manager.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/policy/policy_node.py` & `contrast_agent-8.2.0/src/contrast/agent/policy/policy_node.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/policy/registry.py` & `contrast_agent-8.2.0/src/contrast/agent/policy/registry.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/policy/rewriter.py` & `contrast_agent-8.2.0/src/contrast/agent/policy/rewriter.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/policy/trigger_node.py` & `contrast_agent-8.2.0/src/contrast/agent/policy/trigger_node.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/policy/utils.py` & `contrast_agent-8.2.0/src/contrast/agent/policy/utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/protect/input_analysis.py` & `contrast_agent-8.2.0/src/contrast/agent/protect/input_analysis.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/protect/policy/__init__.py` & `contrast_agent-8.2.0/src/contrast/agent/protect/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/protect/rule/base_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/protect/rule/base_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/protect/rule/cmdi_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/protect/rule/cmdi_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/protect/rule/deserialization/custom_searcher.py` & `contrast_agent-8.2.0/src/contrast/agent/protect/rule/deserialization/custom_searcher.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/protect/rule/deserialization/pickle_searcher.py` & `contrast_agent-8.2.0/src/contrast/agent/protect/rule/deserialization/pickle_searcher.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/protect/rule/deserialization/yaml_searcher.py` & `contrast_agent-8.2.0/src/contrast/agent/protect/rule/deserialization/yaml_searcher.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/protect/rule/deserialization_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/protect/rule/deserialization_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/protect/rule/http_method_tampering.py` & `contrast_agent-8.2.0/src/contrast/agent/protect/rule/http_method_tampering.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/protect/rule/nosql_injection/mongo_nosql_scanner.py` & `contrast_agent-8.2.0/src/contrast/agent/protect/rule/nosql_injection/mongo_nosql_scanner.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/protect/rule/nosqli_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/protect/rule/nosqli_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/protect/rule/path_traversal_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/protect/rule/path_traversal_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/protect/rule/rules_builder.py` & `contrast_agent-8.2.0/src/contrast/agent/protect/rule/rules_builder.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/protect/rule/sqli_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/protect/rule/sqli_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/protect/rule/ssrf_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/protect/rule/ssrf_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/protect/rule/xss_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/protect/rule/xss_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/protect/rule/xxe/entity_wrapper.py` & `contrast_agent-8.2.0/src/contrast/agent/protect/rule/xxe/entity_wrapper.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/protect/rule/xxe_rule.py` & `contrast_agent-8.2.0/src/contrast/agent/protect/rule/xxe_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/reaction_processor.py` & `contrast_agent-8.2.0/src/contrast/agent/reaction_processor.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/request.py` & `contrast_agent-8.2.0/src/contrast/agent/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,27 +24,28 @@
         super().__init__(environ)
 
         self._document_type = None
         self._normalized_uri = None
         self._url_parameters = None
         self._multipart_headers = None
 
-        # Typically, empty fields used only when masking is needed for reporting
+        # These fields are set by an ActivityMasker and will be used for reporting.
+        self._masked = False
         self._masked_body = None
         self._masked_cookies = None
         self._masked_headers = None
         self._masked_params = None
         self._masked_query_string = None
         self._parsed_http = None
 
         self.timestamp_ms = now_ms()
 
     @property
     def reportable_format(self):
-
+        assert self._masked, "Request must be masked before reporting"
         return {
             "body": truncate(ensure_string(self._reportable_body), length=4096),
             # the WSGI environ supports only one value per request header. However
             # the server decides to handle multiple headers, we're guaranteed to
             # have only unique keys in request.request_headers (since we iterate
             # over webob's EnvironHeaders). Thus, each value list here is length-1.
             "headers": {
```

### Comparing `contrast_agent-8.1.0/src/contrast/agent/request_context.py` & `contrast_agent-8.2.0/src/contrast/agent/request_context.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
+from typing import Optional, Callable
+
 from contrast.agent import scope
 
 from contrast.agent.request import Request
 from contrast.agent.settings import Settings
 from contrast.api.route_coverage import Route
 from contrast_vendor import structlog as logging
 from contrast.utils.digest_utils import Digest
@@ -37,18 +39,16 @@
         # For assess: store findings made during a request to report at the end
         self.findings = []
 
         self.user_input_analysis = []
         self.response = None
         self.do_not_track = False
 
-        self.view_func = None
-        self.view_func_str = None
-        # to be populated with a Route instance
-        self.current_route = None
+        self.view_func: Optional[Callable] = None
+        self.view_func_str: Optional[str] = None
 
         self.observed_route = Route("", "", "")
         self.database_info = []
         self.source_count = 0
         self.propagation_count = 0
 
         self.max_sources_logged = False
@@ -98,15 +98,15 @@
             self.max_sources_logged = True
 
         return threshold_reached
 
     @property
     def stop_propagation(self):
         """
-        Compare `source_count` to `max_propagation_events` config option
+        Compare `propagation_count` to `max_propagation_events` config option
         :return: true if propagation_count within this request is equal to or
                  greater than configured threshold for propagation
         """
         if self.max_propagators_logged:
             return True
 
         threshold_reached = self.propagation_count >= Settings().max_propagation
```

### Comparing `contrast_agent-8.1.0/src/contrast/agent/request_state.py` & `contrast_agent-8.2.0/src/contrast/agent/request_state.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/runner.py` & `contrast_agent-8.2.0/src/contrast/agent/runner.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/scope.py` & `contrast_agent-8.2.0/src/contrast/agent/scope.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/server_settings_poll.py` & `contrast_agent-8.2.0/src/contrast/agent/server_settings_poll.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/settings.py` & `contrast_agent-8.2.0/src/contrast/agent/settings.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/sys_monitoring.py` & `contrast_agent-8.2.0/src/contrast/agent/sys_monitoring.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/telemetry.py` & `contrast_agent-8.2.0/src/contrast/agent/telemetry.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/thread_watcher.py` & `contrast_agent-8.2.0/src/contrast/agent/thread_watcher.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/agent/validator.py` & `contrast_agent-8.2.0/src/contrast/agent/validator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/aiohttp/middleware.py` & `contrast_agent-8.2.0/src/contrast/aiohttp/middleware.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,15 @@
 from aiohttp.web_urldispatcher import DynamicResource
 
 from contrast.aiohttp import sources
 from contrast.agent import scope, request_state, agent_state
 from contrast.agent.middlewares.route_coverage.aiohttp_routes import (
     create_aiohttp_routes,
 )
-from contrast.agent.middlewares.route_coverage.common import (
-    build_route,
-    log_discovered_routes,
-)
+from contrast.agent.middlewares.route_coverage import common
 from contrast.agent.policy.trigger_node import TriggerNode
 from contrast_vendor import structlog as logging
 from contrast.utils.decorators import cached_property
 from contrast.agent.middlewares.base_middleware import (
     BaseMiddleware,
     log_request_start_and_end,
 )
@@ -100,29 +97,25 @@
         with scope.contrast_scope():
             return await handler(request)
 
     @fail_quietly()
     def do_aiohttp_first_request_analysis(self) -> None:
         if not agent_state.is_first_request():
             return
-        discovered_routes = create_aiohttp_routes(self.app)
-        agent_state.update_routes(discovered_routes)
-        log_discovered_routes("aiohttp", discovered_routes.values())
+
+        common.handle_route_discovery("aiohttp", create_aiohttp_routes, (self.app,))
 
     @fail_quietly()
     def do_aiohttp_route_observation(self, context, request) -> None:
         view_func = self.get_aiohttp_view_func(request)
         if view_func is None:
             logger.debug("unable to get view function for aiohttp route observation")
             return
 
-        context.view_func = view_func
-        context.view_func_str = build_route(
-            context.request.get_normalized_uri(), context.view_func
-        )
+        context.view_func_str = common.build_route(view_func.__name__, view_func)
         logger.debug("Observed aiohttp route: %s", context.view_func_str)
 
     @fail_quietly("Unable to get view func")
     def get_aiohttp_view_func(self, request):
         """
         This intentionally does not override get_view_func. We're generally making route
         coverage more framework-specific; this minimizes shared machinery between
```

### Comparing `contrast_agent-8.1.0/src/contrast/aiohttp/sources.py` & `contrast_agent-8.2.0/src/contrast/aiohttp/sources.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/api/architecture_component.py` & `contrast_agent-8.2.0/src/contrast/api/architecture_component.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/api/attack.py` & `contrast_agent-8.2.0/src/contrast/api/attack.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/api/finding.py` & `contrast_agent-8.2.0/src/contrast/api/finding.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/api/library.py` & `contrast_agent-8.2.0/src/contrast/api/library.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/api/route_coverage.py` & `contrast_agent-8.2.0/src/contrast/api/route_coverage.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,26 +6,31 @@
 
 
 class Route:
     """
     Route object used for various TS messages
     """
 
-    def __init__(self, verb, url, route):
+    def __init__(self, verb, url, route, framework=None):
         self.verb = verb or "GET"
         self.url = url or "/"
         self.signature = route or ""
         self.sources = []
+        self.framework = framework
+
+    def __repr__(self):
+        return f"<Route({self.verb!r}, {self.url!r}, {self.signature!r}, {self.framework!r})>"
 
     def to_json_inventory(self):
-        """json representation used in v1.0 ApplicationInventory.routes"""
+        """json representation used in v1.1 ApplicationInventory.routes"""
         return {
             "signature": self.signature,
             "verb": self.verb,
             "url": self.url,
+            "framework": self.framework,
         }
 
     def to_json_traces(self):
         """json representation used in ng Traces.routes"""
         return {
             # "The number of times this route was observed; must be more than 0"
             "count": 1,
```

### Comparing `contrast_agent-8.1.0/src/contrast/api/trace_event.py` & `contrast_agent-8.2.0/src/contrast/api/trace_event.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/api/type_checked_property.py` & `contrast_agent-8.2.0/src/contrast/api/type_checked_property.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/api/user_input.py` & `contrast_agent-8.2.0/src/contrast/api/user_input.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/applies/__init__.py` & `contrast_agent-8.2.0/src/contrast/applies/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/applies/assess/unsafe_code_execution.py` & `contrast_agent-8.2.0/src/contrast/applies/assess/unsafe_code_execution.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/applies/sqli.py` & `contrast_agent-8.2.0/src/contrast/applies/sqli.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/asgi/middleware.py` & `contrast_agent-8.2.0/src/contrast/asgi/middleware.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/__init__.py` & `contrast_agent-8.2.0/src/contrast/assess_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/common/cast.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/common/cast.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/common/format.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/common/format.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/common/logging.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/common/logging.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/common/patches.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/common/patches.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/common/propagate.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/common/propagate.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/common/repeat.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/common/repeat.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/common/repr.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/common/repr.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/common/scope.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/common/scope.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/common/streams.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/common/streams.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/common/subscript.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/common/subscript.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/common/trace.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/common/trace.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/cs_str.pyi` & `contrast_agent-8.2.0/src/contrast/assess_extensions/cs_str.pyi`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/.travis.yml` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/.travis.yml`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/LICENSE` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/Makefile.in` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/Makefile.in`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/README.md` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/README.md`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/appveyor.yml` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/appveyor.yml`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/config.guess` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/config.guess`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/config.sub` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/config.sub`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/configure.ac` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/configure.ac`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/COPYING` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/COPYING`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/README.md` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/README.md`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/include/distorm.h` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/include/distorm.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/include/mnemonics.h` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/include/mnemonics.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/linux/Makefile` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/linux/Makefile`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/mac/Makefile` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/mac/Makefile`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj.filters` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/win32/cdistorm.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/win32/distorm.sln` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/win32/distorm.sln`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.rc` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/make/win32/resource.rc`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/setup.py` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/setup.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/config.h` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/config.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.h` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/decoder.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/distorm.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/distorm.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.h` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/instructions.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/insts.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/insts.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/insts.h` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/insts.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/mnemonics.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/mnemonics.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/operands.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/operands.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/operands.h` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/operands.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.h` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/prefix.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.h` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/textdefs.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.h` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/wstring.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/distorm/src/x86defs.h` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/distorm/src/x86defs.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/include/funchook.h` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/include/funchook.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/install-sh` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/install-sh`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/Makefile.in` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/Makefile.in`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/__strerror.h` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/__strerror.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_internal.h` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_internal.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_io.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_io.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_io.h` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_io.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_syscall.S` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_syscall.S`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_unix.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_unix.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_windows.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_windows.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/funchook_x86.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/funchook_x86.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/os_func.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/os_func.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/os_func.h` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/os_func.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/os_func_unix.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/os_func_unix.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/os_func_windows.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/os_func_windows.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/printf_base.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/printf_base.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/src/printf_base.h` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/src/printf_base.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/test/Makefile.in` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/test/Makefile.in`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/test/suffix.list` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/test/suffix.list`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/test/test_main.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/test/test_main.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/test/x86_test.S` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/test/x86_test.S`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook.sln` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook.sln`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj.filters` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj.filters` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook_test.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj.filters` & `contrast_agent-8.2.0/src/contrast/assess_extensions/funchook/win32/funchook_test_dll.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/assess/logging.h` & `contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/assess/logging.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/assess/patches.h` & `contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/assess/patches.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/assess/propagate.h` & `contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/assess/propagate.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/assess/scope.h` & `contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/assess/scope.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/include/contrast/assess/utils.h` & `contrast_agent-8.2.0/src/contrast/assess_extensions/include/contrast/assess/utils.h`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py3/patches.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py3/patches.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py3/str_concat.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py3/str_concat.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py310/bytearray.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py310/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py310/bytes.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py310/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py310/bytesio.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py310/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py310/iobase.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py310/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py310/stringio.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py310/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py310/unicode.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py310/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py311/bytearray.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py311/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py311/bytes.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py311/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py311/bytesio.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py311/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py311/iobase.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py311/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py311/stringio.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py311/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py311/unicode.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py311/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py312/bytearray.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py312/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py312/bytes.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py312/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py312/bytesio.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py312/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py312/iobase.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py312/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py312/stringio.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py312/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py312/unicode.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py312/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py35/bytearray.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py35/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py35/bytes.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py35/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py35/bytesio.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py35/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py35/iobase.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py35/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py35/stringio.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py35/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py35/unicode.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py35/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py36/bytearray.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py36/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py36/bytes.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py36/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py36/bytesio.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py36/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py36/iobase.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py36/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py36/stringio.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py36/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py36/unicode.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py36/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py37/bytearray.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py37/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py37/bytes.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py37/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py37/bytesio.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py37/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py37/iobase.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py37/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py37/stringio.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py37/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py37/unicode.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py37/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py38/bytearray.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py38/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py38/bytes.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py38/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py38/bytesio.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py38/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py38/iobase.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py38/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py38/stringio.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py38/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py38/unicode.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py38/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py39/bytearray.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py39/bytearray.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py39/bytes.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py39/bytes.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py39/bytesio.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py39/bytesio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py39/iobase.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py39/iobase.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py39/stringio.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py39/stringio.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/assess_extensions/py39/unicode.c` & `contrast_agent-8.2.0/src/contrast/assess_extensions/py39/unicode.c`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/configuration/__init__.py` & `contrast_agent-8.2.0/src/contrast/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/configuration/agent.py` & `contrast_agent-8.2.0/src/contrast/configuration/agent.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/configuration/agent_config.py` & `contrast_agent-8.2.0/src/contrast/configuration/agent_config.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/configuration/api.py` & `contrast_agent-8.2.0/src/contrast/configuration/api.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/configuration/application.py` & `contrast_agent-8.2.0/src/contrast/configuration/application.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/configuration/assess.py` & `contrast_agent-8.2.0/src/contrast/configuration/assess.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/configuration/config_builder.py` & `contrast_agent-8.2.0/src/contrast/configuration/config_builder.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/configuration/config_option.py` & `contrast_agent-8.2.0/src/contrast/configuration/config_option.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/configuration/inventory.py` & `contrast_agent-8.2.0/src/contrast/configuration/inventory.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/configuration/protect.py` & `contrast_agent-8.2.0/src/contrast/configuration/protect.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/configuration/server.py` & `contrast_agent-8.2.0/src/contrast/configuration/server.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/loader/sitecustomize.py` & `contrast_agent-8.2.0/src/contrast/loader/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/patches/__init__.py` & `contrast_agent-8.2.0/src/contrast/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/patches/cgi_patch.py` & `contrast_agent-8.2.0/src/contrast/patches/cgi_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/patches/concurrent_futures_thread_patch.py` & `contrast_agent-8.2.0/src/contrast/patches/concurrent_futures_thread_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/patches/cs_io.py` & `contrast_agent-8.2.0/src/contrast/patches/cs_io.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/patches/cs_str.py` & `contrast_agent-8.2.0/src/contrast/patches/cs_str.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/patches/databases/dbapi2.py` & `contrast_agent-8.2.0/src/contrast/patches/databases/dbapi2.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/patches/databases/psycopg2_patch.py` & `contrast_agent-8.2.0/src/contrast/patches/databases/psycopg2_patch.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 """
 Database adapter patch for psycopg2.
 This module's cursor doesn't have an `executescript` method.
 """
 
 import os
+import sys
+from contrast.agent.policy import patch_manager
 from contrast_vendor.wrapt import register_post_import_hook
 
 from contrast.patches.databases import dbapi2
 from contrast.utils.decorators import fail_quietly
 
 PSYCOPG2 = "psycopg2"
 VENDOR = "PostgreSQL"
@@ -51,7 +53,15 @@
     dbapi2.instrument_adapter(
         psycopg2, VENDOR, Psycopg2Patcher, extra_cursors=[psycopg2.extensions.cursor]
     )
 
 
 def register_patches():
     register_post_import_hook(instrument_psycopg2, PSYCOPG2)
+
+
+def reverse_patches():
+    if psycopg2 := sys.modules.get(PSYCOPG2):
+        patch_manager.reverse_patches_by_owner(psycopg2)
+        patch_manager.reverse_patches_by_owner(psycopg2.extensions.connection)
+        patch_manager.reverse_patches_by_owner(psycopg2.extensions.cursor)
+        patch_manager.reverse_patches_by_owner(psycopg2.extras.NamedTupleCursor)
```

### Comparing `contrast_agent-8.1.0/src/contrast/patches/databases/sqlalchemy_patch.py` & `contrast_agent-8.2.0/src/contrast/patches/databases/sqlalchemy_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/patches/databases/sqlite3_patch.py` & `contrast_agent-8.2.0/src/contrast/patches/databases/sqlite3_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/patches/encodings_patch.py` & `contrast_agent-8.2.0/src/contrast/patches/encodings_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/patches/exec_and_eval.py` & `contrast_agent-8.2.0/src/contrast/patches/exec_and_eval.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/patches/frameworks/bottle_patches.py` & `contrast_agent-8.2.0/src/contrast/patches/frameworks/bottle_patches.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 import sys
 from contrast_vendor.wrapt import register_post_import_hook
 
 import contrast
 from contrast.agent import scope
 from contrast.agent.policy.applicator import apply_module_patches
-from contrast.agent.middlewares.route_coverage.common import (
-    build_route,
-    log_discovered_routes,
-)
+from contrast.agent.middlewares.route_coverage import common
 from contrast.agent.middlewares.route_coverage.bottle_routes import create_bottle_routes
 from contrast.agent.policy import patch_manager
 from contrast.utils.patch_utils import build_and_apply_patch, wrap_and_watermark
 from contrast.utils.decorators import fail_quietly
 
 from contrast_vendor import structlog as logging
 
@@ -56,32 +53,32 @@
     This is how we perform route discovery for Bottle. Many different patches could
     probably work here, since we really just need a reference to the Bottle instance
     after all routes have been registered.
     """
     del patch_policy
 
     def call_patch(wrapped, instance, args, kwargs):
-        result = wrapped(*args, **kwargs)
-        do_bottle_route_discovery(instance)
+        try:
+            result = wrapped(*args, **kwargs)
+        finally:
+            do_bottle_route_discovery(instance)
         return result
 
     return wrap_and_watermark(orig_func, call_patch)
 
 
 @fail_quietly("unable to perform Bottle route discovery")
+@scope.with_contrast_scope
 def do_bottle_route_discovery(bottle_instance):
-    with scope.contrast_scope():
-        from contrast.agent import agent_state
+    from contrast.agent import agent_state
 
-        if not agent_state.is_first_request():
-            return
+    if not agent_state.is_first_request():
+        return
 
-        discovered_routes = create_bottle_routes(bottle_instance)
-        agent_state.update_routes(discovered_routes)
-        log_discovered_routes("bottle", discovered_routes.values())
+    common.handle_route_discovery("bottle", create_bottle_routes, (bottle_instance,))
 
 
 def build_match_patch(orig_func, patch_policy):
     """
     Patch for bottle.Router.match()
 
     This sets up request context with all necessary info for current route observation
@@ -95,29 +92,25 @@
         do_bottle_route_observation(result)
         return result
 
     return wrap_and_watermark(orig_func, match_patch)
 
 
 @fail_quietly("unable to perform bottle route coverage in Bottle match patch")
+@scope.with_contrast_scope
 def do_bottle_route_observation(match_result):
-    with scope.contrast_scope():
-        if match_result is None:
-            return
-
-        context = contrast.CS__CONTEXT_TRACKER.current()
-        if context is None:
-            return
-
-        context.view_func = match_result[0].callback
-        context.view_func_str = build_route(
-            context.request.get_normalized_uri(),
-            context.view_func,
-        )
-        logger.debug("Observed Bottle route: %s", context.view_func_str)
+    if match_result is None:
+        return
+
+    context = contrast.CS__CONTEXT_TRACKER.current()
+    if context is None:
+        return
+
+    context.view_func = match_result[0].callback
+    logger.debug("Found Bottle view function", view_func=context.view_func)
 
 
 def patch_bottle(bottle_module):
     # We ask policy to go ahead and do all bottle patches here (even though policy
     # patches will happen later on) because we MUST have some bottle policy patches
     # already applied for these non-policy patches to work.
     # This would not be necessary if in _enable_patches policy_patches were applied
@@ -126,15 +119,20 @@
 
     build_and_apply_patch(
         bottle_module.SimpleTemplate,
         "prepare",
         build_prepare_patch,
         builder_args=(bottle_module,),
     )
-    build_and_apply_patch(bottle_module.Bottle, "__call__", build_call_patch)
+    # If the runner is in use, then CommonMiddlewarePatch has already
+    # patched __call__ for foundational middleware operations. We want
+    # both patches to be applied, so we force this one.
+    build_and_apply_patch(
+        bottle_module.Bottle, "__call__", build_call_patch, force=True
+    )
     build_and_apply_patch(bottle_module.Router, "match", build_match_patch)
 
 
 def register_patches():
     register_post_import_hook(patch_bottle, MODULE_NAME)
```

### Comparing `contrast_agent-8.1.0/src/contrast/patches/frameworks/django_patches.py` & `contrast_agent-8.2.0/src/contrast/patches/frameworks/django_patches.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/patches/frameworks/drf_patches.py` & `contrast_agent-8.2.0/src/contrast/patches/frameworks/drf_patches.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/patches/frameworks/falcon_patches.py` & `contrast_agent-8.2.0/src/contrast/patches/frameworks/falcon_patches.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 import sys
 import contrast
 from contrast_vendor.wrapt import register_post_import_hook
 from contrast.agent import scope
 from contrast.agent.assess.policy.source_policy import apply_stream_source
 from contrast.agent.policy import patch_manager
-from contrast.agent.middlewares.route_coverage.common import log_discovered_routes
+from contrast.agent.middlewares.route_coverage import common
 
 from contrast.utils.patch_utils import build_and_apply_patch, wrap_and_watermark
 from contrast.utils.decorators import fail_quietly
 from contrast_vendor import structlog as logging
 
 
 FALCON_MULTIPART_MIDDLEWARE_MODULE = "falcon_multipart.middleware"
@@ -102,54 +102,40 @@
     )
 
     from contrast.agent import agent_state
 
     if not agent_state.is_first_request():
         return
 
-    discovered_routes = create_falcon_routes(falcon_instance)
-    agent_state.update_routes(discovered_routes)
-
+    common.handle_route_discovery("falcon", create_falcon_routes, (falcon_instance,))
     do_config_scanning(logger, falcon_instance)
-    log_discovered_routes("falcon", discovered_routes.values())
 
 
 @fail_quietly("unable to perform Falcon route observation")
 @scope.with_contrast_scope
 def do_falcon_routes_observation(falcon_app_instance, request_args):
-    from contrast.agent.middlewares.route_coverage.falcon_routes import (
-        get_view_func,
-        build_route,
-    )
+    from contrast.agent.middlewares.route_coverage.falcon_routes import get_view_func
 
     context = contrast.CS__CONTEXT_TRACKER.current()
 
     if context is None:
         return
     if hasattr(falcon_app_instance, "_ASGI") and falcon_app_instance._ASGI:
         request_path = request_args[0]["path"]
         request_method = request_args[0]["method"]
     else:
         request_path = request_args[0]["PATH_INFO"]
         request_method = request_args[0]["REQUEST_METHOD"]
 
-    view_func = get_view_func(
+    context.view_func = get_view_func(
         request_path,
         falcon_app_instance,
         request_method,
     )
-
-    context.view_func = view_func
-    context.view_func_str = build_route(
-        context.view_func,
-        context.request.get_normalized_uri(),
-        falcon_app_instance,
-        request_path,
-    )
-    logger.debug("Observed Falcon route: %s", context.view_func_str)
+    logger.debug("Found Falcon view function", view_func=context.view_func)
 
 
 @fail_quietly("failed to apply Falcon config scanning rules")
 def do_config_scanning(logger, falcon_app_instance):
     from contrast.agent.assess.rules.config.falcon_secure_flag_rule import (
         FalconSecureFlagRule,
     )
@@ -159,15 +145,18 @@
     for rule in [
         FalconSecureFlagRule(),
     ]:
         rule.apply(falcon_app_instance.resp_options)
 
 
 def patch_falcon(falcon_module):
-    build_and_apply_patch(falcon_module.App, "__call__", build_call_patch)
+    # If the runner is in use, then CommonMiddlewarePatch has already
+    # patched __call__ for foundational middleware operations. We want
+    # both patches to be applied, so we force this one.
+    build_and_apply_patch(falcon_module.App, "__call__", build_call_patch, force=True)
 
 
 def patch_falcon_asgi(falcon_asgi_module):
     build_and_apply_patch(
         falcon_asgi_module.App, "__call__", build_call_patch, force=True
     )
 
@@ -178,22 +167,22 @@
 
     register_post_import_hook(
         patch_falcon_multipart, FALCON_MULTIPART_MIDDLEWARE_MODULE
     )
 
 
 def reverse_patches():
-    falcon_module = sys.modules.get(FALCON_MODULE)
-    falcon_asgi_module = sys.modules.get(FALCON_ASGI_MODULE)
-    module = sys.modules.get(FALCON_MULTIPART_MIDDLEWARE_MODULE)
-    if module is None:  # pragma: no cover
-        return
-    middleware_cls = getattr(module, FALCON_MULTIPART_MIDDLEWARE_CLASS)
-    if middleware_cls is None:  # pragma: no cover
-        return
-    if falcon_module:
+    if falcon_module := sys.modules.get(FALCON_MODULE):
         patch_manager.reverse_patches_by_owner(falcon_module.App)
-    if falcon_asgi_module:
+
+    if falcon_asgi_module := sys.modules.get(FALCON_ASGI_MODULE):
         patch_manager.reverse_patches_by_owner(falcon_asgi_module.app.App)
         patch_manager.reverse_patches_by_owner(falcon_asgi_module.App)
         patch_manager.reverse_patches_by_owner(falcon_asgi_module)
-    patch_manager.reverse_patches_by_owner(middleware_cls)
+
+    if falcon_multipart_middleware_module := sys.modules.get(
+        FALCON_MULTIPART_MIDDLEWARE_MODULE
+    ):
+        if middleware_cls := getattr(
+            falcon_multipart_middleware_module, FALCON_MULTIPART_MIDDLEWARE_CLASS
+        ):
+            patch_manager.reverse_patches_by_owner(middleware_cls)
```

### Comparing `contrast_agent-8.1.0/src/contrast/patches/frameworks/flask_and_quart_patches.py` & `contrast_agent-8.2.0/src/contrast/patches/frameworks/flask_and_quart_patches.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,15 @@
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 import sys
 import functools
 from contrast_vendor.wrapt import register_post_import_hook
 
 import contrast
 from contrast.agent import scope
-from contrast.agent.middlewares.route_coverage.common import (
-    build_route,
-    log_discovered_routes,
-)
-from contrast.agent.middlewares.route_coverage.flask_routes import create_routes
+from contrast.agent.middlewares.route_coverage import common, flask_routes
 from contrast.agent.policy import patch_manager
 from contrast.utils.patch_utils import build_and_apply_patch, wrap_and_watermark
 from contrast.utils.decorators import fail_quietly
 from contrast.utils.safe_import import safe_import_list
 
 from contrast.agent.assess.rules.config import (
     FlaskSessionAgeRule,
@@ -43,45 +39,47 @@
 def build_flask_full_dispatch_request_patch(orig_func, patch_policy):
     del patch_policy
 
     def full_dispatch_request_patch(wrapped, instance, args, kwargs):
         try:
             result = wrapped(*args, **kwargs)
         finally:
-            do_first_request_analysis(instance)
+            do_first_request_analysis(instance, "flask")
             do_flask_route_observation(instance)
         return result
 
     return wrap_and_watermark(orig_func, full_dispatch_request_patch)
 
 
 def build_quart_full_dispatch_request_patch(orig_func, patch_policy):
     del patch_policy
 
     async def full_dispatch_request_patch(wrapped, instance, args, kwargs):
         try:
             result = await wrapped(*args, **kwargs)
         finally:
-            do_first_request_analysis(instance)
+            do_first_request_analysis(instance, "quart")
             do_quart_route_observation(instance, *args, **kwargs)
         return result
 
     return wrap_and_watermark(orig_func, full_dispatch_request_patch)
 
 
 @fail_quietly("Failed to run first-request analysis")
 @scope.with_contrast_scope
-def do_first_request_analysis(app_instance):
+def do_first_request_analysis(app_instance, framework: str):
     from contrast.agent import agent_state
 
     if not agent_state.is_first_request():
         return
 
+    common.handle_route_discovery(
+        framework, flask_routes.create_routes, (app_instance,)
+    )
     do_config_scanning(app_instance)
-    do_route_discovery(app_instance)
 
 
 @fail_quietly("unable to perform Flask route observation")
 @scope.with_contrast_scope
 def do_flask_route_observation(flask_instance):
     logger.debug("Performing Flask route observation")
 
@@ -122,34 +120,24 @@
     endpoint = getattr(framework_ctx.request.url_rule, "endpoint", None)
     view_func = app_instance.view_functions.get(endpoint)
     if view_func is None:
         logger.debug("did not find endpoint for route observation")
         return
 
     context.view_func = view_func
-    context.view_func_str = build_route(view_func.__name__, view_func)
-    logger.debug("Observed route: %s", context.view_func_str)
+    logger.debug("Found view function", view_func=context.view_func)
 
 
 @fail_quietly("Failed to run config scanning rules")
 def do_config_scanning(app_instance):
     logger.debug("Running config scanning rules")
     for rule in [FlaskSessionAgeRule, FlaskSecureFlagRule, FlaskHttpOnlyRule]:
         rule().apply(app_instance)
 
 
-@fail_quietly("unable to perform route discovery")
-def do_route_discovery(app_instance):
-    from contrast.agent import agent_state
-
-    discovered_routes = create_routes(app_instance)
-    agent_state.update_routes(discovered_routes)
-    log_discovered_routes("flask/quart", discovered_routes.values())
-
-
 def patch_flask(flask_module):
     build_and_apply_patch(
         flask_module.Flask,
         "full_dispatch_request",
         build_flask_full_dispatch_request_patch,
     )
```

### Comparing `contrast_agent-8.1.0/src/contrast/patches/frameworks/pyramid_patch.py` & `contrast_agent-8.2.0/src/contrast/patches/frameworks/pyramid_patch.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from contrast.agent.policy import patch_manager
 from contrast.agent.policy.applicator import apply_assess_patch
 from contrast.agent.policy import registry
 from contrast.patches import urllib_patch
 from contrast.utils.decorators import fail_quietly
 from contrast.utils.patch_utils import build_and_apply_patch, wrap_and_watermark
 from contrast.agent import scope
-from contrast.agent.middlewares.route_coverage.common import log_discovered_routes
+from contrast.agent.middlewares.route_coverage import common
 
 from contrast_vendor import structlog as logging
 
 
 logger = logging.getLogger("contrast")
 
 PYRAMID_SESSION_MODULE = "pyramid.session"
@@ -103,67 +103,63 @@
     """
     del patch_policy
 
     def call_patch(wrapped, instance, args, kwargs):
         try:
             result = wrapped(*args, **kwargs)
         finally:
-            do_pyramid_routes_discovery(instance)
-            do_pyramid_routes_observation(instance, args)
+            do_pyramid_route_discovery(instance)
+            do_pyramid_route_observation(instance, args)
         return result
 
     return wrap_and_watermark(orig_func, call_patch)
 
 
-@fail_quietly("unable to perform Pyramid routes discovery")
+@fail_quietly("unable to perform Pyramid route discovery")
 @scope.with_contrast_scope
-def do_pyramid_routes_discovery(pyramid_router_instance):
+def do_pyramid_route_discovery(pyramid_router_instance):
     from contrast.agent.middlewares.route_coverage.pyramid_routes import (
         create_pyramid_routes,
     )
 
     from contrast.agent import agent_state
 
     if not agent_state.is_first_request():
         return
 
-    discovered_routes = create_pyramid_routes(pyramid_router_instance.registry)
-    agent_state.update_routes(discovered_routes)
-    log_discovered_routes("pyramid", discovered_routes.values())
+    common.handle_route_discovery(
+        "pyramid", create_pyramid_routes, (pyramid_router_instance.registry,)
+    )
 
 
 @fail_quietly("unable to perform Pyramid route observation")
 @scope.with_contrast_scope
-def do_pyramid_routes_observation(pyramid_router_instance, request_path_arg):
-    from contrast.agent.middlewares.route_coverage.pyramid_routes import (
-        get_view_func,
-        build_route,
-    )
-
-    request_path = request_path_arg[0]["PATH_INFO"]
-    view_func = get_view_func(
-        request_path,
-        pyramid_router_instance.routes_mapper.routelist,
-        pyramid_router_instance.registry,
-    )
+def do_pyramid_route_observation(pyramid_router_instance, request_path_arg):
+    from contrast.agent.middlewares.route_coverage.pyramid_routes import get_view_func
 
     context = contrast.CS__CONTEXT_TRACKER.current()
     if context is None:
         return
 
-    context.view_func = view_func
-    context.view_func_str = build_route(
-        context.view_func,
-        context.request.get_normalized_uri(),
+    request_path = request_path_arg[0]["PATH_INFO"]
+    context.view_func = get_view_func(
+        request_path,
+        pyramid_router_instance.routes_mapper.routelist,
+        pyramid_router_instance.registry,
     )
-    logger.debug("Observed Pyramid route: %s", context.view_func_str)
+    logger.debug("Found Pyramid view function", view_func=context.view_func)
 
 
 def patch_pyramid(pyramid_router_module):
-    build_and_apply_patch(pyramid_router_module.Router, "__call__", build_call_patch)
+    # If the runner is in use, then CommonMiddlewarePatch has already
+    # patched __call__ for foundational middleware operations. We want
+    # both patches to be applied, so we force this one.
+    build_and_apply_patch(
+        pyramid_router_module.Router, "__call__", build_call_patch, force=True
+    )
 
 
 def register_patches():
     register_post_import_hook(patch_pyramid, PYRAMID_ROUTER_MODULE)
     register_post_import_hook(patch_session_pyramid, PYRAMID_SESSION_MODULE)
     register_post_import_hook(patch_encode_pyramid, "pyramid.encode")
```

### Comparing `contrast_agent-8.1.0/src/contrast/patches/frameworks/starlette_patches.py` & `contrast_agent-8.2.0/src/contrast/patches/frameworks/starlette_patches.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 import contrast
 from contrast.agent import scope
 from contrast.agent.assess.policy.analysis import analyze
 from contrast.agent.policy import registry
 from contrast.agent.middlewares.route_coverage.starlette_routes import (
     create_starlette_routes,
 )
-from contrast.agent.middlewares.route_coverage.common import log_discovered_routes
 from contrast.agent.policy import patch_manager
-from contrast.agent.middlewares.route_coverage.common import build_route
+from contrast.agent.middlewares.route_coverage import common
 from contrast.utils.decorators import fail_quietly
 from contrast.utils.patch_utils import build_and_apply_patch, wrap_and_watermark
 
 from contrast_vendor import structlog as logging
 
 logger = logging.getLogger("contrast")
 
@@ -70,18 +69,17 @@
 @scope.with_contrast_scope
 def do_starlette_route_discovery(starlette_router_instance):
     from contrast.agent import agent_state
 
     if not agent_state.is_first_request():
         return
 
-    discovered_routes = create_starlette_routes(starlette_router_instance)
-
-    agent_state.update_routes(discovered_routes)
-    log_discovered_routes("starlette", discovered_routes.values())
+    common.handle_route_discovery(
+        "starlette", create_starlette_routes, (starlette_router_instance,)
+    )
 
 
 @fail_quietly("unable to perform starlette route observation")
 @scope.with_contrast_scope
 def do_starlette_route_observation(starlette_router_instance, *args, **kwargs):
     from starlette.staticfiles import StaticFiles
 
@@ -105,18 +103,16 @@
         logger.debug("did not find endpoint for starlette route observation")
         return
 
     context.view_func = view_func
 
     if isinstance(view_func, StaticFiles):
         context.view_func_str = f"StaticFiles(directory={view_func.directory})"
-    else:
-        context.view_func_str = build_route(view_func.__name__, view_func)
 
-    logger.debug("Observed starlette route: %s", context.view_func_str)
+    logger.debug("Found starlette view function", view_func=context.view_func)
 
 
 class ContrastSessionDictProxy(wrapt.ObjectProxy):
     """
     Custom ObjectProxy we use to wrap dicts returned by starlette's request.session
     property. These proxied dicts have a trigger for trust-boundary-violation on
     __setitem__.
```

### Comparing `contrast_agent-8.1.0/src/contrast/patches/genshi_patch.py` & `contrast_agent-8.2.0/src/contrast/patches/genshi_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/patches/import_patch.py` & `contrast_agent-8.2.0/src/contrast/patches/import_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/patches/lxml_patch.py` & `contrast_agent-8.2.0/src/contrast/patches/lxml_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/patches/middleware/aiohttp.py` & `contrast_agent-8.2.0/src/contrast/patches/middleware/aiohttp.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/patches/middleware/common.py` & `contrast_agent-8.2.0/src/contrast/patches/middleware/common.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/patches/middleware/django.py` & `contrast_agent-8.2.0/src/contrast/patches/middleware/django.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import sys
 
 import contrast
 from contrast.agent import scope
 from contrast.agent.policy import patch_manager
 from contrast.utils.decorators import fail_loudly, fail_quietly
 from contrast.utils.patch_utils import build_and_apply_patch, wrap_and_watermark
-from contrast.agent.middlewares.route_coverage.common import log_discovered_routes
+from contrast.agent.middlewares.route_coverage import common
 
 from contrast_vendor.wrapt import register_post_import_hook
 from contrast_vendor import structlog as logging
 
 DJANGO_WSGI_NAME = "django.core.wsgi"
 DJANGO_ASGI_NAME = "django.core.asgi"
 
@@ -38,46 +38,29 @@
         logger.warning("django settings module not loaded; can't scan config")
         return
 
     for rule in [DjangoSessionAgeRule, DjangoSecureFlagRule, DjangoHttpOnlyRule]:
         rule().apply(app_settings, app_config_module)
 
 
-@fail_quietly("failed to perform django route discovery")
-def do_route_discovery(logger):
-    from contrast.agent import agent_state
-
-    # Lazy import for django
-    from contrast.agent.middlewares.route_coverage.django_routes import (
-        create_django_routes,
-    )
-
-    logger.debug("performing route discovery for django application")
-    discovered_routes = create_django_routes()
-    if discovered_routes is None:
-        logger.warning("no routes discovered for django application")
-        return
-
-    agent_state.update_routes(discovered_routes)
-    log_discovered_routes("django", discovered_routes.values())
-
-
 @fail_quietly("failed to run django first request analysis")
 @scope.with_contrast_scope
 def django_first_request(sender, **kwargs):
-    # Lazy import for django
     from django.core import signals
+    from contrast.agent.middlewares.route_coverage.django_routes import (
+        create_django_routes,
+    )
 
     del sender, kwargs
 
     logger = logging.getLogger("contrast")
     logger.debug("called django first request signal")
 
     do_config_scanning(logger)
-    do_route_discovery(logger)
+    common.handle_route_discovery("django", create_django_routes, ())
 
     # the signal is no longer needed after the first request
     logger.debug("disconnecting django first request signal (first request done)")
     signals.request_finished.disconnect(django_first_request)
 
 
 def _extract_path(signal_kwargs):
@@ -124,15 +107,14 @@
     request_path = _extract_path(kwargs)
 
     view_func = get_view_func(request_path)
     if view_func is None:
         logger.debug("did not find django view function for route observation")
         return
 
-    context.view_func = view_func
     context.view_func_str = build_django_route(view_func)
     logger.debug("Observed route: %s", context.view_func_str)
 
 
 @fail_quietly("Failed to retrieve django application name from settings")
 def get_app_name() -> str:
     # Lazy import for django
```

### Comparing `contrast_agent-8.1.0/src/contrast/patches/middleware/mod_wsgi.py` & `contrast_agent-8.2.0/src/contrast/patches/middleware/mod_wsgi.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/patches/operator.py` & `contrast_agent-8.2.0/src/contrast/patches/operator.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/patches/pathlib_patch.py` & `contrast_agent-8.2.0/src/contrast/patches/pathlib_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/patches/re_patch.py` & `contrast_agent-8.2.0/src/contrast/patches/re_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/patches/str_new.py` & `contrast_agent-8.2.0/src/contrast/patches/str_new.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,28 +24,39 @@
         try:
             if inspect.isclass(obj) and issubclass(obj, (str, bytes, bytearray)):
                 yield obj
         except Exception:
             continue
 
 
+def check_or_enter_scope(func):
+    def wrapper(*args, **kwargs):
+        if scope.in_contrast_or_propagation_scope():
+            return
+        with scope.contrast_scope(), scope.propagation_scope():
+            func(*args, **kwargs)
+            return
+
+    return wrapper
+
+
+@check_or_enter_scope
 @fail_quietly("Failed to propagate string subclass __new__")
-@scope.with_contrast_scope
 def propagate_str_cast(result, args, kwargs):
     string_propagation.propagate_unicode_cast(result, args[0], result, args[1:], kwargs)
 
 
+@check_or_enter_scope
 @fail_quietly("Failed to propagate bytes subclass __new__")
-@scope.with_contrast_scope
 def propagate_bytes_cast(result, args, kwargs):
     string_propagation.propagate_bytes_cast(result, args[0], result, args[1:], kwargs)
 
 
+@check_or_enter_scope
 @fail_quietly("Failed to propagate bytearray subclass __init__")
-@scope.with_contrast_scope
 def propagate_bytearray_init(instance, args, kwargs):
     """
     To make use of our generalized bytearray cast propagation machinery, we need to call
     `propagate_bytearray_cast` as though this were a __new__ patch. The calling
     semantics of __new__ differ from __init__, so we shuffle some things around
     accordingly.
     """
```

### Comparing `contrast_agent-8.1.0/src/contrast/patches/sys_patch.py` & `contrast_agent-8.2.0/src/contrast/patches/sys_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/patches/threading_patch.py` & `contrast_agent-8.2.0/src/contrast/patches/threading_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/patches/urllib_patch.py` & `contrast_agent-8.2.0/src/contrast/patches/urllib_patch.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/patches/utils.py` & `contrast_agent-8.2.0/src/contrast/patches/utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/deadzones.py` & `contrast_agent-8.2.0/src/contrast/policy/deadzones.py`

 * *Files 21% similar despite different names*

```diff
@@ -93,14 +93,38 @@
         # stored in session data. However, the string representing the class being
         # imported is first checked against settings.AUTHENTICATION_BACKENDS, so it's
         # impossible for this function to lead to unsafe code execution. See PYT-3165.
         "module": "django.contrib.auth",
         "method_name": "get_user",
     },
     {
+        # `django-enumfields` is an extension that provides extra django-specific
+        # behavior for enum database types when using the django ORM. `from_db_value`
+        # is a special method to be defined by concrete classes based on
+        # django.db.models.Field - it is used to convert values directly from the
+        # database into python objects. We're not concerned about deadzoning this
+        # function for enumfields for two main reasons:
+        #
+        # 1. It should never be possible to receive tracked data from a database. There
+        #    might be an exception for stored XSS but we're accepting that gap if it
+        #    exists. This means that no meaningful dataflow should be able to take place
+        #    within this function in the first place.
+        # 2. The only actual dataflow in `from_db_value` occurs when formatting the
+        #    exception message for its failure case. Even if tracked data somehow enters
+        #    this function, we would only lose propagation into this exception message.
+        #    It's unlikely this message would find its way to a trigger (xss is probably
+        #    the only possibility, if http responses for server exceptions include
+        #    unsanitized error messages, but this seems like a stretch).
+        #
+        # See PYT-3321.
+        "module": "enumfields.fields",
+        "class_name": "EnumFieldMixin",
+        "method_name": "from_db_value",
+    },
+    {
         # Too much propagation / source creation occurs here. It is not necessary for
         # body tracking since we accomplish this with higher-level source nodes
         "module": "quart.wrappers.request",
         "class_name": "Request",
         "method_name": "_load_form_data",
     },
     {
```

### Comparing `contrast_agent-8.1.0/src/contrast/policy/propagators/codecs.py` & `contrast_agent-8.2.0/src/contrast/policy/propagators/codecs.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/propagators/encodings.py` & `contrast_agent-8.2.0/src/contrast/policy/propagators/encodings.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/propagators/frameworks.py` & `contrast_agent-8.2.0/src/contrast/policy/propagators/frameworks.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/propagators/paths.py` & `contrast_agent-8.2.0/src/contrast/policy/propagators/paths.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/propagators/re.py` & `contrast_agent-8.2.0/src/contrast/policy/propagators/re.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/propagators/serialize.py` & `contrast_agent-8.2.0/src/contrast/policy/propagators/serialize.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/propagators/string.py` & `contrast_agent-8.2.0/src/contrast/policy/propagators/string.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/sources/asgi.py` & `contrast_agent-8.2.0/src/contrast/policy/sources/asgi.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/sources/cgi.py` & `contrast_agent-8.2.0/src/contrast/policy/sources/cgi.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/sources/django.py` & `contrast_agent-8.2.0/src/contrast/policy/sources/django.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/sources/falcon.py` & `contrast_agent-8.2.0/src/contrast/policy/sources/falcon.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/sources/flask.py` & `contrast_agent-8.2.0/src/contrast/policy/sources/flask.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/sources/quart.py` & `contrast_agent-8.2.0/src/contrast/policy/sources/quart.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/sources/webob.py` & `contrast_agent-8.2.0/src/contrast/policy/sources/webob.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/triggers/__init__.py` & `contrast_agent-8.2.0/src/contrast/policy/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/triggers/cmd_injection.py` & `contrast_agent-8.2.0/src/contrast/policy/triggers/cmd_injection.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/triggers/crypto.py` & `contrast_agent-8.2.0/src/contrast/policy/triggers/crypto.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/triggers/httponly.py` & `contrast_agent-8.2.0/src/contrast/policy/triggers/httponly.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/triggers/nosql_injection.py` & `contrast_agent-8.2.0/src/contrast/policy/triggers/nosql_injection.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/triggers/path_traversal.py` & `contrast_agent-8.2.0/src/contrast/policy/triggers/path_traversal.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/triggers/prompt_injection.py` & `contrast_agent-8.2.0/src/contrast/policy/triggers/prompt_injection.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/triggers/redos.py` & `contrast_agent-8.2.0/src/contrast/policy/triggers/redos.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/triggers/reflected_xss.py` & `contrast_agent-8.2.0/src/contrast/policy/triggers/reflected_xss.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/triggers/secure_flag_missing.py` & `contrast_agent-8.2.0/src/contrast/policy/triggers/secure_flag_missing.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/triggers/session_rewriting.py` & `contrast_agent-8.2.0/src/contrast/policy/triggers/session_rewriting.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/triggers/session_timeout.py` & `contrast_agent-8.2.0/src/contrast/policy/triggers/session_timeout.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/triggers/sql_injection.py` & `contrast_agent-8.2.0/src/contrast/policy/triggers/sql_injection.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/triggers/ssrf.py` & `contrast_agent-8.2.0/src/contrast/policy/triggers/ssrf.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/triggers/trust_boundary_violation.py` & `contrast_agent-8.2.0/src/contrast/policy/triggers/trust_boundary_violation.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/triggers/unsafe_code_execution.py` & `contrast_agent-8.2.0/src/contrast/policy/triggers/unsafe_code_execution.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/triggers/untrusted_deserialization.py` & `contrast_agent-8.2.0/src/contrast/policy/triggers/untrusted_deserialization.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/triggers/unvalidated_redirect.py` & `contrast_agent-8.2.0/src/contrast/policy/triggers/unvalidated_redirect.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/triggers/xpath_injection.py` & `contrast_agent-8.2.0/src/contrast/policy/triggers/xpath_injection.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/policy/triggers/xxe.py` & `contrast_agent-8.2.0/src/contrast/policy/triggers/xxe.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/reporting/activity_masker.py` & `contrast_agent-8.2.0/src/contrast/reporting/activity_masker.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,158 +1,166 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 from copy import copy
+from typing import List, TypedDict
 from urllib.parse import parse_qs, urlencode, unquote
 
 from contrast.agent.settings import Settings
 from contrast.api.attack import ProtectResponse
 from contrast_vendor import structlog as logging
 from contrast_vendor.webob.multidict import MultiDict
 
 logger = logging.getLogger("contrast")
 
 MASK = "contrast-redacted-{}"
 BODY_MASK = b"contrast-redacted-body"
 SEMICOLON_URL_ENCODE_VAL = "%25"
 
 
+class SensitiveDataRule(TypedDict):
+    id: str
+    keywords: List[str]
+
+
+class SensitiveDataPolicy(TypedDict):
+    mask_attack_vector: bool
+    mask_http_body: bool
+    rules: List[SensitiveDataRule]
+
+
 class ActivityMasker:
-    def __init__(self, ctx):
-        self.ctx = ctx
+    def mask_sensitive_data(self, request, attacks=None):
+        if request:
+            request._masked = True
 
-        sensitive_data_masking_policy = getattr(
-            Settings(), "sensitive_data_masking_policy", None
-        )
-        self.http_request = self.ctx.request
-        if sensitive_data_masking_policy:
-            self.mask_rules = sensitive_data_masking_policy
-        else:
-            self.mask_rules = None
-
-    def mask_sensitive_data(self):
-        # Check if request is present and return if not
-        if not self.http_request or not self.mask_rules:
+        mask_rules = getattr(Settings(), "sensitive_data_masking_policy", None)
+        if not request or not mask_rules:
             return
 
+        self.request = request
+        self.mask_rules: SensitiveDataPolicy = mask_rules
+        self.attacks = attacks or []
+
         logger.debug("Masker: masking sensitive data")
 
-        self.mask_body()
-        self.mask_query_string()
-        self.mask_request_params()
-        self.mask_request_cookies()
-        self.mask_request_headers()
+        self._mask_body()
+        self._mask_query_string()
+        self._mask_request_params()
+        self._mask_request_cookies()
+        self._mask_request_headers()
 
-    def mask_body(self):
+    def _mask_body(self):
         # Check if mask_http_body is set to False or is None and skip if true
         if not self.mask_rules.get("mask_http_body"):
             return
 
         # Checks if body is not empty or null
-        if self.http_request.body:
-            self.http_request._masked_body = BODY_MASK
+        if self.request.body:
+            self.request._masked_body = BODY_MASK
 
-    def mask_query_string(self):
-        query_string = self.http_request.query_string
-        if query_string:
-            self.http_request._masked_query_string = self.mask_raw_query(query_string)
+    def _mask_query_string(self):
+        if self.request.query_string:
+            self.request._masked_query_string = self._mask_raw_query(
+                self.request.query_string
+            )
 
-    def mask_raw_query(self, query_string):
+    def _mask_raw_query(self, query_string):
         qs_dict = parse_qs(query_string)
-        masked_qs_dict = self.mask_dictionary(qs_dict)
+        masked_qs_dict = self._mask_dictionary(qs_dict)
         return urlencode(masked_qs_dict, doseq=True)
 
-    def mask_request_params(self):
-        params = self.http_request.params
+    def _mask_request_params(self):
+        params = self.request.params
         if not params:
             return
 
-        self.http_request._masked_params = self.mask_dictionary(params)
+        self.request._masked_params = self._mask_dictionary(params)
 
-    def mask_request_cookies(self):
-        cookies = self.http_request.cookies
+    def _mask_request_cookies(self):
+        cookies = self.request.cookies
         if not cookies:
             return
 
-        self.http_request._masked_cookies = self.mask_dictionary(cookies)
+        self.request._masked_cookies = self._mask_dictionary(cookies)
 
-    def mask_request_headers(self):
-        headers = self.http_request.headers
+    def _mask_request_headers(self):
+        headers = self.request.headers
         if not headers:
             return
 
-        self.http_request._masked_headers = self.mask_dictionary(headers)
+        self.request._masked_headers = self._mask_dictionary(headers)
 
-    def mask_dictionary(self, d):
+    def _mask_dictionary(self, d):
         if not d:
-            return None
+            return d
 
         if isinstance(d, MultiDict):
             d = d.mixed()
 
         d_copy = {k: copy(v) for k, v in d.items()}
 
         for k, v in d_copy.items():
-            if k is None or self.find_value_index_in_rules(k.lower()) == -1:
+            if k is None or self._find_value_index_in_rules(k.lower()) == -1:
                 continue
 
             if isinstance(v, list):
-                self.mask_values(k, v, d_copy, self.ctx.attacks)
+                self._mask_values(k, v, d_copy, self.attacks)
             else:
-                self.mask_hash(k, v, d_copy, self.ctx.attacks)
+                self._mask_hash(k, v, d_copy, self.attacks)
         return d_copy
 
-    def mask_values(self, k, v, d, attacks):
+    def _mask_values(self, k, v, d, attacks):
         for idx, item in enumerate(v):
-            if self.mask_rules.get("mask_attack_vector") and self.is_value_vector(
+            if self.mask_rules.get("mask_attack_vector") and self._is_value_vector(
                 attacks, item
             ):
                 d[k][idx] = MASK.format(k.lower())
-            if not self.is_value_vector(attacks, item):
+            if not self._is_value_vector(attacks, item):
                 d[k][idx] = MASK.format(k.lower())
 
-    def mask_hash(self, k, v, d, attacks):
-        if self.mask_rules.get("mask_attack_vector") and self.is_value_vector(
+    def _mask_hash(self, k, v, d, attacks):
+        if self.mask_rules.get("mask_attack_vector") and self._is_value_vector(
             attacks, v
         ):
             d[k] = MASK.format(k.lower())
-        if not self.is_value_vector(attacks, v):
+        if not self._is_value_vector(attacks, v):
             d[k] = MASK.format(k.lower())
 
-    def mask_pair(self, k, v, d, attacks):
+    def _mask_pair(self, k, v, d, attacks):
         for idx, item in enumerate(v):
-            if self.mask_rules.get("mask_attack_vector") and self.is_value_vector(
+            if self.mask_rules.get("mask_attack_vector") and self._is_value_vector(
                 attacks, item
             ):
                 d[k].values[idx] = MASK.format(k.lower())
-            if not self.is_value_vector(attacks, item):
+            if not self._is_value_vector(attacks, item):
                 d[k].values[idx] = MASK.format(k.lower())
 
-    def is_value_vector(self, attacks, value):
+    def _is_value_vector(self, attacks, value):
         if not attacks or not value:
             return False
 
         for attack in attacks:
-            if self.is_value_in_sample(attack.samples, value):
+            if self._is_value_in_sample(attack.samples, value):
                 return attack.response != ProtectResponse.NO_ACTION
 
         return False
 
-    def is_value_in_sample(self, samples, value):
+    def _is_value_in_sample(self, samples, value):
         if not samples:
             return False
 
         # Setting this to remove url encoding of header and cookie values
         value = unquote(value)
 
         for sample in samples:
             if sample.user_input.value == value:
                 return True
         return False
 
-    def find_value_index_in_rules(self, s):
+    def _find_value_index_in_rules(self, s):
         index = -1
         # When looking for header it replaces '_' with '-' and I don't want to risk not
         # properly matching to the rules
         s = s.replace("-", "_")
         for rule in self.mask_rules.get("rules"):
             try:
                 index = rule.get("keywords").index(s)
```

### Comparing `contrast_agent-8.1.0/src/contrast/reporting/reporting_client.py` & `contrast_agent-8.2.0/src/contrast/reporting/reporting_client.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/reporting/request_audit.py` & `contrast_agent-8.2.0/src/contrast/reporting/request_audit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright © 2024 Contrast Security, Inc.
 # See https://www.contrastsecurity.com/enduser-terms-0317a for more details.
 from datetime import datetime
 import json
+import uuid
 import pathlib
 from os import path
 from contrast.reporting.teamserver_messages import BaseTsMessage
 from requests.models import Response
 
 from contrast_vendor import structlog as logging
 from contrast.utils.decorators import fail_quietly
@@ -43,28 +44,29 @@
         for sub_dir in self.SUB_DIRS:
             sub_path = path.join(self.messages_path, sub_dir)
             pathlib.Path(sub_path).mkdir(parents=True, exist_ok=True)
 
         logger.debug("Created request_audit dirs in %s", self.messages_path)
 
     def audit(self, msg, response):
+        uid = uuid.uuid4().hex[:8]
         if self.config.get_value("api.request_audit.requests"):
-            self.write_data(msg, "requests", msg.name)
+            self.write_data(msg, "requests", msg.name, uid)
 
         if self.config.get_value("api.request_audit.responses"):
-            self.write_data(response, "responses", msg.name)
+            self.write_data(response, "responses", msg.name, uid)
 
     @fail_quietly("Unable to write request audit data")
-    def write_data(self, msg, msg_type, msg_name):
+    def write_data(self, msg, msg_type, msg_name, uid):
         now = datetime.now()
         epoch = now.timestamp()
         day = now.strftime("%Y%m%d")
         time = f"{day}-{epoch}"
 
-        file_name = f"{time}-{msg_name}-teamserver.json"
+        file_name = f"{time}-{uid}-{msg_name}-teamserver.json"
         file_path = path.join(self.messages_path, msg_type, file_name)
 
         data = get_message_body(msg)
 
         # In the future, we'd like to somehow include status code + headers
         with pathlib.Path(file_path).open("w", encoding="UTF-8") as target:
             json.dump(data, target, indent=1)
```

### Comparing `contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/__init__.py` & `contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/_traces.py` & `contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/_traces.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/agent_startup.py` & `contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/agent_startup.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/application_activity.py` & `contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/application_activity.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 logger = logging.getLogger("contrast")
 
 
 class ApplicationActivity(BaseTsAppMessage):
     def __init__(self, context):
         super().__init__()
-        ActivityMasker(context).mask_sensitive_data()
 
         self.body = {"lastUpdate": self.since_last_update}
 
         self.body["inventory"] = {
             # Used by TeamServer to aggregate counts across a given time period, for
             # Protect and attacker activity.
             "activityDuration": 0,
@@ -27,14 +26,19 @@
         if context.request and context.request.user_agent:
             self.body["inventory"]["browsers"] = [context.request.user_agent]
         if context.database_info:
             for db_info in context.database_info:
                 self.body["inventory"]["components"].append(db_info)
 
         if context.attacks:
+            # The only sensitive data in this message is the request field
+            # of samples. Since Assess messages won't have samples, we
+            # delay masking until this point.
+            ActivityMasker().mask_sensitive_data(context.request, context.attacks)
+
             self.body["defend"] = {"attackers": []}
 
             for attack in context.attacks:
                 self.body["defend"]["attackers"].append(
                     {
                         "protectionRules": {
                             attack.rule_id: attack.to_json(context.request)
```

### Comparing `contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/application_inventory.py` & `contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/application_inventory.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 from contrast_vendor import structlog as logging
 
 logger = logging.getLogger("contrast")
 
 
 class ApplicationInventory(BaseTsAppMessage):
     def __init__(self, routes):
-        # This message does not need "Application-Path" header but it doesn't hurt
+        # This message does not need "Application-Path" header, but it doesn't hurt
         # either.
         super().__init__()
+        # TODO: PYT-3324 update to 1.1 when TeamServer can accept it
         self.base_url = f"{self.settings.api_url}/agents/v1.0/"
 
         self.body = {
             "routes": [route.to_json_inventory() for route in routes.values()],
         }
 
         session_id = self.settings.config.session_id
```

### Comparing `contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/application_update.py` & `contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/application_update.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/base_ts_message.py` & `contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/base_ts_message.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/effective_config.py` & `contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/effective_config.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/heartbeat.py` & `contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/heartbeat.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/library_usage.py` & `contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/library_usage.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/observed_route.py` & `contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/observed_route.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/preflight.py` & `contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/preflight.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/reporting/teamserver_messages/server_activity.py` & `contrast_agent-8.2.0/src/contrast/reporting/teamserver_messages/server_activity.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/__init__.py` & `contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/application_settings.py` & `contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/application_settings.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/ng_application_settings.py` & `contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/ng_application_settings.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/ng_server_settings.py` & `contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/ng_server_settings.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/protect_rule.py` & `contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/protect_rule.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/sampling.py` & `contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/sampling.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/reporting/teamserver_responses/server_settings.py` & `contrast_agent-8.2.0/src/contrast/reporting/teamserver_responses/server_settings.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/scripts/fix_interpreter_permissions.py` & `contrast_agent-8.2.0/src/contrast/scripts/fix_interpreter_permissions.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/scripts/propagator_check.py` & `contrast_agent-8.2.0/src/contrast/scripts/propagator_check.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/scripts/runner.py` & `contrast_agent-8.2.0/src/contrast/scripts/runner.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/scripts/validate_config.py` & `contrast_agent-8.2.0/src/contrast/scripts/validate_config.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/assess/duck_utils.py` & `contrast_agent-8.2.0/src/contrast/utils/assess/duck_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/assess/formatting/base.py` & `contrast_agent-8.2.0/src/contrast/utils/assess/formatting/base.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/assess/formatting/tokenize_cformat.py` & `contrast_agent-8.2.0/src/contrast/utils/assess/formatting/tokenize_cformat.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/assess/formatting/tokenize_format.py` & `contrast_agent-8.2.0/src/contrast/utils/assess/formatting/tokenize_format.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/assess/stream_utils.py` & `contrast_agent-8.2.0/src/contrast/utils/assess/stream_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/assess/tag_utils.py` & `contrast_agent-8.2.0/src/contrast/utils/assess/tag_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/assess/tracking_util.py` & `contrast_agent-8.2.0/src/contrast/utils/assess/tracking_util.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/base64_utils.py` & `contrast_agent-8.2.0/src/contrast/utils/base64_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/configuration_utils.py` & `contrast_agent-8.2.0/src/contrast/utils/configuration_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/context_tracker.py` & `contrast_agent-8.2.0/src/contrast/utils/context_tracker.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/decorators.py` & `contrast_agent-8.2.0/src/contrast/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/deprecated_middleware.py` & `contrast_agent-8.2.0/src/contrast/utils/deprecated_middleware.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/environ.py` & `contrast_agent-8.2.0/src/contrast/utils/environ.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/exceptions/wrong_django_middleware_exception.py` & `contrast_agent-8.2.0/src/contrast/utils/exceptions/wrong_django_middleware_exception.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/ignored_modules.py` & `contrast_agent-8.2.0/src/contrast/utils/ignored_modules.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/library_reader/library_reader.py` & `contrast_agent-8.2.0/src/contrast/utils/library_reader/library_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,14 @@
 
     Created package is added to the output for the process
 
     :param dist: Name of the python distribution we are analyzing
     :return: A dictionary containing contrast-relevant information about the current distribution
     """
     excluded_files = ("setup.py",)
-    name = dist.lower()
     metadata = importlib_metadata.metadata(dist)
     version = metadata.get("Version", "")
     url = metadata.get("Home-page", "")
     all_files = importlib_get_files(dist)
     path = None
 
     if all_files is None:
@@ -148,19 +147,19 @@
         for f in all_files
         if f.name.endswith((PY_SUFFIX, SO_SUFFIX))
         and f.name not in excluded_files
         and (path := os.path.realpath(str(f.locate())))
     }
 
     file_count = len(all_modules)
-    library_hash = get_hash(name, version)
+    library_hash = get_hash(dist, version)
 
     used_files = search_modules(all_modules)
 
-    result = create_package(version, file_count, name, url, library_hash)
+    result = create_package(version, file_count, dist, url, library_hash)
     result["used_files"] = used_files
 
     return result
 
 
 def create_package(version, class_count, name, url, sha):
     """
```

### Comparing `contrast_agent-8.1.0/src/contrast/utils/library_reader/patched_state.py` & `contrast_agent-8.2.0/src/contrast/utils/library_reader/patched_state.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/library_reader/utils.py` & `contrast_agent-8.2.0/src/contrast/utils/library_reader/utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/loggers/logger.py` & `contrast_agent-8.2.0/src/contrast/utils/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/loggers/structlog.py` & `contrast_agent-8.2.0/src/contrast/utils/loggers/structlog.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/module_parser.py` & `contrast_agent-8.2.0/src/contrast/utils/module_parser.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/namespace.py` & `contrast_agent-8.2.0/src/contrast/utils/namespace.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/object_utils.py` & `contrast_agent-8.2.0/src/contrast/utils/object_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/patch_utils.py` & `contrast_agent-8.2.0/src/contrast/utils/patch_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,17 +85,18 @@
     Not all patches will have policy. Some patch locations are used solely to apply
     proxies or do library analysis, and so no policy exists for those locations.
     Callers can indicate this by passing "" or None for `loc_name`, in which case no
     patch policy will be retrieved.
     """
     original_func = getattr(owner, attr_name)
 
-    # We don't expect this to ever really happen except possibly in test code;
-    # particularly in framework tests. Eventually we may just want to reverse patches
-    # between test cases rather than have some awkward logic here.
+    # In most cases, we don't want to patch a function that has already been patched.
+    # Sometimes we do, though, so we have a `force` flag to allow it.
+    # An examples of when we might want to force a patch is applying automatic
+    # CommonMiddlewarePatch with route coverage patches.
     if patch_manager.is_patched(original_func) and not force:
         return
 
     from contrast.agent.policy import registry
 
     loc_name = owner_name if owner_name is not None else get_name(owner)
```

### Comparing `contrast_agent-8.1.0/src/contrast/utils/pattern_builder.py` & `contrast_agent-8.2.0/src/contrast/utils/pattern_builder.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/profiler.py` & `contrast_agent-8.2.0/src/contrast/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/safe_import.py` & `contrast_agent-8.2.0/src/contrast/utils/safe_import.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/singleton.py` & `contrast_agent-8.2.0/src/contrast/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/stack_trace_utils.py` & `contrast_agent-8.2.0/src/contrast/utils/stack_trace_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/stdlib_modules.py` & `contrast_agent-8.2.0/src/contrast/utils/stdlib_modules.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/utils/string_utils.py` & `contrast_agent-8.2.0/src/contrast/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast/wsgi/middleware.py` & `contrast_agent-8.2.0/src/contrast/wsgi/middleware.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from contrast.agent import agent_state, scope, request_state
 from contrast.agent.policy.trigger_node import TriggerNode
 from contrast.agent.middlewares.base_middleware import (
     BaseMiddleware,
     log_request_start_and_end,
 )
 from contrast.agent.middlewares.environ_tracker import track_environ_sources
-from contrast.utils.decorators import cached_property, fail_quietly
+from contrast.utils.decorators import cached_property
 from contrast.utils.safe_import import safe_import_list
 from contrast.utils.assess.duck_utils import safe_getattr_list
 
 from contrast_vendor import structlog as logging
 from contrast.utils import Profiler
 
 logger = logging.getLogger("contrast")
@@ -155,26 +155,10 @@
         )
 
         return (
             TriggerNode(module, class_name, instance_method, method_name, "RETURN"),
             args,
         )
 
-    @fail_quietly("Unable to get WSGI view func")
-    def get_view_func(self, _):
-        """
-        While most frameworks define view functions, WSGI doesn't so we will rely
-        on the path information for reporting.
-        If there is no path information, return None
-
-        :param request: RequestContext instance
-        :return: string of path information for this request or None
-        """
-        return self.request_path or None
-
-    @fail_quietly("Unable to build route", return_value="")
-    def build_route(self, view_func, url):
-        return url.replace("/", "")
-
     @cached_property
     def name(self):
         return "wsgi"
```

### Comparing `contrast_agent-8.1.0/src/contrast_agent.egg-info/SOURCES.txt` & `contrast_agent-8.2.0/src/contrast_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_rewriter/__init__.py` & `contrast_agent-8.2.0/src/contrast_rewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/__init__.py` & `contrast_agent-8.2.0/src/contrast_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/LICENSE` & `contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/__init__.py` & `contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_adapters.py` & `contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_collections.py` & `contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_compat.py` & `contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_functools.py` & `contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_itertools.py` & `contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_meta.py` & `contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/_text.py` & `contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/importlib_metadata/compat/py39.py` & `contrast_agent-8.2.0/src/contrast_vendor/importlib_metadata/compat/py39.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/isort/LICENSE` & `contrast_agent-8.2.0/src/contrast_vendor/isort/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py27.py` & `contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py27.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py310.py` & `contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py310.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py311.py` & `contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py311.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py312.py` & `contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py312.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py36.py` & `contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py36.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py37.py` & `contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py37.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py38.py` & `contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py38.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/isort/stdlibs/py39.py` & `contrast_agent-8.2.0/src/contrast_vendor/isort/stdlibs/py39.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ported_cpython_code/PYTHON_SOFTWARE_FOUNDATION_LICENSE` & `contrast_agent-8.2.0/src/contrast_vendor/ported_cpython_code/PYTHON_SOFTWARE_FOUNDATION_LICENSE`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ported_cpython_code/import_functionality.py` & `contrast_agent-8.2.0/src/contrast_vendor/ported_cpython_code/import_functionality.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/LICENSE` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/__init__.py` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/comments.py` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/comments.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/compat.py` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/compat.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/composer.py` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/constructor.py` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/cyaml.py` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/dumper.py` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/emitter.py` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/error.py` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/error.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/events.py` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/events.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/loader.py` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/main.py` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/main.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/nodes.py` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/parser.py` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/reader.py` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/representer.py` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/resolver.py` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/scalarbool.py` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/scalarbool.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/scalarfloat.py` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/scalarfloat.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/scalarint.py` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/scalarint.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/scalarstring.py` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/scalarstring.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/scanner.py` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/serializer.py` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/tag.py` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/tag.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/timestamp.py` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/timestamp.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/tokens.py` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/ruamel/yaml/util.py` & `contrast_agent-8.2.0/src/contrast_vendor/ruamel/yaml/util.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/structlog/LICENSE-APACHE` & `contrast_agent-8.2.0/src/contrast_vendor/structlog/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/structlog/LICENSE-MIT` & `contrast_agent-8.2.0/src/contrast_vendor/structlog/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/structlog/__init__.py` & `contrast_agent-8.2.0/src/contrast_vendor/structlog/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/structlog/_base.py` & `contrast_agent-8.2.0/src/contrast_vendor/structlog/_base.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/structlog/_config.py` & `contrast_agent-8.2.0/src/contrast_vendor/structlog/_config.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/structlog/_frames.py` & `contrast_agent-8.2.0/src/contrast_vendor/structlog/_frames.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/structlog/_generic.py` & `contrast_agent-8.2.0/src/contrast_vendor/structlog/_generic.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/structlog/_greenlets.py` & `contrast_agent-8.2.0/src/contrast_vendor/structlog/_greenlets.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/structlog/_log_levels.py` & `contrast_agent-8.2.0/src/contrast_vendor/structlog/_log_levels.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/structlog/_native.py` & `contrast_agent-8.2.0/src/contrast_vendor/structlog/_native.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/structlog/_output.py` & `contrast_agent-8.2.0/src/contrast_vendor/structlog/_output.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/structlog/_utils.py` & `contrast_agent-8.2.0/src/contrast_vendor/structlog/_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/structlog/contextvars.py` & `contrast_agent-8.2.0/src/contrast_vendor/structlog/contextvars.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/structlog/dev.py` & `contrast_agent-8.2.0/src/contrast_vendor/structlog/dev.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/structlog/processors.py` & `contrast_agent-8.2.0/src/contrast_vendor/structlog/processors.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/structlog/stdlib.py` & `contrast_agent-8.2.0/src/contrast_vendor/structlog/stdlib.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/structlog/testing.py` & `contrast_agent-8.2.0/src/contrast_vendor/structlog/testing.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/structlog/threadlocal.py` & `contrast_agent-8.2.0/src/contrast_vendor/structlog/threadlocal.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/structlog/tracebacks.py` & `contrast_agent-8.2.0/src/contrast_vendor/structlog/tracebacks.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/structlog/twisted.py` & `contrast_agent-8.2.0/src/contrast_vendor/structlog/twisted.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/structlog/types.py` & `contrast_agent-8.2.0/src/contrast_vendor/structlog/types.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/structlog/typing.py` & `contrast_agent-8.2.0/src/contrast_vendor/structlog/typing.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/webob/__init__.py` & `contrast_agent-8.2.0/src/contrast_vendor/webob/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/webob/acceptparse.py` & `contrast_agent-8.2.0/src/contrast_vendor/webob/acceptparse.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/webob/byterange.py` & `contrast_agent-8.2.0/src/contrast_vendor/webob/byterange.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/webob/cachecontrol.py` & `contrast_agent-8.2.0/src/contrast_vendor/webob/cachecontrol.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/webob/client.py` & `contrast_agent-8.2.0/src/contrast_vendor/webob/client.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/webob/compat.py` & `contrast_agent-8.2.0/src/contrast_vendor/webob/compat.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/webob/cookies.py` & `contrast_agent-8.2.0/src/contrast_vendor/webob/cookies.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/webob/datetime_utils.py` & `contrast_agent-8.2.0/src/contrast_vendor/webob/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/webob/dec.py` & `contrast_agent-8.2.0/src/contrast_vendor/webob/dec.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/webob/descriptors.py` & `contrast_agent-8.2.0/src/contrast_vendor/webob/descriptors.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/webob/etag.py` & `contrast_agent-8.2.0/src/contrast_vendor/webob/etag.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/webob/exc.py` & `contrast_agent-8.2.0/src/contrast_vendor/webob/exc.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/webob/headers.py` & `contrast_agent-8.2.0/src/contrast_vendor/webob/headers.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/webob/license.txt` & `contrast_agent-8.2.0/src/contrast_vendor/webob/license.txt`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/webob/multidict.py` & `contrast_agent-8.2.0/src/contrast_vendor/webob/multidict.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/webob/request.py` & `contrast_agent-8.2.0/src/contrast_vendor/webob/request.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/webob/response.py` & `contrast_agent-8.2.0/src/contrast_vendor/webob/response.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/webob/static.py` & `contrast_agent-8.2.0/src/contrast_vendor/webob/static.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/webob/util.py` & `contrast_agent-8.2.0/src/contrast_vendor/webob/util.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/wrapt/LICENSE` & `contrast_agent-8.2.0/src/contrast_vendor/wrapt/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/wrapt/__init__.py` & `contrast_agent-8.2.0/src/contrast_vendor/wrapt/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/wrapt/arguments.py` & `contrast_agent-8.2.0/src/contrast_vendor/wrapt/arguments.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/wrapt/decorators.py` & `contrast_agent-8.2.0/src/contrast_vendor/wrapt/decorators.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/wrapt/importer.py` & `contrast_agent-8.2.0/src/contrast_vendor/wrapt/importer.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/wrapt/patches.py` & `contrast_agent-8.2.0/src/contrast_vendor/wrapt/patches.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/wrapt/weakrefs.py` & `contrast_agent-8.2.0/src/contrast_vendor/wrapt/weakrefs.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/wrapt/wrappers.py` & `contrast_agent-8.2.0/src/contrast_vendor/wrapt/wrappers.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/zipp/LICENSE` & `contrast_agent-8.2.0/src/contrast_vendor/zipp/LICENSE`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/zipp/__init__.py` & `contrast_agent-8.2.0/src/contrast_vendor/zipp/__init__.py`

 * *Files identical despite different names*

### Comparing `contrast_agent-8.1.0/src/contrast_vendor/zipp/glob.py` & `contrast_agent-8.2.0/src/contrast_vendor/zipp/glob.py`

 * *Files identical despite different names*

