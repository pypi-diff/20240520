# Comparing `tmp/teaspoon-1.5.2.tar.gz` & `tmp/teaspoon-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teaspoon-1.5.2.tar", last modified: Sun Apr 21 19:14:20 2024, max compression
+gzip compressed data, was "teaspoon-1.5.3.tar", last modified: Mon May 20 19:21:15 2024, max compression
```

## Comparing `teaspoon-1.5.2.tar` & `teaspoon-1.5.3.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:14:20.193150 teaspoon-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35142 2024-04-21 19:13:08.000000 teaspoon-1.5.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-21 19:14:20.193150 teaspoon-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-21 19:13:08.000000 teaspoon-1.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-21 19:13:09.000000 teaspoon-1.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-21 19:14:20.193150 teaspoon-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-21 19:13:09.000000 teaspoon-1.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:14:20.117150 teaspoon-1.5.2/teaspoon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:14:20.121150 teaspoon-1.5.2/teaspoon/teaspoon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:14:20.121150 teaspoon-1.5.2/teaspoon/teaspoon/ML/
--rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/ML/Base.py
--rw-r--r--   0 runner    (1001) docker     (127)    29657 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/ML/PD_Classification.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       77 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/ML/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:14:20.173150 teaspoon-1.5.2/teaspoon/teaspoon/ML/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/ML/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127) 21567451 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/ML/datasets/mnist.pickle
--rw-r--r--   0 runner    (1001) docker     (127) 20646231 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/ML/datasets/mpeg7.pickle
--rw-r--r--   0 runner    (1001) docker     (127)  8765120 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/ML/datasets/shrec14.pickle
--rw-r--r--   0 runner    (1001) docker     (127)    51886 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/ML/feature_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/ML/load_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:14:20.185150 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:14:20.185150 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/
--rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/DynSysLib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/UserGuide.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37504 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/autonomous_dissipative_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/conservative_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/delayed_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)    17123 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/driven_dissipative_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)    23405 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/maps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/medical_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/noise_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/periodic_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21965 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/PointCloud.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/MakeData/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:14:20.185150 teaspoon-1.5.2/teaspoon/teaspoon/SP/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/SP/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26581 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/SP/adaptivePart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:14:20.185150 teaspoon-1.5.2/teaspoon/teaspoon/SP/information/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/SP/information/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/SP/information/entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/SP/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    10001 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/SP/network_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    15583 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/SP/texture_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    27456 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/SP/tsa_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:14:20.189150 teaspoon-1.5.2/teaspoon/teaspoon/TDA/
--rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/TDA/Distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/TDA/Draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/TDA/Magnitude.py
--rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/TDA/PHN.py
--rw-r--r--   0 runner    (1001) docker     (127)     7585 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/TDA/Persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/TDA/SLSP.py
--rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/TDA/SLSP_tools.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/TDA/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/TDA/c_profile_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:14:20.189150 teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/
--rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/FNN_n.py
--rw-r--r--   0 runner    (1001) docker     (127)    23996 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/MI_delay.py
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/MsPE.py
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/PAMI_delay.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/autocorrelation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-04-21 19:13:09.000000 teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/delay_LMS.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:14:20.193150 teaspoon-1.5.2/teaspoon/teaspoon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-21 19:14:20.000000 teaspoon-1.5.2/teaspoon/teaspoon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-21 19:14:20.000000 teaspoon-1.5.2/teaspoon/teaspoon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-21 19:14:20.000000 teaspoon-1.5.2/teaspoon/teaspoon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-21 19:14:20.000000 teaspoon-1.5.2/teaspoon/teaspoon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 19:14:20.000000 teaspoon-1.5.2/teaspoon/teaspoon.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:14:20.193150 teaspoon-1.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-21 19:13:09.000000 teaspoon-1.5.2/tests/test_MakeData.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-21 19:13:09.000000 teaspoon-1.5.2/tests/test_OrdinalPartition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-21 19:13:09.000000 teaspoon-1.5.2/tests/test_PointSummariesPHN.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-21 19:13:09.000000 teaspoon-1.5.2/tests/test_SLSP.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-21 19:13:09.000000 teaspoon-1.5.2/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-21 19:13:09.000000 teaspoon-1.5.2/tests/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-21 19:13:09.000000 teaspoon-1.5.2/tests/test_featureFunctions.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-21 19:13:09.000000 teaspoon-1.5.2/tests/test_magnitude.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-21 19:13:09.000000 teaspoon-1.5.2/tests/test_parameterSelection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-04-21 19:13:09.000000 teaspoon-1.5.2/tests/test_signalProcessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-21 19:13:09.000000 teaspoon-1.5.2/tests/test_texture_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:15.029278 teaspoon-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35142 2024-05-20 19:20:02.000000 teaspoon-1.5.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-20 19:21:15.029278 teaspoon-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-20 19:20:02.000000 teaspoon-1.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-20 19:20:04.000000 teaspoon-1.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-20 19:21:15.029278 teaspoon-1.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-20 19:20:04.000000 teaspoon-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:14.953277 teaspoon-1.5.3/teaspoon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:14.957277 teaspoon-1.5.3/teaspoon/teaspoon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:14.961277 teaspoon-1.5.3/teaspoon/teaspoon/ML/
+-rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/ML/Base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29657 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/ML/PD_Classification.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       77 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/ML/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:15.009278 teaspoon-1.5.3/teaspoon/teaspoon/ML/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/ML/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127) 21567451 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/ML/datasets/mnist.pickle
+-rw-r--r--   0 runner    (1001) docker     (127) 20646231 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/ML/datasets/mpeg7.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)  8765120 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/ML/datasets/shrec14.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)    51886 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/ML/feature_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/ML/load_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:15.021278 teaspoon-1.5.3/teaspoon/teaspoon/MakeData/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:15.025278 teaspoon-1.5.3/teaspoon/teaspoon/MakeData/DynSysLib/
+-rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/MakeData/DynSysLib/DynSysLib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/MakeData/DynSysLib/UserGuide.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/MakeData/DynSysLib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37504 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/MakeData/DynSysLib/autonomous_dissipative_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/MakeData/DynSysLib/conservative_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/MakeData/DynSysLib/delayed_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17123 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/MakeData/DynSysLib/driven_dissipative_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23405 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/MakeData/DynSysLib/maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/MakeData/DynSysLib/medical_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/MakeData/DynSysLib/noise_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/MakeData/DynSysLib/periodic_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21965 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/MakeData/PointCloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/MakeData/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:15.025278 teaspoon-1.5.3/teaspoon/teaspoon/SP/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/SP/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26581 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/SP/adaptivePart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:15.025278 teaspoon-1.5.3/teaspoon/teaspoon/SP/information/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/SP/information/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/SP/information/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/SP/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10001 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/SP/network_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15583 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/SP/texture_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27456 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/SP/tsa_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:15.025278 teaspoon-1.5.3/teaspoon/teaspoon/TDA/
+-rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/TDA/Distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/TDA/Draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/TDA/Magnitude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/TDA/PHN.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7585 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/TDA/Persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/TDA/SLSP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/TDA/SLSP_tools.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/TDA/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/TDA/c_profile_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:15.029278 teaspoon-1.5.3/teaspoon/teaspoon/parameter_selection/
+-rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/parameter_selection/FNN_n.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23996 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/parameter_selection/MI_delay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/parameter_selection/MsPE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/parameter_selection/PAMI_delay.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/parameter_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/parameter_selection/autocorrelation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-20 19:20:04.000000 teaspoon-1.5.3/teaspoon/teaspoon/parameter_selection/delay_LMS.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:15.029278 teaspoon-1.5.3/teaspoon/teaspoon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-20 19:21:14.000000 teaspoon-1.5.3/teaspoon/teaspoon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-20 19:21:14.000000 teaspoon-1.5.3/teaspoon/teaspoon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-20 19:21:14.000000 teaspoon-1.5.3/teaspoon/teaspoon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-20 19:21:14.000000 teaspoon-1.5.3/teaspoon/teaspoon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 19:21:14.000000 teaspoon-1.5.3/teaspoon/teaspoon.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:21:15.029278 teaspoon-1.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-20 19:20:04.000000 teaspoon-1.5.3/tests/test_MakeData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-20 19:20:04.000000 teaspoon-1.5.3/tests/test_OrdinalPartition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-20 19:20:04.000000 teaspoon-1.5.3/tests/test_PointSummariesPHN.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-20 19:20:04.000000 teaspoon-1.5.3/tests/test_SLSP.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-20 19:20:04.000000 teaspoon-1.5.3/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-20 19:20:04.000000 teaspoon-1.5.3/tests/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-20 19:20:04.000000 teaspoon-1.5.3/tests/test_featureFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-20 19:20:04.000000 teaspoon-1.5.3/tests/test_magnitude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-20 19:20:04.000000 teaspoon-1.5.3/tests/test_parameterSelection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-05-20 19:20:04.000000 teaspoon-1.5.3/tests/test_signalProcessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-20 19:20:04.000000 teaspoon-1.5.3/tests/test_texture_analysis.py
```

### Comparing `teaspoon-1.5.2/LICENSE.txt` & `teaspoon-1.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/PKG-INFO` & `teaspoon-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teaspoon
-Version: 1.5.2
+Version: 1.5.3
 Summary: A Topological Signal Processing Package
 Author-email: Elizabeth Munch <muncheli@msu.edu>
 Project-URL: repository, https://github.com/TeaspoonTDA/teaspoon
 Project-URL: homepage, https://github.com/TeaspoonTDA/teaspoon
 Project-URL: documentation, https://teaspoontda.github.io/teaspoon/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `teaspoon-1.5.2/README.md` & `teaspoon-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/pyproject.toml` & `teaspoon-1.5.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build]
 
 [project]
 name = "teaspoon"
-version = "1.5.2"
+version = "1.5.3"
 authors = [
   { name="Elizabeth Munch", email="muncheli@msu.edu" },
 ]
 description = "A Topological Signal Processing Package"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/ML/Base.py` & `teaspoon-1.5.3/teaspoon/teaspoon/ML/Base.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/ML/PD_Classification.py` & `teaspoon-1.5.3/teaspoon/teaspoon/ML/PD_Classification.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/ML/datasets/mnist.pickle` & `teaspoon-1.5.3/teaspoon/teaspoon/ML/datasets/mnist.pickle`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/ML/datasets/mpeg7.pickle` & `teaspoon-1.5.3/teaspoon/teaspoon/ML/datasets/mpeg7.pickle`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/ML/datasets/shrec14.pickle` & `teaspoon-1.5.3/teaspoon/teaspoon/ML/datasets/shrec14.pickle`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/ML/feature_functions.py` & `teaspoon-1.5.3/teaspoon/teaspoon/ML/feature_functions.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/ML/load_datasets.py` & `teaspoon-1.5.3/teaspoon/teaspoon/ML/load_datasets.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/DynSysLib.py` & `teaspoon-1.5.3/teaspoon/teaspoon/MakeData/DynSysLib/DynSysLib.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/UserGuide.py` & `teaspoon-1.5.3/teaspoon/teaspoon/MakeData/DynSysLib/UserGuide.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/autonomous_dissipative_flows.py` & `teaspoon-1.5.3/teaspoon/teaspoon/MakeData/DynSysLib/autonomous_dissipative_flows.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/conservative_flows.py` & `teaspoon-1.5.3/teaspoon/teaspoon/MakeData/DynSysLib/conservative_flows.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/delayed_flows.py` & `teaspoon-1.5.3/teaspoon/teaspoon/MakeData/DynSysLib/delayed_flows.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/driven_dissipative_flows.py` & `teaspoon-1.5.3/teaspoon/teaspoon/MakeData/DynSysLib/driven_dissipative_flows.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/maps.py` & `teaspoon-1.5.3/teaspoon/teaspoon/MakeData/DynSysLib/maps.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/medical_data.py` & `teaspoon-1.5.3/teaspoon/teaspoon/MakeData/DynSysLib/medical_data.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/noise_models.py` & `teaspoon-1.5.3/teaspoon/teaspoon/MakeData/DynSysLib/noise_models.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/MakeData/DynSysLib/periodic_functions.py` & `teaspoon-1.5.3/teaspoon/teaspoon/MakeData/DynSysLib/periodic_functions.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/MakeData/PointCloud.py` & `teaspoon-1.5.3/teaspoon/teaspoon/MakeData/PointCloud.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/SP/adaptivePart.py` & `teaspoon-1.5.3/teaspoon/teaspoon/SP/adaptivePart.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/SP/information/entropy.py` & `teaspoon-1.5.3/teaspoon/teaspoon/SP/information/entropy.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/SP/network.py` & `teaspoon-1.5.3/teaspoon/teaspoon/SP/network.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/SP/network_tools.py` & `teaspoon-1.5.3/teaspoon/teaspoon/SP/network_tools.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/SP/texture_analysis.py` & `teaspoon-1.5.3/teaspoon/teaspoon/SP/texture_analysis.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/SP/tsa_tools.py` & `teaspoon-1.5.3/teaspoon/teaspoon/SP/tsa_tools.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/TDA/Distance.py` & `teaspoon-1.5.3/teaspoon/teaspoon/TDA/Distance.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/TDA/Draw.py` & `teaspoon-1.5.3/teaspoon/teaspoon/TDA/Draw.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/TDA/Magnitude.py` & `teaspoon-1.5.3/teaspoon/teaspoon/TDA/Magnitude.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/TDA/PHN.py` & `teaspoon-1.5.3/teaspoon/teaspoon/TDA/PHN.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/TDA/Persistence.py` & `teaspoon-1.5.3/teaspoon/teaspoon/TDA/Persistence.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/TDA/SLSP.py` & `teaspoon-1.5.3/teaspoon/teaspoon/TDA/SLSP.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/TDA/SLSP_tools.py` & `teaspoon-1.5.3/teaspoon/teaspoon/TDA/SLSP_tools.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/FNN_n.py` & `teaspoon-1.5.3/teaspoon/teaspoon/parameter_selection/FNN_n.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/MI_delay.py` & `teaspoon-1.5.3/teaspoon/teaspoon/parameter_selection/MI_delay.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/MsPE.py` & `teaspoon-1.5.3/teaspoon/teaspoon/parameter_selection/MsPE.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/PAMI_delay.py` & `teaspoon-1.5.3/teaspoon/teaspoon/parameter_selection/PAMI_delay.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/autocorrelation.py` & `teaspoon-1.5.3/teaspoon/teaspoon/parameter_selection/autocorrelation.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon/parameter_selection/delay_LMS.py` & `teaspoon-1.5.3/teaspoon/teaspoon/parameter_selection/delay_LMS.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon.egg-info/PKG-INFO` & `teaspoon-1.5.3/teaspoon/teaspoon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teaspoon
-Version: 1.5.2
+Version: 1.5.3
 Summary: A Topological Signal Processing Package
 Author-email: Elizabeth Munch <muncheli@msu.edu>
 Project-URL: repository, https://github.com/TeaspoonTDA/teaspoon
 Project-URL: homepage, https://github.com/TeaspoonTDA/teaspoon
 Project-URL: documentation, https://teaspoontda.github.io/teaspoon/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `teaspoon-1.5.2/teaspoon/teaspoon.egg-info/SOURCES.txt` & `teaspoon-1.5.3/teaspoon/teaspoon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/tests/test_MakeData.py` & `teaspoon-1.5.3/tests/test_MakeData.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/tests/test_OrdinalPartition.py` & `teaspoon-1.5.3/tests/test_OrdinalPartition.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/tests/test_PointSummariesPHN.py` & `teaspoon-1.5.3/tests/test_PointSummariesPHN.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/tests/test_SLSP.py` & `teaspoon-1.5.3/tests/test_SLSP.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/tests/test_basics.py` & `teaspoon-1.5.3/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/tests/test_classification.py` & `teaspoon-1.5.3/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/tests/test_featureFunctions.py` & `teaspoon-1.5.3/tests/test_featureFunctions.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/tests/test_magnitude.py` & `teaspoon-1.5.3/tests/test_magnitude.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/tests/test_parameterSelection.py` & `teaspoon-1.5.3/tests/test_parameterSelection.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/tests/test_signalProcessing.py` & `teaspoon-1.5.3/tests/test_signalProcessing.py`

 * *Files identical despite different names*

### Comparing `teaspoon-1.5.2/tests/test_texture_analysis.py` & `teaspoon-1.5.3/tests/test_texture_analysis.py`

 * *Files identical despite different names*

