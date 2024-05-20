# Comparing `tmp/goblin_cbm_runner-0.3.4.tar.gz` & `tmp/goblin_cbm_runner-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goblin_cbm_runner-0.3.4.tar", max compression
+gzip compressed data, was "goblin_cbm_runner-0.3.5.tar", max compression
```

## Comparing `goblin_cbm_runner-0.3.4.tar` & `goblin_cbm_runner-0.3.5.tar`

### file list

```diff
@@ -1,359 +1,359 @@
--rw-r--r--   0        0        0     1088 2023-05-25 19:51:14.000000 goblin_cbm_runner-0.3.4/LICENSE
--rw-r--r--   0        0        0     2542 2024-05-08 08:34:25.114471 goblin_cbm_runner-0.3.4/README.md
--rw-r--r--   0        0        0      485 2024-05-08 08:34:25.146471 goblin_cbm_runner-0.3.4/pyproject.toml
--rw-r--r--   0        0        0    19488 2024-05-08 08:34:25.146471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/cbm/cbm_methods.py
--rw-r--r--   0        0        0        0 2024-05-08 08:34:25.146471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/cbm_validation/__init__.py
--rw-r--r--   0        0        0     3345 2024-05-08 08:34:25.146471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/cbm_validation/validation.py
--rw-r--r--   0        0        0     5535 2024-05-08 08:34:25.146471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/cbm_validation/validation_runner.py
--rw-r--r--   0        0        0      211 2024-05-08 08:34:25.146471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/configuration_data/__init__.py
--rw-r--r--   0        0        0     8627 2024-05-08 08:34:25.146471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/configuration_data/config.yaml
--rw-r--r--   0        0        0     5622 2024-05-08 08:34:25.146471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/configuration_data/geo_config.yaml
--rw-r--r--   0        0        0      222 2024-05-08 08:34:25.146471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/database/__init__.py
--rw-r--r--   0        0        0   765952 2024-05-08 08:34:25.150471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/database/cbm_runner_database.db
--rw-r--r--   0        0        0  1900544 2024-05-08 08:34:25.162471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/database/ireland_cbm_defaults_v3.db
--rw-r--r--   0        0        0        0 2024-05-08 08:34:25.166471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/__init__.py
--rw-r--r--   0        0        0      212 2024-05-08 08:34:25.166471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/baseline_input_conf/__init__.py
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.166471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/baseline_input_conf/age_classes.csv
--rw-r--r--   0        0        0      675 2024-05-08 08:34:25.166471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/baseline_input_conf/classifiers.csv
--rw-r--r--   0        0        0   500354 2024-05-08 08:34:25.166471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/baseline_input_conf/disturbance_events.csv
--rw-r--r--   0        0        0      115 2024-05-08 08:34:25.166471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/baseline_input_conf/disturbance_types.csv
--rw-r--r--   0        0        0     7500 2024-05-08 08:34:25.166471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/baseline_input_conf/growth.csv
--rw-r--r--   0        0        0    34610 2024-05-08 08:34:25.166471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/baseline_input_conf/inventory.csv
--rw-r--r--   0        0        0     3210 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/baseline_input_conf/sit_config.json
--rw-r--r--   0        0        0     3216 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/baseline_input_conf/spinup_config.json
--rw-r--r--   0        0        0     7600 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/baseline_input_conf/standing_vol.csv
--rw-r--r--   0        0        0      220 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/baseline_input_conf/transitions.csv
--rw-r--r--   0        0        0    24550 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/cbm_data_factory.py
--rw-r--r--   0        0        0     6617 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/create_json.py
--rw-r--r--   0        0        0    36739 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/disturbances.py
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/-1/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/-1/classifiers.csv
--rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/-1/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/-1/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/-1/growth.csv
--rw-r--r--   0        0        0     1656 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/-1/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/-1/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/-1/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/0/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/0/classifiers.csv
--rw-r--r--   0        0        0   110930 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/0/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/0/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/0/growth.csv
--rw-r--r--   0        0        0     1670 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/0/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/0/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/0/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/1/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/1/classifiers.csv
--rw-r--r--   0        0        0   118716 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/1/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/1/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/1/growth.csv
--rw-r--r--   0        0        0     1676 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/1/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/1/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/1/transitions.csv
--rw-r--r--   0        0        0      212 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/__init__.py
--rw-r--r--   0        0        0    25246 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/inventory.py
--rw-r--r--   0        0        0    11793 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/runner.py
--rw-r--r--   0        0        0     5398 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/transition.py
--rw-r--r--   0        0        0     5020 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/yield_curves.py
--rw-r--r--   0        0        0        0 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/__init__.py
--rw-r--r--   0        0        0      212 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/baseline_input_conf/__init__.py
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/baseline_input_conf/age_classes.csv
--rw-r--r--   0        0        0      675 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/baseline_input_conf/classifiers.csv
--rw-r--r--   0        0        0   500354 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/baseline_input_conf/disturbance_events.csv
--rw-r--r--   0        0        0      115 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/baseline_input_conf/disturbance_types.csv
--rw-r--r--   0        0        0     7500 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/baseline_input_conf/growth.csv
--rw-r--r--   0        0        0    34610 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/baseline_input_conf/inventory.csv
--rw-r--r--   0        0        0     3210 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/baseline_input_conf/sit_config.json
--rw-r--r--   0        0        0     3216 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/baseline_input_conf/spinup_config.json
--rw-r--r--   0        0        0     7600 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/baseline_input_conf/standing_vol.csv
--rw-r--r--   0        0        0      220 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/baseline_input_conf/transitions.csv
--rw-r--r--   0        0        0    19776 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/forestsim_disturbances.py
--rw-r--r--   0        0        0     9649 2024-05-08 08:34:25.178471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/forestsim_factory.py
--rw-r--r--   0        0        0    25454 2024-05-08 08:34:25.178471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/forestsim_inventory.py
--rw-r--r--   0        0        0    10801 2024-05-08 08:34:25.178471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/forestsim_runner.py
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.178471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.178471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/classifiers.csv
--rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.178471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.178471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.178471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/growth.csv
--rw-r--r--   0        0        0     1656 2024-05-08 08:34:25.178471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.178471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.178471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.178471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/0/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.178471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/0/classifiers.csv
--rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/0/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/0/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/0/growth.csv
--rw-r--r--   0        0        0     1642 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/0/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/0/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/0/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/1/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/1/classifiers.csv
--rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/1/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/1/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/1/growth.csv
--rw-r--r--   0        0        0     1642 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/1/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/1/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/1/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/10/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/10/classifiers.csv
--rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/10/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/10/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/10/growth.csv
--rw-r--r--   0        0        0     1656 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/10/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/10/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/10/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/11/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/11/classifiers.csv
--rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/11/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/11/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/11/growth.csv
--rw-r--r--   0        0        0     1656 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/11/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/11/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/11/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/12/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/12/classifiers.csv
--rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/12/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/12/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/12/growth.csv
--rw-r--r--   0        0        0     1656 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/12/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/12/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/12/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/13/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/13/classifiers.csv
--rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/13/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/13/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/13/growth.csv
--rw-r--r--   0        0        0     1656 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/13/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/13/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/13/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/14/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/14/classifiers.csv
--rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/14/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/14/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/14/growth.csv
--rw-r--r--   0        0        0     1656 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/14/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/14/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/14/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/15/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/15/classifiers.csv
--rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/15/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/15/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/15/growth.csv
--rw-r--r--   0        0        0     1674 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/15/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/15/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.186471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/15/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/16/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/16/classifiers.csv
--rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/16/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/16/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/16/growth.csv
--rw-r--r--   0        0        0     1675 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/16/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/16/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/16/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/17/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/17/classifiers.csv
--rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/17/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/17/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/17/growth.csv
--rw-r--r--   0        0        0     1677 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/17/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/17/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/17/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/18/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/18/classifiers.csv
--rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/18/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/18/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/18/growth.csv
--rw-r--r--   0        0        0     1679 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/18/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/18/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/18/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/19/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/19/classifiers.csv
--rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/19/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/19/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/19/growth.csv
--rw-r--r--   0        0        0     1679 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/19/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/19/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/19/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/2/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.190471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/2/classifiers.csv
--rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.194471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/2/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.194471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/2/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.194471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/2/growth.csv
--rw-r--r--   0        0        0     1642 2024-05-08 08:34:25.194471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/2/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.194471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/2/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.194471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/2/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.194471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/20/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.194471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/20/classifiers.csv
--rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.194471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/20/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.194471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/20/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.194471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/20/growth.csv
--rw-r--r--   0        0        0     1656 2024-05-08 08:34:25.194471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/20/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.194471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/20/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.194471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/20/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.194471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/21/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.194471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/21/classifiers.csv
--rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.194471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/21/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.194471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/21/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.194471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/21/growth.csv
--rw-r--r--   0        0        0     1677 2024-05-08 08:34:25.194471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/21/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.194471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/21/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.194471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/21/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.194471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/22/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/22/classifiers.csv
--rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/22/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/22/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/22/growth.csv
--rw-r--r--   0        0        0     1677 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/22/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/22/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/22/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/23/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/23/classifiers.csv
--rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/23/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/23/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/23/growth.csv
--rw-r--r--   0        0        0     1679 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/23/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/23/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/23/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/24/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/24/classifiers.csv
--rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/24/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/24/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/24/growth.csv
--rw-r--r--   0        0        0     1676 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/24/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/24/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/24/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/3/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/3/classifiers.csv
--rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/3/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/3/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/3/growth.csv
--rw-r--r--   0        0        0     1642 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/3/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/3/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/3/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/4/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/4/classifiers.csv
--rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/4/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/4/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/4/growth.csv
--rw-r--r--   0        0        0     1642 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/4/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/4/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/4/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/5/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/5/classifiers.csv
--rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/5/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/5/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/5/growth.csv
--rw-r--r--   0        0        0     1641 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/5/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/5/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/5/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/6/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/6/classifiers.csv
--rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/6/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/6/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/6/growth.csv
--rw-r--r--   0        0        0     1641 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/6/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/6/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/6/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/7/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/7/classifiers.csv
--rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/7/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/7/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/7/growth.csv
--rw-r--r--   0        0        0     1641 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/7/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/7/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/7/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/8/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/8/classifiers.csv
--rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/8/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/8/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/8/growth.csv
--rw-r--r--   0        0        0     1641 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/8/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.206471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/8/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.210471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/8/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.210471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/9/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.210471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/9/classifiers.csv
--rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.210471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/9/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.210471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/9/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.210471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/9/growth.csv
--rw-r--r--   0        0        0     1641 2024-05-08 08:34:25.210471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/9/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.210471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/9/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.210471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/9/transitions.csv
--rw-r--r--   0        0        0      212 2024-05-08 08:34:25.210471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 08:34:25.210471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/__init__.py
--rw-r--r--   0        0        0      212 2024-05-08 08:34:25.210471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/__init__.py
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.210471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/age_classes.csv
--rw-r--r--   0        0        0      474 2024-05-08 08:34:25.210471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/classifiers.csv
--rw-r--r--   0        0        0   254147 2024-05-08 08:34:25.210471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/disturbance_events.csv
--rw-r--r--   0        0        0       71 2024-05-08 08:34:25.210471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/disturbance_types.csv
--rw-r--r--   0        0        0     2445 2024-05-08 08:34:25.210471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/growth.csv
--rw-r--r--   0        0        0     5011 2024-05-08 08:34:25.210471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/inventory.csv
--rw-r--r--   0        0        0     2448 2024-05-08 08:34:25.210471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/sit_config.json
--rw-r--r--   0        0        0     2454 2024-05-08 08:34:25.210471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/spinup_config.json
--rw-r--r--   0        0        0     2429 2024-05-08 08:34:25.210471 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/standing_vol.csv
--rw-r--r--   0        0        0     2262 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/transitions.csv
--rw-r--r--   0        0        0     3978 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/catchment_forest_cover.py
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/age_classes.csv
--rw-r--r--   0        0        0      591 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/classifiers.csv
--rw-r--r--   0        0        0      534 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/disturbance_types.csv
--rw-r--r--   0        0        0     4188 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/growth.csv
--rw-r--r--   0        0        0      840 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/inventory.csv
--rw-r--r--   0        0        0     3064 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/sit_config.json
--rw-r--r--   0        0        0     3990 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/age_classes.csv
--rw-r--r--   0        0        0      591 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/classifiers.csv
--rw-r--r--   0        0        0    28328 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/disturbance_types.csv
--rw-r--r--   0        0        0     4188 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/growth.csv
--rw-r--r--   0        0        0      895 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/inventory.csv
--rw-r--r--   0        0        0     3064 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/sit_config.json
--rw-r--r--   0        0        0     3990 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/age_classes.csv
--rw-r--r--   0        0        0      591 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/classifiers.csv
--rw-r--r--   0        0        0    28339 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/disturbance_types.csv
--rw-r--r--   0        0        0     4188 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/growth.csv
--rw-r--r--   0        0        0      895 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/inventory.csv
--rw-r--r--   0        0        0     3064 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/sit_config.json
--rw-r--r--   0        0        0     3990 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/transitions.csv
--rw-r--r--   0        0        0      212 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/__init__.py
--rw-r--r--   0        0        0    23748 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/geo_cbm_data_factory.py
--rw-r--r--   0        0        0     6801 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/geo_create_json.py
--rw-r--r--   0        0        0    27793 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/geo_disturbances.py
--rw-r--r--   0        0        0    16271 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/geo_inventory.py
--rw-r--r--   0        0        0    12543 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/geo_runner.py
--rw-r--r--   0        0        0     5416 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/geo_transition.py
--rw-r--r--   0        0        0        0 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/harvest_manager/__init__.py
--rw-r--r--   0        0        0     9116 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/harvest_manager/harvest.py
--rw-r--r--   0        0        0        0 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/__init__.py
--rw-r--r--   0        0        0      212 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/baseline_input_conf/__init__.py
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/classifiers.csv
--rw-r--r--   0        0        0    96076 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/growth.csv
--rw-r--r--   0        0        0     1656 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/transitions.csv
--rw-r--r--   0        0        0      208 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/0/age_classes.csv
--rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/0/classifiers.csv
--rw-r--r--   0        0        0   113644 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/0/disturbance_events.csv
--rw-r--r--   0        0        0       93 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/0/disturbance_types.csv
--rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/0/growth.csv
--rw-r--r--   0        0        0     1669 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/0/inventory.csv
--rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/0/sit_config.json
--rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/0/transitions.csv
--rw-r--r--   0        0        0      212 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/__init__.py
--rw-r--r--   0        0        0     8869 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/historic_affor_runner.py
--rw-r--r--   0        0        0        0 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/resource_manager/__init__.py
--rw-r--r--   0        0        0     8459 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/resource_manager/cbm_pools.py
--rw-r--r--   0        0        0    13895 2024-05-08 08:34:25.222470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/resource_manager/cbm_runner_data_manager.py
--rw-r--r--   0        0        0    12601 2024-05-08 08:34:25.222470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/resource_manager/database_manager.py
--rw-r--r--   0        0        0    13513 2024-05-08 08:34:25.222470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/resource_manager/flux_manager.py
--rw-r--r--   0        0        0    13923 2024-05-08 08:34:25.222470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/resource_manager/geo_cbm_runner_data_manager.py
--rw-r--r--   0        0        0     5846 2024-05-08 08:34:25.222470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/resource_manager/loader.py
--rw-r--r--   0        0        0     4755 2024-05-08 08:34:25.222470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/resource_manager/parser.py
--rw-r--r--   0        0        0    12233 2024-05-08 08:34:25.222470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/resource_manager/paths.py
--rw-r--r--   0        0        0     3599 2024-05-08 08:34:25.222470 goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/resource_manager/scenario_data_fetcher.py
--rw-r--r--   0        0        0     3234 1970-01-01 00:00:00.000000 goblin_cbm_runner-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-05-25 19:51:14.000000 goblin_cbm_runner-0.3.5/LICENSE
+-rw-r--r--   0        0        0     2542 2024-05-08 08:34:25.114471 goblin_cbm_runner-0.3.5/README.md
+-rw-r--r--   0        0        0      485 2024-05-20 09:06:25.793324 goblin_cbm_runner-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0    19488 2024-05-08 08:34:25.146471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/cbm/cbm_methods.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:34:25.146471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/cbm_validation/__init__.py
+-rw-r--r--   0        0        0     3345 2024-05-08 08:34:25.146471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/cbm_validation/validation.py
+-rw-r--r--   0        0        0     5535 2024-05-08 08:34:25.146471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/cbm_validation/validation_runner.py
+-rw-r--r--   0        0        0      211 2024-05-08 08:34:25.146471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/configuration_data/__init__.py
+-rw-r--r--   0        0        0     8627 2024-05-08 08:34:25.146471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/configuration_data/config.yaml
+-rw-r--r--   0        0        0     5622 2024-05-08 08:34:25.146471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/configuration_data/geo_config.yaml
+-rw-r--r--   0        0        0      222 2024-05-08 08:34:25.146471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/database/__init__.py
+-rw-r--r--   0        0        0   765952 2024-05-08 08:34:25.150471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/database/cbm_runner_database.db
+-rw-r--r--   0        0        0  1900544 2024-05-08 08:34:25.162471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/database/ireland_cbm_defaults_v3.db
+-rw-r--r--   0        0        0        0 2024-05-08 08:34:25.166471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/__init__.py
+-rw-r--r--   0        0        0      212 2024-05-08 08:34:25.166471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/baseline_input_conf/__init__.py
+-rw-r--r--   0        0        0      208 2024-05-20 08:55:55.554794 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/baseline_input_conf/age_classes.csv
+-rw-r--r--   0        0        0      675 2024-05-20 08:55:55.550794 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/baseline_input_conf/classifiers.csv
+-rw-r--r--   0        0        0   500354 2024-05-20 08:55:55.654794 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/baseline_input_conf/disturbance_events.csv
+-rw-r--r--   0        0        0      115 2024-05-20 08:55:55.654794 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/baseline_input_conf/disturbance_types.csv
+-rw-r--r--   0        0        0     7500 2024-05-20 08:55:55.558794 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/baseline_input_conf/growth.csv
+-rw-r--r--   0        0        0    34610 2024-05-20 08:55:55.570794 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/baseline_input_conf/inventory.csv
+-rw-r--r--   0        0        0     3210 2024-05-20 08:55:55.550794 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/baseline_input_conf/sit_config.json
+-rw-r--r--   0        0        0     3216 2024-05-20 08:55:55.550794 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/baseline_input_conf/spinup_config.json
+-rw-r--r--   0        0        0     7600 2024-05-20 08:55:55.562794 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/baseline_input_conf/standing_vol.csv
+-rw-r--r--   0        0        0      220 2024-05-20 08:55:55.662794 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/baseline_input_conf/transitions.csv
+-rw-r--r--   0        0        0    24550 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/cbm_data_factory.py
+-rw-r--r--   0        0        0     6617 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/create_json.py
+-rw-r--r--   0        0        0    36739 2024-05-08 08:34:25.170471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/disturbances.py
+-rw-r--r--   0        0        0      208 2024-05-20 08:56:28.518932 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/-1/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-20 08:56:28.514932 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/-1/classifiers.csv
+-rw-r--r--   0        0        0    90722 2024-05-20 08:56:41.890988 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/-1/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-20 08:56:41.898988 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/-1/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-20 08:56:28.874933 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/-1/growth.csv
+-rw-r--r--   0        0        0     1656 2024-05-20 08:56:32.826950 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/-1/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-20 08:56:28.518932 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/-1/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-20 08:56:42.110989 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/-1/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-20 08:56:42.134989 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/0/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-20 08:56:42.130989 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/0/classifiers.csv
+-rw-r--r--   0        0        0   110930 2024-05-20 08:56:56.147047 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/0/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-20 08:56:56.155047 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/0/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-20 08:56:42.478990 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/0/growth.csv
+-rw-r--r--   0        0        0     1670 2024-05-20 08:56:45.791004 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/0/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-20 08:56:42.130989 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/0/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-20 08:56:56.363048 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/0/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-20 08:56:56.387048 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/1/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-20 08:56:56.383048 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/1/classifiers.csv
+-rw-r--r--   0        0        0   118716 2024-05-20 08:57:10.623107 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/1/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-20 08:57:10.631107 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/1/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-20 08:56:56.739050 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/1/growth.csv
+-rw-r--r--   0        0        0     1676 2024-05-20 08:57:00.055063 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/1/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-20 08:56:56.383048 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/1/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-20 08:57:10.839108 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/1/transitions.csv
+-rw-r--r--   0        0        0      212 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/__init__.py
+-rw-r--r--   0        0        0    25246 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/inventory.py
+-rw-r--r--   0        0        0    11793 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/runner.py
+-rw-r--r--   0        0        0     5398 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/transition.py
+-rw-r--r--   0        0        0     5020 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/yield_curves.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/__init__.py
+-rw-r--r--   0        0        0      212 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/baseline_input_conf/__init__.py
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/baseline_input_conf/age_classes.csv
+-rw-r--r--   0        0        0      675 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/baseline_input_conf/classifiers.csv
+-rw-r--r--   0        0        0   500354 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/baseline_input_conf/disturbance_events.csv
+-rw-r--r--   0        0        0      115 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/baseline_input_conf/disturbance_types.csv
+-rw-r--r--   0        0        0     7500 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/baseline_input_conf/growth.csv
+-rw-r--r--   0        0        0    34610 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/baseline_input_conf/inventory.csv
+-rw-r--r--   0        0        0     3210 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/baseline_input_conf/sit_config.json
+-rw-r--r--   0        0        0     3216 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/baseline_input_conf/spinup_config.json
+-rw-r--r--   0        0        0     7600 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/baseline_input_conf/standing_vol.csv
+-rw-r--r--   0        0        0      220 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/baseline_input_conf/transitions.csv
+-rw-r--r--   0        0        0    19776 2024-05-08 08:34:25.174471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/forestsim_disturbances.py
+-rw-r--r--   0        0        0     9649 2024-05-08 08:34:25.178471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/forestsim_factory.py
+-rw-r--r--   0        0        0    25454 2024-05-08 08:34:25.178471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/forestsim_inventory.py
+-rw-r--r--   0        0        0    10801 2024-05-08 08:34:25.178471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/forestsim_runner.py
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.178471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.178471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/classifiers.csv
+-rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.178471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.178471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.178471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/growth.csv
+-rw-r--r--   0        0        0     1656 2024-05-08 08:34:25.178471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.178471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.178471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.178471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/0/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.178471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/0/classifiers.csv
+-rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/0/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/0/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/0/growth.csv
+-rw-r--r--   0        0        0     1642 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/0/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/0/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/0/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/1/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/1/classifiers.csv
+-rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/1/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/1/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/1/growth.csv
+-rw-r--r--   0        0        0     1642 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/1/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/1/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/1/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/10/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/10/classifiers.csv
+-rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/10/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/10/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/10/growth.csv
+-rw-r--r--   0        0        0     1656 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/10/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/10/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/10/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/11/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/11/classifiers.csv
+-rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/11/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/11/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/11/growth.csv
+-rw-r--r--   0        0        0     1656 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/11/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/11/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.182471 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/11/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/12/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/12/classifiers.csv
+-rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/12/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/12/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/12/growth.csv
+-rw-r--r--   0        0        0     1656 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/12/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/12/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/12/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/13/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/13/classifiers.csv
+-rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/13/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/13/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/13/growth.csv
+-rw-r--r--   0        0        0     1656 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/13/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/13/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/13/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/14/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/14/classifiers.csv
+-rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/14/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/14/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/14/growth.csv
+-rw-r--r--   0        0        0     1656 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/14/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/14/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/14/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/15/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/15/classifiers.csv
+-rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/15/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/15/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/15/growth.csv
+-rw-r--r--   0        0        0     1674 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/15/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/15/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.186470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/15/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/16/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/16/classifiers.csv
+-rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/16/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/16/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/16/growth.csv
+-rw-r--r--   0        0        0     1675 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/16/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/16/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/16/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/17/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/17/classifiers.csv
+-rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/17/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/17/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/17/growth.csv
+-rw-r--r--   0        0        0     1677 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/17/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/17/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/17/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/18/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/18/classifiers.csv
+-rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/18/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/18/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/18/growth.csv
+-rw-r--r--   0        0        0     1679 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/18/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/18/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/18/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/19/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/19/classifiers.csv
+-rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/19/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/19/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/19/growth.csv
+-rw-r--r--   0        0        0     1679 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/19/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/19/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/19/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/2/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.190470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/2/classifiers.csv
+-rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.194470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/2/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.194470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/2/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.194470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/2/growth.csv
+-rw-r--r--   0        0        0     1642 2024-05-08 08:34:25.194470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/2/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.194470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/2/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.194470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/2/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.194470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/20/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.194470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/20/classifiers.csv
+-rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.194470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/20/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.194470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/20/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.194470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/20/growth.csv
+-rw-r--r--   0        0        0     1656 2024-05-08 08:34:25.194470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/20/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.194470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/20/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.194470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/20/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.194470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/21/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.194470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/21/classifiers.csv
+-rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.194470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/21/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.194470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/21/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.194470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/21/growth.csv
+-rw-r--r--   0        0        0     1677 2024-05-08 08:34:25.194470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/21/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.194470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/21/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.194470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/21/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.194470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/22/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/22/classifiers.csv
+-rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/22/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/22/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/22/growth.csv
+-rw-r--r--   0        0        0     1677 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/22/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/22/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/22/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/23/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/23/classifiers.csv
+-rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/23/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/23/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/23/growth.csv
+-rw-r--r--   0        0        0     1679 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/23/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.198470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/23/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/23/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/24/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/24/classifiers.csv
+-rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/24/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/24/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/24/growth.csv
+-rw-r--r--   0        0        0     1676 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/24/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/24/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/24/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/3/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/3/classifiers.csv
+-rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/3/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/3/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/3/growth.csv
+-rw-r--r--   0        0        0     1642 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/3/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/3/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/3/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/4/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/4/classifiers.csv
+-rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/4/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/4/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/4/growth.csv
+-rw-r--r--   0        0        0     1642 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/4/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/4/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/4/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/5/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.202470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/5/classifiers.csv
+-rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/5/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/5/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/5/growth.csv
+-rw-r--r--   0        0        0     1641 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/5/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/5/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/5/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/6/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/6/classifiers.csv
+-rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/6/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/6/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/6/growth.csv
+-rw-r--r--   0        0        0     1641 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/6/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/6/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/6/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/7/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/7/classifiers.csv
+-rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/7/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/7/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/7/growth.csv
+-rw-r--r--   0        0        0     1641 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/7/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/7/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/7/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/8/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/8/classifiers.csv
+-rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/8/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/8/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/8/growth.csv
+-rw-r--r--   0        0        0     1641 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/8/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.206470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/8/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.210470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/8/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.210470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/9/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.210470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/9/classifiers.csv
+-rw-r--r--   0        0        0    90722 2024-05-08 08:34:25.210470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/9/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.210470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/9/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.210470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/9/growth.csv
+-rw-r--r--   0        0        0     1641 2024-05-08 08:34:25.210470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/9/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.210470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/9/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.210470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/9/transitions.csv
+-rw-r--r--   0        0        0      212 2024-05-08 08:34:25.210470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:34:25.210470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/__init__.py
+-rw-r--r--   0        0        0      212 2024-05-08 08:34:25.210470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/__init__.py
+-rw-r--r--   0        0        0      208 2024-05-20 08:53:44.178232 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/age_classes.csv
+-rw-r--r--   0        0        0      474 2024-05-20 08:53:44.178232 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/classifiers.csv
+-rw-r--r--   0        0        0   253929 2024-05-20 09:06:25.793324 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/disturbance_events.csv
+-rw-r--r--   0        0        0       71 2024-05-20 08:54:10.298345 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/disturbance_types.csv
+-rw-r--r--   0        0        0     2445 2024-05-20 08:53:44.254233 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/growth.csv
+-rw-r--r--   0        0        0     5010 2024-05-20 09:06:25.793324 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/inventory.csv
+-rw-r--r--   0        0        0     2448 2024-05-20 08:53:44.178232 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/sit_config.json
+-rw-r--r--   0        0        0     2454 2024-05-20 08:53:44.178232 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/spinup_config.json
+-rw-r--r--   0        0        0     2429 2024-05-20 08:53:44.326233 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/standing_vol.csv
+-rw-r--r--   0        0        0     2262 2024-05-20 08:54:10.338345 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/transitions.csv
+-rw-r--r--   0        0        0     4046 2024-05-20 09:06:25.793324 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/catchment_forest_cover.py
+-rw-r--r--   0        0        0      208 2024-05-20 08:54:31.058435 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/age_classes.csv
+-rw-r--r--   0        0        0      591 2024-05-20 08:54:31.054435 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/classifiers.csv
+-rw-r--r--   0        0        0      534 2024-05-20 08:54:31.306436 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-20 08:54:31.314436 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/disturbance_types.csv
+-rw-r--r--   0        0        0     4188 2024-05-20 08:54:31.222435 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/growth.csv
+-rw-r--r--   0        0        0      840 2024-05-20 08:54:31.274435 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/inventory.csv
+-rw-r--r--   0        0        0     3064 2024-05-20 08:54:31.058435 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/sit_config.json
+-rw-r--r--   0        0        0     3990 2024-05-20 08:54:31.362436 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-20 08:54:31.374436 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/age_classes.csv
+-rw-r--r--   0        0        0      591 2024-05-20 08:54:31.370436 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/classifiers.csv
+-rw-r--r--   0        0        0    28328 2024-05-20 08:54:33.002443 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-20 08:54:33.010443 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/disturbance_types.csv
+-rw-r--r--   0        0        0     4188 2024-05-20 08:54:31.542437 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/growth.csv
+-rw-r--r--   0        0        0      895 2024-05-20 08:54:31.598437 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/inventory.csv
+-rw-r--r--   0        0        0     3064 2024-05-20 08:54:31.374436 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/sit_config.json
+-rw-r--r--   0        0        0     3990 2024-05-20 08:54:33.054443 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-20 08:54:33.066443 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/age_classes.csv
+-rw-r--r--   0        0        0      591 2024-05-20 08:54:33.066443 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/classifiers.csv
+-rw-r--r--   0        0        0    28339 2024-05-20 08:54:34.654450 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-20 08:54:34.662450 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/disturbance_types.csv
+-rw-r--r--   0        0        0     4188 2024-05-20 08:54:33.234444 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/growth.csv
+-rw-r--r--   0        0        0      895 2024-05-20 08:54:33.290444 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/inventory.csv
+-rw-r--r--   0        0        0     3064 2024-05-20 08:54:33.066443 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/sit_config.json
+-rw-r--r--   0        0        0     3990 2024-05-20 08:54:34.706450 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/transitions.csv
+-rw-r--r--   0        0        0      212 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/__init__.py
+-rw-r--r--   0        0        0    23748 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/geo_cbm_data_factory.py
+-rw-r--r--   0        0        0     6801 2024-05-08 08:34:25.214470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/geo_create_json.py
+-rw-r--r--   0        0        0    27793 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/geo_disturbances.py
+-rw-r--r--   0        0        0    16271 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/geo_inventory.py
+-rw-r--r--   0        0        0    12543 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/geo_runner.py
+-rw-r--r--   0        0        0     5416 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/geo_transition.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/harvest_manager/__init__.py
+-rw-r--r--   0        0        0     9116 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/harvest_manager/harvest.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/__init__.py
+-rw-r--r--   0        0        0      212 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/baseline_input_conf/__init__.py
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/classifiers.csv
+-rw-r--r--   0        0        0    96076 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/growth.csv
+-rw-r--r--   0        0        0     1656 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/transitions.csv
+-rw-r--r--   0        0        0      208 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/0/age_classes.csv
+-rw-r--r--   0        0        0     1035 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/0/classifiers.csv
+-rw-r--r--   0        0        0   113644 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/0/disturbance_events.csv
+-rw-r--r--   0        0        0       93 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/0/disturbance_types.csv
+-rw-r--r--   0        0        0     7361 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/0/growth.csv
+-rw-r--r--   0        0        0     1669 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/0/inventory.csv
+-rw-r--r--   0        0        0     4927 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/0/sit_config.json
+-rw-r--r--   0        0        0    15258 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/0/transitions.csv
+-rw-r--r--   0        0        0      212 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/__init__.py
+-rw-r--r--   0        0        0     8869 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/historic_affor_runner.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/resource_manager/__init__.py
+-rw-r--r--   0        0        0     8459 2024-05-08 08:34:25.218470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/resource_manager/cbm_pools.py
+-rw-r--r--   0        0        0    13895 2024-05-08 08:34:25.222470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/resource_manager/cbm_runner_data_manager.py
+-rw-r--r--   0        0        0    12601 2024-05-08 08:34:25.222470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/resource_manager/database_manager.py
+-rw-r--r--   0        0        0    13513 2024-05-08 08:34:25.222470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/resource_manager/flux_manager.py
+-rw-r--r--   0        0        0    13923 2024-05-08 08:34:25.222470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/resource_manager/geo_cbm_runner_data_manager.py
+-rw-r--r--   0        0        0     5846 2024-05-08 08:34:25.222470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/resource_manager/loader.py
+-rw-r--r--   0        0        0     4755 2024-05-08 08:34:25.222470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/resource_manager/parser.py
+-rw-r--r--   0        0        0    12233 2024-05-08 08:34:25.222470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/resource_manager/paths.py
+-rw-r--r--   0        0        0     3599 2024-05-08 08:34:25.222470 goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/resource_manager/scenario_data_fetcher.py
+-rw-r--r--   0        0        0     3234 1970-01-01 00:00:00.000000 goblin_cbm_runner-0.3.5/PKG-INFO
```

### Comparing `goblin_cbm_runner-0.3.4/LICENSE` & `goblin_cbm_runner-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/README.md` & `goblin_cbm_runner-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/cbm/cbm_methods.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/cbm/cbm_methods.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/cbm_validation/validation.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/cbm_validation/validation.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/cbm_validation/validation_runner.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/cbm_validation/validation_runner.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/configuration_data/config.yaml` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/configuration_data/config.yaml`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/configuration_data/geo_config.yaml` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/configuration_data/geo_config.yaml`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/database/cbm_runner_database.db` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/database/cbm_runner_database.db`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/database/ireland_cbm_defaults_v3.db` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/database/ireland_cbm_defaults_v3.db`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/baseline_input_conf/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/baseline_input_conf/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/baseline_input_conf/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/baseline_input_conf/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/baseline_input_conf/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/baseline_input_conf/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/baseline_input_conf/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/baseline_input_conf/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/baseline_input_conf/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/baseline_input_conf/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/baseline_input_conf/spinup_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/baseline_input_conf/spinup_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/baseline_input_conf/standing_vol.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/baseline_input_conf/standing_vol.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/cbm_data_factory.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/cbm_data_factory.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/create_json.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/create_json.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/disturbances.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/disturbances.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/-1/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/-1/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/-1/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/-1/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/-1/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/-1/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/-1/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/-1/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/-1/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/-1/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/-1/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/-1/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/0/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/0/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/0/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/0/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/0/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/0/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/0/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/0/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/0/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/0/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/0/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/0/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/1/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/1/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/1/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/1/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/1/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/1/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/1/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/1/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/1/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/1/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/generated_input_data/1/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/generated_input_data/1/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/inventory.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/inventory.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/runner.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/runner.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/transition.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/transition.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/default_runner/yield_curves.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/default_runner/yield_curves.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/baseline_input_conf/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/baseline_input_conf/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/baseline_input_conf/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/baseline_input_conf/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/baseline_input_conf/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/baseline_input_conf/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/baseline_input_conf/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/baseline_input_conf/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/baseline_input_conf/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/baseline_input_conf/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/baseline_input_conf/spinup_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/baseline_input_conf/spinup_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/baseline_input_conf/standing_vol.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/baseline_input_conf/standing_vol.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/forestsim_disturbances.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/forestsim_disturbances.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/forestsim_factory.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/forestsim_factory.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/forestsim_inventory.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/forestsim_inventory.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/forestsim_runner.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/forestsim_runner.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/-1/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/0/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/0/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/0/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/0/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/0/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/0/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/0/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/0/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/0/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/0/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/0/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/0/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/1/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/1/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/1/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/1/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/1/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/1/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/1/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/1/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/1/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/1/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/1/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/1/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/10/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/10/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/10/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/10/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/10/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/10/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/10/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/10/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/10/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/10/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/10/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/10/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/11/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/11/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/11/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/11/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/11/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/11/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/11/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/11/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/11/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/11/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/11/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/11/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/12/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/12/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/12/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/12/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/12/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/12/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/12/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/12/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/12/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/12/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/12/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/12/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/13/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/13/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/13/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/13/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/13/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/13/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/13/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/13/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/13/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/13/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/13/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/13/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/14/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/14/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/14/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/14/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/14/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/14/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/14/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/14/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/14/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/14/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/14/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/14/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/15/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/15/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/15/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/15/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/15/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/15/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/15/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/15/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/15/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/15/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/15/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/15/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/16/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/16/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/16/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/16/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/16/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/16/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/16/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/16/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/16/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/16/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/16/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/16/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/17/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/17/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/17/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/17/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/17/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/17/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/17/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/17/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/17/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/17/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/17/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/17/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/18/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/18/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/18/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/18/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/18/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/18/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/18/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/18/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/18/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/18/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/18/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/18/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/19/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/19/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/19/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/19/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/19/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/19/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/19/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/19/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/19/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/19/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/19/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/19/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/2/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/2/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/2/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/2/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/2/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/2/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/2/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/2/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/2/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/2/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/2/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/2/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/20/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/20/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/20/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/20/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/20/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/20/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/20/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/20/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/20/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/20/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/20/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/20/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/21/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/21/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/21/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/21/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/21/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/21/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/21/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/21/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/21/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/21/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/21/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/21/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/22/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/22/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/22/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/22/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/22/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/22/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/22/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/22/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/22/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/22/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/22/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/22/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/23/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/23/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/23/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/23/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/23/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/23/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/23/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/23/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/23/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/23/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/23/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/23/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/24/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/24/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/24/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/24/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/24/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/24/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/24/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/24/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/24/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/24/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/24/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/24/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/3/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/3/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/3/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/3/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/3/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/3/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/3/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/3/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/3/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/3/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/3/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/3/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/4/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/4/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/4/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/4/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/4/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/4/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/4/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/4/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/4/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/4/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/4/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/4/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/5/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/5/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/5/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/5/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/5/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/5/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/5/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/5/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/5/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/5/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/5/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/5/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/6/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/6/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/6/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/6/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/6/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/6/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/6/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/6/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/6/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/6/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/6/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/6/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/7/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/7/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/7/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/7/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/7/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/7/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/7/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/7/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/7/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/7/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/7/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/7/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/8/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/8/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/8/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/8/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/8/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/8/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/8/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/8/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/8/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/8/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/8/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/8/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/9/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/9/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/9/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/9/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/9/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/9/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/9/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/9/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/9/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/9/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/forest_sim/generated_input_data/9/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/forest_sim/generated_input_data/9/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/disturbance_events.csv`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Classifier1,Classifier2,Classifier3,Classifier4,UsingID,sw_age_min,sw_age_max,hw_age_min,hw_age_max,MinYearsSinceDist,MaxYearsSinceDist,LastDistTypeID,MinTotBiomassC,MaxTotBiomassC,MinSWMerchBiomassC,MaxSWMerchBiomassC,MinHWMerchBiomassC,MaxHWMerchBiomassC,MinTotalStemSnagC,MaxTotalStemSnagC,MinSWStemSnagC,MaxSWStemSnagC,MinHWStemSnagC,MaxHWStemSnagC,MinTotalStemSnagMerchC,MaxTotalStemSnagMerchC,MinSWMerchStemSnagC,MaxSWMerchStemSnagC,MinHWMerchStemSnagC,MaxHWMerchStemSnagC,Efficiency,SortType,MeasureType,Amount,DistTypeID,Year
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,229.47289972402763,DISTID2,1
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2157.9272995816664,DISTID2,1
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,223.81060753180526,DISTID1,1
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,100.71477338931246,DISTID1,1
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,145.47689489567367,DISTID1,1
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,162.32379353270773,DISTID1,1
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,105.5104657962602,DISTID1,1
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,124.86445656362133,DISTID2,1
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,124.86445656362133,DISTID2,1
@@ -18,24 +18,24 @@
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,106.13478807907812,DISTID1,1
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,47.760654635585205,DISTID1,1
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,68.9876122514009,DISTID1,1
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,124.86445656362132,DISTID1,1
 Sitka,L,mineral,YC20_24,False,10,27,10,27,4,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,223.8106075318053,DISTID2,1
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,73.04570708971853,DISTID1,1
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,171.14928811255726,DISTID1,1
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,360.60027099490054,DISTID2,1
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,229.47289972402757,DISTID1,1
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,103.2628048758125,DISTID1,1
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3391.028613628333,DISTID2,1
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2157.927299581666,DISTID1,1
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,971.0672848117506,DISTID1,1
 Sitka,L,mineral,YC20_24,False,10,27,10,27,4,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,223.8106075318053,DISTID2,1
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,40.162898083514904,DISTID2,1
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,63.11312555980913,DISTID2,1
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,40.1628980835149,DISTID1,1
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,18.07330413758172,DISTID1,1
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,26.105883754284726,DISTID1,1
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,149.1573848206182,DISTID1,1
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,751.9000344457107,DISTID2,1
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1181.5571969861169,DISTID2,1
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,751.9000344457106,DISTID1,1
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,338.35501550057006,DISTID1,1
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,488.73502238971275,DISTID1,1
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1402.6527447280853,DISTID1,1
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,154.0343593013014,DISTID1,1
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,222.4940745463244,DISTID1,1
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,263.30659709624155,DISTID2,1
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,263.30659709624155,DISTID2,1
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,413.76750972266524,DISTID2,1
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,579.2745136117313,DISTID1,1
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,263.3065970962415,DISTID1,1
@@ -52,29 +52,29 @@
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,70.04896013219157,DISTID1,2
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,14.328196390675561,DISTID1,2
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,20.696283675420272,DISTID1,2
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,30.214432016793744,DISTID1,2
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,16.856701636088896,DISTID1,2
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,67.14318225954159,DISTID1,2
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,147.7150009709915,DISTID1,2
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,504.8403793928607,DISTID1,2
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,68.84186991720829,DISTID1,2
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,30.97884146274376,DISTID1,2
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,44.747215446185464,DISTID1,2
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,88.35837578373277,DISTID1,2
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,12.04886942505447,DISTID1,2
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.421991241274516,DISTID1,2
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4747.440059079666,DISTID1,2
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,647.3781898745,DISTID1,2
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,291.3201854435252,DISTID1,2
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,420.79582341842564,DISTID1,2
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1654.1800757805636,DISTID1,2
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,225.57001033371318,DISTID1,2
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,101.50650465017104,DISTID1,2
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,51.34478643376718,DISTID1,2
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,102.6895728675342,DISTID1,2
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,46.210307790390424,DISTID1,2
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,66.74822236389733,DISTID1,2
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,173.7823540835194,DISTID1,2
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,78.99197912887246,DISTID1,2
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,35.54639060799264,DISTID1,2
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.831765126285418,DISTID1,2
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,146.62050671691384,DISTID1,2
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.064329605038123,DISTID1,3
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,13.092920540610635,DISTID1,3
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,14.609141417943697,DISTID1,3
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.574113638074671,DISTID1,3
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.495941921663421,DISTID1,3
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,24.72316239959703,DISTID1,3
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,21.014688039657475,DISTID1,3
@@ -84,27 +84,27 @@
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.298458917202669,DISTID1,3
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.208885102626083,DISTID1,3
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,20.142954677862477,DISTID1,3
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,11.237801090725924,DISTID1,3
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,15.403435930130158,DISTID1,3
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,20.0244667091692,DISTID1,3
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,10.663917182397794,DISTID1,3
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,151.45211381785825,DISTID1,3
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,20.652560975162487,DISTID1,3
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.293652438823129,DISTID1,3
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,13.424164633855641,DISTID1,3
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1424.2320177239,DISTID1,3
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,194.21345696235002,DISTID1,3
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,87.39605563305759,DISTID1,3
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,126.2387470255277,DISTID1,3
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,44.31450029129746,DISTID1,3
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.6146608275163414,DISTID1,3
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,26.507512735119835,DISTID1,3
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.3495295378856262,DISTID1,3
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,67.67100310011396,DISTID1,3
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,496.25402273416915,DISTID1,3
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,43.98615201507416,DISTID1,3
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,30.806871860260262,DISTID1,3
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,13.86309233711713,DISTID1,3
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,52.13470622505583,DISTID1,3
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,23.69759373866174,DISTID1,3
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.6265973723823552,DISTID1,3
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,30.451951395051317,DISTID1,3
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.41694871987911,DISTID1,4
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.927876162183191,DISTID1,4
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.3827424253831095,DISTID1,4
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.9722340914224017,DISTID1,4
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.848782576499027,DISTID1,4
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.3713403272177778,DISTID1,4
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.042886403358744,DISTID1,4
@@ -113,28 +113,28 @@
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.8656392781351103,DISTID1,4
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.2895376751608008,DISTID1,4
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.862665530787825,DISTID1,4
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.5171031472480012,DISTID1,4
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,13.294350087389242,DISTID1,4
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.719298881511438,DISTID1,4
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.1991751547193386,DISTID1,4
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,45.43563414535748,DISTID1,4
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.195768292548747,DISTID1,4
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.7880957316469392,DISTID1,4
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.027249390156693,DISTID1,4
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.952253820535951,DISTID1,4
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.0843982482549026,DISTID1,4
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.48797921171470665,DISTID1,4
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,427.26960531717003,DISTID1,4
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,58.26403708870502,DISTID1,4
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,26.21881668991728,DISTID1,4
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,37.87162410765832,DISTID1,4
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,148.8762068202508,DISTID1,4
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,20.30130093003419,DISTID1,4
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.135585418515396,DISTID1,4
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.621030779039049,DISTID1,4
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.24206155807808,DISTID1,4
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.1589277011351395,DISTID1,4
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.0073400127507615,DISTID1,4
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,15.64041186751675,DISTID1,4
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.109278121598523,DISTID1,4
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.704858861365688,DISTID1,4
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,13.19584560452225,DISTID1,4
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.8157896644534314,DISTID1,5
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.1783628486549573,DISTID1,5
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.5916702274267206,DISTID1,5
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.8546347729497082,DISTID1,5
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.225084615963733,DISTID1,5
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.6574113638074678,DISTID1,5
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.4551309441744004,DISTID1,5
@@ -144,27 +144,27 @@
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.38686130254824036,DISTID1,5
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.5587996592363476,DISTID1,5
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.0114020981653333,DISTID1,5
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.3863092337117149,DISTID1,5
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.3148227276149331,DISTID1,5
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.988305026216773,DISTID1,5
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.9597525464158017,DISTID1,5
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,13.630690243607248,DISTID1,5
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.8587304877646245,DISTID1,5
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.8364287194940818,DISTID1,5
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.385676146160786,DISTID1,5
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.32531947447647086,DISTID1,5
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.208174817047008,DISTID1,5
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.21145765840970643,DISTID1,5
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,128.18088159515105,DISTID1,5
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,17.479211126611506,DISTID1,5
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.865645006975185,DISTID1,5
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,44.66286204607525,DISTID1,5
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.0903902790102595,DISTID1,5
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,11.361487232297497,DISTID1,5
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.9587536813566753,DISTID1,5
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.7726184674234244,DISTID1,5
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.2476783103405422,DISTID1,5
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.8022020038252284,DISTID1,5
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.692123560255026,DISTID1,5
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.1327834364795573,DISTID1,5
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.14639376351441202,DISTID1,5
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.7406756255546196,DISTID1,5
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.1775010682280162,DISTID1,6
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.1964915078650322,DISTID1,6
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.5438597763022871,DISTID1,6
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.24473689933602943,DISTID1,6
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.3535088545964873,DISTID1,6
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.39444681828447997,DISTID1,6
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.2563904318849125,DISTID1,6
@@ -175,28 +175,28 @@
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.5673965770707521,DISTID1,6
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.25790753503216,DISTID1,6
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.1676398977709043,DISTID1,6
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.66752538478912,DISTID1,6
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.11605839076447212,DISTID1,6
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.28792576392474056,DISTID1,6
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.407637068076508,DISTID1,6
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,229.47289972402763,DISTID2,6
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.089207073082175,DISTID1,6
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.5576191463293875,DISTID1,6
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.2509286158482246,DISTID1,6
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.3624524451141024,DISTID1,6
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,40.162898083514904,DISTID2,6
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2157.9272995816664,DISTID2,6
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,38.45426447854532,DISTID1,6
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.243763337983453,DISTID1,6
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.359693502092556,DISTID1,6
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.40844616968925,DISTID1,6
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,751.9000344457107,DISTID2,6
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.6398350309438673,DISTID1,6
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.09759584234294126,DISTID1,6
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.04391812905432361,DISTID1,6
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.06343729752291194,DISTID1,6
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.8271170837030781,DISTID1,6
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.8222026876663859,DISTID1,6
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.1876261044070027,DISTID1,6
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.8317855402270273,DISTID1,6
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.3743034931021627,DISTID1,6
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.5406606011475686,DISTID1,6
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.7157028438482358,DISTID1,6
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,13.398858613822576,DISTID1,6
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.16315793289068614,DISTID1,7
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.07342106980080884,DISTID1,7
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.10605265637894619,DISTID1,7
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.11833404548534401,DISTID1,7
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.053250320468404874,DISTID1,7
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.07691712956547375,DISTID1,7
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.059167022742672125,DISTID1,7
@@ -207,26 +207,26 @@
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.03481751722934164,DISTID1,7
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.3589474523595097,DISTID1,7
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.20025761543673604,DISTID1,7
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0502919693312713,DISTID1,7
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.1247678310340544,DISTID1,7
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.19195050928316024,DISTID1,7
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.08637772917742217,DISTID1,7
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.2267621219246527,DISTID1,7
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.16728574389881626,DISTID1,7
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.07527858475446739,DISTID1,7
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.21471085315447078,DISTID1,7
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.029278752702882386,DISTID1,7
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.10873573353423074,DISTID1,7
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.019031189256873582,DISTID1,7
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,11.536279343563598,DISTID1,7
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.573129001395036,DISTID1,7
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.7079080506277668,DISTID1,7
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.019657584146773,DISTID1,7
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.5481351251109235,DISTID1,7
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.022533850906775,DISTID1,7
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.3562878313221009,DISTID1,7
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.24953566206810823,DISTID1,7
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.11229104793064884,DISTID1,7
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.1621981803442706,DISTID1,7
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.42229112042295247,DISTID1,7
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.013175438716297085,DISTID1,7
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.24666080629991582,DISTID1,7
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.02307513886964213,DISTID1,8
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.022026320940242657,DISTID1,8
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.031815796913683865,DISTID1,8
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.03550021364560321,DISTID1,8
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.015975096140521464,DISTID1,8
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.06007728463102082,DISTID1,8
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.015087590799381394,DISTID1,8
@@ -234,29 +234,29 @@
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.017750106822801637,DISTID1,8
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0510656919363677,DISTID1,8
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.023211678152894405,DISTID1,8
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.010445255168802493,DISTID1,8
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.04894737986720585,DISTID1,8
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.027307856650464018,DISTID1,8
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.10768423570785293,DISTID1,8
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.06441325594634124,DISTID1,8
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.2058972752440322,DISTID1,8
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.025913318753226656,DISTID1,8
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.3680286365773959,DISTID1,8
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.05018572316964489,DISTID1,8
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.022583575426340218,DISTID1,8
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.4608838030690796,DISTID1,8
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.4719387004185109,DISTID1,8
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.21237241518833008,DISTID1,8
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.037430349310216326,DISTID1,8
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.008783625810864717,DISTID1,8
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0039526316148891264,DISTID1,8
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.032620720060269226,DISTID1,8
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.1644405375332771,DISTID1,8
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.07399824188997477,DISTID1,8
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.30676015527203254,DISTID1,8
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.07486069862043249,DISTID1,8
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.03368731437919466,DISTID1,8
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.048659454103281194,DISTID1,8
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.12668733612688576,DISTID1,8
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.05758515278494808,DISTID1,8
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.005709356777062076,DISTID1,8
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.10688634939663029,DISTID1,8
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.018023185389306248,DISTID1,9
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00954473907410516,DISTID1,9
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.010650064093680965,DISTID1,9
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00479252884215644,DISTID1,9
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.006922541660892639,DISTID1,9
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,174.81023918906985,DISTID1,9
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.008192356995139207,DISTID1,9
@@ -268,22 +268,22 @@
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.003133576550640748,DISTID1,9
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0066078962820727985,DISTID1,9
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0036865606478126453,DISTID1,9
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.03230527071235588,DISTID1,9
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.014684213960161757,DISTID1,9
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.011229104793064899,DISTID1,9
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,313.3348505445274,DISTID1,9
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.11040859097321877,DISTID1,9
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.01505571695089347,DISTID1,9
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.006775072627902066,DISTID1,9
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00978621601808077,DISTID1,9
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0026350877432594153,DISTID1,9
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.001185789484466738,DISTID1,9
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0017128070331186229,DISTID1,9
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.019323976783902377,DISTID1,9
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.038265140920724,DISTID1,9
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.1415816101255533,DISTID1,9
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.06371172455649904,DISTID1,9
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.09202804658160978,DISTID1,9
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.04933216125998313,DISTID1,9
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.02219947256699243,DISTID1,9
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.03206590481898909,DISTID1,9
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.36176918257320967,DISTID1,9
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.010106194313758398,DISTID1,9
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.01459783623098436,DISTID1,9
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,368.6292359347381,DISTID1,9
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.03800620083806573,DISTID1,9
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.017275545835484428,DISTID1,9
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.007773995625967998,DISTID1,9
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.02245820958612975,DISTID1,9
@@ -301,24 +301,24 @@
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.001597509614052148,DISTID1,10
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,44.576610993212824,DISTID1,10
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.004595912274273094,DISTID1,10
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.002089051033760497,DISTID1,10
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.004405264188048528,DISTID1,10
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0024577070985417624,DISTID1,10
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.009691581213706765,DISTID1,10
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00035573684534002145,DISTID1,10
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00665984177009773,DISTID1,10
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0033687314379194705,DISTID1,10
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,94.00045516335823,DISTID1,10
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.03312257729196564,DISTID1,10
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0020325217883706203,DISTID1,10
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.002935864805424231,DISTID1,10
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0057971930351707135,DISTID1,10
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0007905263229778248,DISTID1,10
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0005138421099355869,DISTID1,10
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.004516715085268041,DISTID1,10
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.31147954227621727,DISTID1,10
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.019113517366949714,DISTID1,10
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.02760841397448294,DISTID1,10
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.10853075477196292,DISTID1,10
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.014799648377994941,DISTID1,10
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.009619771445696729,DISTID1,10
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.04247448303766599,DISTID1,10
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.006737462875838926,DISTID1,10
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00303185829412752,DISTID1,10
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.004379350869295308,DISTID1,10
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,110.58877078042146,DISTID1,10
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.011401860251419722,DISTID1,10
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0051826637506453286,DISTID1,10
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,753.0568676952506,DISTID1,10
@@ -347,22 +347,22 @@
 Sitka,L,peat,YC20_24,False,10,27,10,27,4,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,53.06739403953906,DISTID2,11
 Sitka,L,peat,YC20_24,False,10,27,10,27,4,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,23.880327317792602,DISTID2,11
 Sitka,L,peat,YC20_24,False,10,27,10,27,4,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,34.49380612570045,DISTID2,11
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,137.35090221998345,DISTID2,11
 Sitka,L,mineral,YC20_24,False,10,27,10,27,4,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,246.1916682849858,DISTID2,11
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.000594710665386552,DISTID1,11
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0013215792564145587,DISTID1,11
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.009936773187589693,DISTID1,11
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0013550145255804126,DISTID1,11
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0006097565365111861,DISTID1,11
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0008807594416272695,DISTID1,11
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0017391579105512144,DISTID1,11
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00023715789689334748,DISTID1,11
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00010672105360200646,DISTID1,11
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0001541526329806761,DISTID1,11
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.09344386268286518,DISTID1,11
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.012742344911299799,DISTID1,11
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.005734055210084915,DISTID1,11
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.008282524192344884,DISTID1,11
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.03255922643158888,DISTID1,11
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.004439894513398483,DISTID1,11
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0019979525310293194,DISTID1,11
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.002885931433709019,DISTID1,11
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,225.9170603085752,DISTID1,11
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.002021238862751678,DISTID1,11
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0009095574882382561,DISTID1,11
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0008590265166694645,DISTID1,11
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,33.17663123412644,DISTID1,11
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0034205580754259174,DISTID1,11
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.001554799125193599,DISTID1,11
@@ -400,26 +400,26 @@
 Sitka,L,mineral,YC20_24,False,10,27,10,27,4,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,73.85750048549575,DISTID2,12
 Sitka,L,peat,YC20_24,False,10,27,10,27,4,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,10.348141837710136,DISTID2,12
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,41.205270665995045,DISTID2,12
 Sitka,L,peat,YC20_24,False,10,27,10,27,4,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.164098195337781,DISTID2,12
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0002577079550008394,DISTID1,12
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0003964737769243676,DISTID1,12
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00017841319961596562,DISTID1,12
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,321.26205961363866,DISTID1,12
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0029810319562769082,DISTID1,12
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00040650435767412385,DISTID1,12
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00018292696095335587,DISTID1,12
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0002642278324881809,DISTID1,12
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,56.22805731692086,DISTID1,12
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.114736906800425e-05,DISTID1,12
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.201631608060194e-05,DISTID1,12
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.624578989420284e-05,DISTID1,12
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3021.0982194143326,DISTID1,12
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.02803315880485956,DISTID1,12
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0038227034733899403,DISTID1,12
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0017202165630254747,DISTID1,12
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0024847572577034655,DISTID1,12
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1052.6600482239949,DISTID1,12
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.001331968354019545,DISTID1,12
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.000599385759308796,DISTID1,12
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0008657794301127058,DISTID1,12
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,67.77511809257257,DISTID1,12
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0006063716588255036,DISTID1,12
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0005217473731653643,DISTID1,12
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.009767767929476664,DISTID1,12
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0003941415782365779,DISTID1,12
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00027286724647147684,DISTID1,12
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.460040964702243,DISTID1,12
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,25.67239321688359,DISTID2,12
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,17.77319530399632,DISTID2,12
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,39.49598956443623,DISTID2,12
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,86.8911770417597,DISTID2,12
@@ -454,27 +454,27 @@
 Sitka,L,peat,YC20_24,False,10,27,10,27,4,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.776065463558517,DISTID2,13
 Sitka,L,peat,YC20_24,False,10,27,10,27,4,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.1492294586013343,DISTID2,13
 Sitka,L,peat,YC20_24,False,10,27,10,27,4,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.1044425513130416,DISTID2,13
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,12.361581199798515,DISTID2,13
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.731238650025183e-05,DISTID1,13
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,11.84879686933087,DISTID2,13
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0001189421330773103,DISTID1,13
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0008943095868830727,DISTID1,13
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00012195130730223716,DISTID1,13
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.4878088286006766e-05,DISTID1,13
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.926834974645428e-05,DISTID1,13
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,16.868417195076262,DISTID1,13
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00015652421194960932,DISTID1,13
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.1344210720401276e-05,DISTID1,13
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.604894824180583e-06,DISTID1,13
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.3873736968260852e-05,DISTID1,13
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.008409947641457869,DISTID1,13
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0011468110420169823,DISTID1,13
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0005160649689076425,DISTID1,13
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0007454271773110398,DISTID1,13
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,315.7980144671985,DISTID1,13
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.002930330378843,DISTID1,13
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0003995905062058636,DISTID1,13
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00017981572779263882,DISTID1,13
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00025973382903381176,DISTID1,13
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,20.332535427771774,DISTID1,13
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0001819114976476511,DISTID1,13
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.186017394144307e-05,DISTID1,13
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,96.37861788409161,DISTID1,13
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,906.3294658242999,DISTID1,13
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.9858968110713806,DISTID1,13
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00030785022678833266,DISTID1,13
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00013993192126742396,DISTID1,13
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.296936457034082e-05,DISTID1,13
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.095574882382574e-05,DISTID1,13
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,26.067353112527915,DISTID2,13
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.3523959884789684e-05,DISTID1,13
@@ -506,28 +506,28 @@
 Sitka,L,peat,YC20_24,False,10,27,10,27,4,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.4328196390675552,DISTID2,14
 Sitka,L,peat,YC20_24,False,10,27,10,27,4,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.6447688375804004,DISTID2,14
 Sitka,L,peat,YC20_24,False,10,27,10,27,4,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.9313327653939125,DISTID2,14
 Sitka,L,mineral,YC20_24,False,10,27,10,27,4,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.021443201679372,DISTID2,14
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.6856701636088889,DISTID2,14
 Sitka,L,mineral,YC20_24,False,10,27,10,27,4,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.647175043694621,DISTID2,14
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.319371595007555e-05,DISTID1,14
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,28.91358536522749,DISTID1,14
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,271.89883974729,DISTID1,14
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.605718796543691e-05,DISTID1,14
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00026829287606492183,DISTID1,14
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.658539219067116e-05,DISTID1,14
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.6463426485802032e-05,DISTID1,14
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.3780504923936286e-05,DISTID1,14
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.0605251585228785,DISTID1,14
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.695726358488281e-05,DISTID1,14
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.8814684472541754e-06,DISTID1,14
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.162121090478256e-06,DISTID1,14
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.002522984292437361,DISTID1,14
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00034404331260509474,DISTID1,14
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00015481949067229275,DISTID1,14
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00022362815319331198,DISTID1,14
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,94.73940434015957,DISTID1,14
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0008790991136529002,DISTID1,14
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.394471833779166e-05,DISTID1,14
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.792014871014355e-05,DISTID1,14
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.099760628331534,DISTID1,14
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.457344929429534e-05,DISTID1,14
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.4558052182432926e-05,DISTID1,14
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.4032632161203834e-06,DISTID1,14
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0001198771518617591,DISTID1,14
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.8957690433214143,DISTID1,14
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.547274204129202e-05,DISTID1,14
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.850180783102487e-05,DISTID1,14
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.761403686823202,DISTID1,14
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.3105153895195243,DISTID2,14
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.5995875773596693,DISTID2,14
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.5546390607992615,DISTID2,14
@@ -562,28 +562,28 @@
 Sitka,L,peat,YC20_24,False,10,27,10,27,4,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.4298458917202666,DISTID2,15
 Sitka,L,peat,YC20_24,False,10,27,10,27,4,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.19343065127412018,DISTID2,15
 Sitka,L,peat,YC20_24,False,10,27,10,27,4,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.2793998296181738,DISTID2,15
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.1125423079818666,DISTID2,15
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.817156389631073e-06,DISTID1,15
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.4937535259320486e-06,DISTID1,15
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.3550542349307462e-05,DISTID1,15
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.674075609568249,DISTID1,15
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.048786281947657e-05,DISTID1,15
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.0975617657201348e-05,DISTID1,15
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.9390279457406106e-06,DISTID1,15
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.1341514771808876e-06,DISTID1,15
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.5181575475568638,DISTID1,15
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.4087179075464842e-05,DISTID1,15
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.644405341762528e-07,DISTID1,15
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.2486363271434772e-06,DISTID1,15
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,81.56965192418701,DISTID1,15
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0007568952877312085,DISTID1,15
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00010321299378152844,DISTID1,15
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.644584720168784e-05,DISTID1,15
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.70884459579936e-05,DISTID1,15
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,28.42182130204787,DISTID1,15
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00026372973409587007,DISTID1,15
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.61834155013375e-05,DISTID1,15
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.337604461304307e-05,DISTID1,15
 SGB,L,mineral,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,39.861324655606886,DISTID1,15
 SGB,L,peat,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.424692764052778,DISTID1,15
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.8299281884994605,DISTID1,15
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.6372034788288605e-05,DISTID1,15
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.9209789648361154e-06,DISTID1,15
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.5963145558527736e-05,DISTID1,15
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.0641822612387608e-05,DISTID1,15
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.367415654729878e-06,DISTID1,15
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.22842110604696067,DISTID1,15
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.6931546168558574,DISTID2,15
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.4798762732079008,DISTID2,15
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.346061780127513,DISTID2,15
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.18601739414432e-06,DISTID1,15
@@ -623,32 +623,32 @@
 Sitka,L,peat,YC20_24,False,10,27,10,27,4,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.05802919538223606,DISTID2,16
 Sitka,L,peat,YC20_24,False,10,27,10,27,4,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.08381994888545215,DISTID2,16
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.062508136766264e-07,DISTID1,16
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.20794638505675728,DISTID2,16
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.065162704792239e-06,DISTID1,16
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.31991751547193364,DISTID2,16
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.14396288196237028,DISTID2,16
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.6022226828704746,DISTID1,16
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.4146358845842973e-05,DISTID1,16
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.292685297160405e-06,DISTID1,16
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.4817083837221834e-06,DISTID1,16
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.1402454431542664e-06,DISTID1,16
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,114.73644986201379,DISTID2,16
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,51.63140243790625,DISTID2,16
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.4554472642670592,DISTID1,16
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.226153722639453e-06,DISTID1,16
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.762936894508347e-07,DISTID1,16
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.593321602528759e-07,DISTID1,16
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.745908981430432e-07,DISTID1,16
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,20.08144904175745,DISTID2,16
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.03665206879086,DISTID2,16
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,74.5786924103091,DISTID2,16
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,24.47089557725611,DISTID1,16
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00022706858631936258,DISTID1,16
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.0963898134458537e-05,DISTID1,16
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.3933754160506353e-05,DISTID1,16
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.0126533787398085e-05,DISTID1,16
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1078.963649790833,DISTID2,16
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,485.5336424058753,DISTID2,16
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.526546390614362,DISTID1,16
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.911892022876103e-05,DISTID1,16
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.0788943667558323e-05,DISTID1,16
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.85502465040125e-06,DISTID1,16
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.012813383912922e-06,DISTID1,16
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,375.9500172228553,DISTID2,16
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,169.17750775028503,DISTID2,16
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,701.3263723640426,DISTID2,16
 SGB,L,mineral,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,27.5963016846509,DISTID1,16
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.703818534038254,DISTID2,16
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,13.052941877142363,DISTID2,16
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,244.36751119485638,DISTID2,16
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.455805218243296e-06,DISTID1,16
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.700172843399203e-06,DISTID1,16
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.7781618742204484e-06,DISTID1,16
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0806192138989273,DISTID1,16
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.192546783716283e-06,DISTID1,16
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.311956123284985e-06,DISTID1,16
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.911610436486582e-06,DISTID1,16
@@ -688,44 +688,44 @@
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.10012880771836802,DISTID2,17
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.493753525932051e-07,DISTID1,17
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.41875244102988e-07,DISTID1,17
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.009748904824215653,DISTID1,17
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.04318886458871109,DISTID2,17
 SGB,L,peat,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.9096585263170334,DISTID1,17
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.21114556021147624,DISTID2,17
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.7806668048611426,DISTID1,17
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.243907653752894e-06,DISTID1,17
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.878055891481216e-07,DISTID1,17
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.4451251511665514e-07,DISTID1,17
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.4207363294628e-07,DISTID1,17
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,252.42018969643036,DISTID2,17
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,34.42093495860414,DISTID2,17
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,15.48942073137188,DISTID2,17
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,22.373607723092732,DISTID2,17
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.13663417928011778,DISTID1,17
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.2678461167918362e-06,DISTID1,17
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.7288810683525045e-07,DISTID1,17
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.779964807586277e-08,DISTID1,17
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.1237726944291298e-07,DISTID1,17
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,44.179187891866384,DISTID2,17
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.341268673176833,DISTID1,17
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.812057589580877e-05,DISTID1,17
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.289169440337563e-06,DISTID1,17
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.180126248151906e-06,DISTID1,17
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.037960136219426e-06,DISTID1,17
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2373.720029539833,DISTID2,17
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,323.68909493725,DISTID2,17
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,145.6600927217626,DISTID2,17
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,210.39791170921282,DISTID2,17
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.5579639171843094,DISTID1,17
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.3735676068628312e-05,DISTID1,17
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.236683100267497e-06,DISTID1,17
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.4565073951203754e-06,DISTID1,17
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.103844015173877e-06,DISTID1,17
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,827.0900378902818,DISTID2,17
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.09597525464158012,DISTID2,17
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.710995620637258,DISTID2,17
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.024434712527235,DISTID2,17
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,50.75325232508552,DISTID2,17
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,112.78500516685659,DISTID2,17
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.367415654729889e-07,DISTID1,17
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.10051853019761e-07,DISTID1,17
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.1334485622661348e-06,DISTID1,17
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.024185764169678197,DISTID1,17
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.57764035114885e-07,DISTID1,17
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.4935868369854964e-06,DISTID1,17
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.4734831309459748e-06,DISTID1,17
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.16469353696495148,DISTID1,17
 SGB,L,peat,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.8794539064528046,DISTID1,17
 SGB,L,mineral,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,35.221466465694235,DISTID1,17
 SGB,L,mineral,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,25.940523583571846,DISTID1,17
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.915882563142709,DISTID2,17
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,73.31025335845692,DISTID2,17
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.630674089256893e-07,DISTID1,17
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.02343014100609813,DISTID1,18
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.003440789937958467,DISTID1,18
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.3625638751135e-07,DISTID1,18
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.433134520016535e-08,DISTID1,18
 Sitka,L,peat,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.0962521155592278e-07,DISTID1,18
 Sitka,L,mineral,YC20_24,False,10,27,10,27,4,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.015907898456841933,DISTID2,18
@@ -753,34 +753,34 @@
 Sitka,L,peat,YC20_24,False,10,27,10,27,4,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.005222627584401247,DISTID2,18
 Sitka,L,peat,YC20_24,False,10,27,10,27,4,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.007543795399690697,DISTID2,18
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.018715174655108163,DISTID2,18
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.25625732308964e-08,DISTID1,18
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.012956659376613328,DISTID2,18
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.006167369863267941,DISTID1,18
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.06334366806344288,DISTID2,18
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.37131808328739e-08,DISTID1,18
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.3339894422758838e-08,DISTID1,18
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.186643205057514e-08,DISTID1,18
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.803538350375509e-07,DISTID1,18
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.04099025378403534,DISTID1,18
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.646826219411564,DISTID2,18
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,13.253756367559918,DISTID2,18
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,10.326280487581244,DISTID2,18
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.9262208988388406e-07,DISTID1,18
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.3335375453499657e-07,DISTID1,18
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.963416767444365e-07,DISTID1,18
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.1731722961258683e-06,DISTID1,18
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.23420004145834278,DISTID1,18
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.311532045521632e-07,DISTID1,18
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.3695221853611267e-07,DISTID1,18
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.710049300802492e-07,DISTID1,18
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.120702820588495e-06,DISTID1,18
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.7673891751552929,DISTID1,18
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,43.69802781652879,DISTID2,18
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,248.12701136708458,DISTID2,18
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,97.10672848117501,DISTID2,18
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.8113880408658281e-06,DISTID1,18
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.2540378744455723e-06,DISTID1,18
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.7867508321012692e-06,DISTID1,18
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.0436172768742637e-05,DISTID1,18
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.20238060195305,DISTID1,18
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.02879257639247404,DISTID2,18
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,75.72605690892912,DISTID2,18
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.8073304137581707,DISTID2,18
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.7120823169278205,DISTID2,18
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.1747647689428131,DISTID2,18
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,712.11600886195,DISTID2,18
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,33.83550155005698,DISTID2,18
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,63.11937351276385,DISTID2,18
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,21.99307600753708,DISTID2,18
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.2102246964189672e-07,DISTID1,18
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.8132986861911776,DISTID2,18
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,15.225975697525659,DISTID2,18
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.530155559059283e-07,DISTID1,18
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.400345686798405e-07,DISTID1,18
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.48076051095649e-07,DISTID1,18
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.8732921053446557e-07,DISTID1,18
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.9892022267770682e-07,DISTID1,18
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.007255729250903461,DISTID1,18
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.04940806108948545,DISTID1,18
@@ -822,34 +822,34 @@
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0026625160234202464,DISTID2,19
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0018432803239063226,DISTID2,19
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.004096178497569603,DISTID2,19
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.009011592694653124,DISTID2,19
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,87.40511959453492,DISTID2,19
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.046134129451743e-08,DISTID1,19
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,313.3348505445274,DISTID1,19
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.0978841462743736,DISTID2,19
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,29.13201854435251,DISTID2,19
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.003886997812983999,DISTID2,19
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.5421991241274513,DISTID2,19
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.9761269102679755,DISTID2,19
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.0113954249862172e-08,DISTID1,19
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.001968326827651e-09,DISTID1,19
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.5559929615172543e-08,DISTID1,19
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.1410615051126529e-07,DISTID1,19
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.0136246950783465,DISTID2,19
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.3940478658234696,DISTID2,19
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,22.71781707267874,DISTID2,19
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.7786626965165224e-08,DISTID1,19
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.000612636049898e-08,DISTID1,19
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.890250302333098e-08,DISTID1,19
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.519516888377606e-07,DISTID1,19
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.07026001243750284,DISTID1,19
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,10.150650465017096,DISTID2,19
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,74.4381034101254,DISTID2,19
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.8934596136564898e-07,DISTID1,19
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.3108566556083382e-07,DISTID1,19
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.913014790240748e-07,DISTID1,19
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.1362108461765485e-06,DISTID1,19
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,18.93581205382916,DISTID2,19
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,13.10940834495864,DISTID2,19
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,213.63480265858502,DISTID2,19
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.434164122597485e-07,DISTID1,19
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.762113623336717e-07,DISTID1,19
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.36025249630381e-07,DISTID1,19
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.130851830622793e-06,DISTID1,19
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.6607141805859151,DISTID1,19
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.005614552396532449,DISTID2,19
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.24398960585735333,DISTID2,19
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.352429430682844,DISTID2,19
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.012297076135210605,DISTID1,19
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.567792709257698,DISTID2,19
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.597922802261125,DISTID2,19
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.2302167525465879,DISTID1,19
 SGB,L,mineral,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,31.121687769087426,DISTID1,19
 SGB,L,mineral,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,22.92104663844408,DISTID1,19
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.019003100419032866,DISTID2,19
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,184.31461796736906,DISTID2,19
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.630674089256902e-08,DISTID1,19
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.5904666771778496e-08,DISTID1,19
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.0201037060395216e-07,DISTID1,19
@@ -899,32 +899,32 @@
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0012288535492708812,DISTID2,20
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0027034778083959376,DISTID2,20
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,26.221535878360484,DISTID2,20
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.7138402388355236e-08,DISTID1,20
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,94.00045516335823,DISTID1,20
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.989202226777071e-08,DISTID1,20
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0011660993438951997,DISTID2,20
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.16265973723823543,DISTID2,20
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.192838073080393,DISTID2,20
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.034186274958652e-09,DISTID1,20
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.1005904980482957e-09,DISTID1,20
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.667978884551764e-09,DISTID1,20
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.423184515337959e-08,DISTID1,20
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0036891228405631824,DISTID1,20
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.604087408523504,DISTID2,20
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.4182143597470409,DISTID2,20
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.9293652438823122,DISTID2,20
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.815345121803624,DISTID2,20
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.733598808954957e-08,DISTID1,20
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.2001837908149696e-08,DISTID1,20
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.6670750906999297e-08,DISTID1,20
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.9558550665132823e-07,DISTID1,20
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.07319688175720601,DISTID2,20
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.10572882920485321,DISTID2,20
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.021078003731250853,DISTID1,20
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.0451951395051298,DISTID2,20
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,22.331431023037624,DISTID2,20
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.6803788409694705e-08,DISTID1,20
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.932569966825015e-08,DISTID1,20
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.739044370722245e-08,DISTID1,20
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.408632538529647e-07,DISTID1,20
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.06906502576397638,DISTID1,20
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.680743616148749,DISTID2,20
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.9328225034875923,DISTID2,20
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.739605563305753,DISTID2,20
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,64.09044079757552,DISTID2,20
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.6302492367792457e-07,DISTID1,20
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.1286340870010154e-07,DISTID1,20
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.5080757488911433e-07,DISTID1,20
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.8392555491868382e-06,DISTID1,20
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.3703378127773098,DISTID2,20
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.9793768406783376,DISTID2,20
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.19821425417577454,DISTID1,20
 SGB,L,mineral,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,29.254386502942182,DISTID1,20
 SGB,L,mineral,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,21.54578384013743,DISTID1,20
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0025913318753226643,DISTID2,20
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.005700930125709861,DISTID2,20
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,55.29438539021073,DISTID2,20
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0016843657189597352,DISTID2,20
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.060311118118565e-08,DISTID1,20
@@ -973,34 +973,34 @@
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00016589522915156908,DISTID2,21
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0003686560647812644,DISTID2,21
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0008110433425187815,DISTID2,21
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.8664607635081465,DISTID2,21
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.7006912347757147e-09,DISTID1,21
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0001665189863082345,DISTID1,21
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,28.20013654900747,DISTID1,21
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0011067368521689549,DISTID1,21
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.021959064527161804,DISTID2,21
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.3578514219241179,DISTID2,21
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.102558824875957e-10,DISTID1,21
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.301771494144888e-10,DISTID1,21
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.4003936653655295e-09,DISTID1,21
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.0269553546013879e-08,DISTID1,21
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.1812262225570512,DISTID2,21
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.03171864876145597,DISTID2,21
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.1254643079241123,DISTID2,21
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.0446035365410875,DISTID2,21
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.200796426864872e-09,DISTID1,21
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.6005513724449094e-09,DISTID1,21
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.00122527209979e-09,DISTID1,21
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.867565199539848e-08,DISTID1,21
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.006323401119375257,DISTID1,21
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.020719507729192916,DISTID1,21
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.41110134383319297,DISTID2,21
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.699429306911288,DISTID2,21
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.7041136522908415e-08,DISTID1,21
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.1797709900475048e-08,DISTID1,21
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.621713311216674e-08,DISTID1,21
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.9225897615588942e-07,DISTID1,21
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.704223084844625,DISTID2,21
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.5938130522035013,DISTID2,21
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.179846751046278,DISTID2,21
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,19.22713223927266,DISTID2,21
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.890747710337738e-08,DISTID1,21
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.385902261003047e-08,DISTID1,21
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.524227246673432e-08,DISTID1,21
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.517766647560516e-07,DISTID1,21
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.05946427625273237,DISTID1,21
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0005053097156879206,DISTID2,21
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.27880957316469374,DISTID2,21
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.6218816689917266,DISTID2,21
 SGB,L,mineral,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,20.253036809729185,DISTID1,21
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.04879792117147063,DISTID2,21
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.9135585418515391,DISTID2,21
 SGB,L,peat,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.248130642830964,DISTID1,21
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00034982980316856,DISTID2,21
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0007773995625967995,DISTID2,21
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0017102790377129587,DISTID2,21
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,16.58831561706322,DISTID2,21
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.967606680331214e-09,DISTID1,21
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.131420009460066e-09,DISTID1,21
@@ -1050,37 +1050,37 @@
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.976856874547074e-05,DISTID2,22
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00011059681943437934,DISTID2,22
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0002433130027556345,DISTID2,22
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.359938229052444,DISTID2,22
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.489821068014889e-10,DISTID1,22
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.3689838722844055e-05,DISTID1,22
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00015159291470637622,DISTID2,22
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0018970203358125775,DISTID1,22
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.017839282875819713,DISTID1,22
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00023321986877903987,DISTID2,22
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.10735542657723539,DISTID2,22
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.7307676474627875e-10,DISTID1,22
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.8905314482434665e-10,DISTID1,22
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.2011809960965896e-10,DISTID1,22
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.0808660638041645e-09,DISTID1,22
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00033202105565068653,DISTID1,22
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,56.22805731692086,DISTID1,22
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.014639376351441193,DISTID2,22
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.05436786676711537,DISTID2,22
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.08364287194940813,DISTID2,22
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.6133810609623264,DISTID2,22
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.5602389280594618e-09,DISTID1,22
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.080165411733473e-09,DISTID1,22
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.4003675816299375e-09,DISTID1,22
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.7602695598619546e-08,DISTID1,22
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.0098287920733866,DISTID2,22
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.112340956872525e-09,DISTID1,22
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.539312970142515e-09,DISTID1,22
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.865139933650023e-09,DISTID1,22
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.7677692846766836e-08,DISTID1,22
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.006215852318757876,DISTID1,22
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1052.6600482239949,DISTID1,22
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.2740675625554618,DISTID2,22
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.5112669254533875,DISTID2,22
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.786564500697518,DISTID2,22
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.768139671781799,DISTID2,22
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.4672243131013215e-08,DISTID1,22
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.0157706783009141e-08,DISTID1,22
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.2572681740020298e-08,DISTID1,22
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.6553299942681548e-07,DISTID1,22
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00010494894095056802,DISTID2,22
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.037639292377233693,DISTID2,22
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.006587719358148543,DISTID2,22
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,321.26205961363866,DISTID1,22
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.3539540253138834,DISTID2,22
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.12333040314995791,DISTID2,22
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3021.0982194143326,DISTID1,22
 SGB,L,mineral,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,19.03785460114543,DISTID1,22
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.009515594628436791,DISTID2,22
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.17814391566105045,DISTID2,22
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.976494685118967,DISTID2,22
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.7902820040993644e-09,DISTID1,22
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.23942600283802e-09,DISTID1,22
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.7542800063067097e-09,DISTID1,22
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.05941601387476e-09,DISTID1,22
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.877140693231807e-05,DISTID1,22
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.952989370237933,DISTID1,22
@@ -1129,40 +1129,40 @@
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.31790458303138e-05,DISTID2,23
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.299390082669037e-05,DISTID2,23
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.7079814687157334,DISTID2,23
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.330622111298144e-10,DISTID1,23
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.547787441191287e-05,DISTID2,23
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.4986708767741107e-05,DISTID1,23
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.996596063371198e-05,DISTID2,23
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.03220662797317062,DISTID2,23
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.192302942388365e-11,DISTID1,23
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.6715943447304007e-11,DISTID1,23
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.260354298828977e-10,DISTID1,23
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.242598191412494e-10,DISTID1,23
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.960631669520597e-05,DISTID1,23
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,16.868417195076262,DISTID1,23
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.004391812905432359,DISTID2,23
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.016310360030134613,DISTID2,23
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.025092861584822445,DISTID2,23
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.18401431828869794,DISTID2,23
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.680716784178386e-10,DISTID1,23
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.2404962352004197e-10,DISTID1,23
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.201102744889814e-10,DISTID1,23
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.280808679585865e-09,DISTID1,23
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0005691061007437733,DISTID1,23
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.011291787713170109,DISTID2,23
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0019763158074445632,DISTID2,23
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,96.37861788409161,DISTID1,23
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.6029486376220161,DISTID2,23
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.5337022870617577e-09,DISTID1,23
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.0617938910427545e-09,DISTID1,23
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.359541980095007e-09,DISTID1,23
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.7303307854030053e-08,DISTID1,23
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0018647556956273633,DISTID1,23
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,315.7980144671985,DISTID1,23
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.08222026876663854,DISTID2,23
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.15338007763601627,DISTID2,23
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.23596935020925544,DISTID2,23
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.7304419015345398,DISTID2,23
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.401672939303965e-09,DISTID1,23
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.047312034902743e-09,DISTID1,23
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.77180452200609e-09,DISTID1,23
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.965989982804465e-08,DISTID1,23
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0053517848627459156,DISTID1,23
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.10618620759416504,DISTID2,23
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.03699912094498738,DISTID2,23
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,906.3294658242999,DISTID1,23
 SGB,L,mineral,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,17.895583325076704,DISTID1,23
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00015392511339416633,DISTID2,23
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.148468228517041e-05,DISTID2,23
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.4929484055356903,DISTID2,23
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.370846012298093e-10,DISTID1,23
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.7182780085140606e-10,DISTID1,23
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.002854678388531038,DISTID2,23
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.053443174698315145,DISTID2,23
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.8178248041624282e-09,DISTID1,23
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.7631422079695425e-05,DISTID1,23
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.26284001892013e-10,DISTID1,23
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.982099815987518e-10,DISTID1,23
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.83376141106828e-10,DISTID1,23
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.0741692024596168e-09,DISTID1,23
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00012006158844744973,DISTID1,23
@@ -1208,35 +1208,35 @@
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.189817024800711e-05,DISTID2,24
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.21239444061472007,DISTID2,24
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.640838961213403e-11,DISTID1,24
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.1755136863405217e-10,DISTID1,24
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.3643362323573863e-05,DISTID2,24
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.445404685551124e-06,DISTID2,24
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.0989788190113595e-05,DISTID2,24
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.009661988391951188,DISTID2,24
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.4576908827165096e-11,DISTID1,24
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.7014783034191207e-11,DISTID1,24
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.7810628964869314e-11,DISTID1,24
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.772779457423749e-10,DISTID1,24
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.9881895008561794e-05,DISTID1,24
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.004893108009040385,DISTID2,24
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0013175438716297077,DISTID2,24
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.003387536313951033,DISTID2,24
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.055204295486609385,DISTID2,24
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.404215035253516e-10,DISTID1,24
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.72148870560126e-11,DISTID1,24
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.1603308234669444e-10,DISTID1,24
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.5842426038757598e-09,DISTID1,24
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00017073183022313203,DISTID1,24
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,28.91358536522749,DISTID1,24
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.007527858475446735,DISTID2,24
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.000592894742233369,DISTID2,24
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.0605251585228785,DISTID1,24
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.18088459128660483,DISTID2,24
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.601106861185274e-10,DISTID1,24
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.185381673128264e-10,DISTID1,24
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.078625940285023e-10,DISTID1,24
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.190992356209017e-09,DISTID1,24
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.000559426708688209,DISTID1,24
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.04601402329080489,DISTID2,24
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.024666080629991566,DISTID2,24
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.03185586227824952,DISTID2,24
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.519132570460362,DISTID2,24
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.32050188179119e-09,DISTID1,24
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.14193610470823e-10,DISTID1,24
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.0315413566018275e-09,DISTID1,24
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.4897969948413398e-08,DISTID1,24
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.001605535458823775,DISTID1,24
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,271.89883974729,DISTID1,24
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.07079080506277664,DISTID2,24
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.011099736283496215,DISTID2,24
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,94.73940434015957,DISTID1,24
 SGB,L,mineral,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,16.821848325572102,DISTID1,24
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0008564035165593114,DISTID2,24
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.016032952409494546,DISTID2,24
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.44788452166070714,DISTID2,24
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.6112538036894283e-10,DISTID1,24
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.1154834025542185e-10,DISTID1,24
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.478852005676039e-10,DISTID1,24
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.453474412487286e-10,DISTID1,24
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.289426623908628e-06,DISTID1,24
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.8957690433214143,DISTID1,24
@@ -1284,37 +1284,37 @@
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.3437513561277104e-06,DISTID2,25
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.9861141247282434e-06,DISTID2,25
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.569451074402135e-06,DISTID2,25
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.06371833218441603,DISTID2,25
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.292251688364021e-11,DISTID1,25
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.5265410590215654e-11,DISTID1,25
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.09300869707216e-06,DISTID2,25
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.674075609568249,DISTID1,25
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,81.56965192418701,DISTID1,25
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.29693645703408e-06,DISTID2,25
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0028985965175853568,DISTID2,25
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.37307264814953e-12,DISTID1,25
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.104434910257363e-12,DISTID1,25
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.1343188689460795e-11,DISTID1,25
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.318338372271248e-11,DISTID1,25
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.96456850256854e-06,DISTID1,25
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.5181575475568638,DISTID1,25
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0003952631614889124,DISTID2,25
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0010162608941853102,DISTID2,25
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.01656128864598282,DISTID2,25
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.2126451057605485e-11,DISTID1,25
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.916446611680378e-11,DISTID1,25
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.480992470400834e-11,DISTID1,25
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.75272781162728e-10,DISTID1,25
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.121954906693962e-05,DISTID1,25
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.05426537738598146,DISTID2,25
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.3803320583555824e-10,DISTID1,25
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.556145019384794e-11,DISTID1,25
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.1235877820855072e-10,DISTID1,25
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.5572977068627053e-09,DISTID1,25
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00016782801260646274,DISTID1,25
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,28.42182130204787,DISTID1,25
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.007399824188997471,DISTID2,25
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.009556758683474857,DISTID2,25
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.15573977113810863,DISTID2,25
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.9615056453735706e-10,DISTID1,25
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.7425808314124693e-10,DISTID1,25
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.094624069805484e-10,DISTID1,25
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.4693909845240206e-09,DISTID1,25
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00048166063764713254,DISTID1,25
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.833621405665338e-06,DISTID2,25
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0022583575426340205,DISTID2,25
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00017786842267001072,DISTID2,25
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0014679324027121155,DISTID2,25
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.021237241518832994,DISTID2,25
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.003329920885048865,DISTID2,25
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.01380420698724147,DISTID2,25
 SGB,L,mineral,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,15.812537426037775,DISTID1,25
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00025692105496779346,DISTID2,25
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.004809885722848364,DISTID2,25
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.13436535649821216,DISTID2,25
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.833761411068286e-11,DISTID1,25
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.346450207662656e-11,DISTID1,25
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.43655601702812e-11,DISTID1,25
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.636042323746186e-10,DISTID1,25
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.5868279871725887e-06,DISTID1,25
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.2687307129964243,DISTID1,25
@@ -1365,35 +1365,35 @@
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.019115499655324813,DISTID2,26
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.8767550650920644e-12,DISTID1,26
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.760830429679119e-12,DISTID1,26
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.3275170989542337e-11,DISTID1,26
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.500864216996015e-07,DISTID2,26
 SGB,L,mineral,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,61.32511485477973,DISTID1,26
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.155978061642493e-06,DISTID2,26
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.2119217944448593e-12,DISTID1,26
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.531330473077209e-12,DISTID1,26
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.402956606838239e-12,DISTID1,26
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.4955015116813747e-11,DISTID1,26
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.6893705507705625e-06,DISTID1,26
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.4554472642670592,DISTID1,26
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00030487826825559305,DISTID2,26
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0008695789552756072,DISTID2,26
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0006775072627902063,DISTID2,26
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.2637935317281648e-11,DISTID1,26
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.749339835041136e-12,DISTID1,26
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.9442977411202503e-11,DISTID1,26
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.4258183434881842e-10,DISTID1,26
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.5365864720081888e-05,DISTID1,26
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.6022226828704746,DISTID1,26
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.1409961750667484e-11,DISTID1,26
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.8668435058154385e-11,DISTID1,26
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.370763346256523e-11,DISTID1,26
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.671893120588116e-10,DISTID1,26
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.0348403781938827e-05,DISTID1,26
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.526546390614362,DISTID1,26
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0028670276050424574,DISTID2,26
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.01627961321579444,DISTID2,26
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.006371172455649899,DISTID2,26
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.1884516936120713e-10,DISTID1,26
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.22774249423741e-11,DISTID1,26
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.8283872209416455e-10,DISTID1,26
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.3408172953572063e-09,DISTID1,26
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00014449819129413977,DISTID1,26
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,24.47089557725611,DISTID1,26
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.8890809371102242e-06,DISTID2,26
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.004968386593794847,DISTID2,26
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00011857894844667374,DISTID2,26
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00044037972081363477,DISTID2,26
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.707631649033805e-05,DISTID2,26
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.336052680100323e-05,DISTID2,26
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.04672193134143259,DISTID2,26
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0022199472566992416,DISTID2,26
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.004141262096172442,DISTID2,26
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0014429657168545094,DISTID2,26
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0009989762655146597,DISTID2,26
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.4501284233204858e-11,DISTID1,26
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.003935062298797e-11,DISTID1,26
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.2309668051084362e-11,DISTID1,26
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.908126971238558e-11,DISTID1,26
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.760483961517767e-07,DISTID1,26
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0806192138989273,DISTID1,26
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.8851669503166308e-11,DISTID1,26
@@ -1444,37 +1444,37 @@
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.6875027122554195e-07,DISTID2,27
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.912505966961924e-07,DISTID2,27
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.005734649896597444,DISTID2,27
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.06302651952762e-12,DISTID1,27
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.17388695311941e-12,DISTID1,27
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.550259265098805e-07,DISTID2,27
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.667242811330674e-07,DISTID2,27
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.7806668048611426,DISTID1,27
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,28.11402865846043,DISTID2,27
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.635765383334579e-13,DISTID1,27
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.593991419231628e-13,DISTID1,27
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.020886982051472e-12,DISTID1,27
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.486504535044125e-12,DISTID1,27
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.068111652311688e-07,DISTID1,27
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00013211391624409045,DISTID2,27
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.146348047667794e-05,DISTID2,27
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00020325217883706192,DISTID2,27
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0014905159781384541,DISTID2,27
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,160.63102980681933,DISTID2,27
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.791380595184495e-12,DISTID1,27
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.6248019505123413e-12,DISTID1,27
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.832893223360752e-12,DISTID1,27
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.277455030464553e-11,DISTID1,27
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.609759416024567e-06,DISTID1,27
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.341268673176833,DISTID1,27
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,526.3300241119974,DISTID2,27
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.2422988525200247e-11,DISTID1,27
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.600530517446317e-12,DISTID1,27
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.911229003876957e-11,DISTID1,27
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.4015679361764352e-10,DISTID1,27
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.5104521134581651e-05,DISTID1,27
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0012423786288517328,DISTID2,27
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0008601082815127373,DISTID2,27
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0019113517366949702,DISTID2,27
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.01401657940242978,DISTID2,27
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1510.5491097071663,DISTID2,27
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.5653550808362145e-11,DISTID1,27
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.4683227482712236e-11,DISTID1,27
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.485161662824937e-11,DISTID1,27
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.022451886071619e-10,DISTID1,27
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.334945738824194e-05,DISTID1,27
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.2467934184927482e-06,DISTID2,27
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00026087368658268215,DISTID2,27
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.557368453400213e-05,DISTID2,27
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.13663417928011778,DISTID1,27
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.312289494710142e-05,DISTID2,27
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.600815804030097e-05,DISTID2,27
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.004883883964738332,DISTID2,27
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0006659841770097725,DISTID2,27
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.5579639171843094,DISTID1,27
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0004328897150563529,DISTID2,27
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.000299692879654398,DISTID2,27
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.350385269961459e-12,DISTID1,27
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.0118051868963915e-12,DISTID1,27
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.69290041532531e-12,DISTID1,27
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.4724380913715676e-11,DISTID1,27
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.42814518845533e-07,DISTID1,27
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.024185764169678197,DISTID1,27
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.655500850949893e-12,DISTID1,27
@@ -1526,39 +1526,39 @@
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.06250813676626e-08,DISTID2,28
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.7737517900885774e-07,DISTID2,28
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0017203949689792335,DISTID2,28
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.18907955858286e-13,DISTID1,28
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.2847473867112084e-13,DISTID1,28
 Sitka,L,peat,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.7269892428953334e-08,DISTID1,28
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.7001728433992026e-07,DISTID2,28
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.1374141785553486e-12,DISTID1,28
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.0696065242508645e-11,DISTID1,28
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0036278646254517305,DISTID2,28
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.434208597538131,DISTID2,28
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.9907296150003736e-13,DISTID1,28
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.3781974257694886e-13,DISTID1,28
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.062660946154416e-13,DISTID1,28
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.245951360513238e-12,DISTID1,28
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.420433495693507e-07,DISTID1,28
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.04099025378403534,DISTID1,28
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.963417487322714e-05,DISTID2,28
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.7439044143003383e-05,DISTID2,28
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00044715479344153633,DISTID2,28
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,48.189308942045805,DISTID2,28
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.874405851537025e-13,DISTID1,28
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.749867967008226e-12,DISTID1,28
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.283236509139366e-11,DISTID1,28
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.3829278248073703e-06,DISTID1,28
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.23420004145834278,DISTID1,28
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,157.89900723359926,DISTID2,28
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.726896557560074e-12,DISTID1,28
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.5801591552338954e-12,DISTID1,28
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.7336870116308726e-12,DISTID1,28
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.204703808529306e-11,DISTID1,28
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.531356340374496e-06,DISTID1,28
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.7673891751552929,DISTID1,28
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0003727135886555199,DISTID2,28
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00025803248445382124,DISTID2,28
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.004204973820728934,DISTID2,28
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,453.16473291214993,DISTID2,28
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.404968244813672e-12,DISTID1,28
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.6455484988474813e-11,DISTID1,28
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.206735565821486e-10,DISTID1,28
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.3004837216472582e-05,DISTID1,28
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.20238060195305,DISTID1,28
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.740380255478245e-07,DISTID2,28
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.826210597480466e-05,DISTID2,28
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.0672105360200638e-05,DISTID2,28
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.097565365111858e-05,DISTID2,28
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.936868484130426e-06,DISTID2,28
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0014651651894215,DISTID2,28
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0001997952531029318,DISTID2,28
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0005734055210084912,DISTID2,28
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00012986691451690588,DISTID2,28
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.305115580988438e-12,DISTID1,28
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.802447412090292e-06,DISTID2,28
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.990786389631941e-05,DISTID2,28
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.035415560689175e-13,DISTID1,28
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.0078701245975933e-12,DISTID1,28
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.4173142741147034e-12,DISTID1,28
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.284435565365991e-08,DISTID1,28
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.696650255284968e-12,DISTID1,28
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.174604022889593e-12,DISTID1,28
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.007255729250903461,DISTID1,28
@@ -1618,41 +1618,41 @@
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.4187524410298784e-08,DISTID2,29
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.321255370265732e-08,DISTID2,29
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0005161184906937701,DISTID2,29
 Sitka,L,peat,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,87.40511959453492,DISTID2,29
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,56.813327736447796,DISTID1,29
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,87.40511959453492,DISTID1,29
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.1264151398992503e-12,DISTID1,29
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.231713242901016e-06,DISTID2,29
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.740974533614638e-05,DISTID2,29
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0018502109589803827,DISTID1,29
 SGB,L,mineral,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,50.93565919654235,DISTID1,29
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.081060545239128e-06,DISTID2,29
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.4407342236270877e-06,DISTID2,29
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.2016316080601917e-06,DISTID2,29
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.3478631792441403e-05,DISTID2,29
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.5302625792614393,DISTID2,29
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.972188845001122e-14,DISTID1,29
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.134592277308466e-14,DISTID1,29
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.187982838463249e-14,DISTID1,29
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.737854081539714e-13,DISTID1,29
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.8960074355071775e-05,DISTID2,29
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.697235916889583e-05,DISTID2,29
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.993857593087955e-05,DISTID2,29
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0004395495568264501,DISTID2,29
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,47.36970217007978,DISTID2,29
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.1180689672680226e-12,DISTID1,29
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.740477465701687e-13,DISTID1,29
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.720106103489262e-12,DISTID1,29
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.2614111425587918e-11,DISTID1,29
 SGB,L,mineral,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,12.345622150340068,DISTID1,29
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.261300487080522e-08,DISTID1,29
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.829269609533558e-05,DISTID2,29
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00013414643803246092,DISTID2,29
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,14.456792682613745,DISTID2,29
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.4122425356660465e-13,DISTID1,29
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.362321755461108e-13,DISTID1,29
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.249603901024679e-13,DISTID1,29
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.849709527418099e-12,DISTID1,29
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.148783474422111e-07,DISTID1,29
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.07026001243750284,DISTID1,29
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.359406902112349e-06,DISTID1,29
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00017202165630254737,DISTID2,29
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0012614921462186805,DISTID2,29
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,135.949419873645,DISTID2,29
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.208819572752594e-12,DISTID1,29
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.221490473444102e-12,DISTID1,29
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.936645496542445e-12,DISTID1,29
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.620206697464459e-11,DISTID1,29
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.901451164941775e-06,DISTID1,29
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.6607141805859151,DISTID1,29
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.0925310691683276e-08,DISTID1,29
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.1890252461968143e-05,DISTID2,29
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00011181407659665599,DISTID2,29
 SGB,L,mineral,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,16.76261140857286,DISTID1,29
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.012297076135210605,DISTID1,29
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.2302167525465879,DISTID1,29
 SGB,L,peat,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.37039060965215,DISTID1,29
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.315337044628451e-08,DISTID2,29
 SGB,L,peat,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.653967714981547,DISTID1,29
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.2952333385889248e-08,DISTID2,29
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.100518530197608e-08,DISTID2,29
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.1221140766434735e-07,DISTID2,29
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0010883593876355193,DISTID2,29
@@ -1733,38 +1733,38 @@
 Sitka,L,peat,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,17.043998320934342,DISTID1,30
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.984134194561547e-14,DISTID1,30
 Sitka,L,mineral,YC17_20,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0006530156325813117,DISTID1,30
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.536020645317158e-13,DISTID1,30
 SGB,L,mineral,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,15.756854724058485,DISTID1,30
 SGB,L,mineral,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,11.604884821319661,DISTID1,30
 SGB,L,mineral,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,47.87951964474981,DISTID1,30
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.243181635717386e-07,DISTID2,30
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.322202670881264e-07,DISTID2,30
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.604894824180577e-07,DISTID2,30
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.043589537732421e-06,DISTID2,30
-CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.7590787737784319,DISTID2,30
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.7916566535003368e-14,DISTID1,30
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.24037768319254e-14,DISTID1,30
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.7563948515389752e-14,DISTID1,30
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.0213562244619147e-13,DISTID1,30
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.1688022306521534e-05,DISTID2,30
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8.09170775066875e-06,DISTID2,30
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.7981572779263868e-05,DISTID2,30
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00013186486704793503,DISTID2,30
+CBmix,L,peat,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,14.210910651023935,DISTID2,30
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.354206901804068e-13,DISTID1,30
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.322143239710507e-13,DISTID1,30
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.160318310467786e-13,DISTID1,30
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.784233427676376e-12,DISTID1,30
 SGB,L,peat,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.3147296520826535,DISTID1,30
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.1783901461241567e-08,DISTID1,30
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.5670757385904438e-06,DISTID2,30
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.4695139728703053e-06,DISTID2,30
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.487808828600674e-06,DISTID2,30
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.0243931409738284e-05,DISTID2,30
-CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.337037804784124,DISTID2,30
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.0236727606998141e-13,DISTID1,30
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,7.086965266383325e-14,DISTID1,30
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.5748811703074038e-13,DISTID1,30
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.1549128582254297e-12,DISTID1,30
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.2446350423266335e-07,DISTID1,30
-CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.021078003731250853,DISTID1,30
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,4.0782207063370473e-07,DISTID1,30
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.35442229789968e-05,DISTID2,30
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.322292360084392e-05,DISTID2,30
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,5.160649689076422e-05,DISTID2,30
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.00037844764386560424,DISTID2,30
+CBmix,L,mineral,YC10,False,15,39,15,39,5,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,40.78482596209351,DISTID2,30
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.626458718257784e-13,DISTID1,30
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,6.664471420332306e-13,DISTID1,30
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.4809936489627337e-12,DISTID1,30
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.0860620092393379e-11,DISTID1,30
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.170435349482533e-06,DISTID1,30
+CBmix,L,mineral,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.19821425417577454,DISTID1,30
 Sitka,L,peat,YC20_24,False,10,27,10,27,4,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,2.7755184260817875e-09,DISTID2,30
-CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0036891228405631824,DISTID1,30
+CBmix,L,peat,YC10,False,31,200,31,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.06906502576397638,DISTID1,30
 SGB,L,peat,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.2881671730730209,DISTID1,30
 SGB,L,peat,YC6,False,65,210,65,210,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,1.7490447616613685,DISTID1,30
 Sitka,L,mineral,YC13_16,False,39,200,39,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,479.21800671515956,DISTID1,30
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.3792454196977513e-13,DISTID1,30
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,3.2775932075049835e-09,DISTID1,30
 Sitka,L,mineral,YC20_24,False,28,200,28,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,0.0005550632876941148,DISTID1,30
 Sitka,L,mineral,YC17_20,False,10,33,10,33,3,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,9.946011133885355e-09,DISTID2,30
```

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/inventory.csv`

 * *Files 2% similar despite different names*

```diff
@@ -55,19 +55,19 @@
 SGB,L,mineral,YC6,False,51,664.3554109267815,0,0,DISTID3,DISTID3
 SGB,L,peat,YC6,False,10,158.83512486343278,0,0,DISTID3,DISTID3
 SGB,L,peat,YC6,False,20,158.83512486343278,0,0,DISTID3,DISTID3
 SGB,L,peat,YC6,False,30,249.59805335682293,0,0,DISTID3,DISTID3
 SGB,L,peat,YC6,False,40,113.4536606167377,0,0,DISTID3,DISTID3
 SGB,L,peat,YC6,False,50,51.054147277532,0,0,DISTID3,DISTID3
 SGB,L,peat,YC6,False,51,73.74487940087963,0,0,DISTID3,DISTID3
-CBmix,L,mineral,YC10,False,10,458.94579944805525,0,0,DISTID3,DISTID3
-CBmix,L,mineral,YC10,False,20,458.94579944805525,0,0,DISTID3,DISTID3
-CBmix,L,mineral,YC10,False,30,721.2005419898011,0,0,DISTID3,DISTID3
-CBmix,L,mineral,YC10,False,40,327.8184281771823,0,0,DISTID3,DISTID3
-CBmix,L,mineral,YC10,False,50,147.51829267973216,0,0,DISTID3,DISTID3
-CBmix,L,mineral,YC10,False,51,213.08197831516887,0,0,DISTID3,DISTID3
-CBmix,L,peat,YC10,False,10,80.32579616702981,0,0,DISTID3,DISTID3
-CBmix,L,peat,YC10,False,20,80.32579616702981,0,0,DISTID3,DISTID3
-CBmix,L,peat,YC10,False,30,126.22625111961825,0,0,DISTID3,DISTID3
-CBmix,L,peat,YC10,False,40,57.37556869073557,0,0,DISTID3,DISTID3
-CBmix,L,peat,YC10,False,50,25.819005910831027,0,0,DISTID3,DISTID3
-CBmix,L,peat,YC10,False,51,37.29411964897818,0,0,DISTID3,DISTID3
+CBmix,L,mineral,YC10,False,10,4315.854599163333,0,0,DISTID3,DISTID3
+CBmix,L,mineral,YC10,False,20,4315.854599163333,0,0,DISTID3,DISTID3
+CBmix,L,mineral,YC10,False,30,6782.057227256666,0,0,DISTID3,DISTID3
+CBmix,L,mineral,YC10,False,40,3082.753285116666,0,0,DISTID3,DISTID3
+CBmix,L,mineral,YC10,False,50,1387.238978302501,0,0,DISTID3,DISTID3
+CBmix,L,mineral,YC10,False,51,2003.7896353258363,0,0,DISTID3,DISTID3
+CBmix,L,peat,YC10,False,10,1503.8000688914215,0,0,DISTID3,DISTID3
+CBmix,L,peat,YC10,False,20,1503.8000688914215,0,0,DISTID3,DISTID3
+CBmix,L,peat,YC10,False,30,2363.1143939722338,0,0,DISTID3,DISTID3
+CBmix,L,peat,YC10,False,40,1074.1429063510152,0,0,DISTID3,DISTID3
+CBmix,L,peat,YC10,False,50,483.3643078579573,0,0,DISTID3,DISTID3
+CBmix,L,peat,YC10,False,51,698.1928891281611,0,0,DISTID3,DISTID3
```

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/spinup_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/spinup_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/standing_vol.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/standing_vol.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/baseline_input_conf/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/catchment_forest_cover.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/catchment_forest_cover.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,22 +50,23 @@
             pandas.DataFrame: A DataFrame containing aggregated forest cover data for the specified catchment,
             structured by forest species, with columns for different soil types and their corresponding
             total hectares.
         """
         forest_df = self.api.get_catchment_forest_data_by_catchment_name(catchment)
 
         # Filter for specific types of forests and then group
-        forest_types = ['Broadleaved Forest and Woodland', 'Coniferous Forest', 'Mixed Forest']
+        forest_types = ['Broadleaved Forest and Woodland', 'Coniferous Forest', 'Mixed Forest', 'Transitional Forest']
         filtered_df = forest_df[forest_df['cover_type'].isin(forest_types)].copy()
 
         # Mapping for cover_type and soil_type
         cover_type_mapping = {
             'Mixed Forest': 'CBmix',
             'Coniferous Forest': 'Sitka',
-            'Broadleaved Forest and Woodland': 'SGB'
+            'Broadleaved Forest and Woodland': 'SGB',
+            'Transitional Forest': 'CBmix'
         }
 
         soil_type_mapping = {
             'mineral': 'mineral',
             'misc': 'mineral',
             'peaty_mineral': 'peat',
             'peat': 'peat'
@@ -84,9 +85,9 @@
         # Reset index to make 'catchment' and 'cover_type' back to columns and rename columns
         pivot_df.reset_index(inplace=True)
         pivot_df.columns.name = None  # Remove the name of the columns axis
         pivot_df = pivot_df.rename(columns={'cover_type': 'species', 'Peat': 'peat', 'Mineral': 'mineral'})
 
         # Select only the required columns
         final_df = pivot_df[['species', 'peat', 'mineral']]
-
+ 
         return final_df
```

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/-1/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/0/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/generated_input_data/1/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/geo_cbm_data_factory.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/geo_cbm_data_factory.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/geo_create_json.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/geo_create_json.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/geo_disturbances.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/geo_disturbances.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/geo_inventory.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/geo_inventory.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/geo_runner.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/geo_runner.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/geo_cbm_runner/geo_transition.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/geo_cbm_runner/geo_transition.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/harvest_manager/harvest.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/harvest_manager/harvest.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/-1/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/0/classifiers.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/0/classifiers.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/0/disturbance_events.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/0/disturbance_events.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/0/growth.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/0/growth.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/0/inventory.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/0/inventory.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/0/sit_config.json` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/0/sit_config.json`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/generated_input_data/0/transitions.csv` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/generated_input_data/0/transitions.csv`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/historic_affor/historic_affor_runner.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/historic_affor/historic_affor_runner.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/resource_manager/cbm_pools.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/resource_manager/cbm_pools.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/resource_manager/cbm_runner_data_manager.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/resource_manager/cbm_runner_data_manager.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/resource_manager/database_manager.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/resource_manager/database_manager.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/resource_manager/flux_manager.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/resource_manager/flux_manager.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/resource_manager/geo_cbm_runner_data_manager.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/resource_manager/geo_cbm_runner_data_manager.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/resource_manager/loader.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/resource_manager/loader.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/resource_manager/parser.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/resource_manager/parser.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/resource_manager/paths.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/resource_manager/paths.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/src/goblin_cbm_runner/resource_manager/scenario_data_fetcher.py` & `goblin_cbm_runner-0.3.5/src/goblin_cbm_runner/resource_manager/scenario_data_fetcher.py`

 * *Files identical despite different names*

### Comparing `goblin_cbm_runner-0.3.4/PKG-INFO` & `goblin_cbm_runner-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goblin_cbm_runner
-Version: 0.3.4
+Version: 0.3.5
 Summary: An interface between the CBM CFS3, libcbm_py, model and the GOBLIN model.
 License: MIT
 Author: Colm Duffy
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

