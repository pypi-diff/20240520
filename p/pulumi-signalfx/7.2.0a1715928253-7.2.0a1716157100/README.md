# Comparing `tmp/pulumi_signalfx-7.2.0a1715928253.tar.gz` & `tmp/pulumi_signalfx-7.2.0a1716157100.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_signalfx-7.2.0a1715928253.tar", last modified: Fri May 17 06:55:27 2024, max compression
+gzip compressed data, was "pulumi_signalfx-7.2.0a1716157100.tar", last modified: Sun May 19 22:22:25 2024, max compression
```

## Comparing `pulumi_signalfx-7.2.0a1715928253.tar` & `pulumi_signalfx-7.2.0a1716157100.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:55:27.409935 pulumi_signalfx-7.2.0a1715928253/
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-17 06:55:27.409935 pulumi_signalfx-7.2.0a1715928253/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:55:27.401934 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/
--rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   153334 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    19007 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/alert_muting_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:55:27.405934 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/aws/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10582 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/aws/external_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    82462 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/aws/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9992 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/aws/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/aws/token_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:55:27.405934 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/azure/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    56590 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/azure/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/azure/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:55:27.405934 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    54932 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    33368 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/dashboard_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    26221 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/data_link.py
--rw-r--r--   0 runner    (1001) docker     (127)    65421 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/detector.py
--rw-r--r--   0 runner    (1001) docker     (127)    18692 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/event_feed_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:55:27.405934 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/gcp/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    34998 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/gcp/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/gcp/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/get_dimension_values.py
--rw-r--r--   0 runner    (1001) docker     (127)    44252 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/heatmap_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:55:27.405934 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/jira/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/jira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34217 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/jira/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    65676 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/list_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:55:27.409935 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/log/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/log/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/log/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/log/timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    26770 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/log/view.py
--rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/metric_ruleset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:55:27.409935 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/opsgenie/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/opsgenie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12501 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/opsgenie/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    24829 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/org_token.py
--rw-r--r--   0 runner    (1001) docker     (127)   138325 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:55:27.409935 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/pagerduty/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/pagerduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/pagerduty/get_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    10441 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/pagerduty/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:55:27.409935 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/servicenow/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/servicenow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28846 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/servicenow/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    44927 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/single_value_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:55:27.409935 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/slack/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/slack/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    30506 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/slo.py
--rw-r--r--   0 runner    (1001) docker     (127)    32559 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/table_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    29851 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    11236 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/text_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    85614 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/time_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:55:27.409935 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/victorops/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/victorops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/victorops/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14929 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/webhook_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:55:27.409935 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-17 06:55:27.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-17 06:55:27.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 06:55:27.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-17 06:55:27.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-17 06:55:27.000000 pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-17 06:55:21.000000 pulumi_signalfx-7.2.0a1715928253/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 06:55:27.409935 pulumi_signalfx-7.2.0a1715928253/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:22:25.744620 pulumi_signalfx-7.2.0a1716157100/
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-19 22:22:25.744620 pulumi_signalfx-7.2.0a1716157100/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:22:25.736620 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/
+-rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   154935 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19007 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/alert_muting_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:22:25.736620 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/aws/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10582 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/aws/external_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82462 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/aws/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9992 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/aws/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/aws/token_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:22:25.736620 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/azure/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56590 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/azure/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/azure/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:22:25.740620 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54932 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33368 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/dashboard_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26221 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/data_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65421 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18692 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/event_feed_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:22:25.740620 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/gcp/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34998 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/gcp/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/gcp/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/get_dimension_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44252 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/heatmap_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:22:25.740620 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/jira/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/jira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34217 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/jira/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65676 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/list_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:22:25.740620 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/log/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/log/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/log/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/log/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26770 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/log/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/metric_ruleset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:22:25.740620 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/opsgenie/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/opsgenie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12501 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/opsgenie/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24829 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/org_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)   139713 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:22:25.740620 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/pagerduty/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/pagerduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/pagerduty/get_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10441 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/pagerduty/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:22:25.740620 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/servicenow/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/servicenow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28846 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/servicenow/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44927 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/single_value_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:22:25.740620 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/slack/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/slack/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31432 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/slo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32559 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/table_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29851 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11236 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/text_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85614 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/time_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:22:25.740620 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/victorops/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/victorops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/victorops/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14929 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/webhook_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:22:25.740620 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-19 22:22:25.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-19 22:22:25.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 22:22:25.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-19 22:22:25.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-19 22:22:25.000000 pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-19 22:22:19.000000 pulumi_signalfx-7.2.0a1716157100/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 22:22:25.744620 pulumi_signalfx-7.2.0a1716157100/setup.cfg
```

### Comparing `pulumi_signalfx-7.2.0a1715928253/PKG-INFO` & `pulumi_signalfx-7.2.0a1716157100/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_signalfx
-Version: 7.2.0a1715928253
+Version: 7.2.0a1716157100
 Summary: A Pulumi package for creating and managing SignalFx resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-signalfx
 Keywords: pulumi,signalfx
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_signalfx-7.2.0a1715928253/README.md` & `pulumi_signalfx-7.2.0a1716157100/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/__init__.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/_inputs.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2713,26 +2713,34 @@
 
 @pulumi.input_type
 class SloTargetArgs:
     def __init__(__self__, *,
                  alert_rules: pulumi.Input[Sequence[pulumi.Input['SloTargetAlertRuleArgs']]],
                  slo: pulumi.Input[float],
                  type: pulumi.Input[str],
-                 compliance_period: Optional[pulumi.Input[str]] = None):
+                 compliance_period: Optional[pulumi.Input[str]] = None,
+                 cycle_start: Optional[pulumi.Input[str]] = None,
+                 cycle_type: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[Sequence[pulumi.Input['SloTargetAlertRuleArgs']]] alert_rules: SLO alert rules
         :param pulumi.Input[float] slo: Target value in the form of a percentage
         :param pulumi.Input[str] type: SLO target type can be the following type: `RollingWindow`
         :param pulumi.Input[str] compliance_period: (Required for `RollingWindow` type) Compliance period of this SLO. This value must be within the range of 1d (1 days) to 30d (30 days), inclusive.
+        :param pulumi.Input[str] cycle_start: (Optional for `CalendarWindow` type)  It can be used to change the cycle start time. For example, you can specify sunday as the start of the week (instead of the default monday)
+        :param pulumi.Input[str] cycle_type: (Required for `CalendarWindow` type) The cycle type of the calendar window, e.g. week, month.
         """
         pulumi.set(__self__, "alert_rules", alert_rules)
         pulumi.set(__self__, "slo", slo)
         pulumi.set(__self__, "type", type)
         if compliance_period is not None:
             pulumi.set(__self__, "compliance_period", compliance_period)
+        if cycle_start is not None:
+            pulumi.set(__self__, "cycle_start", cycle_start)
+        if cycle_type is not None:
+            pulumi.set(__self__, "cycle_type", cycle_type)
 
     @property
     @pulumi.getter(name="alertRules")
     def alert_rules(self) -> pulumi.Input[Sequence[pulumi.Input['SloTargetAlertRuleArgs']]]:
         """
         SLO alert rules
         """
@@ -2774,14 +2782,38 @@
         """
         return pulumi.get(self, "compliance_period")
 
     @compliance_period.setter
     def compliance_period(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "compliance_period", value)
 
+    @property
+    @pulumi.getter(name="cycleStart")
+    def cycle_start(self) -> Optional[pulumi.Input[str]]:
+        """
+        (Optional for `CalendarWindow` type)  It can be used to change the cycle start time. For example, you can specify sunday as the start of the week (instead of the default monday)
+        """
+        return pulumi.get(self, "cycle_start")
+
+    @cycle_start.setter
+    def cycle_start(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cycle_start", value)
+
+    @property
+    @pulumi.getter(name="cycleType")
+    def cycle_type(self) -> Optional[pulumi.Input[str]]:
+        """
+        (Required for `CalendarWindow` type) The cycle type of the calendar window, e.g. week, month.
+        """
+        return pulumi.get(self, "cycle_type")
+
+    @cycle_type.setter
+    def cycle_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cycle_type", value)
+
 
 @pulumi.input_type
 class SloTargetAlertRuleArgs:
     def __init__(__self__, *,
                  rules: pulumi.Input[Sequence[pulumi.Input['SloTargetAlertRuleRuleArgs']]],
                  type: pulumi.Input[str]):
         """
```

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/_utilities.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/alert_muting_rule.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/alert_muting_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/aws/_inputs.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/aws/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/aws/external_integration.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/aws/external_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/aws/integration.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/aws/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/aws/outputs.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/aws/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/aws/token_integration.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/aws/token_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/azure/_inputs.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/azure/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/azure/integration.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/azure/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/azure/outputs.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/azure/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/config/__init__.pyi` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/config/vars.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/dashboard.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/dashboard_group.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/dashboard_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/data_link.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/data_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/detector.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/detector.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/event_feed_chart.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/event_feed_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/gcp/_inputs.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/gcp/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/gcp/integration.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/gcp/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/gcp/outputs.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/gcp/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/get_dimension_values.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/get_dimension_values.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/heatmap_chart.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/heatmap_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/jira/integration.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/jira/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/list_chart.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/list_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/log/_inputs.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/log/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/log/outputs.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/log/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/log/timeline.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/log/timeline.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/log/view.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/log/view.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/metric_ruleset.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/metric_ruleset.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/opsgenie/integration.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/opsgenie/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/org_token.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/org_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/outputs.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2576,14 +2576,18 @@
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "alertRules":
             suggest = "alert_rules"
         elif key == "compliancePeriod":
             suggest = "compliance_period"
+        elif key == "cycleStart":
+            suggest = "cycle_start"
+        elif key == "cycleType":
+            suggest = "cycle_type"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in SloTarget. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         SloTarget.__key_warning(key)
         return super().__getitem__(key)
@@ -2592,26 +2596,34 @@
         SloTarget.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  alert_rules: Sequence['outputs.SloTargetAlertRule'],
                  slo: float,
                  type: str,
-                 compliance_period: Optional[str] = None):
+                 compliance_period: Optional[str] = None,
+                 cycle_start: Optional[str] = None,
+                 cycle_type: Optional[str] = None):
         """
         :param Sequence['SloTargetAlertRuleArgs'] alert_rules: SLO alert rules
         :param float slo: Target value in the form of a percentage
         :param str type: SLO target type can be the following type: `RollingWindow`
         :param str compliance_period: (Required for `RollingWindow` type) Compliance period of this SLO. This value must be within the range of 1d (1 days) to 30d (30 days), inclusive.
+        :param str cycle_start: (Optional for `CalendarWindow` type)  It can be used to change the cycle start time. For example, you can specify sunday as the start of the week (instead of the default monday)
+        :param str cycle_type: (Required for `CalendarWindow` type) The cycle type of the calendar window, e.g. week, month.
         """
         pulumi.set(__self__, "alert_rules", alert_rules)
         pulumi.set(__self__, "slo", slo)
         pulumi.set(__self__, "type", type)
         if compliance_period is not None:
             pulumi.set(__self__, "compliance_period", compliance_period)
+        if cycle_start is not None:
+            pulumi.set(__self__, "cycle_start", cycle_start)
+        if cycle_type is not None:
+            pulumi.set(__self__, "cycle_type", cycle_type)
 
     @property
     @pulumi.getter(name="alertRules")
     def alert_rules(self) -> Sequence['outputs.SloTargetAlertRule']:
         """
         SLO alert rules
         """
@@ -2637,14 +2649,30 @@
     @pulumi.getter(name="compliancePeriod")
     def compliance_period(self) -> Optional[str]:
         """
         (Required for `RollingWindow` type) Compliance period of this SLO. This value must be within the range of 1d (1 days) to 30d (30 days), inclusive.
         """
         return pulumi.get(self, "compliance_period")
 
+    @property
+    @pulumi.getter(name="cycleStart")
+    def cycle_start(self) -> Optional[str]:
+        """
+        (Optional for `CalendarWindow` type)  It can be used to change the cycle start time. For example, you can specify sunday as the start of the week (instead of the default monday)
+        """
+        return pulumi.get(self, "cycle_start")
+
+    @property
+    @pulumi.getter(name="cycleType")
+    def cycle_type(self) -> Optional[str]:
+        """
+        (Required for `CalendarWindow` type) The cycle type of the calendar window, e.g. week, month.
+        """
+        return pulumi.get(self, "cycle_type")
+
 
 @pulumi.output_type
 class SloTargetAlertRule(dict):
     def __init__(__self__, *,
                  rules: Sequence['outputs.SloTargetAlertRuleRule'],
                  type: str):
         """
```

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/pagerduty/get_integration.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/pagerduty/get_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/pagerduty/integration.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/pagerduty/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/provider.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/servicenow/integration.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/servicenow/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/single_value_chart.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/single_value_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/slack/integration.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/slack/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/slo.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/slo.py`

 * *Files 6% similar despite different names*

```diff
@@ -252,42 +252,44 @@
 
         ## Arguments
 
         * `name` - (Required) Name of the SLO. Each SLO name must be unique within an organization.
         * `description` - (Optional) Description of the SLO.
         * `type` - (Required) Type of the SLO. Currently just: `"RequestBased"` is supported.
         * `input` - (Required) Properties to configure an SLO object inputs
-          * `program_text` - (Required) SignalFlow program and arguments text strings that define the streams used as successful event count and total event count
-          * `good_events_label` - (Required) Label used in `"program_text"` that refers to the data block which contains the stream of successful events
-          * `total_events_label` - (Required) Label used in `"program_text"` that refers to the data block which contains the stream of total events
+            * `program_text` - (Required) SignalFlow program and arguments text strings that define the streams used as successful event count and total event count
+            * `good_events_label` - (Required) Label used in `"program_text"` that refers to the data block which contains the stream of successful events
+            * `total_events_label` - (Required) Label used in `"program_text"` that refers to the data block which contains the stream of total events
         * `target` - (Required) Define target value of the service level indicator in the appropriate time period.
-          * `type` - (Required) SLO target type can be the following type: `"RollingWindow"`
-          * `compliance_period` - (Required for `"RollingWindow"` type) Compliance period of this SLO. This value must be within the range of 1d (1 days) to 30d (30 days), inclusive.
-          * `slo` - (Required) Target value in the form of a percentage
-          * `alert_rule` - (Required) List of alert rules you want to set for this SLO target. An SLO alert rule of type BREACH is always required.
-            * `type` - (Required) SLO alert rule can be one of the following types: BREACH, ERROR_BUDGET_LEFT, BURN_RATE. Within an SLO object, you can only specify one SLO alert_rule per type. For example, you can't specify two alert_rule of type BREACH. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
-            * `rule` - (Required) Set of rules used for alerting.
-                * `severity` - (Required) The severity of the rule, must be one of: `"Critical"`, `"Major"`, `"Minor"`, `"Warning"`, `"Info"`.
-                * `description` - (Optional) Description for the rule. Displays as the alert condition in the Alert Rules tab of the detector editor in the web UI.
-                * `disabled` - (Optional) When true, notifications and events will not be generated for the detect label. `false` by default.
-                * `notifications` - (Optional) List of strings specifying where notifications will be sent when an incident occurs. See [Create SLO](https://dev.splunk.com/observability/reference/api/slo/latest#endpoint-create-new-slo) for more info.
-                * `parameterized_body` - (Optional) Custom notification message body when an alert is triggered. See [Alert message](https://docs.splunk.com/observability/en/alerts-detectors-notifications/create-detectors-for-alerts.html#alert-messages) for more info.
-                * `parameterized_subject` - (Optional) Custom notification message subject when an alert is triggered. See [Alert message](https://docs.splunk.com/observability/en/alerts-detectors-notifications/create-detectors-for-alerts.html#alert-messages) for more info.
-                * `runbook_url` - (Optional) URL of page to consult when an alert is triggered. This can be used with custom notification messages.
-                * `tip` - (Optional) Plain text suggested first course of action, such as a command line to execute. This can be used with custom notification messages.
-                * `parameters` - (Optional) Parameters for the SLO alert rule. Each SLO alert rule type accepts different parameters. If not specified, default parameters are used.
-                  * `fire_lasting` - (Optional) Duration that indicates how long the alert condition is met before the alert is triggered. The value must be positive and smaller than the compliance period of the SLO target. Note: `"BREACH"` and `"ERROR_BUDGET_LEFT"` alert rules use the fireLasting parameter. Default: `"5m"`
-                  * `percent_of_lasting` - (Optional) Percentage of the `"fire_lasting"` duration that the alert condition is met before the alert is triggered. Note: `"BREACH"` and `"ERROR_BUDGET_LEFT"` alert rules use the `"percent_of_lasting"` parameter. Default: `100`
-                  * `percent_error_budget_left` - (Optional) Error budget must be equal to or smaller than this percentage for the alert to be triggered. Note: `"ERROR_BUDGET_LEFT"` alert rules use the `"percent_error_budget_left"` parameter. Default: `100`
-                  * `short_window_1` - (Optional) Short window 1 used in burn rate alert calculation. This value must be longer than 1/30 of `"long_window_1"`. Note: `"BURN_RATE"` alert rules use the `"short_window_1"` parameter. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
-                  * `short_window_2` - (Optional) Short window 2 used in burn rate alert calculation. This value must be longer than 1/30 of `"long_window_2"`. Note: `"BURN_RATE"` alert rules use the `"short_window_2"` parameter. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
-                  * `long_window_1` - (Optional) Long window 1 used in burn rate alert calculation. This value must be longer than `"short_window_1"` and shorter than 90 days. Note: `"BURN_RATE"` alert rules use the `"long_window_1"` parameter. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
-                  * `long_window_2` - (Optional) Long window 2 used in burn rate alert calculation. This value must be longer than `"short_window_2"` and shorter than 90 days. Note: `"BURN_RATE"` alert rules use the `"long_window_2"` parameter. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
-                  * `burn_rate_threshold_1` - (Optional) Burn rate threshold 1 used in burn rate alert calculation. This value must be between 0 and 100/(100-SLO target). Note: `"BURN_RATE"` alert rules use the `"burn_rate_threshold_1"` parameter. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
-                  * `burn_rate_threshold_2` - (Optional) Burn rate threshold 2 used in burn rate alert calculation. This value must be between 0 and 100/(100-SLO target). Note: `"BURN_RATE"` alert rules use the `"burn_rate_threshold_2"` parameter. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
+            * `type` - (Required) SLO target type can be the following type: `"RollingWindow"`, `"CalendarWindow"`
+            * `compliance_period` - (Required for `"RollingWindow"` type) Compliance period of this SLO. This value must be within the range of 1d (1 days) to 30d (30 days), inclusive.
+            * `cycle_type` - (Required for `CalendarWindow` type) The cycle type of the calendar window, e.g. week, month.
+            * `cycle_start` - (Optional for `CalendarWindow` type)  It can be used to change the cycle start time. For example, you can specify sunday as the start of the week (instead of the default monday)
+            * `slo` - (Required) Target value in the form of a percentage
+            * `alert_rule` - (Required) List of alert rules you want to set for this SLO target. An SLO alert rule of type BREACH is always required.
+                * `type` - (Required) SLO alert rule can be one of the following types: BREACH, ERROR_BUDGET_LEFT, BURN_RATE. Within an SLO object, you can only specify one SLO alert_rule per type. For example, you can't specify two alert_rule of type BREACH. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
+                * `rule` - (Required) Set of rules used for alerting.
+                    * `severity` - (Required) The severity of the rule, must be one of: `"Critical"`, `"Major"`, `"Minor"`, `"Warning"`, `"Info"`.
+                    * `description` - (Optional) Description for the rule. Displays as the alert condition in the Alert Rules tab of the detector editor in the web UI.
+                    * `disabled` - (Optional) When true, notifications and events will not be generated for the detect label. `false` by default.
+                    * `notifications` - (Optional) List of strings specifying where notifications will be sent when an incident occurs. See [Create SLO](https://dev.splunk.com/observability/reference/api/slo/latest#endpoint-create-new-slo) for more info.
+                    * `parameterized_body` - (Optional) Custom notification message body when an alert is triggered. See [Alert message](https://docs.splunk.com/observability/en/alerts-detectors-notifications/create-detectors-for-alerts.html#alert-messages) for more info.
+                    * `parameterized_subject` - (Optional) Custom notification message subject when an alert is triggered. See [Alert message](https://docs.splunk.com/observability/en/alerts-detectors-notifications/create-detectors-for-alerts.html#alert-messages) for more info.
+                    * `runbook_url` - (Optional) URL of page to consult when an alert is triggered. This can be used with custom notification messages.
+                    * `tip` - (Optional) Plain text suggested first course of action, such as a command line to execute. This can be used with custom notification messages.
+                    * `parameters` - (Optional) Parameters for the SLO alert rule. Each SLO alert rule type accepts different parameters. If not specified, default parameters are used.
+                        * `fire_lasting` - (Optional) Duration that indicates how long the alert condition is met before the alert is triggered. The value must be positive and smaller than the compliance period of the SLO target. Note: `"BREACH"` and `"ERROR_BUDGET_LEFT"` alert rules use the fireLasting parameter. Default: `"5m"`
+                        * `percent_of_lasting` - (Optional) Percentage of the `"fire_lasting"` duration that the alert condition is met before the alert is triggered. Note: `"BREACH"` and `"ERROR_BUDGET_LEFT"` alert rules use the `"percent_of_lasting"` parameter. Default: `100`
+                        * `percent_error_budget_left` - (Optional) Error budget must be equal to or smaller than this percentage for the alert to be triggered. Note: `"ERROR_BUDGET_LEFT"` alert rules use the `"percent_error_budget_left"` parameter. Default: `100`
+                        * `short_window_1` - (Optional) Short window 1 used in burn rate alert calculation. This value must be longer than 1/30 of `"long_window_1"`. Note: `"BURN_RATE"` alert rules use the `"short_window_1"` parameter. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
+                        * `short_window_2` - (Optional) Short window 2 used in burn rate alert calculation. This value must be longer than 1/30 of `"long_window_2"`. Note: `"BURN_RATE"` alert rules use the `"short_window_2"` parameter. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
+                        * `long_window_1` - (Optional) Long window 1 used in burn rate alert calculation. This value must be longer than `"short_window_1"` and shorter than 90 days. Note: `"BURN_RATE"` alert rules use the `"long_window_1"` parameter. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
+                        * `long_window_2` - (Optional) Long window 2 used in burn rate alert calculation. This value must be longer than `"short_window_2"` and shorter than 90 days. Note: `"BURN_RATE"` alert rules use the `"long_window_2"` parameter. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
+                        * `burn_rate_threshold_1` - (Optional) Burn rate threshold 1 used in burn rate alert calculation. This value must be between 0 and 100/(100-SLO target). Note: `"BURN_RATE"` alert rules use the `"burn_rate_threshold_1"` parameter. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
+                        * `burn_rate_threshold_2` - (Optional) Burn rate threshold 2 used in burn rate alert calculation. This value must be between 0 and 100/(100-SLO target). Note: `"BURN_RATE"` alert rules use the `"burn_rate_threshold_2"` parameter. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: Description of the SLO
         :param pulumi.Input[pulumi.InputType['SloInputArgs']] input: SignalFlow program and arguments text strings that define the streams used as successful event count and total event
                count
         :param pulumi.Input[str] name: Name of the SLO
@@ -351,42 +353,44 @@
 
         ## Arguments
 
         * `name` - (Required) Name of the SLO. Each SLO name must be unique within an organization.
         * `description` - (Optional) Description of the SLO.
         * `type` - (Required) Type of the SLO. Currently just: `"RequestBased"` is supported.
         * `input` - (Required) Properties to configure an SLO object inputs
-          * `program_text` - (Required) SignalFlow program and arguments text strings that define the streams used as successful event count and total event count
-          * `good_events_label` - (Required) Label used in `"program_text"` that refers to the data block which contains the stream of successful events
-          * `total_events_label` - (Required) Label used in `"program_text"` that refers to the data block which contains the stream of total events
+            * `program_text` - (Required) SignalFlow program and arguments text strings that define the streams used as successful event count and total event count
+            * `good_events_label` - (Required) Label used in `"program_text"` that refers to the data block which contains the stream of successful events
+            * `total_events_label` - (Required) Label used in `"program_text"` that refers to the data block which contains the stream of total events
         * `target` - (Required) Define target value of the service level indicator in the appropriate time period.
-          * `type` - (Required) SLO target type can be the following type: `"RollingWindow"`
-          * `compliance_period` - (Required for `"RollingWindow"` type) Compliance period of this SLO. This value must be within the range of 1d (1 days) to 30d (30 days), inclusive.
-          * `slo` - (Required) Target value in the form of a percentage
-          * `alert_rule` - (Required) List of alert rules you want to set for this SLO target. An SLO alert rule of type BREACH is always required.
-            * `type` - (Required) SLO alert rule can be one of the following types: BREACH, ERROR_BUDGET_LEFT, BURN_RATE. Within an SLO object, you can only specify one SLO alert_rule per type. For example, you can't specify two alert_rule of type BREACH. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
-            * `rule` - (Required) Set of rules used for alerting.
-                * `severity` - (Required) The severity of the rule, must be one of: `"Critical"`, `"Major"`, `"Minor"`, `"Warning"`, `"Info"`.
-                * `description` - (Optional) Description for the rule. Displays as the alert condition in the Alert Rules tab of the detector editor in the web UI.
-                * `disabled` - (Optional) When true, notifications and events will not be generated for the detect label. `false` by default.
-                * `notifications` - (Optional) List of strings specifying where notifications will be sent when an incident occurs. See [Create SLO](https://dev.splunk.com/observability/reference/api/slo/latest#endpoint-create-new-slo) for more info.
-                * `parameterized_body` - (Optional) Custom notification message body when an alert is triggered. See [Alert message](https://docs.splunk.com/observability/en/alerts-detectors-notifications/create-detectors-for-alerts.html#alert-messages) for more info.
-                * `parameterized_subject` - (Optional) Custom notification message subject when an alert is triggered. See [Alert message](https://docs.splunk.com/observability/en/alerts-detectors-notifications/create-detectors-for-alerts.html#alert-messages) for more info.
-                * `runbook_url` - (Optional) URL of page to consult when an alert is triggered. This can be used with custom notification messages.
-                * `tip` - (Optional) Plain text suggested first course of action, such as a command line to execute. This can be used with custom notification messages.
-                * `parameters` - (Optional) Parameters for the SLO alert rule. Each SLO alert rule type accepts different parameters. If not specified, default parameters are used.
-                  * `fire_lasting` - (Optional) Duration that indicates how long the alert condition is met before the alert is triggered. The value must be positive and smaller than the compliance period of the SLO target. Note: `"BREACH"` and `"ERROR_BUDGET_LEFT"` alert rules use the fireLasting parameter. Default: `"5m"`
-                  * `percent_of_lasting` - (Optional) Percentage of the `"fire_lasting"` duration that the alert condition is met before the alert is triggered. Note: `"BREACH"` and `"ERROR_BUDGET_LEFT"` alert rules use the `"percent_of_lasting"` parameter. Default: `100`
-                  * `percent_error_budget_left` - (Optional) Error budget must be equal to or smaller than this percentage for the alert to be triggered. Note: `"ERROR_BUDGET_LEFT"` alert rules use the `"percent_error_budget_left"` parameter. Default: `100`
-                  * `short_window_1` - (Optional) Short window 1 used in burn rate alert calculation. This value must be longer than 1/30 of `"long_window_1"`. Note: `"BURN_RATE"` alert rules use the `"short_window_1"` parameter. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
-                  * `short_window_2` - (Optional) Short window 2 used in burn rate alert calculation. This value must be longer than 1/30 of `"long_window_2"`. Note: `"BURN_RATE"` alert rules use the `"short_window_2"` parameter. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
-                  * `long_window_1` - (Optional) Long window 1 used in burn rate alert calculation. This value must be longer than `"short_window_1"` and shorter than 90 days. Note: `"BURN_RATE"` alert rules use the `"long_window_1"` parameter. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
-                  * `long_window_2` - (Optional) Long window 2 used in burn rate alert calculation. This value must be longer than `"short_window_2"` and shorter than 90 days. Note: `"BURN_RATE"` alert rules use the `"long_window_2"` parameter. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
-                  * `burn_rate_threshold_1` - (Optional) Burn rate threshold 1 used in burn rate alert calculation. This value must be between 0 and 100/(100-SLO target). Note: `"BURN_RATE"` alert rules use the `"burn_rate_threshold_1"` parameter. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
-                  * `burn_rate_threshold_2` - (Optional) Burn rate threshold 2 used in burn rate alert calculation. This value must be between 0 and 100/(100-SLO target). Note: `"BURN_RATE"` alert rules use the `"burn_rate_threshold_2"` parameter. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
+            * `type` - (Required) SLO target type can be the following type: `"RollingWindow"`, `"CalendarWindow"`
+            * `compliance_period` - (Required for `"RollingWindow"` type) Compliance period of this SLO. This value must be within the range of 1d (1 days) to 30d (30 days), inclusive.
+            * `cycle_type` - (Required for `CalendarWindow` type) The cycle type of the calendar window, e.g. week, month.
+            * `cycle_start` - (Optional for `CalendarWindow` type)  It can be used to change the cycle start time. For example, you can specify sunday as the start of the week (instead of the default monday)
+            * `slo` - (Required) Target value in the form of a percentage
+            * `alert_rule` - (Required) List of alert rules you want to set for this SLO target. An SLO alert rule of type BREACH is always required.
+                * `type` - (Required) SLO alert rule can be one of the following types: BREACH, ERROR_BUDGET_LEFT, BURN_RATE. Within an SLO object, you can only specify one SLO alert_rule per type. For example, you can't specify two alert_rule of type BREACH. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
+                * `rule` - (Required) Set of rules used for alerting.
+                    * `severity` - (Required) The severity of the rule, must be one of: `"Critical"`, `"Major"`, `"Minor"`, `"Warning"`, `"Info"`.
+                    * `description` - (Optional) Description for the rule. Displays as the alert condition in the Alert Rules tab of the detector editor in the web UI.
+                    * `disabled` - (Optional) When true, notifications and events will not be generated for the detect label. `false` by default.
+                    * `notifications` - (Optional) List of strings specifying where notifications will be sent when an incident occurs. See [Create SLO](https://dev.splunk.com/observability/reference/api/slo/latest#endpoint-create-new-slo) for more info.
+                    * `parameterized_body` - (Optional) Custom notification message body when an alert is triggered. See [Alert message](https://docs.splunk.com/observability/en/alerts-detectors-notifications/create-detectors-for-alerts.html#alert-messages) for more info.
+                    * `parameterized_subject` - (Optional) Custom notification message subject when an alert is triggered. See [Alert message](https://docs.splunk.com/observability/en/alerts-detectors-notifications/create-detectors-for-alerts.html#alert-messages) for more info.
+                    * `runbook_url` - (Optional) URL of page to consult when an alert is triggered. This can be used with custom notification messages.
+                    * `tip` - (Optional) Plain text suggested first course of action, such as a command line to execute. This can be used with custom notification messages.
+                    * `parameters` - (Optional) Parameters for the SLO alert rule. Each SLO alert rule type accepts different parameters. If not specified, default parameters are used.
+                        * `fire_lasting` - (Optional) Duration that indicates how long the alert condition is met before the alert is triggered. The value must be positive and smaller than the compliance period of the SLO target. Note: `"BREACH"` and `"ERROR_BUDGET_LEFT"` alert rules use the fireLasting parameter. Default: `"5m"`
+                        * `percent_of_lasting` - (Optional) Percentage of the `"fire_lasting"` duration that the alert condition is met before the alert is triggered. Note: `"BREACH"` and `"ERROR_BUDGET_LEFT"` alert rules use the `"percent_of_lasting"` parameter. Default: `100`
+                        * `percent_error_budget_left` - (Optional) Error budget must be equal to or smaller than this percentage for the alert to be triggered. Note: `"ERROR_BUDGET_LEFT"` alert rules use the `"percent_error_budget_left"` parameter. Default: `100`
+                        * `short_window_1` - (Optional) Short window 1 used in burn rate alert calculation. This value must be longer than 1/30 of `"long_window_1"`. Note: `"BURN_RATE"` alert rules use the `"short_window_1"` parameter. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
+                        * `short_window_2` - (Optional) Short window 2 used in burn rate alert calculation. This value must be longer than 1/30 of `"long_window_2"`. Note: `"BURN_RATE"` alert rules use the `"short_window_2"` parameter. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
+                        * `long_window_1` - (Optional) Long window 1 used in burn rate alert calculation. This value must be longer than `"short_window_1"` and shorter than 90 days. Note: `"BURN_RATE"` alert rules use the `"long_window_1"` parameter. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
+                        * `long_window_2` - (Optional) Long window 2 used in burn rate alert calculation. This value must be longer than `"short_window_2"` and shorter than 90 days. Note: `"BURN_RATE"` alert rules use the `"long_window_2"` parameter. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
+                        * `burn_rate_threshold_1` - (Optional) Burn rate threshold 1 used in burn rate alert calculation. This value must be between 0 and 100/(100-SLO target). Note: `"BURN_RATE"` alert rules use the `"burn_rate_threshold_1"` parameter. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
+                        * `burn_rate_threshold_2` - (Optional) Burn rate threshold 2 used in burn rate alert calculation. This value must be between 0 and 100/(100-SLO target). Note: `"BURN_RATE"` alert rules use the `"burn_rate_threshold_2"` parameter. See [SLO alerts](https://docs.splunk.com/observability/en/alerts-detectors-notifications/slo/burn-rate-alerts.html) for more info.
 
         :param str resource_name: The name of the resource.
         :param SloArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/table_chart.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/table_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/team.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/text_chart.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/text_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/time_chart.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/time_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/victorops/integration.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/victorops/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx/webhook_integration.py` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx/webhook_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx.egg-info/PKG-INFO` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_signalfx
-Version: 7.2.0a1715928253
+Version: 7.2.0a1716157100
 Summary: A Pulumi package for creating and managing SignalFx resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-signalfx
 Keywords: pulumi,signalfx
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_signalfx-7.2.0a1715928253/pulumi_signalfx.egg-info/SOURCES.txt` & `pulumi_signalfx-7.2.0a1716157100/pulumi_signalfx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1715928253/pyproject.toml` & `pulumi_signalfx-7.2.0a1716157100/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_signalfx"
   description = "A Pulumi package for creating and managing SignalFx resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "signalfx"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "7.2.0a1715928253"
+  version = "7.2.0a1716157100"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-signalfx"
 
 [build-system]
```

