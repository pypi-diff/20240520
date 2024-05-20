# Comparing `tmp/he6_cres_spec_sims-0.1.5.tar.gz` & `tmp/he6_cres_spec_sims-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/he6_cres_spec_sims-0.1.5.tar", last modified: Fri Aug 26 20:50:16 2022, max compression
+gzip compressed data, was "C:\Users\RJ\OneDrive - North Carolina State University\Research\CRES\he6-cres-spec-sims\dist\.tmp-gwasvqtx\he6_cres_spec_sims-0", last modified: Mon May 20 16:15:34 2024, max compression
```

## Comparing `he6_cres_spec_sims-0.1.5.tar` & `he6_cres_spec_sims-0.2.0.tar`

### file list

```diff
@@ -1,53 +1,80 @@
-drwxr-xr-x   0 drew      (1000) drew      (1000)        0 2022-08-26 20:50:16.000000 he6_cres_spec_sims-0.1.5/
--rw-r--r--   0 drew      (1000) drew      (1000)       60 2022-08-04 14:42:11.000000 he6_cres_spec_sims-0.1.5/MANIFEST.in
--rw-r--r--   0 drew      (1000) drew      (1000)      361 2022-08-26 20:50:16.000000 he6_cres_spec_sims-0.1.5/PKG-INFO
--rw-r--r--   0 drew      (1000) drew      (1000)       37 2022-08-04 14:42:11.000000 he6_cres_spec_sims-0.1.5/README.md
-drwxr-xr-x   0 drew      (1000) drew      (1000)        0 2022-08-26 20:50:16.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/
--rw-r--r--   0 drew      (1000) drew      (1000)      170 2022-08-26 20:49:04.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/__init__.py
-drwxr-xr-x   0 drew      (1000) drew      (1000)        0 2022-08-26 20:50:16.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/daq/
--rw-r--r--   0 drew      (1000) drew      (1000)        0 2021-10-15 20:05:56.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/daq/__init__.py
-drwxr-xr-x   0 drew      (1000) drew      (1000)        0 2022-08-26 20:50:16.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/daq/example_spec/
--rw-r--r--   0 drew      (1000) drew      (1000)    32896 2021-10-21 18:47:37.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/daq/example_spec/example_spec_file.spec
--rwxr-xr-x   0 drew      (1000) drew      (1000)     3999 2022-08-04 16:48:11.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/daq/frequency_domain_packet.py
-drwxr-xr-x   0 drew      (1000) drew      (1000)        0 2022-08-26 20:50:16.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/daq/gain_noise_measurements/
--rw-r--r--   0 drew      (1000) drew      (1000)   819200 2021-10-07 23:16:35.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/daq/gain_noise_measurements/gain.csv
--rw-r--r--   0 drew      (1000) drew      (1000)   819200 2021-10-07 23:16:35.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/daq/gain_noise_measurements/noise.csv
--rw-r--r--   0 drew      (1000) drew      (1000)     9089 2022-08-04 14:42:11.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/experiment.py
--rw-r--r--   0 drew      (1000) drew      (1000)     5326 2022-08-04 14:42:11.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/simulation.py
--rw-r--r--   0 drew      (1000) drew      (1000)    37758 2022-08-10 00:54:04.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/simulation_blocks.py
-drwxr-xr-x   0 drew      (1000) drew      (1000)        0 2022-08-26 20:50:16.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/
--rw-r--r--   0 drew      (1000) drew      (1000)        0 2021-09-20 16:42:21.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/__init__.py
-drwxr-xr-x   0 drew      (1000) drew      (1000)        0 2022-08-26 20:50:16.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/beta_source/
--rw-r--r--   0 drew      (1000) drew      (1000)        0 2022-08-04 14:42:11.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/beta_source/__init__.py
--rw-r--r--   0 drew      (1000) drew      (1000)     2483 2022-08-04 14:42:11.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/beta_source/beta_source.py
--rw-r--r--   0 drew      (1000) drew      (1000)     5500 2022-08-04 14:42:11.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/beta_source/beta_spectrum.py
-drwxr-xr-x   0 drew      (1000) drew      (1000)        0 2022-08-26 20:50:16.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/creating_trap_geometries/
--rw-r--r--   0 drew      (1000) drew      (1000)        0 2022-08-04 14:42:11.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/creating_trap_geometries/__init__.py
-drwxr-xr-x   0 drew      (1000) drew      (1000)        0 2022-08-26 20:50:16.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/creating_trap_geometries/coil_classes/
--rw-r--r--   0 drew      (1000) drew      (1000)        0 2022-08-04 14:42:11.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/creating_trap_geometries/coil_classes/__init__.py
--rw-r--r--   0 drew      (1000) drew      (1000)     8939 2022-08-04 14:42:11.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/creating_trap_geometries/coil_classes/coil_form.py
--rw-r--r--   0 drew      (1000) drew      (1000)     8361 2022-08-04 14:42:11.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/creating_trap_geometries/coil_classes/field_profile.py
--rw-r--r--   0 drew      (1000) drew      (1000)     2989 2022-08-04 14:42:11.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/creating_trap_geometries/coil_classes/trap_profile.py
--rw-r--r--   0 drew      (1000) drew      (1000)     6790 2022-08-04 14:42:11.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/creating_trap_geometries/load_default_field_profiles.py
--rw-r--r--   0 drew      (1000) drew      (1000)     1919 2022-08-04 14:42:11.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/creating_trap_geometries/load_field_profile.py
--rw-r--r--   0 drew      (1000) drew      (1000)     1919 2022-08-04 14:42:11.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/load_field_profile.py
-drwxr-xr-x   0 drew      (1000) drew      (1000)        0 2022-08-26 20:50:16.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/spec_calc/
--rw-r--r--   0 drew      (1000) drew      (1000)        0 2021-09-20 16:42:21.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/spec_calc/__init__.py
--rw-r--r--   0 drew      (1000) drew      (1000)     4796 2021-10-15 20:05:56.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/spec_calc/power_calc.py
--rw-r--r--   0 drew      (1000) drew      (1000)    20252 2022-08-04 14:42:11.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/spec_calc/spec_calc.py
--rw-r--r--   0 drew      (1000) drew      (1000)     2711 2022-08-04 14:42:11.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/trap_field_profile.py
-drwxr-xr-x   0 drew      (1000) drew      (1000)        0 2022-08-26 20:50:16.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/trap_field_profile_pkl/
--rw-r--r--   0 drew      (1000) drew      (1000)   104985 2022-08-04 14:42:11.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/trap_field_profile_pkl/2021_trap_profile_mainfield_0T_trap_1A.csv
--rw-r--r--   0 drew      (1000) drew      (1000)      114 2022-08-04 14:42:11.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/trap_field_profile_pkl/__init__.py
-drwxr-xr-x   0 drew      (1000) drew      (1000)        0 2022-08-26 20:50:16.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims.egg-info/
--rw-r--r--   0 drew      (1000) drew      (1000)      361 2022-08-26 20:50:16.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims.egg-info/PKG-INFO
--rw-r--r--   0 drew      (1000) drew      (1000)     1894 2022-08-26 20:50:16.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims.egg-info/SOURCES.txt
--rw-r--r--   0 drew      (1000) drew      (1000)        1 2022-08-26 20:50:16.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims.egg-info/dependency_links.txt
--rw-r--r--   0 drew      (1000) drew      (1000)       77 2022-08-26 20:50:16.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims.egg-info/requires.txt
--rw-r--r--   0 drew      (1000) drew      (1000)       24 2022-08-26 20:50:16.000000 he6_cres_spec_sims-0.1.5/he6_cres_spec_sims.egg-info/top_level.txt
--rw-r--r--   0 drew      (1000) drew      (1000)       38 2022-08-26 20:50:16.000000 he6_cres_spec_sims-0.1.5/setup.cfg
--rw-r--r--   0 drew      (1000) drew      (1000)      673 2022-08-26 20:49:06.000000 he6_cres_spec_sims-0.1.5/setup.py
-drwxr-xr-x   0 drew      (1000) drew      (1000)        0 2022-08-26 20:50:16.000000 he6_cres_spec_sims-0.1.5/test/
--rw-r--r--   0 drew      (1000) drew      (1000)        0 2021-09-20 16:42:21.000000 he6_cres_spec_sims-0.1.5/test/__init__.py
--rw-r--r--   0 drew      (1000) drew      (1000)     1620 2021-09-20 16:42:21.000000 he6_cres_spec_sims-0.1.5/test/conftest.py
--rw-r--r--   0 drew      (1000) drew      (1000)     4005 2021-10-15 20:05:56.000000 he6_cres_spec_sims-0.1.5/test/test_simulation_blocks.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:15:34.000000 he6_cres_spec_sims-0.2.0/
+-rw-rw-rw-   0        0        0     1528 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      416 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    17308 2024-05-20 16:15:34.000000 he6_cres_spec_sims-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    16575 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 16:15:34.000000 he6_cres_spec_sims-0.2.0/config_files/
+-rw-rw-rw-   0        0        0     1074 2023-08-15 16:54:35.000000 he6_cres_spec_sims-0.2.0/config_files/local_base_config_example.yaml
+-rw-rw-rw-   0        0        0      504 2023-08-15 16:54:35.000000 he6_cres_spec_sims-0.2.0/config_files/local_exp_config_example.json
+-rw-rw-rw-   0        0        0     1074 2023-08-15 16:54:35.000000 he6_cres_spec_sims-0.2.0/config_files/rocks_base_config_example.yaml
+-rw-rw-rw-   0        0        0      528 2023-08-15 16:54:35.000000 he6_cres_spec_sims-0.2.0/config_files/rocks_exp_config_example.json
+-rw-rw-rw-   0        0        0      341 2024-05-20 16:06:49.000000 he6_cres_spec_sims-0.2.0/config_files/spec_example.json
+-rw-rw-rw-   0        0        0     1688 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/config_files/spec_example.yaml
+drwxrwxrwx   0        0        0        0 2024-05-20 16:15:34.000000 he6_cres_spec_sims-0.2.0/demo/
+-rw-rw-rw-   0        0        0    32210 2023-08-15 16:54:35.000000 he6_cres_spec_sims-0.2.0/demo/local_sim_experiment_demo.ipynb
+drwxrwxrwx   0        0        0        0 2024-05-20 16:15:34.000000 he6_cres_spec_sims-0.2.0/demo/readme_imgs/
+-rw-rw-rw-   0        0        0    22234 2023-08-15 16:54:35.000000 he6_cres_spec_sims-0.2.0/demo/readme_imgs/he6-cres_logo.png
+-rw-rw-rw-   0        0        0    40824 2023-08-15 16:54:35.000000 he6_cres_spec_sims-0.2.0/demo/readme_imgs/make_plot.png
+-rw-rw-rw-   0        0        0   120648 2023-08-15 16:54:35.000000 he6_cres_spec_sims-0.2.0/demo/readme_imgs/make_plot_1.png
+-rw-rw-rw-   0        0        0    31927 2023-08-15 16:54:35.000000 he6_cres_spec_sims-0.2.0/demo/readme_imgs/plot_stuff.png
+-rw-rw-rw-   0        0        0    29614 2023-08-15 16:54:35.000000 he6_cres_spec_sims-0.2.0/demo/readme_imgs/plot_stuff_1.png
+-rw-rw-rw-   0        0        0    34867 2023-08-15 16:54:35.000000 he6_cres_spec_sims-0.2.0/demo/rocks_sim_experiment_demo.ipynb
+-rw-rw-rw-   0        0        0     1178 2024-05-20 16:15:18.000000 he6_cres_spec_sims-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1070 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/run_local_experiment.py
+-rw-rw-rw-   0        0        0       42 2024-05-20 16:15:34.000000 he6_cres_spec_sims-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 16:15:34.000000 he6_cres_spec_sims-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-20 16:15:34.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/
+-rw-rw-rw-   0        0        0       25 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/__init__.py
+-rw-rw-rw-   0        0        0      581 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/constants.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:15:34.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/daq/
+-rw-rw-rw-   0        0        0        0 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/daq/__init__.py
+-rw-rw-rw-   0        0        0     4142 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/daq/frequency_domain_packet.py
+-rw-rw-rw-   0        0        0    10963 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/experiment.py
+-rw-rw-rw-   0        0        0     1432 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/run_simulation.py
+-rw-rw-rw-   0        0        0     5060 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/simulation.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:15:34.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/simulation_blocks/
+-rw-rw-rw-   0        0        0    17905 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/simulation_blocks/DAQ.py
+-rw-rw-rw-   0        0        0     1341 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/simulation_blocks/__init__.py
+-rw-rw-rw-   0        0        0     2981 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/simulation_blocks/bandBuilder.py
+-rw-rw-rw-   0        0        0     4590 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/simulation_blocks/config.py
+-rw-rw-rw-   0        0        0      899 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/simulation_blocks/dmTrackBuilder.py
+-rw-rw-rw-   0        0        0     7766 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/simulation_blocks/eventBuilder.py
+-rw-rw-rw-   0        0        0     1942 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/simulation_blocks/physics.py
+-rw-rw-rw-   0        0        0     8971 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/simulation_blocks/segmentBuilder.py
+-rw-rw-rw-   0        0        0     4442 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/simulation_blocks/trackBuilder.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:15:34.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/
+-rw-rw-rw-   0        0        0        0 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:15:34.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/beta_source/
+-rw-rw-rw-   0        0        0        0 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/beta_source/__init__.py
+-rw-rw-rw-   0        0        0     2610 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/beta_source/beta_source.py
+-rw-rw-rw-   0        0        0     5032 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/beta_source/beta_spectrum.py
+-rw-rw-rw-   0        0        0     7021 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/beta_source/beta_spectrum_alej_OLD.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:15:34.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/beta_source/pickled_spectra/
+-rw-rw-rw-   0        0        0   516585 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/beta_source/pickled_spectra/He6.json
+-rw-rw-rw-   0        0        0   516085 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/beta_source/pickled_spectra/Ne19.json
+drwxrwxrwx   0        0        0        0 2024-05-20 16:15:34.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/creating_trap_geometries/
+-rw-rw-rw-   0        0        0        0 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/creating_trap_geometries/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:15:34.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/creating_trap_geometries/coil_classes/
+-rw-rw-rw-   0        0        0        0 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/creating_trap_geometries/coil_classes/__init__.py
+-rw-rw-rw-   0        0        0     9188 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/creating_trap_geometries/coil_classes/coil_form.py
+-rw-rw-rw-   0        0        0     8637 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/creating_trap_geometries/coil_classes/field_profile.py
+-rw-rw-rw-   0        0        0     3083 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/creating_trap_geometries/coil_classes/trap_profile.py
+-rw-rw-rw-   0        0        0     6962 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/creating_trap_geometries/load_default_field_profiles.py
+-rw-rw-rw-   0        0        0     1980 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/creating_trap_geometries/load_field_profile.py
+-rw-rw-rw-   0        0        0     1980 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/load_field_profile.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:15:34.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/spec_calc/
+-rw-rw-rw-   0        0        0        0 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/spec_calc/__init__.py
+-rw-rw-rw-   0        0        0     1391 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/spec_calc/power_calc.py
+-rw-rw-rw-   0        0        0    23842 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/spec_calc/spec_calc.py
+-rw-rw-rw-   0        0        0     2794 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/trap_field_profile.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:15:34.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/trap_field_profile_pkl/
+-rw-rw-rw-   0        0        0   105260 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/trap_field_profile_pkl/2021_trap_profile_mainfield_0T_trap_1A.csv
+-rw-rw-rw-   0        0        0      122 2024-05-20 16:08:35.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/trap_field_profile_pkl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:15:34.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims.egg-info/
+-rw-rw-rw-   0        0        0    17308 2024-05-20 16:15:34.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3057 2024-05-20 16:15:34.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 16:15:34.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      202 2024-05-20 16:15:34.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-20 16:15:34.000000 he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 16:15:34.000000 he6_cres_spec_sims-0.2.0/test/
+-rw-rw-rw-   0        0        0     4134 2023-08-15 16:54:35.000000 he6_cres_spec_sims-0.2.0/test/test_simulation_blocks.py
```

### Comparing `he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/daq/frequency_domain_packet.py` & `he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/daq/frequency_domain_packet.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-#!/usr/bin/env python3
-
-from struct import unpack
-from numpy import (
-    array,
-    int8,
-    uint64,
-    uint32,
-    uint8,
-    zeros,
-    )
-
-class FDpacket:
-    """
-    Encapsulate packet of frequency domain data.
-    Header length and structure are based on R2DAQ (aka ArtooDaq)
-    """
-
-    BYTES_IN_PAYLOAD = 4096
-    BYTES_IN_HEADER = 32
-    BYTES_IN_PACKET = BYTES_IN_PAYLOAD + BYTES_IN_HEADER
-
-#    @property
-#    def bytes_in_payload(self):
-#        return self.bytes_in_payload
-#
-#    @property
-#    def bytes_in_header(self):
-#        return self.bytes_in_header
-
-    @property
-    def unix_time(self):
-        return self._unix_time
-
-    @property
-    def pkt_in_batch(self):
-        return self._pkt_in_batch
-
-    @property
-    def digital_id(self):
-        return self._digital_id
-
-    @property
-    def if_id(self):
-        return self._if_id
-
-    @property
-    def user_data_1(self):
-        return self._user_data_1
-
-    @property
-    def user_data_0(self):
-        return self._user_data_0
-
-    @property
-    def reserved_0(self):
-        return self._reserved_0
-
-    @property
-    def reserved_1(self):
-        return self._reserved_1
-
-    @property
-    def freq_not_time(self):
-        return self._freq_not_time
-
-    @property
-    def data(self):
-        return self._data
-
-    def __init__(self,ut=0,pktnum=0,did=0,ifid=0,ud0=0,ud1=0,res0=0,
-    res1=0,fnt=False,data=None):
-        """
-        Initialize Packet with the given attributes
-        """
-        # assign attributes
-        self._unix_time = ut
-        self._pkt_in_batch = pktnum
-        self._digital_id = did
-        self._if_id = ifid
-        self._user_data_0 = ud0
-        self._user_data_1 = ud1
-        self._reserved_0 = res0
-        self._reserved_1 = res1
-        self._freq_not_time = fnt
-        self._data = data
-
-    def interpret_data(self):
-        """
-        Returns
-        -------
-        x : ndarray
-            real-valued array represented by the data.
-        """
-        x = array(self.data, dtype = uint8)
-        return x
-
-    @classmethod
-    def from_byte_string(cls,bytestr, BYTES_IN_PAYLOAD = 4096 ):
-        """
-        Parse header and data from the given byte string,
-        return an object of type Packet
-        """
-        cls.BYTES_IN_PAYLOAD = BYTES_IN_PAYLOAD
-        cls.BYTES_IN_PACKET = cls.BYTES_IN_PAYLOAD + cls.BYTES_IN_HEADER
-        
-        # check correct size packet
-        len_bytes = len(bytestr)
-        if not len_bytes == cls.BYTES_IN_PACKET:
-            raise ValueError(
-            "Packet length is {0} bytes, should have {1} bytes".format(
-            len_bytes,cls.BYTES_IN_PACKET))
-
-        # unpack header
-        hdr = unpack(">{0}Q".format(cls.BYTES_IN_HEADER//8),
-        bytestr[:cls.BYTES_IN_HEADER])
-
-        ut = uint32(hdr[0] & 0xFFFFFFFF)
-        pktnum = uint32((hdr[0]>>uint32(32)) & 0xFFFFF)
-        #print "Packet number = {0}".format(pktnum)
-        did = uint8(hdr[0]>>uint32(52) & 0x3F)
-        ifid = uint8(hdr[0]>>uint32(58) & 0x3F)
-        ud1 = uint32(hdr[1] & 0xFFFFFFFF)
-        ud0 = uint32((hdr[1]>>uint32(32)) & 0xFFFFFFFF)
-        res0 = uint64(hdr[2])
-        res1 = uint64(hdr[3]&0x7FFFFFFFFFFFFFFF)
-        fnt = not (hdr[3]&0x8000000000000000 == 0)
-        # print("printing header word 4: hdr[3]", hex(uint64(hdr[3])))
-        # pre-allocate data array long enough to hold 8192-byte payload as
-        #8-bit integer numbers
-        data = zeros(cls.BYTES_IN_PAYLOAD,dtype=uint8)
-
-        # use a holder array of 64-bit data because struct.unpack requires
-        #the payload to be unpacked in 64-bit words
-        data_64bit = array(unpack(">{0}Q".format(cls.BYTES_IN_PAYLOAD//8),
-        bytestr[cls.BYTES_IN_HEADER:]),dtype=uint64)
-
-        #fill data array word by word from data_64bit
-        for i in range(len(data_64bit)):
-            for j in range(8):
-                data[i*8+j] = uint8((data_64bit[i]>>uint64(8*j))&uint64(0xFF))
-
-        return FDpacket(ut,pktnum,did,ifid,ud0,ud1,res0,res1,fnt,data)
+#!/usr/bin/env python3
+
+from struct import unpack
+from numpy import (
+    array,
+    int8,
+    uint64,
+    uint32,
+    uint8,
+    zeros,
+    )
+
+class FDpacket:
+    """
+    Encapsulate packet of frequency domain data.
+    Header length and structure are based on R2DAQ (aka ArtooDaq)
+    """
+
+    BYTES_IN_PAYLOAD = 4096
+    BYTES_IN_HEADER = 32
+    BYTES_IN_PACKET = BYTES_IN_PAYLOAD + BYTES_IN_HEADER
+
+#    @property
+#    def bytes_in_payload(self):
+#        return self.bytes_in_payload
+#
+#    @property
+#    def bytes_in_header(self):
+#        return self.bytes_in_header
+
+    @property
+    def unix_time(self):
+        return self._unix_time
+
+    @property
+    def pkt_in_batch(self):
+        return self._pkt_in_batch
+
+    @property
+    def digital_id(self):
+        return self._digital_id
+
+    @property
+    def if_id(self):
+        return self._if_id
+
+    @property
+    def user_data_1(self):
+        return self._user_data_1
+
+    @property
+    def user_data_0(self):
+        return self._user_data_0
+
+    @property
+    def reserved_0(self):
+        return self._reserved_0
+
+    @property
+    def reserved_1(self):
+        return self._reserved_1
+
+    @property
+    def freq_not_time(self):
+        return self._freq_not_time
+
+    @property
+    def data(self):
+        return self._data
+
+    def __init__(self,ut=0,pktnum=0,did=0,ifid=0,ud0=0,ud1=0,res0=0,
+    res1=0,fnt=False,data=None):
+        """
+        Initialize Packet with the given attributes
+        """
+        # assign attributes
+        self._unix_time = ut
+        self._pkt_in_batch = pktnum
+        self._digital_id = did
+        self._if_id = ifid
+        self._user_data_0 = ud0
+        self._user_data_1 = ud1
+        self._reserved_0 = res0
+        self._reserved_1 = res1
+        self._freq_not_time = fnt
+        self._data = data
+
+    def interpret_data(self):
+        """
+        Returns
+        -------
+        x : ndarray
+            real-valued array represented by the data.
+        """
+        x = array(self.data, dtype = uint8)
+        return x
+
+    @classmethod
+    def from_byte_string(cls,bytestr, BYTES_IN_PAYLOAD = 4096 ):
+        """
+        Parse header and data from the given byte string,
+        return an object of type Packet
+        """
+        cls.BYTES_IN_PAYLOAD = BYTES_IN_PAYLOAD
+        cls.BYTES_IN_PACKET = cls.BYTES_IN_PAYLOAD + cls.BYTES_IN_HEADER
+        
+        # check correct size packet
+        len_bytes = len(bytestr)
+        if not len_bytes == cls.BYTES_IN_PACKET:
+            raise ValueError(
+            "Packet length is {0} bytes, should have {1} bytes".format(
+            len_bytes,cls.BYTES_IN_PACKET))
+
+        # unpack header
+        hdr = unpack(">{0}Q".format(cls.BYTES_IN_HEADER//8),
+        bytestr[:cls.BYTES_IN_HEADER])
+
+        ut = uint32(hdr[0] & 0xFFFFFFFF)
+        pktnum = uint32((hdr[0]>>uint32(32)) & 0xFFFFF)
+        #print "Packet number = {0}".format(pktnum)
+        did = uint8(hdr[0]>>uint32(52) & 0x3F)
+        ifid = uint8(hdr[0]>>uint32(58) & 0x3F)
+        ud1 = uint32(hdr[1] & 0xFFFFFFFF)
+        ud0 = uint32((hdr[1]>>uint32(32)) & 0xFFFFFFFF)
+        res0 = uint64(hdr[2])
+        res1 = uint64(hdr[3]&0x7FFFFFFFFFFFFFFF)
+        fnt = not (hdr[3]&0x8000000000000000 == 0)
+        # print("printing header word 4: hdr[3]", hex(uint64(hdr[3])))
+        # pre-allocate data array long enough to hold 8192-byte payload as
+        #8-bit integer numbers
+        data = zeros(cls.BYTES_IN_PAYLOAD,dtype=uint8)
+
+        # use a holder array of 64-bit data because struct.unpack requires
+        #the payload to be unpacked in 64-bit words
+        data_64bit = array(unpack(">{0}Q".format(cls.BYTES_IN_PAYLOAD//8),
+        bytestr[cls.BYTES_IN_HEADER:]),dtype=uint64)
+
+        #fill data array word by word from data_64bit
+        for i in range(len(data_64bit)):
+            for j in range(8):
+                data[i*8+j] = uint8((data_64bit[i]>>uint64(8*j))&uint64(0xFF))
+
+        return FDpacket(ut,pktnum,did,ifid,ud0,ud1,res0,res1,fnt,data)
```

### Comparing `he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/experiment.py` & `he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/experiment.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,247 +1,301 @@
-from dataclasses import dataclass
-from natsort import natsorted
-import numpy as np
-import pandas as pd
-import pathlib
-from shutil import copyfile
-from shutil import rmtree
-import typing
-from typing import List
-import yaml
-
-from . import simulation as sim
-from .simulation_blocks import Config
-# from .spec_tools import beta_source as source
-import he6_cres_spec_sims.spec_tools.beta_source.beta_source as source
-import he6_cres_spec_sims.spec_tools.spec_calc.spec_calc as sc
-
-# Utility function:
-def get_experiment_dir(experiment_params: dict) -> pathlib.Path:
-
-    base_config_path = pathlib.Path(experiment_params["base_config_path"])
-    experiment_name = experiment_params["experiment_name"]
-    parent_dir = base_config_path.parents[0]
-    experiment_dir = parent_dir / experiment_name
-
-    return experiment_dir
-
-
-# Utility function:
-def get_config_paths(experiment_params: dict) -> List[pathlib.Path]:
-
-    experiment_dir = get_experiment_dir(experiment_params)
-
-    suffix = "T.yaml"
-    config_paths = [
-        x
-        for x in experiment_dir.glob("**/*{}".format(suffix))
-        if (x.is_file() and ("ipynb" not in str(x)))
-    ]
-
-    if len(config_paths) == 0:
-        raise ValueError(
-            "No config files found in experiment_dir: {}. \n\
-            Have you run the experiment?\
-            (run: exp = exp.Experiment(experiment_params))".format(
-                experiment_dir
-            )
-        )
-
-    # The natsort ensures that you get a good ordering in terms of consecutive integers
-    # within the config file name.
-    config_paths = natsorted(config_paths, key=str)
-
-    return config_paths
-
-
-class Experiment:
-    def __init__(self, experiment_params: dict) -> None:
-
-        self.experiment_params = experiment_params
-
-        self.run_experiment(self.experiment_params)
-
-    def run_experiment(self, experiment_params: dict) -> None:
-
-        # Make all the config files specified by the experiment dictionary.
-        self.create_configs_for_experiment(experiment_params)
-
-        # Make the experiment config file.
-        self.create_experiment_config_file(experiment_params)
-
-        # Collect all the config path names.
-        self.config_paths = get_config_paths(experiment_params)
-
-        # Run all of those simulations.
-        self.run_sims(self.config_paths)
-
-        return None
-
-    def create_configs_for_experiment(self, experiment_params: dict) -> None:
-
-        base_config_path = pathlib.Path(experiment_params["base_config_path"])
-        experiment_dir = get_experiment_dir(experiment_params)
-
-        # Make the experiments_dir if it doesn't exist. May want to delete contents here?
-        if not experiment_dir.is_dir():
-            experiment_dir.mkdir()
-            print("Created directory: {} ".format(experiment_dir))
-
-        else:
-            print("Directory already exists: {} ".format(experiment_dir))
-            print(
-                "CAREFUL: Continuing will delete the contents of the above directory.\n"
-            )
-            input("Press Enter to continue...")
-            rmtree(experiment_dir)
-            experiment_dir.mkdir()
-
-        # Grab data from experiment_params dict.
-        isotope = experiment_params["isotope"]
-        events_to_simulate = experiment_params["events_to_simulate"]
-        betas_to_simulate = experiment_params["betas_to_simulate"]
-        seeds = experiment_params["rand_seeds"]
-        fields = experiment_params["fields_T"]
-        traps = experiment_params["traps_A"]
-
-        for i, (seed, field, trap) in enumerate(zip(seeds, fields, traps)):
-
-            # Round the field because there are often small rounding errors.
-            field = np.around(field, 6)
-            config_path = experiment_dir / "{}_field_{}T{}".format(
-                i, field, base_config_path.suffix
-            )
-
-            copyfile(base_config_path, config_path)
-
-            # Open the config file and grab the contents.
-            with open(config_path, "r") as f:
-                config_dict = yaml.load(f, Loader=yaml.FullLoader)
-
-            # Make the appropriate altercations to the config_dict
-            config_dict["Settings"]["rand_seed"] = int(seed)
-            config_dict["Physics"]["events_to_simulate"] = int(events_to_simulate)
-            config_dict["Physics"]["betas_to_simulate"] = int(betas_to_simulate)
-            config_dict["Physics"]["energy_spectrum"]["beta_source"] = str(isotope)
-            config_dict["EventBuilder"]["main_field"] = float(field)
-            config_dict["EventBuilder"]["trap_current"] = float(trap)
-
-            with open(config_path, "w") as f:
-                yaml.dump(config_dict, f, default_flow_style=False, sort_keys=False)
-
-        return None
-
-    def create_experiment_config_file(self, experiment_params: dict) -> None:
-
-        experiment_dir = get_experiment_dir(experiment_params)
-
-        # Define path for experiment config.
-        experiment_config = experiment_dir / (
-            experiment_params["experiment_name"] + "_exp.yaml"
-        )
-
-        with open(experiment_config, "w") as f:
-            yaml.dump(experiment_params, f, default_flow_style=False, sort_keys=False)
-
-        return None
-
-    def run_sims(self, config_paths: List[pathlib.Path]) -> None:
-
-        for i, config_path in enumerate(config_paths):
-            print("+++++++++++++++++++++++++++++++++++++++++++++++++\n\n")
-            print("Running simulation {} / {}\n\n".format(i, len(config_paths)))
-            print("+++++++++++++++++++++++++++++++++++++++++++++++++")
-            simulation = sim.Simulation(config_path)
-            simulation.run_full()
-
-        return None
-
-
-@dataclass
-class ExpResults:
-
-    experiment_params: dict
-    base_config: object
-    config_paths: List[pathlib.Path]
-    sampled_gammas: pd.DataFrame
-    experiment_results: pd.DataFrame
-
-    @classmethod
-    def load(cls, experiment_params: dict = None, experiment_config_path: str = None, include_sampled_gammas = False):
-
-        # Can either provide the experiment_params dict if you have it or a path to the
-        # exp_config.yaml file.
-
-        if experiment_params is None:
-            experiment_config_path = pathlib.Path(experiment_config_path)
-
-            # Open the config file and grab the contents.
-            with open(experiment_config_path, "r") as f:
-                experiment_params = yaml.load(f, Loader=yaml.FullLoader)
-
-        if (experiment_params is None) and (experiment_config_path is None):
-
-            raise ValueError(
-                "Need to provide either experiment_params or exp_config_path."
-            )
-
-        exp_results_dict = {
-            "experiment_params": experiment_params,
-            "base_config": Config(experiment_params["base_config_path"]),
-            "config_paths": None,
-            "sampled_gammas": None,
-            "experiment_results": None,
-        }
-
-        # Then collect all the config path names.
-        config_paths = get_config_paths(experiment_params)
-        exp_results_dict["config_paths"] = config_paths
-
-        tracks_list = []
-        sampled_gammas = []
-        fields = []
-
-        # Figure out how many betas were sampled; depends on the mode (beta_num or event_num).
-        # Note that if this is -1 then you get the entire array (event_mode).
-        beta_num = experiment_params["betas_to_simulate"]
-
-        for i, config_path in enumerate(config_paths):
-
-            print("+++++++++++++++++++++++++++++++++++++++++++++++++\n\n")
-            print("Loading simulation {} / {}\n\n".format(i, len(config_paths)))
-            print("+++++++++++++++++++++++++++++++++++++++++++++++++")
-
-            # Get the simulation parameters from the config.
-            config = Config(config_path)
-            field = config.eventbuilder.main_field
-            trap_current = config.eventbuilder.trap_current
-            print("\nSet field: {}, Trap current: {}\n".format(field, trap_current))
-            results = sim.Results.load(config_path)
-            tracks = results.dmtracks
-            tracks["simulation_num"] = i
-            tracks["field"] = field
-            tracks["trap_current"] = trap_current
-            tracks_list.append(tracks)
-
-            if include_sampled_gammas: 
-                # Get the betas that were sampled during the simulation.
-                beta_source_ne19 = source.BetaSource(config)
-                sampled_energies = beta_source_ne19.energy_array[: int(beta_num)]
-                sampled_gammas.append(sc.gamma(sampled_energies))
-                fields.append(field)
-
-        if include_sampled_gammas:
-            exp_results_dict["sampled_gammas"] = pd.DataFrame.from_dict(
-                dict(zip(fields, sampled_gammas))
-            )
-        exp_results_dict["experiment_results"] = pd.concat(tracks_list)
-
-        exp_results = cls(
-            exp_results_dict["experiment_params"],
-            exp_results_dict["base_config"],
-            exp_results_dict["config_paths"],
-            exp_results_dict["sampled_gammas"],
-            exp_results_dict["experiment_results"],
-        )
-
-        return exp_results
+from dataclasses import dataclass
+from natsort import natsorted
+import numpy as np
+import pandas as pd
+import pathlib
+from shutil import copyfile
+from shutil import rmtree
+import typing
+from typing import List
+import yaml
+from pathlib import Path
+import json
+
+import he6_cres_spec_sims.simulation as sim
+from he6_cres_spec_sims.simulation_blocks import Config
+
+# from .spec_tools import beta_source as source
+import he6_cres_spec_sims.spec_tools.beta_source.beta_source as source
+import he6_cres_spec_sims.spec_tools.spec_calc.spec_calc as sc
+
+#this function runs everything, previously in run_local_experiment.py script, 
+# putting it here allows you to more easily run experiments interactively
+def run_local_experiment(dict_path):
+
+    print(f"\n\n\n Beginning local simulation.\n\n\n")
+
+    experiment_name = Path(dict_path).stem
+
+    sim_experiment_params = json.load(open(dict_path))
+    sim_experiment_params["experiment_name"] = experiment_name
+
+    for key, val in sim_experiment_params.items():
+        print("{}: {}".format(key, val))
+
+    sim_experiment = Experiment(sim_experiment_params)
+
+    print(f"\n\n\n Done running simulation. {sim_experiment_params}")
+
+    return None
+
+# Utility function:
+def get_experiment_dir(experiment_params: dict) -> pathlib.Path:
+
+    base_config_path = pathlib.Path(experiment_params["base_config_path"])
+    experiment_name = experiment_params["experiment_name"]
+    parent_dir = base_config_path.parents[0]
+    experiment_dir = parent_dir / experiment_name
+
+    return experiment_dir
+
+
+# Utility function:
+def get_config_paths(experiment_params: dict) -> List[pathlib.Path]:
+
+    experiment_dir = get_experiment_dir(experiment_params)
+
+    suffix = "T.yaml"
+    config_paths = [
+        x
+        for x in experiment_dir.glob("**/*{}".format(suffix))
+        if (x.is_file() and ("ipynb" not in str(x)))
+    ]
+
+    if len(config_paths) == 0:
+        raise ValueError(
+            "No config files found in experiment_dir: {}. \n\
+            Have you run the experiment?\
+            (run: exp = exp.Experiment(experiment_params))".format(
+                experiment_dir
+            )
+        )
+
+    # The natsort ensures that you get a good ordering in terms of consecutive integers
+    # within the config file name.
+    config_paths = natsorted(config_paths, key=str)
+
+    return config_paths
+
+
+class Experiment:
+    def __init__(self, experiment_params: dict) -> None:
+
+        self.experiment_params = experiment_params
+
+        self.run_experiment(self.experiment_params)
+
+    def run_experiment(self, experiment_params: dict) -> None:
+
+        # Make all the config files specified by the experiment dictionary.
+        self.create_configs_for_experiment(experiment_params)
+
+        # Make the experiment config file.
+        self.create_experiment_config_file(experiment_params)
+
+        # Collect all the config path names.
+        self.config_paths = get_config_paths(experiment_params)
+
+        # Run all of those simulations.
+        self.run_sims(self.config_paths)
+
+        return None
+
+    def create_configs_for_experiment(self, experiment_params: dict) -> None:
+
+        base_config_path = pathlib.Path(experiment_params["base_config_path"])
+        experiment_dir = get_experiment_dir(experiment_params)
+
+        # Make the experiments_dir if it doesn't exist. May want to delete contents here?
+        if not experiment_dir.is_dir():
+            experiment_dir.mkdir()
+            print("Created directory: {} ".format(experiment_dir))
+
+        else:
+            print("Directory already exists: {} ".format(experiment_dir))
+            print(
+                "CAREFUL: Continuing will delete the contents of the above directory.\n"
+            )
+            input("Press Enter to continue...")
+            rmtree(experiment_dir)
+            experiment_dir.mkdir()
+
+        # Grab data from experiment_params dict.
+        isotope = experiment_params["isotope"]
+        events_to_simulate = experiment_params["events_to_simulate"]
+        betas_to_simulate = experiment_params["betas_to_simulate"]
+        seeds = experiment_params["rand_seeds"]
+        fields = experiment_params["fields_T"]
+        traps = experiment_params["traps_A"]
+
+        for i, (seed, field, trap) in enumerate(zip(seeds, fields, traps)):
+
+            # Round the field because there are often small rounding errors.
+            field = np.around(field, 6)
+            config_path = experiment_dir / "{}_field_{}T{}".format(
+                i, field, base_config_path.suffix
+            )
+
+            copyfile(base_config_path, config_path)
+
+            # Open the config file and grab the contents.
+            with open(config_path, "r") as f:
+                config_dict = yaml.load(f, Loader=yaml.FullLoader)
+
+            # Make the appropriate altercations to the config_dict
+            # For seed = None, rng pulls from hardware entropy
+            if seed is not None:
+                config_dict["Settings"]["rand_seed"] = int(seed)
+            else:
+                config_dict["Settings"]["rand_seed"] = None
+            config_dict["Physics"]["events_to_simulate"] = int(events_to_simulate)
+            config_dict["Physics"]["betas_to_simulate"] = int(betas_to_simulate)
+            config_dict["Physics"]["energy_spectrum"]["beta_source"] = str(isotope)
+            config_dict["EventBuilder"]["main_field"] = float(field)
+            config_dict["EventBuilder"]["trap_current"] = float(trap)
+
+            with open(config_path, "w") as f:
+                yaml.dump(config_dict, f, default_flow_style=False, sort_keys=False)
+
+        return None
+
+    def create_experiment_config_file(self, experiment_params: dict) -> None:
+
+        experiment_dir = get_experiment_dir(experiment_params)
+
+        # Define path for experiment config.
+        experiment_config = experiment_dir / (
+            experiment_params["experiment_name"] + "_exp.yaml"
+        )
+
+        with open(experiment_config, "w") as f:
+            yaml.dump(experiment_params, f, default_flow_style=False, sort_keys=False)
+
+        return None
+
+    def run_sims(self, config_paths: List[pathlib.Path]) -> None:
+
+        for i, config_path in enumerate(config_paths):
+            print("+++++++++++++++++++++++++++++++++++++++++++++++++\n\n")
+            print("Running simulation {} / {}\n\n".format(i, len(config_paths)))
+            print("+++++++++++++++++++++++++++++++++++++++++++++++++")
+            simulation = sim.Simulation(config_path)
+            simulation.run_full()
+
+        return None
+
+
+@dataclass
+class ExpResults:
+
+    experiment_params: dict
+    # base_config: object
+    config_paths: List[pathlib.Path]
+    sampled_gammas: pd.DataFrame
+    tracks: pd.DataFrame
+
+    @classmethod
+    def load(cls, experiment_config_path: str = None, include_sampled_gammas=False):
+
+        # Path to the exp_config.yaml file.
+        experiment_config_path = pathlib.Path(experiment_config_path)
+
+        # Open the config file and grab the contents.
+        with open(experiment_config_path, "r") as f:
+            experiment_params = yaml.load(f, Loader=yaml.FullLoader)
+
+        if experiment_config_path is None:
+
+            raise ValueError("Need to provide experiment_config_path.")
+
+        exp_results_dict = {
+            "experiment_params": experiment_params,
+            # "base_config": Config(experiment_params["base_config_path"]),
+            "config_paths": None,
+            "sampled_gammas": None,
+            "tracks": None,
+        }
+
+        # Then collect all the config path names.
+        # Note that the path in the experiment_params may be misleading if the
+        # experiment was run on rocks.
+        config_paths = get_config_paths_results(experiment_config_path)
+        exp_results_dict["config_paths"] = config_paths
+
+        tracks_list = []
+        sampled_gammas = []
+        fields = []
+
+        # Figure out how many betas were sampled; depends on the mode (beta_num or event_num).
+        # Note that if this is -1 then you get the entire array (event_mode).
+        beta_num = experiment_params["betas_to_simulate"]
+
+        for i, config_path in enumerate(config_paths):
+
+            print("+++++++++++++++++++++++++++++++++++++++++++++++++\n\n")
+            print("Loading simulation {} / {}\n\n".format(i, len(config_paths)))
+            print("+++++++++++++++++++++++++++++++++++++++++++++++++")
+
+            # Get the simulation parameters from the config.
+            config = Config(config_path)
+            field = config.eventbuilder.main_field
+            trap_current = config.eventbuilder.trap_current
+            print("\nSet field: {}, Trap current: {}\n".format(field, trap_current))
+            results = sim.Results.load(config_path)
+            tracks = results.dmtracks
+            tracks["simulation_num"] = i
+            tracks["field"] = field
+            tracks["trap_current"] = trap_current
+            tracks_list.append(tracks)
+
+            if include_sampled_gammas:
+                # Get the betas that were sampled during the simulation.
+                beta_source_ne19 = source.BetaSource(config)
+                sampled_energies = beta_source_ne19.energy_array[: int(beta_num)]
+                sampled_gammas.append(sc.gamma(sampled_energies))
+                fields.append(field)
+
+        if include_sampled_gammas:
+            exp_results_dict["sampled_gammas"] = pd.DataFrame.from_dict(
+                dict(zip(fields, sampled_gammas))
+            )
+        exp_results_dict["tracks"] = pd.concat(tracks_list)
+
+        exp_results = cls(
+            exp_results_dict["experiment_params"],
+            # exp_results_dict["base_config"],
+            exp_results_dict["config_paths"],
+            exp_results_dict["sampled_gammas"],
+            exp_results_dict["tracks"],
+        )
+
+        return exp_results
+
+
+def get_config_paths_results(
+    experiment_config_path: pathlib.Path,
+) -> List[pathlib.Path]:
+
+    experiment_dir = experiment_config_path.parents[0]
+    print(experiment_dir)
+
+    suffix = "T.yaml"
+    config_paths = [
+        x
+        for x in experiment_dir.glob("**/*{}".format(suffix))
+        if (x.is_file() and ("ipynb" not in str(x)))
+    ]
+
+    if len(config_paths) == 0:
+        raise ValueError(
+            "No config files found in experiment_dir: {}. \n\
+            Have you run the experiment?\
+            (run: exp = exp.Experiment(experiment_params))".format(
+                experiment_dir
+            )
+        )
+
+    # The natsort ensures that you get a good ordering in terms of consecutive integers
+    # within the config file name.
+    config_paths = natsorted(config_paths, key=str)
+
+    return config_paths
```

### Comparing `he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/beta_source/beta_source.py` & `he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/beta_source/beta_source.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-import numpy as np
-
-# Local modules.
-from .beta_spectrum import BetaSpectrum
-from ..spec_calc import spec_calc as sc
-
-ME = 5.10998950e5  # Electron rest mass (eV).
-
-
-class BetaSource:
-    """A class used to ...
-
-    ...
-
-    Attributes
-    ----------
-
-
-    Methods
-    -------
-
-    """
-
-    def __init__(self, config):
-        """
-        DOCUMENT
-        """
-        self.config = config
-        self.source = self.config.physics.energy_spectrum
-        self.energy_array_len = 10**6
-        self.energy_array = None
-
-        # Include all the sources here.
-        self.isotopes = {
-            "Ne19": {"Wmax": 5.337377690802349, "Z": 9, "A": 19},
-            "He6": {"Wmax": 7.864593361688904, "Z": 2, "A": 6},
-        }
-
-        if (self.source["beta_source"] == "Ne19") or (
-            self.source["beta_source"] == "He6"
-        ):
-            print("\nSource: {}\n".format(self.source["beta_source"]))
-            self.beta_spectrum = BetaSpectrum(self.isotopes[self.source["beta_source"]])
-
-            self.make_energy_samples()
-
-    def make_energy_samples(self):
-
-        if (self.source["beta_source"] == "Ne19") or (
-            self.source["beta_source"] == "He6"
-        ):
-            if type(self.energy_array) != np.ndarray:
-
-                print("Creating energy_array to pull beta energies from.")
-                # Freq acceptance cut:
-                main_field = self.config.eventbuilder.main_field
-
-                freq_acceptance_high = self.config.physics.freq_acceptance_high
-                freq_acceptance_low = self.config.physics.freq_acceptance_low
-
-                self.energy_acceptance_high = sc.freq_to_energy(
-                    freq_acceptance_high, main_field
-                )
-                self.energy_acceptance_low = sc.freq_to_energy(
-                    freq_acceptance_low, main_field
-                )
-
-                # Now energy_array has units of eV.
-                (
-                    self.energy_array,
-                    self.fraction_of_spectrum,
-                ) = self.beta_spectrum.energy_samples(
-                    self.energy_array_len,
-                    self.energy_acceptance_low,
-                    self.energy_acceptance_high,
-                    self.config.settings.rand_seed,
-                )
-
-                print("Fraction of total spectrum: {}\n ".format(self.fraction_of_spectrum))
-
-            return None
-
-        else:
-
-            raise NotImplementedError("Kr needs to be reimplimented.")
+import numpy as np
+
+# Local modules.
+from .beta_spectrum import BetaSpectrum
+import he6_cres_spec_sims.spec_tools.spec_calc.spec_calc as sc
+
+from he6_cres_spec_sims.constants import ME
+
+
+class BetaSource:
+    """A class used to ...
+
+    ...
+
+    Attributes
+    ----------
+
+
+    Methods
+    -------
+
+    """
+
+    def __init__(self, config):
+        """
+        DOCUMENT
+        """
+        self.config = config
+        self.source = self.config.physics.energy_spectrum
+        self.energy_array_len = 10**6 + 100 # Just making this bigger than the sim size.
+        self.energy_array = None
+
+        # Include all the sources here.
+        self.isotopes = {
+            "Ne19": {"Wmax": 5.337377690802349, "Z": 9, "A": 19},
+            "He6": {"Wmax": 7.864593361688904, "Z": 2, "A": 6},
+        }
+
+        if (self.source["beta_source"] == "Ne19") or (
+            self.source["beta_source"] == "He6"
+        ):
+            print("\nSource: {}\n".format(self.source["beta_source"]))
+            self.beta_spectrum = BetaSpectrum(self.source["beta_source"])
+
+            self.make_energy_samples()
+
+    def make_energy_samples(self):
+
+        if (self.source["beta_source"] == "Ne19") or (
+            self.source["beta_source"] == "He6"
+        ):
+            if type(self.energy_array) != np.ndarray:
+
+                print("Creating energy_array to pull beta energies from.")
+                # Freq acceptance cut:
+                main_field = self.config.eventbuilder.main_field
+
+                freq_acceptance_high = self.config.physics.freq_acceptance_high
+                freq_acceptance_low = self.config.physics.freq_acceptance_low
+
+                self.energy_acceptance_high = sc.freq_to_energy(
+                    freq_acceptance_high, main_field
+                )
+                self.energy_acceptance_low = sc.freq_to_energy(
+                    freq_acceptance_low, main_field
+                )
+
+                # Now energy_array has units of eV.
+                (
+                    self.energy_array,
+                    self.fraction_of_spectrum,
+                ) = self.beta_spectrum.energy_samples(
+                    self.energy_array_len,
+                    self.energy_acceptance_low,
+                    self.energy_acceptance_high,
+                    self.config.rng,
+                )
+
+                print("Fraction of total spectrum: {}\n ".format(self.fraction_of_spectrum))
+
+            return None
+
+        else:
+
+            raise NotImplementedError("Kr needs to be reimplimented.")
```

### Comparing `he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/creating_trap_geometries/coil_classes/coil_form.py` & `he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/creating_trap_geometries/coil_classes/coil_form.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,249 +1,249 @@
-import math
-import numpy as np
-from scipy.integrate import romberg
-from scipy.misc import derivative
-
-
-class Coil_form:
-    """
-    Generates object that contains geometric data of current coil. Note that num_windings is the number of windings per unit length (winding density).
-    """
-    
-    def __init__(self,inner_radius,outer_radius,left_edge,right_edge,z_center,num_windings,current_per_wire,name=None):
-    
-        if not name == None:
-            self._name = str(name)
-        else:
-            self._name = name
-            
-        self._inner_radius = inner_radius
-        self._outer_radius = outer_radius
-        self._left_edge = left_edge
-        self._right_edge = right_edge
-        self._z_center = z_center
-        self._num_windings = num_windings
-        self._current_per_wire = current_per_wire
-        
-        while self._inner_radius >= self._outer_radius:
-        
-            print("ERROR: inner radius greater than outer radius")
-            self._inner_radius = input("Reset inner radius: ")
-        
-    def get_coil_dimensions(self):
-        """
-        Returns coil dimensions.
-        """
-        
-        return self._inner_radius,self._outer_radius,self._left_edge,self._right_edge
-        
-    def get_coil_properties(self):
-        """
-        Returns coil center z-coordinate, winding length density, and current per wire.
-        """
-        
-        return self._z_center,self._num_windings, self._current_per_wire
-                
-    def set_coil_dimensions(self,inner_radius,outer_radius,left_edge,right_edge):
-        """
-        Set coil dimensions.
-        """
-        self._inner_radius = inner_radius
-        self._outer_radius = outer_radius
-        self._left_edge = left_edge
-        self._right_edge = right_edge
-        
-    def set_coil_properties(self,z_center,num_windings,current_per_wire):
-        """
-        Set coil center z-coordinate, winding length density, and current per wire.
-        """
-        self._z_center = z_center
-        self._num_windings = num_windings
-        self._current_per_wire = current_per_wire
-        
-    def field_values(self,position,sheets=20,field_coordinates="Cartesian",calculate_Br=True):
-        """
-        Calculates the magnetic field T in coordinates field_coordinates at position = (radius,phi,z) in cylindrical coordinates
-        with phi in radians. Can choose field_coordinates 'Cartesian' or 'cylindrical'.
-        """
-        
-        mu0 = 4 * math.pi * 1e-7
-        current_density = self._num_windings * self._current_per_wire
-        
-        #break down position vector
-        radius = position[0]
-        phi = position[1]
-        zpos = position[2]
-        
-        #shift coordinate system for integral calculation
-        zpos = zpos - self._z_center
-        
-        if radius == 0:
-            
-            def logterm(z,zedge,Ro,Ri):
-                    numerator = Ro + math.sqrt(Ro**2 + (z-zedge)**2)
-                    denominator = Ri + math.sqrt(Ri**2 + (z-zedge)**2)
-                    value = (z-zedge)*math.log(numerator / denominator)
-       
-                    return value
-       
-            Br = 0
-            Bz = (mu0 / 2)* (current_density /(self._outer_radius - self._inner_radius))*(logterm(zpos,self._left_edge,self._outer_radius,self._inner_radius)-logterm(zpos,self._right_edge,self._outer_radius,self._inner_radius))
-            
-        else:
-            
-            def Q_func(z, zedge, r, R, theta):
-                return math.sqrt((z-zedge)**2 + r**2 + R**2 - 2*r*R*math.cos(theta))
-                
-                
-            def Br_integrand(z,z1,z2,r,R,theta):
-            
-                try:
-                    Q_one = Q_func(z,z1,r,R,theta)
-                    Q_two =  Q_func(z,z2,r,R,theta)
-                    
-                    first_term_numerator = R*math.cos(theta) * (1 + (z-z2)/Q_two)
-                    first_term_denominator = (z-z2) + Q_two
-                    first_term = first_term_numerator/first_term_denominator
-                    
-                    second_term_numerator = -R*math.cos(theta) * (1 + (z-z1)/Q_one)
-                    second_term_denominator = (z-z1) + Q_one
-                    second_term = second_term_numerator/second_term_denominator
-                    
-                    integrand = first_term + second_term
-                    
-                except:
-                    print("WARNING: Unhandled value for Br integrand at radius = {}, theta = {}, z = {}".format(r,theta,z))
-                    print("Returning 0 for integrand; may affect accuracy")
-                    
-                    
-                    integrand = 0
-                
-                return integrand
-                
-            def Bz_integrand(z,z1,z2,r,R,theta):
-            
-                try:
-    
-                    Q_one = Q_func(z,z1,r,R,theta)
-                    Q_two =  Q_func(z,z2,r,R,theta)
-                    
-                    first_term_numerator = R*math.cos(theta) * (2 * r - 2 * R * math.cos(theta))
-                    first_term_denominator = 2 * Q_one * (z-z1 + Q_one)
-                    first_term = first_term_numerator / first_term_denominator
-    
-    
-                    second_term_numerator = -R*math.cos(theta) * (2 * r - 2 * R * math.cos(theta))
-                    second_term_denominator = 2 * Q_two * (z-z2 + Q_two)
-                    second_term = second_term_numerator / second_term_denominator
-    
-                    third_term = R * math.cos(theta) / r * math.log((z-z1+Q_one)/(z-z2+Q_two))
-    
-                    integrand = first_term +  second_term + third_term
-                    
-                except:
-                    print("WARNING: Unhandled value for Bz integrand at radius = {}, theta = {}, z = {}".format(r,theta,z))
-                    print("Returning 0 for integrand; may affect accuracy")
-                    integrand = 0
-    
-                return integrand
-            
-            current_per_sheet = current_density / sheets
-            Br = 0
-            Bz = 0
-            curr_sheets = 0
-            for k in range(sheets):
-            
-                def Br_field_function(theta):
-                    return Br_integrand(zpos,self._left_edge,self._right_edge,radius,self._inner_radius + k * (self._outer_radius - self._inner_radius)/(sheets-1),theta)
-    
-                def Bz_field_function(theta):
-                    return Bz_integrand(zpos,self._left_edge,self._right_edge,radius,self._inner_radius + k * (self._outer_radius - self._inner_radius)/(sheets-1),theta)
-                    
-                if calculate_Br == True:
-                    Br = Br + (mu0 / (2*math.pi)) * current_per_sheet * romberg(Br_field_function,0,math.pi,divmax=20)
-                else:
-                    Br = 0
-                
-                Bz = Bz + (mu0 / (2*math.pi)) * current_per_sheet * romberg(Bz_field_function,0,math.pi,divmax=20)
-              
-        if field_coordinates == "cylindrical":
-            return (Br, 0 , Bz)
-        
-        elif field_coordinates == "Cartesian":
-              
-            Bx = Br * math.cos(phi)
-            By = Br * math.sin(phi)
-    
-            return (Bx,By,Bz)
-            
-        else:
-            print("ERROR: {} not a valid coordinate system".format(return_coordinates))
-            
-    def field_strength(self,radius,zpos):
-        """
-        Calculates Bz magnetic field strength in T at radius, zpos.
-        """
-    
-        position = (radius,0,zpos)
-        total_field = self.field_values(position,calculate_Br=False)[2]
-     
-        return total_field
-        
-    def field_derivative(self,radius,zpos,deriv_order=1,dx=1e-6):
-        """
-        Calculates dBz / dz derivative on z-axis.
-        """
-
-        def f(x):
-            return self.field_strength(radius,x)
-
-        return derivative(f,zpos,dx=dx,n=deriv_order,order=(deriv_order*2 + 1))
-   
-    @property
-    def inner_radius(self):
-        return self._inner_radius
-    
-    @property
-    def outer_radius(self):
-        return self._outer_radius
-           
-    @property
-    def left_edge(self):
-        return self._left_edge
-           
-    @property
-    def right_edge(self):
-        return self._right_edge
-           
-    @property
-    def z_center(self):
-        return self._z_center
-        
-    @z_center.setter
-    def z_center(self,value):
-        self._z_center = value
-        
-    @property
-    def num_windings(self):
-        return self._num_windings
-        
-    @num_windings.setter
-    def num_windings(self,value):
-        self._num_windings = value
-        
-    @property
-    def current_per_wire(self):
-        return self._current_per_wire
-        
-    @current_per_wire.setter
-    def current_per_wire(self,value):
-        self._current_per_wire = value
-        
-    @property
-    def name(self):
-        return self._name
-        
-    @name.setter
-    def name(self,value):
-        self._name = str(value)
-
+import math
+import numpy as np
+from scipy.integrate import romberg
+from scipy.misc import derivative
+
+
+class Coil_form:
+    """
+    Generates object that contains geometric data of current coil. Note that num_windings is the number of windings per unit length (winding density).
+    """
+    
+    def __init__(self,inner_radius,outer_radius,left_edge,right_edge,z_center,num_windings,current_per_wire,name=None):
+    
+        if not name == None:
+            self._name = str(name)
+        else:
+            self._name = name
+            
+        self._inner_radius = inner_radius
+        self._outer_radius = outer_radius
+        self._left_edge = left_edge
+        self._right_edge = right_edge
+        self._z_center = z_center
+        self._num_windings = num_windings
+        self._current_per_wire = current_per_wire
+        
+        while self._inner_radius >= self._outer_radius:
+        
+            print("ERROR: inner radius greater than outer radius")
+            self._inner_radius = input("Reset inner radius: ")
+        
+    def get_coil_dimensions(self):
+        """
+        Returns coil dimensions.
+        """
+        
+        return self._inner_radius,self._outer_radius,self._left_edge,self._right_edge
+        
+    def get_coil_properties(self):
+        """
+        Returns coil center z-coordinate, winding length density, and current per wire.
+        """
+        
+        return self._z_center,self._num_windings, self._current_per_wire
+                
+    def set_coil_dimensions(self,inner_radius,outer_radius,left_edge,right_edge):
+        """
+        Set coil dimensions.
+        """
+        self._inner_radius = inner_radius
+        self._outer_radius = outer_radius
+        self._left_edge = left_edge
+        self._right_edge = right_edge
+        
+    def set_coil_properties(self,z_center,num_windings,current_per_wire):
+        """
+        Set coil center z-coordinate, winding length density, and current per wire.
+        """
+        self._z_center = z_center
+        self._num_windings = num_windings
+        self._current_per_wire = current_per_wire
+        
+    def field_values(self,position,sheets=20,field_coordinates="Cartesian",calculate_Br=True):
+        """
+        Calculates the magnetic field T in coordinates field_coordinates at position = (radius,phi,z) in cylindrical coordinates
+        with phi in radians. Can choose field_coordinates 'Cartesian' or 'cylindrical'.
+        """
+        
+        mu0 = 4 * math.pi * 1e-7
+        current_density = self._num_windings * self._current_per_wire
+        
+        #break down position vector
+        radius = position[0]
+        phi = position[1]
+        zpos = position[2]
+        
+        #shift coordinate system for integral calculation
+        zpos = zpos - self._z_center
+        
+        if radius == 0:
+            
+            def logterm(z,zedge,Ro,Ri):
+                    numerator = Ro + math.sqrt(Ro**2 + (z-zedge)**2)
+                    denominator = Ri + math.sqrt(Ri**2 + (z-zedge)**2)
+                    value = (z-zedge)*math.log(numerator / denominator)
+       
+                    return value
+       
+            Br = 0
+            Bz = (mu0 / 2)* (current_density /(self._outer_radius - self._inner_radius))*(logterm(zpos,self._left_edge,self._outer_radius,self._inner_radius)-logterm(zpos,self._right_edge,self._outer_radius,self._inner_radius))
+            
+        else:
+            
+            def Q_func(z, zedge, r, R, theta):
+                return math.sqrt((z-zedge)**2 + r**2 + R**2 - 2*r*R*math.cos(theta))
+                
+                
+            def Br_integrand(z,z1,z2,r,R,theta):
+            
+                try:
+                    Q_one = Q_func(z,z1,r,R,theta)
+                    Q_two =  Q_func(z,z2,r,R,theta)
+                    
+                    first_term_numerator = R*math.cos(theta) * (1 + (z-z2)/Q_two)
+                    first_term_denominator = (z-z2) + Q_two
+                    first_term = first_term_numerator/first_term_denominator
+                    
+                    second_term_numerator = -R*math.cos(theta) * (1 + (z-z1)/Q_one)
+                    second_term_denominator = (z-z1) + Q_one
+                    second_term = second_term_numerator/second_term_denominator
+                    
+                    integrand = first_term + second_term
+                    
+                except:
+                    print("WARNING: Unhandled value for Br integrand at radius = {}, theta = {}, z = {}".format(r,theta,z))
+                    print("Returning 0 for integrand; may affect accuracy")
+                    
+                    
+                    integrand = 0
+                
+                return integrand
+                
+            def Bz_integrand(z,z1,z2,r,R,theta):
+            
+                try:
+    
+                    Q_one = Q_func(z,z1,r,R,theta)
+                    Q_two =  Q_func(z,z2,r,R,theta)
+                    
+                    first_term_numerator = R*math.cos(theta) * (2 * r - 2 * R * math.cos(theta))
+                    first_term_denominator = 2 * Q_one * (z-z1 + Q_one)
+                    first_term = first_term_numerator / first_term_denominator
+    
+    
+                    second_term_numerator = -R*math.cos(theta) * (2 * r - 2 * R * math.cos(theta))
+                    second_term_denominator = 2 * Q_two * (z-z2 + Q_two)
+                    second_term = second_term_numerator / second_term_denominator
+    
+                    third_term = R * math.cos(theta) / r * math.log((z-z1+Q_one)/(z-z2+Q_two))
+    
+                    integrand = first_term +  second_term + third_term
+                    
+                except:
+                    print("WARNING: Unhandled value for Bz integrand at radius = {}, theta = {}, z = {}".format(r,theta,z))
+                    print("Returning 0 for integrand; may affect accuracy")
+                    integrand = 0
+    
+                return integrand
+            
+            current_per_sheet = current_density / sheets
+            Br = 0
+            Bz = 0
+            curr_sheets = 0
+            for k in range(sheets):
+            
+                def Br_field_function(theta):
+                    return Br_integrand(zpos,self._left_edge,self._right_edge,radius,self._inner_radius + k * (self._outer_radius - self._inner_radius)/(sheets-1),theta)
+    
+                def Bz_field_function(theta):
+                    return Bz_integrand(zpos,self._left_edge,self._right_edge,radius,self._inner_radius + k * (self._outer_radius - self._inner_radius)/(sheets-1),theta)
+                    
+                if calculate_Br == True:
+                    Br = Br + (mu0 / (2*math.pi)) * current_per_sheet * romberg(Br_field_function,0,math.pi,divmax=20)
+                else:
+                    Br = 0
+                
+                Bz = Bz + (mu0 / (2*math.pi)) * current_per_sheet * romberg(Bz_field_function,0,math.pi,divmax=20)
+              
+        if field_coordinates == "cylindrical":
+            return (Br, 0 , Bz)
+        
+        elif field_coordinates == "Cartesian":
+              
+            Bx = Br * math.cos(phi)
+            By = Br * math.sin(phi)
+    
+            return (Bx,By,Bz)
+            
+        else:
+            print("ERROR: {} not a valid coordinate system".format(return_coordinates))
+            
+    def field_strength(self,radius,zpos):
+        """
+        Calculates Bz magnetic field strength in T at radius, zpos.
+        """
+    
+        position = (radius,0,zpos)
+        total_field = self.field_values(position,calculate_Br=False)[2]
+     
+        return total_field
+        
+    def field_derivative(self,radius,zpos,deriv_order=1,dx=1e-6):
+        """
+        Calculates dBz / dz derivative on z-axis.
+        """
+
+        def f(x):
+            return self.field_strength(radius,x)
+
+        return derivative(f,zpos,dx=dx,n=deriv_order,order=(deriv_order*2 + 1))
+   
+    @property
+    def inner_radius(self):
+        return self._inner_radius
+    
+    @property
+    def outer_radius(self):
+        return self._outer_radius
+           
+    @property
+    def left_edge(self):
+        return self._left_edge
+           
+    @property
+    def right_edge(self):
+        return self._right_edge
+           
+    @property
+    def z_center(self):
+        return self._z_center
+        
+    @z_center.setter
+    def z_center(self,value):
+        self._z_center = value
+        
+    @property
+    def num_windings(self):
+        return self._num_windings
+        
+    @num_windings.setter
+    def num_windings(self,value):
+        self._num_windings = value
+        
+    @property
+    def current_per_wire(self):
+        return self._current_per_wire
+        
+    @current_per_wire.setter
+    def current_per_wire(self,value):
+        self._current_per_wire = value
+        
+    @property
+    def name(self):
+        return self._name
+        
+    @name.setter
+    def name(self,value):
+        self._name = str(value)
+
```

### Comparing `he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/creating_trap_geometries/coil_classes/trap_profile.py` & `he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/creating_trap_geometries/coil_classes/trap_profile.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-import math
-import numpy as np
-from scipy.misc import derivative
-from scipy.optimize import fmin
-
-from he6_cres_spec_sims.spec_tools.creating_trap_geometries.coil_classes.field_profile import Field_profile
-
-class Trap_profile(Field_profile):
-    """
-    Generates object that calculates field strength of magnetic mirror trap of given coils in list_coils. Returns None if list_coils does not represent a proper trap.
-    """
-    
-    #elements in Field_profile
-    #self._list_coils
-    #self._main_field
-    #get_coil_list(self)
-    #set_coil_list(self,list_coils)
-    #field_values(self,position,field_coordinates="Cartesian")
-    #field_grad(self,position,deriv_order=1,dx=1e-6,grad_coordinates="Cartesian")
-    #field_strength(self,position,field_coordinates="Cartesian")
-    #field_derivative(self,position,deriv_order=1,dx=1e-6)
-    #@property main_field(self), main_field(self,value)
-    
-    
-    def __init__(self,list_coils,main_field=0,trap_current=1, field_scales=True):
-    
-        
-        super().__init__(list_coils,main_field, trap_current)
-        self._field_scales = field_scales
-        
-        if not main_field > 0:
-            print("WARNING: Main field not greater than 0")
-            print("Not a valid trap...")
-            self._is_trap = False
-            return None
-            
-        elif not (self.field_derivative(0,0) == 0
-                and self.field_derivative(0,0,2) > 0):
-            print("WARNING: Given field profile does not have a local minimum at z=0")
-            print("Not a valid trap...")
-            self._is_trap = False
-            return None
-            
-        self._is_trap = True
-        self._trap_width = self.trap_width_calc()
-        
-    def trap_width_calc(self):
-        """
-        Calculates the trap width of the object trap_profile.
-        """
-    
-        field_func = self.field_strength
-        def func(z):
-            return -1 * field_func(0,z)
-        
-        maximum = fmin(func,0,xtol=1e-12)[0]
-        print("Trap width: ({},{})".format(-maximum,maximum))
-        print("Maximum Field: {}".format(-1 * func(maximum)))
-    
-        trap_width = (-maximum,maximum)
-        return trap_width
-        
-
-    @property
-    def main_field(self):
-        return self._main_field
-        
-    @main_field.setter
-    def main_field(self,value):
-        
-        if not value > 0:
-            print("ERROR: New main field must be greater than 0")
-            return
-        
-        else:
-            if self._field_scales == True:
-                for coil in self._list_coils:
-                    base_current = coil.current_per_wire / self._main_field
-                    coil.current_per_wire = base_current * value
-            self._main_field = value
-        
-    @property
-    def is_trap(self):
-        return self._is_trap
-        
-    @property
-    def field_scales(self):
-        return self._field_scales
-        
-    @property
-    def trap_width(self):
-        return self._trap_width
-        
-    
+import math
+import numpy as np
+from scipy.misc import derivative
+from scipy.optimize import fmin
+
+from he6_cres_spec_sims.spec_tools.creating_trap_geometries.coil_classes.field_profile import Field_profile
+
+class Trap_profile(Field_profile):
+    """
+    Generates object that calculates field strength of magnetic mirror trap of given coils in list_coils. Returns None if list_coils does not represent a proper trap.
+    """
+    
+    #elements in Field_profile
+    #self._list_coils
+    #self._main_field
+    #get_coil_list(self)
+    #set_coil_list(self,list_coils)
+    #field_values(self,position,field_coordinates="Cartesian")
+    #field_grad(self,position,deriv_order=1,dx=1e-6,grad_coordinates="Cartesian")
+    #field_strength(self,position,field_coordinates="Cartesian")
+    #field_derivative(self,position,deriv_order=1,dx=1e-6)
+    #@property main_field(self), main_field(self,value)
+    
+    
+    def __init__(self,list_coils,main_field=0,trap_current=1, field_scales=True):
+    
+        
+        super().__init__(list_coils,main_field, trap_current)
+        self._field_scales = field_scales
+        
+        if not main_field > 0:
+            print("WARNING: Main field not greater than 0")
+            print("Not a valid trap...")
+            self._is_trap = False
+            return None
+            
+        elif not (self.field_derivative(0,0) == 0
+                and self.field_derivative(0,0,2) > 0):
+            print("WARNING: Given field profile does not have a local minimum at z=0")
+            print("Not a valid trap...")
+            self._is_trap = False
+            return None
+            
+        self._is_trap = True
+        self._trap_width = self.trap_width_calc()
+        
+    def trap_width_calc(self):
+        """
+        Calculates the trap width of the object trap_profile.
+        """
+    
+        field_func = self.field_strength
+        def func(z):
+            return -1 * field_func(0,z)
+        
+        maximum = fmin(func,0,xtol=1e-12)[0]
+        print("Trap width: ({},{})".format(-maximum,maximum))
+        print("Maximum Field: {}".format(-1 * func(maximum)))
+    
+        trap_width = (-maximum,maximum)
+        return trap_width
+        
+
+    @property
+    def main_field(self):
+        return self._main_field
+        
+    @main_field.setter
+    def main_field(self,value):
+        
+        if not value > 0:
+            print("ERROR: New main field must be greater than 0")
+            return
+        
+        else:
+            if self._field_scales == True:
+                for coil in self._list_coils:
+                    base_current = coil.current_per_wire / self._main_field
+                    coil.current_per_wire = base_current * value
+            self._main_field = value
+        
+    @property
+    def is_trap(self):
+        return self._is_trap
+        
+    @property
+    def field_scales(self):
+        return self._field_scales
+        
+    @property
+    def trap_width(self):
+        return self._trap_width
+        
+
```

### Comparing `he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/creating_trap_geometries/load_field_profile.py` & `he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/creating_trap_geometries/load_field_profile.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-import json
-import os
-import os.path
-
-from he6_cres_spec_sims.spec_tools.creating_trap_geometries.coil_classes.coil_form import Coil_form
-from he6_cres_spec_sims.spec_tools.creating_trap_geometries.coil_classes.field_profile import Field_profile
-
-from scipy.misc import derivative
-from scipy.optimize import fminbound
-
-
-def load_field_profile(filename):
-
-    #Finding repository home directory
-    home_dir  = os.path.dirname(os.path.abspath(__file__))
-    home_dir  = os.path.dirname(home_dir)
-    
-    
-    if not filename[0] == "/":
-        data_file = home_dir + "/" + filename
-    else:
-        data_file = home_dir + filename
- 
-    #Loading JSON test file
-    with open(data_file,"r") as read_file:
-        try:
-            config_dict = json.load(read_file)
-            field_coils = config_dict["field_coils"]
-            main_field = config_dict["main_field"]
-        except:
-            print('Loaded file "{}" does not contain a valid field profile config dictionary'.format(filename))
-            return
-            
-    print("Field profile {} loaded".format(filename))
-
-    list_coils= []
-    for coil_dict in field_coils:
-        
-        inner_radius = coil_dict["inner_radius"]
-        outer_radius = coil_dict["outer_radius"]
-        left_edge = coil_dict["left_edge"]
-        right_edge = coil_dict["right_edge"]
-        z_center = coil_dict["z_center"]
-        num_windings = coil_dict["num_windings"]
-        current_per_wire = coil_dict["current_per_wire"]
-        name = coil_dict["name"]
-
-        curr_coil = Coil_form(inner_radius=inner_radius,
-        outer_radius=outer_radius,
-        left_edge=left_edge,
-        right_edge=right_edge,
-        z_center=z_center,
-        num_windings=num_windings,
-        current_per_wire=current_per_wire,
-        name=name)
-        
-        list_coils.append(curr_coil)
-
-    field_profile = Field_profile(list_coils,main_field)
-
-    return field_profile
+import json
+import os
+import os.path
+
+from he6_cres_spec_sims.spec_tools.creating_trap_geometries.coil_classes.coil_form import Coil_form
+from he6_cres_spec_sims.spec_tools.creating_trap_geometries.coil_classes.field_profile import Field_profile
+
+from scipy.misc import derivative
+from scipy.optimize import fminbound
+
+
+def load_field_profile(filename):
+
+    #Finding repository home directory
+    home_dir  = os.path.dirname(os.path.abspath(__file__))
+    home_dir  = os.path.dirname(home_dir)
+    
+    
+    if not filename[0] == "/":
+        data_file = home_dir + "/" + filename
+    else:
+        data_file = home_dir + filename
+ 
+    #Loading JSON test file
+    with open(data_file,"r") as read_file:
+        try:
+            config_dict = json.load(read_file)
+            field_coils = config_dict["field_coils"]
+            main_field = config_dict["main_field"]
+        except:
+            print('Loaded file "{}" does not contain a valid field profile config dictionary'.format(filename))
+            return
+            
+    print("Field profile {} loaded".format(filename))
+
+    list_coils= []
+    for coil_dict in field_coils:
+        
+        inner_radius = coil_dict["inner_radius"]
+        outer_radius = coil_dict["outer_radius"]
+        left_edge = coil_dict["left_edge"]
+        right_edge = coil_dict["right_edge"]
+        z_center = coil_dict["z_center"]
+        num_windings = coil_dict["num_windings"]
+        current_per_wire = coil_dict["current_per_wire"]
+        name = coil_dict["name"]
+
+        curr_coil = Coil_form(inner_radius=inner_radius,
+        outer_radius=outer_radius,
+        left_edge=left_edge,
+        right_edge=right_edge,
+        z_center=z_center,
+        num_windings=num_windings,
+        current_per_wire=current_per_wire,
+        name=name)
+        
+        list_coils.append(curr_coil)
+
+    field_profile = Field_profile(list_coils,main_field)
+
+    return field_profile
```

### Comparing `he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/load_field_profile.py` & `he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/load_field_profile.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-import json
-import os
-import os.path
-
-from he6_cres_spec_sims.spec_tools.creating_trap_geometries.coil_classes.coil_form import Coil_form
-from he6_cres_spec_sims.spec_tools.creating_trap_geometries.coil_classes.field_profile import Field_profile
-
-from scipy.misc import derivative
-from scipy.optimize import fminbound
-
-
-def load_field_profile(filename):
-
-    #Finding repository home directory
-    home_dir  = os.path.dirname(os.path.abspath(__file__))
-    home_dir  = os.path.dirname(home_dir)
-    
-    
-    if not filename[0] == "/":
-        data_file = home_dir + "/" + filename
-    else:
-        data_file = home_dir + filename
- 
-    #Loading JSON test file
-    with open(data_file,"r") as read_file:
-        try:
-            config_dict = json.load(read_file)
-            field_coils = config_dict["field_coils"]
-            main_field = config_dict["main_field"]
-        except:
-            print('Loaded file "{}" does not contain a valid field profile config dictionary'.format(filename))
-            return
-            
-    print("Field profile {} loaded".format(filename))
-
-    list_coils= []
-    for coil_dict in field_coils:
-        
-        inner_radius = coil_dict["inner_radius"]
-        outer_radius = coil_dict["outer_radius"]
-        left_edge = coil_dict["left_edge"]
-        right_edge = coil_dict["right_edge"]
-        z_center = coil_dict["z_center"]
-        num_windings = coil_dict["num_windings"]
-        current_per_wire = coil_dict["current_per_wire"]
-        name = coil_dict["name"]
-
-        curr_coil = Coil_form(inner_radius=inner_radius,
-        outer_radius=outer_radius,
-        left_edge=left_edge,
-        right_edge=right_edge,
-        z_center=z_center,
-        num_windings=num_windings,
-        current_per_wire=current_per_wire,
-        name=name)
-        
-        list_coils.append(curr_coil)
-
-    field_profile = Field_profile(list_coils,main_field)
-
-    return field_profile
+import json
+import os
+import os.path
+
+from he6_cres_spec_sims.spec_tools.creating_trap_geometries.coil_classes.coil_form import Coil_form
+from he6_cres_spec_sims.spec_tools.creating_trap_geometries.coil_classes.field_profile import Field_profile
+
+from scipy.misc import derivative
+from scipy.optimize import fminbound
+
+
+def load_field_profile(filename):
+
+    #Finding repository home directory
+    home_dir  = os.path.dirname(os.path.abspath(__file__))
+    home_dir  = os.path.dirname(home_dir)
+    
+    
+    if not filename[0] == "/":
+        data_file = home_dir + "/" + filename
+    else:
+        data_file = home_dir + filename
+ 
+    #Loading JSON test file
+    with open(data_file,"r") as read_file:
+        try:
+            config_dict = json.load(read_file)
+            field_coils = config_dict["field_coils"]
+            main_field = config_dict["main_field"]
+        except:
+            print('Loaded file "{}" does not contain a valid field profile config dictionary'.format(filename))
+            return
+            
+    print("Field profile {} loaded".format(filename))
+
+    list_coils= []
+    for coil_dict in field_coils:
+        
+        inner_radius = coil_dict["inner_radius"]
+        outer_radius = coil_dict["outer_radius"]
+        left_edge = coil_dict["left_edge"]
+        right_edge = coil_dict["right_edge"]
+        z_center = coil_dict["z_center"]
+        num_windings = coil_dict["num_windings"]
+        current_per_wire = coil_dict["current_per_wire"]
+        name = coil_dict["name"]
+
+        curr_coil = Coil_form(inner_radius=inner_radius,
+        outer_radius=outer_radius,
+        left_edge=left_edge,
+        right_edge=right_edge,
+        z_center=z_center,
+        num_windings=num_windings,
+        current_per_wire=current_per_wire,
+        name=name)
+        
+        list_coils.append(curr_coil)
+
+    field_profile = Field_profile(list_coils,main_field)
+
+    return field_profile
```

### Comparing `he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/spec_calc/spec_calc.py` & `he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/spec_calc/spec_calc.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,683 +1,723 @@
-"""spec_calc
-
-This set of calculators takes cres electron properties (such as energy, pitch angle), as 
-well as information about the trap (instance of a trap_profile object) and outputs other 
-cres electron properties such as axial frequency, z_max, B_avg.
-
----
-Units for all module functions' inputs/outputs: 
-
-Energy   : eV
-B-field  : T
-Time     : s
-Angle    : degrees
-Distance : m
-Frequency: Hz
-Power    : W
-
-
----
-"""
-# TODO: Organize the imports.
-import math
-import os
-
-import numpy as np
-
-# from numpy.random import uniform
-
-import scipy.integrate as integrate
-from scipy.fft import fft
-from scipy.optimize import fmin, fminbound
-from scipy.interpolate import interp1d
-import scipy.special as ss
-
-# Math constants.
-
-PI = math.pi
-RAD_TO_DEG = 180 / math.pi
-P11_PRIME = 1.84118  # first zero of J1 prime (bessel functions)
-
-# Physics constants.
-
-ME = 5.10998950e5  # Electron rest mass (eV).
-M = 9.1093837015e-31  # Electron rest mass (kg).
-Q = 1.602176634e-19  # Electron charge (Coulombs).
-C = 299792458  # Speed of light in vacuum, in m/s
-J_TO_EV = 6.241509074e18  # Joule-ev conversion
-EPS_0 = 8.8541878128 * 10**-12  # Vacuum Permittivity (F/m)
-
-
-# Simple special relativity functions.
-
-
-def gamma(energy):
-    gamma = (energy + ME) / ME
-    return gamma
-
-
-def momentum(energy):
-    momentum = (((energy + ME) ** 2 - ME**2) / C**2) ** 0.5 / J_TO_EV
-    return momentum
-
-
-def velocity(energy):
-    velocity = momentum(energy) / (gamma(energy) * M)
-    return velocity
-
-
-# CRES functions.
-
-
-def energy_to_freq(energy, field):
-
-    """Converts kinetic energy to cyclotron frequency."""
-
-    cycl_freq = Q * field / (2 * PI * gamma(energy) * M)
-
-    return cycl_freq
-
-
-def freq_to_energy(frequency, field):
-
-    """Calculates energy of beta particle in eV given cyclotron
-    frequency in Hz, magnetic field in Tesla, and pitch angle
-    at 90 degrees.
-    """
-
-    gamma = Q * field / (2 * PI * frequency * M)
-    if np.any(gamma < 1):
-        gamma = 1
-        max_freq = Q * field / (2 * PI * M)
-        warning = "Warning: {} higher than maximum cyclotron frequency {}".format(
-            frequency, max_freq
-        )
-        print(warning)
-    return gamma * ME - ME
-
-
-def energy_and_freq_to_field(energy, freq):
-
-    """Converts kinetic energy to cyclotron frequency."""
-
-    field = (2 * PI * gamma(energy) * M * freq) / Q
-
-    return field
-
-
-def power_from_slope(energy, slope, field):
-
-    """Converts slope, energy, field into the associated cres power."""
-
-    energy_Joules = (energy + ME) / J_TO_EV
-
-    power = slope * (2 * PI) * ((energy_Joules) ** 2) / (Q * field * C**2)
-
-    return power
-
-
-def random_beta_generator(parameter_dict, rand_seed):
-
-    """TODO(byron): Think about if the phi_initial parameter has an
-    effect.
-
-    Generates a random beta in the trap with pitch angle between
-    min_theta and max_theta , and initial position (rho,0,z) between
-    min_rho and max_rho and min_z and max_z.
-    """
-    # Initialize rng. Mult by arbitrary int because seed may be used elsewhere.
-    rng = np.random.default_rng(rand_seed * 11)
-
-    min_rho = parameter_dict["min_rho"]
-    max_rho = parameter_dict["max_rho"]
-
-    min_z = parameter_dict["min_z"]
-    max_z = parameter_dict["max_z"]
-
-    min_theta = parameter_dict["min_theta"] / RAD_TO_DEG
-    max_theta = parameter_dict["max_theta"] / RAD_TO_DEG
-
-    # TODO: Explain this in words. Had to change this 10122021 because
-    # it only worked if min_rho was zero.
-    rho_initial = min_rho + np.sqrt(rng.uniform(0, 1) * (max_rho**2 - min_rho**2))
-    phi_initial = 2 * PI * rng.uniform(0, 1) * RAD_TO_DEG
-    # phi_initial = 0
-    z_initial = rng.uniform(min_z, max_z)
-
-    u_min = (1 - np.cos(min_theta)) / 2
-    u_max = (1 - np.cos(max_theta)) / 2
-
-    sphere_theta_initial = np.arccos(1 - 2 * (rng.uniform(u_min, u_max))) * RAD_TO_DEG
-    sphere_phi_initial = 2 * PI * rng.uniform(0, 1) * RAD_TO_DEG
-
-    position = [rho_initial, phi_initial, z_initial]
-    direction = [sphere_theta_initial, sphere_phi_initial]
-
-    return position, direction
-
-
-def theta_center(zpos, rho, pitch_angle, trap_profile):
-
-    """Calculates the pitch angle an electron with current z-coordinate
-    zpos, rho, and current pitch angle pitch_angle takes at the center
-    of given trap.
-    """
-
-    if trap_profile.is_trap:
-
-        Bmin = trap_profile.field_strength(rho, 0.0)
-        Bcurr = trap_profile.field_strength(rho, zpos)
-
-        theta_center_calc = (
-            np.arcsin((np.sqrt(Bmin / Bcurr)) * np.sin(pitch_angle / RAD_TO_DEG))
-            * RAD_TO_DEG
-        )
-
-        return theta_center_calc
-
-    else:
-        print("ERROR: Given trap profile is not a valid trap")
-        return False
-
-
-def cyc_radius(energy, field, pitch_angle):
-
-    """Calculates the instantaneous cyclotron radius of a beta electron
-    given the energy, magnetic field, and current pitch angle.
-    """
-
-    vel_perp = velocity(energy) * np.sin(pitch_angle / RAD_TO_DEG)
-
-    cyc_radius = (gamma(energy) * M * vel_perp) / (Q * field)
-
-    return cyc_radius
-
-
-def max_radius(energy, center_pitch_angle, rho, trap_profile):
-
-    """Calculates the maximum cyclotron radius of a beta electron given
-    the kinetic energy, trap_profile, and center pitch angle (pitch angle
-    at center of trap).
-    """
-
-    if trap_profile.is_trap:
-
-        min_field = trap_profile.field_strength(rho, 0)
-        max_field = min_field / (np.sin(center_pitch_angle / RAD_TO_DEG)) ** 2
-
-        center_radius = cyc_radius(energy, min_field, center_pitch_angle)
-        end_radius = cyc_radius(energy, max_field, pitch_angle=90)
-
-        if np.all(center_radius >= end_radius):
-            return center_radius
-        else:
-            print(
-                "Warning: max_radius is occuring at end of trap (theta=90). \
-                Something odd may be going on."
-            )
-            return False
-
-    else:
-        print("ERROR: Given trap profile is not a valid trap")
-        return False
-
-
-def min_radius(energy, center_pitch_angle, rho, trap_profile):
-
-    """Calculates the minimum cyclotron radius of a beta electron given
-    the kinetic energy, trap_profile, and center pitch angle (pitch angle
-    at center of trap).
-    """
-
-    if trap_profile.is_trap:
-
-        min_field = trap_profile.field_strength(rho, 0)
-        max_field = min_field / (np.sin(center_pitch_angle / RAD_TO_DEG)) ** 2
-
-        center_radius = cyc_radius(energy, min_field, center_pitch_angle)
-        end_radius = cyc_radius(energy, max_field, pitch_angle=90)
-
-        if np.all(center_radius >= end_radius):
-            return end_radius
-        else:
-            print(
-                "Warning: min_radius is occuring at center of trap, something \
-                odd may be going on."
-            )
-            return False
-
-    else:
-        print("ERROR: Given trap profile is not a valid trap")
-        return False
-
-
-def min_theta(rho, zpos, trap_profile):
-
-    """Calculates the minimum pitch angle theta at which an electron at
-    zpos is trapped given trap_profile.
-    """
-
-    if trap_profile.is_trap:
-
-        # Be careful here. Technically the Bmax doesn't occur at a constant z.
-        Bmax = trap_profile.field_strength(rho, trap_profile.trap_width[1])
-        Bz = trap_profile.field_strength(rho, zpos)
-
-        theta = np.arcsin((Bz / Bmax) ** 0.5) * RAD_TO_DEG
-        return theta
-
-    else:
-        print("ERROR: Given trap profile is not a valid trap")
-        return False
-
-
-def max_zpos_not_vectorized(energy, center_pitch_angle, rho, trap_profile, debug=False):
-
-    """Calculates the maximum axial length from center of trap as a
-    function of center_pitch_angle and rho. Not vectorized. See below
-    for vectorized version.
-    """
-
-    if trap_profile.is_trap:
-
-        if center_pitch_angle < min_theta(rho, 0, trap_profile):
-            print("WARNING: Electron not trapped (zpos)")
-            return False
-
-        else:
-            # Ok, so does this mean we now have an energy dependence on zmax? Yes.
-            c_r = cyc_radius(
-                energy, trap_profile.field_strength(rho, 0), center_pitch_angle
-            )
-            rho_p = np.sqrt(rho**2 + c_r**2 / 2)
-
-            min_field = trap_profile.field_strength(rho_p, 0)
-            max_field = trap_profile.field_strength(rho_p, trap_profile.trap_width[1])
-
-            max_reached_field = min_field / pow(
-                math.sin(center_pitch_angle * math.pi / 180), 2
-            )
-
-            # initial guess based on treating magnetic well as v-shaped
-            slope = (max_field - min_field) / (trap_profile.trap_width[1])
-            initial_z = (max_reached_field - min_field) / slope
-
-            if initial_z == trap_profile.trap_width[1]:
-                return initial_z
-
-            def func(z):
-                curr_field = trap_profile.field_strength(rho_p, z)
-                return abs(curr_field - max_reached_field)
-
-            max_z = fminbound(func, 0, trap_profile.trap_width[1], xtol=1e-14)
-            curr_field = trap_profile.field_strength(rho_p, max_z)
-
-            if (curr_field > max_reached_field) and debug == True:
-                print(
-                    "Final field greater than max allowed field by: ",
-                    curr_field - max_reached_field,
-                )
-                print("Bmax reached: ", curr_field)
-
-            if debug == True:
-                print("zlength: ", max_z)
-
-            if max_z > trap_profile.trap_width[1]:
-                print("Error Rate: ", max_z - trap_profile.trap_width[1])
-
-            return max_z
-
-    else:
-        print("ERROR: Given trap profile is not a valid trap")
-        return False
-
-
-def max_zpos(energy, center_pitch_angle, rho, trap_profile, debug=False):
-
-    """Vectorized version of max_zpos_not_vectorized function."""
-
-    max_zpos_vectorized = np.vectorize(max_zpos_not_vectorized)
-
-    return max_zpos_vectorized(energy, center_pitch_angle, rho, trap_profile)
-
-
-def mod_index(avg_cycl_freq, zmax):
-
-    """Calculates modulation index from average cyclotron frequency
-    (avg_cycl_freq) and maximum axial amplitude (zmax).
-    """
-
-    # fixed experiment parameters
-    waveguide_radius = 0.578e-2
-    kc = P11_PRIME / waveguide_radius
-
-    # calculated parameters
-    omega = 2 * PI * avg_cycl_freq
-    k_wave = omega / C
-    beta = np.sqrt(k_wave**2 - kc**2)
-
-    mod_index = zmax * beta
-
-    return mod_index
-
-
-def df_dt(energy, field, power):
-
-    """Calculates cyclotron frequency rate of change of electron with
-    given kinetic energy at field in T radiating energy at rate power.
-    """
-
-    energy_Joules = (energy + ME) / J_TO_EV
-
-    slope = (Q * field * C**2) / (2 * PI) * (power) / (energy_Joules) ** 2
-
-    return slope
-
-
-def curr_pitch_angle(rho, zpos, center_pitch_angle, trap_profile):
-
-    """Calculates the current pitch angle of an electron at zpos given
-    center pitch angle and main field strength.
-    """
-
-    if trap_profile.is_trap:
-
-        min_field = trap_profile.field_strength(rho, 0)
-        max_z = max_zpos(center_pitch_angle, rho, trap_profile)
-        max_reached_field = trap_profile.field_strength(rho, max_z)
-
-        if np.any(abs(zpos) > max_z):
-            print("Electron does not reach given zpos")
-            curr_pitch = "FAIL"
-        else:
-            curr_field = trap_profile.field_strength(rho, zpos)
-            curr_pitch = np.arcsin(np.sqrt(curr_field / max_reached_field)) * RAD_TO_DEG
-
-        return curr_pitch
-
-    else:
-        print("ERROR: Given trap profile is not a valid trap")
-        return False
-
-
-def axial_freq_not_vect(energy, center_pitch_angle, rho, trap_profile):
-
-    """Caculates the axial frequency of a trapped electron."""
-
-    if trap_profile.is_trap:
-        # center_pitch_angle = np.where(center_pitch_angle == 90.0, 89.999, center_pitch_angle)
-        if center_pitch_angle == 90.0:
-            center_pitch_angle = 89.999
-
-        zmax = max_zpos(energy, center_pitch_angle, rho, trap_profile)
-
-        c_r = cyc_radius(
-            energy, trap_profile.field_strength(rho, 0), center_pitch_angle
-        )
-        rho_p = np.sqrt(rho**2 + c_r**2 / 2)
-
-        B = lambda z: trap_profile.field_strength(rho_p, z)
-        Bmax = trap_profile.field_strength(rho_p, zmax)
-
-        # Secant of theta as function of z. Use conserved mu to derive.
-        sec_theta = lambda z: (1 - B(z) / Bmax) ** (-0.5)
-        T_a = 4 / velocity(energy) * integrate.quad(sec_theta, 0, zmax)[0]
-
-        axial_frequency = 1 / T_a
-
-        return axial_frequency
-
-    else:
-        print("ERROR: Given trap profile is not a valid trap")
-        return False
-
-
-def axial_freq(energy, center_pitch_angle, rho, trap_profile):
-
-    """Vectorized version of axial_freq_not_vectorized function."""
-
-    axial_freq_vect = np.vectorize(axial_freq_not_vect)
-
-    return axial_freq_vect(energy, center_pitch_angle, rho, trap_profile)
-
-
-def avg_cycl_freq_not_vect(energy, center_pitch_angle, rho, trap_profile):
-
-    """Calculates the average cyclotron frquency of an electron given
-    kinetic energy, main field, and center pitch angle.
-    Returns 0 if electron is not trapped.
-    """
-
-    if trap_profile.is_trap:
-
-        Bmin = trap_profile.field_strength(rho, 0)
-        min_trapped_angle = min_theta(rho, 0, trap_profile)
-
-        if center_pitch_angle < min_trapped_angle:
-            print("Warning: (avg_cyc) electron not trapped.")
-            return False
-
-        if center_pitch_angle == 90.0:
-            avg_cyc_freq = energy_to_freq(energy, Bmin)
-
-        else:
-            zmax = max_zpos(energy, center_pitch_angle, rho, trap_profile)
-            B = lambda z: trap_profile.field_strength(rho, z)
-            Bmax = trap_profile.field_strength(rho, zmax)
-            integrand = lambda z: B(z) * ((1 - B(z) / Bmax) ** (-0.5))
-
-            ax_freq = axial_freq(energy, center_pitch_angle, rho, trap_profile)
-
-            # Similar to axial_freq calculation.
-            avg_cyc_freq = (
-                4
-                * Q
-                * ax_freq
-                / (2 * PI * momentum(energy))
-                * integrate.quad(integrand, 0, zmax, epsrel=10**-2)[0]
-            )
-
-        return avg_cyc_freq
-
-    else:
-        print("ERROR: Given trap profile is not a valid trap")
-        return False
-
-
-def avg_cycl_freq(energy, center_pitch_angle, rho, trap_profile):
-
-    field = b_avg(energy, center_pitch_angle, rho, trap_profile)
-
-    return energy_to_freq(energy, field)
-
-
-def b_avg_not_vect(energy, center_pitch_angle, rho, trap_profile):
-
-    """Calculates the average magnetic field experienced by an electron
-    of a given kinetic energy, main field, and center pitch angle.
-    Returns 0 if electron is not trapped.
-    """
-
-    c_r = cyc_radius(energy, trap_profile.field_strength(rho, 0), center_pitch_angle)
-
-    rho_p = np.sqrt(rho**2 + c_r**2 / 2)
-    rho_pp = np.sqrt(rho**2 + c_r**2)
-
-    if trap_profile.is_trap:
-
-        Bmin = trap_profile.field_strength(rho_p, 0)
-        min_trapped_angle = min_theta(rho_p, 0, trap_profile)
-
-        if center_pitch_angle < min_trapped_angle:
-            print("Warning: (avg_cyc) electron not trapped.")
-            return False
-
-        if center_pitch_angle == 90.0:
-            avg_cyc_freq = energy_to_freq(energy, Bmin)
-
-        else:
-
-            zmax = max_zpos(energy, center_pitch_angle, rho, trap_profile)
-            B1 = lambda z: trap_profile.field_strength(rho_pp, z)
-            B = lambda z: trap_profile.field_strength(rho_p, z)
-            Bmax = trap_profile.field_strength(rho_p, zmax)
-            integrand = lambda z: B1(z) * ((1 - B(z) / Bmax) ** (-0.5))
-
-            ax_freq = axial_freq(energy, center_pitch_angle, rho, trap_profile)
-
-            # Similar to axial_freq calculation.
-            b_avg = (
-                4
-                * ax_freq
-                / (velocity(energy))
-                * integrate.quad(integrand, 0, zmax, epsrel=10**-3)[0]
-            )
-
-        return b_avg
-
-    else:
-        print("ERROR: Given trap profile is not a valid trap")
-        return False
-
-
-def b_avg(energy, center_pitch_angle, rho, trap_profile):
-
-    """Vectorized version of b_avg_not_vectorized function."""
-
-    b_avg_vect = np.vectorize(b_avg_not_vect)
-
-    return b_avg_vect(energy, center_pitch_angle, rho, trap_profile)
-
-
-def t_not_vect(energy, zpos, center_pitch_angle, rho, trap_profile):
-
-    """DEBUG(byron): This is returning negative times.
-    Caculates the time for electron to travel from z = 0 to zpos.
-    """
-
-    if trap_profile.is_trap:
-
-        if center_pitch_angle == 90.0:
-            center_pitch_angle = 89.999
-
-        zmax = max_zpos(energy, center_pitch_angle, rho, trap_profile)
-        B = lambda z: trap_profile.field_strength(rho, z)
-        Bmax = trap_profile.field_strength(rho, zmax)
-
-        # Secant of theta as function of z. Use conserved mu to derive.
-        sec_theta = lambda z: (1 - B(z) / Bmax) ** (-0.5)
-        t = (
-            1
-            / velocity(energy)
-            * integrate.quad(sec_theta, 0, zpos, epsrel=10**-2)[0]
-        )
-
-        if zpos > zmax:
-            print("ERROR: zpos equal to or larger than zmax.")
-
-        return t
-
-    else:
-        print("ERROR: Given trap profile is not a valid trap")
-        return False
-
-
-def t(energy, zpos, center_pitch_angle, rho, trap_profile):
-
-    """Vectorized version of t_not_vect function."""
-
-    t_vect = np.vectorize(t_not_vect)
-
-    return t_vect(energy, zpos, center_pitch_angle, rho, trap_profile)
-
-
-def sideband_calc(avg_cycl_freq, axial_freq, zmax, num_sidebands=7):
-
-    """Calculates relative magnitudes of num_sidebands sidebands from
-    average cyclotron frequency (avg_cycl_freq), axial frequency
-    (axial_freq), and maximum axial amplitude (zmax).
-    """
-
-    # fixed experiment parameters
-    waveguide_radius = 0.578e-2
-    kc = P11_PRIME / waveguide_radius
-
-    # calculated parameters
-    omega = 2 * PI * avg_cycl_freq
-    k_wave = omega / C
-    beta = np.sqrt(k_wave**2 - kc**2)
-
-    phase_vel = omega / beta
-
-    mod_index = omega * zmax / phase_vel
-
-    # Calculate K factor
-    K = 2 * PI * avg_cycl_freq * zmax / phase_vel
-
-    # Calculate list of (frequency, amplitude) of sidebands
-    sidebands = []
-
-    for k in range(-num_sidebands, num_sidebands + 1):
-
-        freq = avg_cycl_freq + k * axial_freq
-        magnitude = abs(ss.jv(k, K))
-
-        pair = (freq, magnitude)
-        sidebands.append(pair)
-
-    return sidebands, mod_index
-
-def anharmonic_axial_trajectory():
-    """ Computes the time series of the beta axial motion over a single
-    found by integrating the relevant ODE. Returns [z(t), vz(t)].
-    """
-    T  = 1. / axial_freq()
-    nHarmonics = 128
-    dt = T/ nHarmonics
-    t = np.arange(0,T,dt)
-
-    mu = p0**2 * np.sin(theta0)**2 / (2. * me * B0) #### XXX: Check gammas!!!
-    ### Coupled ODE for z-motion: z = y[0], vz = y[1]. z'=vz. vz' = -mu * B'(z) / m
-    ode = lambda t, y: [y[1], - mu / me * dfTot(y[0])]
-    result = integrate.solve_ivp(ode, [t[0], t[-1]], (zmax, 0), t_eval=t,rtol=1e-7)
-
-    ####### [0] is z array, [1] is vz array ######
-    return result.y
-
-def instantaneous_frequency(z, vz):
-    """ Computes the instantaneous (angular) frequency as a function of time
-    """
-    return q * B(z) / (me * gamma) * ( 1. + vz / v_ph)
-
-def anharmonic_sideband_powers(num_sidebands=7):
-    omega_c -= np.mean(omega_c)
-    Phi = np.cumsum(omega_c) * dt
-    expPhi = np.exp(1j * Phi)
-    yf = np.abs(fft(expPhi,norm="forward"))
-    yf = yf[:nHarmonics//2]
-
-    # Calculate list of (frequency, amplitude) of sidebands
-    sidebands = []
-
-    for k in range(-num_sidebands, num_sidebands + 1):
-        freq = avg_cycl_freq + k * axial_freq
-        magnitude = yf[abs(k)]
-        pair = (freq, magnitude)
-        sidebands.append(pair)
-
-    ### Intentionally returns modulation index of nan as it is not (meaningfully) defined for harmonic traps
-    return sidebands, np.nan
-
-def power_larmor(field, frequency):
-
-    omega = 2 * PI * frequency
-    energy = freq_to_energy(frequency, field)
-    r_c = cyc_radius(energy, field, 90)
-    beta = velocity(energy) / C
-    p = gamma(energy) * M * velocity(energy)
-
-    power_larmor = (2 / 3 * Q**2 * C * beta**4 * gamma(energy) ** 4) / (
-        4 * PI * EPS_0 * r_c**2
-    )
-
-    return power_larmor
+"""spec_calc
+
+This set of calculators takes cres electron properties (such as energy, pitch angle), as 
+well as information about the trap (instance of a trap_profile object) and outputs other 
+cres electron properties such as axial frequency, z_max, B_avg.
+
+---
+Units for all module functions' inputs/outputs: 
+
+Energy   : eV
+B-field  : T
+Time     : s
+Angle    : degrees
+Distance : m
+Frequency: Hz
+Power    : W
+
+
+---
+"""
+# TODO: Organize the imports.
+import math
+import os
+
+import numpy as np
+
+import scipy.integrate as integrate
+from scipy.fft import fft
+from scipy.optimize import fmin, fminbound
+from scipy.interpolate import interp1d
+from scipy.misc import derivative
+import scipy.special as ss
+
+#import constants
+from he6_cres_spec_sims.constants import *
+
+
+
+# Simple special relativity functions.
+
+
+def gamma(energy):
+    gamma = (energy + ME) / ME
+    return gamma
+
+def energy(gamma):
+    energy = ME*(gamma - 1)
+    return energy
+
+def momentum(energy):
+    momentum = (((energy + ME) ** 2 - ME**2) / C**2) ** 0.5 / J_TO_EV
+    return momentum
+
+
+def velocity(energy):
+    velocity = momentum(energy) / (gamma(energy) * M)
+    return velocity
+
+
+# CRES functions.
+
+
+def energy_to_freq(energy, field):
+
+    """Converts kinetic energy to cyclotron frequency."""
+
+    cycl_freq = Q * field / (2 * PI * gamma(energy) * M)
+
+    return cycl_freq
+
+
+def freq_to_energy(frequency, field):
+
+    """Calculates energy of beta particle in eV given cyclotron
+    frequency in Hz, magnetic field in Tesla, and pitch angle
+    at 90 degrees.
+    """
+
+    gamma = Q * field / (2 * PI * frequency * M)
+    if np.any(gamma < 1):
+        gamma = 1
+        max_freq = Q * field / (2 * PI * M)
+        warning = "Warning: {} higher than maximum cyclotron frequency {}".format(
+            frequency, max_freq
+        )
+        print(warning)
+    return gamma * ME - ME
+
+
+def energy_and_freq_to_field(energy, freq):
+
+    """Converts kinetic energy to cyclotron frequency."""
+
+    field = (2 * PI * gamma(energy) * M * freq) / Q
+
+    return field
+
+
+def power_from_slope(energy, slope, field):
+
+    """Converts slope, energy, field into the associated cres power."""
+
+    energy_Joules = (energy + ME) / J_TO_EV
+
+    power = slope * (2 * PI) * ((energy_Joules) ** 2) / (Q * field * C**2)
+
+    return power
+
+
+def random_beta_generator(parameter_dict, rng):
+
+    """
+    Generates a random beta in the trap with pitch angle between
+    min_theta and max_theta , and initial position (rho,0,z) between
+    min_rho and max_rho and min_z and max_z.
+    """
+    min_rho = parameter_dict["min_rho"]
+    max_rho = parameter_dict["max_rho"]
+
+    min_z = parameter_dict["min_z"]
+    max_z = parameter_dict["max_z"]
+
+    min_theta = parameter_dict["min_theta"] / RAD_TO_DEG
+    max_theta = parameter_dict["max_theta"] / RAD_TO_DEG
+
+    # Uniform distribution in an annulus in cylindrical coordinates, found by inverse transform sampling
+    rho_initial = np.sqrt(min_rho**2 + rng.uniform(0, 1) * (max_rho**2 - min_rho**2))
+    phi_initial = 2 * PI * rng.uniform(0, 1) * RAD_TO_DEG
+    z_initial = rng.uniform(min_z, max_z)
+
+    u_min = (1 - np.cos(min_theta)) / 2
+    u_max = (1 - np.cos(max_theta)) / 2
+
+    sphere_theta_initial = np.arccos(1 - 2 * (rng.uniform(u_min, u_max))) * RAD_TO_DEG
+    sphere_phi_initial = 2 * PI * rng.uniform(0, 1) * RAD_TO_DEG
+
+    position = [rho_initial, phi_initial, z_initial]
+    direction = [sphere_theta_initial, sphere_phi_initial]
+
+    return position, direction
+
+
+def theta_center(zpos, rho, pitch_angle, trap_profile):
+
+    """Calculates the pitch angle an electron with current z-coordinate
+    zpos, rho, and current pitch angle pitch_angle takes at the center
+    of given trap.
+    """
+
+    if trap_profile.is_trap:
+
+        Bmin = trap_profile.field_strength(rho, 0.0)
+        Bcurr = trap_profile.field_strength(rho, zpos)
+
+        theta_center_calc = (
+            np.arcsin((np.sqrt(Bmin / Bcurr)) * np.sin(pitch_angle / RAD_TO_DEG))
+            * RAD_TO_DEG
+        )
+
+        return theta_center_calc
+
+    else:
+        print("ERROR: Given trap profile is not a valid trap")
+        return False
+
+
+def cyc_radius(energy, field, pitch_angle):
+
+    """Calculates the instantaneous cyclotron radius of a beta electron
+    given the energy, magnetic field, and current pitch angle.
+    """
+
+    vel_perp = velocity(energy) * np.sin(pitch_angle / RAD_TO_DEG)
+
+    cyc_radius = (gamma(energy) * M * vel_perp) / (Q * field)
+
+    return cyc_radius
+
+
+def max_radius(energy, center_pitch_angle, rho, trap_profile):
+
+    """Calculates the maximum cyclotron radius of a beta electron given
+    the kinetic energy, trap_profile, and center pitch angle (pitch angle
+    at center of trap).
+    """
+
+    if trap_profile.is_trap:
+
+        min_field = trap_profile.field_strength(rho, 0)
+        max_field = min_field / (np.sin(center_pitch_angle / RAD_TO_DEG)) ** 2
+
+        center_radius = cyc_radius(energy, min_field, center_pitch_angle)
+        end_radius = cyc_radius(energy, max_field, pitch_angle=90)
+
+        if np.all(center_radius >= end_radius):
+            return center_radius
+        else:
+            print(
+                "Warning: max_radius is occuring at end of trap (theta=90). \
+                Something odd may be going on."
+            )
+            return False
+
+    else:
+        print("ERROR: Given trap profile is not a valid trap")
+        return False
+
+
+def min_radius(energy, center_pitch_angle, rho, trap_profile):
+
+    """Calculates the minimum cyclotron radius of a beta electron given
+    the kinetic energy, trap_profile, and center pitch angle (pitch angle
+    at center of trap).
+    """
+
+    if trap_profile.is_trap:
+
+        min_field = trap_profile.field_strength(rho, 0)
+        max_field = min_field / (np.sin(center_pitch_angle / RAD_TO_DEG)) ** 2
+
+        center_radius = cyc_radius(energy, min_field, center_pitch_angle)
+        end_radius = cyc_radius(energy, max_field, pitch_angle=90)
+
+        if np.all(center_radius >= end_radius):
+            return end_radius
+        else:
+            print(
+                "Warning: min_radius is occuring at center of trap, something \
+                odd may be going on."
+            )
+            return False
+
+    else:
+        print("ERROR: Given trap profile is not a valid trap")
+        return False
+
+
+def min_theta(rho, zpos, trap_profile):
+
+    """Calculates the minimum pitch angle theta at which an electron at
+    zpos is trapped given trap_profile.
+    """
+
+    if trap_profile.is_trap:
+
+        # Be careful here. Technically the Bmax doesn't occur at a constant z.
+        Bmax = trap_profile.field_strength(rho, trap_profile.trap_width[1])
+        Bz = trap_profile.field_strength(rho, zpos)
+
+        theta = np.arcsin((Bz / Bmax) ** 0.5) * RAD_TO_DEG
+        return theta
+
+    else:
+        print("ERROR: Given trap profile is not a valid trap")
+        return False
+
+
+def max_zpos_not_vectorized(energy, center_pitch_angle, rho, trap_profile, debug=False):
+
+    """Calculates the maximum axial length from center of trap as a
+    function of center_pitch_angle and rho. Not vectorized. See below
+    for vectorized version.
+    """
+
+    if trap_profile.is_trap:
+
+        if center_pitch_angle < min_theta(rho, 0, trap_profile):
+            print("WARNING: Electron not trapped (zpos)")
+            return False
+
+        else:
+            # Ok, so does this mean we now have an energy dependence on zmax? Yes.
+            c_r = cyc_radius(
+                energy, trap_profile.field_strength(rho, 0), center_pitch_angle
+            )
+            rho_p = np.sqrt(rho**2 + c_r**2 / 2)
+
+            min_field = trap_profile.field_strength(rho_p, 0)
+            max_field = trap_profile.field_strength(rho_p, trap_profile.trap_width[1])
+
+            max_reached_field = min_field / pow(
+                math.sin(center_pitch_angle * math.pi / 180), 2
+            )
+
+            # initial guess based on treating magnetic well as v-shaped
+            slope = (max_field - min_field) / (trap_profile.trap_width[1])
+            initial_z = (max_reached_field - min_field) / slope
+
+            if initial_z == trap_profile.trap_width[1]:
+                return initial_z
+
+            def func(z):
+                curr_field = trap_profile.field_strength(rho_p, z)
+                return abs(curr_field - max_reached_field)
+
+            max_z = fminbound(func, 0, trap_profile.trap_width[1], xtol=1e-14)
+            curr_field = trap_profile.field_strength(rho_p, max_z)
+
+            if (curr_field > max_reached_field) and debug == True:
+                print(
+                    "Final field greater than max allowed field by: ",
+                    curr_field - max_reached_field,
+                )
+                print("Bmax reached: ", curr_field)
+
+            if debug == True:
+                print("zlength: ", max_z)
+
+            if max_z > trap_profile.trap_width[1]:
+                print("Error Rate: ", max_z - trap_profile.trap_width[1])
+
+            return max_z
+
+    else:
+        print("ERROR: Given trap profile is not a valid trap")
+        return False
+
+
+def max_zpos(energy, center_pitch_angle, rho, trap_profile, debug=False):
+
+    """Vectorized version of max_zpos_not_vectorized function."""
+
+    max_zpos_vectorized = np.vectorize(max_zpos_not_vectorized)
+
+    return max_zpos_vectorized(energy, center_pitch_angle, rho, trap_profile)
+
+
+def mod_index(avg_cycl_freq, zmax):
+
+    """Calculates modulation index from average cyclotron frequency
+    (avg_cycl_freq) and maximum axial amplitude (zmax).
+    """
+    # calculated parameters
+    omega = 2 * PI * avg_cycl_freq
+    beta = waveguide_beta(omega)
+
+    mod_index = zmax * beta
+
+    return mod_index
+
+
+def df_dt(energy, field, power):
+
+    """Calculates cyclotron frequency rate of change of electron with
+    given kinetic energy at field in T radiating energy at rate power.
+    """
+
+    energy_Joules = (energy + ME) / J_TO_EV
+
+    slope = (Q * field * C**2) / (2 * PI) * (power) / (energy_Joules) ** 2
+
+    return slope
+
+
+def curr_pitch_angle(rho, zpos, center_pitch_angle, trap_profile):
+
+    """Calculates the current pitch angle of an electron at zpos given
+    center pitch angle and main field strength.
+    """
+
+    if trap_profile.is_trap:
+
+        min_field = trap_profile.field_strength(rho, 0)
+        max_z = max_zpos(center_pitch_angle, rho, trap_profile)
+        max_reached_field = trap_profile.field_strength(rho, max_z)
+
+        if np.any(abs(zpos) > max_z):
+            print("Electron does not reach given zpos")
+            curr_pitch = "FAIL"
+        else:
+            curr_field = trap_profile.field_strength(rho, zpos)
+            curr_pitch = np.arcsin(np.sqrt(curr_field / max_reached_field)) * RAD_TO_DEG
+
+        return curr_pitch
+
+    else:
+        print("ERROR: Given trap profile is not a valid trap")
+        return False
+
+
+def axial_freq_not_vect(energy, center_pitch_angle, rho, trap_profile):
+
+    """Caculates the axial frequency of a trapped electron."""
+
+    if trap_profile.is_trap:
+        # center_pitch_angle = np.where(center_pitch_angle == 90.0, 89.999, center_pitch_angle)
+        if center_pitch_angle == 90.0:
+            center_pitch_angle = 89.999
+
+        zmax = max_zpos(energy, center_pitch_angle, rho, trap_profile)
+
+        c_r = cyc_radius(
+            energy, trap_profile.field_strength(rho, 0), center_pitch_angle
+        )
+        rho_p = np.sqrt(rho**2 + c_r**2 / 2)
+
+        B = lambda z: trap_profile.field_strength(rho_p, z)
+        Bmax = trap_profile.field_strength(rho_p, zmax)
+
+        # Secant of theta as function of z. Use conserved mu to derive.
+        sec_theta = lambda z: (1 - B(z) / Bmax) ** (-0.5)
+        T_a = 4 / velocity(energy) * integrate.quad(sec_theta, 0, zmax)[0]
+
+        axial_frequency = 1 / T_a
+
+        return axial_frequency
+
+    else:
+        print("ERROR: Given trap profile is not a valid trap")
+        return False
+
+
+def axial_freq(energy, center_pitch_angle, rho, trap_profile):
+
+    """Vectorized version of axial_freq_not_vectorized function."""
+
+    axial_freq_vect = np.vectorize(axial_freq_not_vect)
+
+    return axial_freq_vect(energy, center_pitch_angle, rho, trap_profile)
+
+
+def avg_cycl_freq_not_vect(energy, center_pitch_angle, rho, trap_profile):
+
+    """Calculates the average cyclotron frquency of an electron given
+    kinetic energy, main field, and center pitch angle.
+    Returns 0 if electron is not trapped.
+    """
+
+    if trap_profile.is_trap:
+
+        Bmin = trap_profile.field_strength(rho, 0)
+        min_trapped_angle = min_theta(rho, 0, trap_profile)
+
+        if center_pitch_angle < min_trapped_angle:
+            print("Warning: (avg_cyc) electron not trapped.")
+            return False
+
+        if center_pitch_angle == 90.0:
+            avg_cyc_freq = energy_to_freq(energy, Bmin)
+
+        else:
+            zmax = max_zpos(energy, center_pitch_angle, rho, trap_profile)
+            B = lambda z: trap_profile.field_strength(rho, z)
+            Bmax = trap_profile.field_strength(rho, zmax)
+            integrand = lambda z: B(z) * ((1 - B(z) / Bmax) ** (-0.5))
+
+            ax_freq = axial_freq(energy, center_pitch_angle, rho, trap_profile)
+
+            # Similar to axial_freq calculation.
+            avg_cyc_freq = (
+                4
+                * Q
+                * ax_freq
+                / (2 * PI * momentum(energy))
+                * integrate.quad(integrand, 0, zmax, epsrel=10**-2)[0]
+            )
+
+        return avg_cyc_freq
+
+    else:
+        print("ERROR: Given trap profile is not a valid trap")
+        return False
+
+
+def avg_cycl_freq(energy, center_pitch_angle, rho, trap_profile):
+
+    field = b_avg(energy, center_pitch_angle, rho, trap_profile)
+
+    return energy_to_freq(energy, field)
+
+
+def b_avg_not_vect(energy, center_pitch_angle, rho, trap_profile):
+
+    """Calculates the average magnetic field experienced by an electron
+    of a given kinetic energy, main field, and center pitch angle.
+    Returns 0 if electron is not trapped.
+    """
+
+    c_r = cyc_radius(energy, trap_profile.field_strength(rho, 0), center_pitch_angle)
+
+    rho_p = np.sqrt(rho**2 + c_r**2 / 2)
+    rho_pp = np.sqrt(rho**2 + c_r**2)
+
+    if trap_profile.is_trap:
+
+        Bmin = trap_profile.field_strength(rho_p, 0)
+        min_trapped_angle = min_theta(rho_p, 0, trap_profile)
+
+        if center_pitch_angle < min_trapped_angle:
+            print("Warning: (avg_cyc) electron not trapped.")
+            return False
+
+        if center_pitch_angle == 90.0:
+            avg_cyc_freq = energy_to_freq(energy, Bmin)
+
+        else:
+
+            zmax = max_zpos(energy, center_pitch_angle, rho, trap_profile)
+            B1 = lambda z: trap_profile.field_strength(rho_pp, z)
+            B = lambda z: trap_profile.field_strength(rho_p, z)
+            Bmax = trap_profile.field_strength(rho_p, zmax)
+            integrand = lambda z: B1(z) * ((1 - B(z) / Bmax) ** (-0.5))
+
+            ax_freq = axial_freq(energy, center_pitch_angle, rho, trap_profile)
+
+            # Similar to axial_freq calculation.
+            b_avg = (
+                4
+                * ax_freq
+                / (velocity(energy))
+                * integrate.quad(integrand, 0, zmax, epsrel=10**-3)[0]
+            )
+
+        return b_avg
+
+    else:
+        print("ERROR: Given trap profile is not a valid trap")
+        return False
+
+
+def b_avg(energy, center_pitch_angle, rho, trap_profile):
+
+    """Vectorized version of b_avg_not_vectorized function."""
+
+    b_avg_vect = np.vectorize(b_avg_not_vect)
+
+    return b_avg_vect(energy, center_pitch_angle, rho, trap_profile)
+
+
+def t_not_vect(energy, zpos, center_pitch_angle, rho, trap_profile):
+
+    """DEBUG(byron): This is returning negative times.
+    Caculates the time for electron to travel from z = 0 to zpos.
+    """
+
+    if trap_profile.is_trap:
+
+        if center_pitch_angle == 90.0:
+            center_pitch_angle = 89.999
+
+        zmax = max_zpos(energy, center_pitch_angle, rho, trap_profile)
+        B = lambda z: trap_profile.field_strength(rho, z)
+        Bmax = trap_profile.field_strength(rho, zmax)
+
+        # Secant of theta as function of z. Use conserved mu to derive.
+        sec_theta = lambda z: (1 - B(z) / Bmax) ** (-0.5)
+        t = (
+            1
+            / velocity(energy)
+            * integrate.quad(sec_theta, 0, zpos, epsrel=10**-2)[0]
+        )
+
+        if zpos > zmax:
+            print("ERROR: zpos equal to or larger than zmax.")
+
+        return t
+
+    else:
+        print("ERROR: Given trap profile is not a valid trap")
+        return False
+
+
+def t(energy, zpos, center_pitch_angle, rho, trap_profile):
+
+    """Vectorized version of t_not_vect function."""
+
+    t_vect = np.vectorize(t_not_vect)
+
+    return t_vect(energy, zpos, center_pitch_angle, rho, trap_profile)
+
+def waveguide_beta(omega):
+    """  Computes the (waveguide definition) of beta (propagation constant for TE11 mode
+    """
+    # fixed experiment parameters
+    waveguide_radius = 0.578e-2
+    P11_PRIME = 1.84118  # first zero of J1 prime (bessel functions)
+    kc = P11_PRIME / waveguide_radius
+
+    # calculated parameters
+    k_wave = omega / C
+    beta = np.sqrt(k_wave**2 - kc**2)
+    return beta
+
+def sideband_calc(energy, rho, avg_cycl_freq, axial_freq, zmax, trap_profile, magnetic_modulation=True, num_sidebands=7, nHarmonics=128):
+
+    """Calculates relative magnitudes of num_sidebands sidebands from
+    average cyclotron frequency (avg_cycl_freq), axial frequency
+    (axial_freq), and maximum axial amplitude (zmax).
+    """
+    if magnetic_modulation:
+        T = 1./ axial_freq
+        dt = T/ nHarmonics
+        t = np.arange(0,T,dt)
+        omegaA = 2. * np.pi * axial_freq
+
+        z = zmax*np.sin(omegaA * t)
+        vz = zmax*omegaA*np.cos(omegaA * t)
+
+        sidebands =  FFT_sideband_amplitudes(energy, rho, avg_cycl_freq, axial_freq, vz, z, trap_profile, True, nHarmonics)
+        return format_sideband_array(sidebands, avg_cycl_freq, axial_freq, np.nan, num_sidebands)
+
+    else:
+        h =  mod_index(avg_cycl_freq, zmax)
+        sidebands = [abs(ss.jv(k, h)) for k in range(num_sidebands+1)]
+        return format_sideband_array(sidebands, avg_cycl_freq, axial_freq, h, num_sidebands)
+
+
+
+def anharmonic_sideband_calc(energy, center_pitch_angle, rho, avg_cycl_freq, axial_freq, zmax, trap_profile, magnetic_modulation=True, num_sidebands=7, nHarmonics=128):
+
+    #c_r = cyc_radius(energy, trap_profile.field_strength(rho, 0), center_pitch_angle)
+    #rho= np.sqrt(rho**2 + c_r**2 / 2)
+
+    ### Compute particle trajectory over single period
+    sol = anharmonic_axial_trajectory(energy, center_pitch_angle, rho, axial_freq, zmax, trap_profile, nHarmonics)
+    z = sol[0]
+    vz = sol[1]
+
+    sidebands =  FFT_sideband_amplitudes(energy, rho, avg_cycl_freq, axial_freq, vz, z, trap_profile, magnetic_modulation, nHarmonics)
+    return format_sideband_array(sidebands, avg_cycl_freq, axial_freq, np.nan, num_sidebands)
+
+
+def anharmonic_axial_trajectory(energy, center_pitch_angle, rho, axial_freq, zmax, trap_profile, nHarmonics):
+    """ Computes the time series of the beta axial motion over a single
+    found by integrating the relevant ODE. Returns [z(t), vz(t)].
+    """
+    if not trap_profile.is_trap:
+        print("ERROR: Given trap profile is not a valid trap")
+        return False
+
+    T = 1./ axial_freq
+    dt = T/ nHarmonics
+    t = np.arange(0,T,dt)
+
+    p0 = M * velocity(energy)
+    ### Note: This is the non-relativistic magnetic moment. One gets the same ODE if M -> gamma M in the lambda ode.
+    Bmin = trap_profile.field_strength(rho, 0)
+    mu = p0**2 * np.sin(center_pitch_angle / RAD_TO_DEG )**2 / (2. * M * Bmin)
+    Bz = lambda z: trap_profile.field_strength(rho,z) 
+    dBdz = lambda z: derivative(Bz, z, dx=1e-6)
+    ### Coupled ODE for z-motion: z = y[0], vz = y[1]. z'=vz. vz' = -mu * B'(z) / m
+    ode = lambda t, y: [y[1], - mu / M * dBdz(y[0])]
+    result = integrate.solve_ivp(ode, [t[0], t[-1]], (zmax, 0), t_eval=t,rtol=1e-7)
+
+    ####### [0] is z array, [1] is vz array ######
+    return result.y
+
+def instantaneous_frequency(energy, rho, avg_cycl_freq, vz, z=None, trap_profile=None, magnetic_modulation=False):
+    """ Computes the instantaneous (angular) frequency as a function of time. Magnetic modulation controls whether 
+        instantaneous changes in magnetic field are included, or just the Doppler effect. Defaults chosen so one could pass
+        fewer arguments if not using magnetic_modulation
+    """
+    omega = 2 * PI * avg_cycl_freq
+    beta = waveguide_beta(omega)
+    phase_vel = omega / beta
+
+    if magnetic_modulation:
+        if not trap_profile.is_trap:
+            print("ERROR: Given trap profile is not a valid trap")
+            return False
+        Bz = lambda z: trap_profile.field_strength(rho, z)
+        return Q * Bz(z) / (M * gamma(energy)) * ( 1. + vz / phase_vel)
+    else:
+        ### Instead of evaluating at B(0), use average_cyc_freq to say B field contribution is const. equal to avg
+        return omega * ( 1. + vz / phase_vel)
+
+
+def FFT_sideband_amplitudes(energy, rho, avg_cycl_freq, axial_freq, vz, z, trap_profile, magnetic_modulation, nHarmonics=128):
+    """  Computes sideband amplitudes as a function of axial trajectory, magnetic field profile. Returns list with sidebands
+    """
+    ### Convert particle trajectory to instantaneous radiated frequency (Doppler + B-field)
+    dt = 1./ (nHarmonics * axial_freq)
+
+    omega_c = instantaneous_frequency(energy, rho, avg_cycl_freq, vz, z, trap_profile, magnetic_modulation)
+    omega_c -= np.mean(omega_c)
+    Phi = np.cumsum(omega_c) * dt
+    expPhi = np.exp(1j * Phi)
+    yf = np.abs(fft(expPhi,norm="forward"))
+    yf = yf[:nHarmonics//2]
+    return yf
+
+def format_sideband_array(sidebands_one, avg_cyc_freq, axial_freq, mod_index=np.nan, num_sidebands = 7):
+    """ Does formatting for array with list of sideband magnitudes (normalized), and their start frequencies. 
+        Takes in 1-sided list of sideband magnitudes
+    """
+    # Calculate (2-sided) list of (frequency, amplitude) of sidebands
+    sidebands = []
+
+    for k in range(-num_sidebands, num_sidebands + 1):
+        freq = avg_cyc_freq + k * axial_freq
+        magnitude = sidebands_one[abs(k)]
+        pair = (freq, magnitude)
+        sidebands.append(pair)
+
+    ### Intentionally returns modulation index of nan as it is only (meaningfully) defined for harmonic traps
+    return sidebands, mod_index
+
+def power_larmor(field, frequency):
+
+    omega = 2 * PI * frequency
+    energy = freq_to_energy(frequency, field)
+    r_c = cyc_radius(energy, field, 90)
+    beta = velocity(energy) / C
+    p = gamma(energy) * M * velocity(energy)
+
+    power_larmor = (2 / 3 * Q**2 * C * beta**4 * gamma(energy) ** 4) / (
+        4 * PI * EPS_0 * r_c**2
+    )
+
+    return power_larmor
+
+def power_larmor_e(field, energy):
+    """Takes energy instead of frequency as input. """
+
+    r_c = cyc_radius(energy, field, 90)
+    beta = velocity(energy) / C
+    p = gamma(energy) * M * velocity(energy)
+
+    power_larmor = (2 / 3 * Q**2 * C * beta**4 * gamma(energy) ** 4) / (
+        4 * PI * EPS_0 * r_c**2
+    )
+
+    return power_larmor
```

### Comparing `he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/trap_field_profile.py` & `he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/trap_field_profile.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-import csv
-import math
-import os
-import pathlib
-import time
-
-import numpy as np
-from scipy.interpolate import interp2d
-from scipy.misc import derivative
-from scipy.optimize import fmin
-
-
-class TrapFieldProfile:
-    def __init__(self, main_field, trap_current):
-
-        # TODO: May want to protect these variables with underscores?
-        # TODO: Would be nice to have an attribute be the relative trap depth.
-        # TODO: Add in trap radius as an attribute?
-        
-        self.trap_current = trap_current
-        self.main_field = main_field
-
-        self.field_strength = self.initialize_field_strength_interp()
-        self.trap_width = self.trap_width_calc()
-
-        # TODO: Actually test to be sure it is a trap.
-        self.is_trap = True
-
-        self.relative_depth = (main_field - self.field_strength(0, 0)) / main_field
-
-    def initialize_field_strength_interp(self):
-        """Document"""
-        # TODO: hmm I guess these need to be hardcoded for the moment.
-        waveguide_radius = 0.578e-2  # (m)
-        trap_zmax = 5.5e-2  # (m)
-
-        grid_edge_length = 4e-4  # (m), it was found that grid_edge_length = 5e-4 results in 1ppm agreement between field_stength and field_strength_interp
-
-        rho_array = np.arange(0, waveguide_radius, grid_edge_length)
-        z_array = np.arange(-trap_zmax, trap_zmax, grid_edge_length)
-
-        dir_path = pathlib.Path(__file__).parents[0]
-
-        pkl_path = (
-            dir_path
-            / "trap_field_profile_pkl/2021_trap_profile_mainfield_0T_trap_1A.csv"
-        )
-
-        try:
-            with open(pkl_path, "r") as pkl_file:
-                map_array = np.loadtxt(pkl_file)
-
-        except IOError as e:
-            print("Do you have a field map here: {} ".format(pkl_path))
-            raise e
-
-        # Adjust the field values so they align with the given trap configuration.
-        map_array = map_array * self.trap_current + self.main_field
-        # Now use the map_array to do the interpolation.
-        B_interp2d = interp2d(rho_array, z_array, map_array, kind="cubic")
-
-        # Making it vectorized, meaning float or np array can be inputs.
-        def B_interp(rho, z):
-            return B_interp2d(rho, z)[0]
-
-        return np.vectorize(B_interp)
-
-    def trap_width_calc(self):
-        """
-        Calculates the trap width of the object trap_profile.
-        """
-
-        field_func = self.field_strength
-
-        def func(z):
-            return -1 * field_func(0, z)
-
-        maximum = fmin(func, 0, xtol=1e-12)[0]
-        print("Trap width: ({},{})".format(-maximum, maximum))
-        print("Maximum Field: {}".format(-1 * func(maximum)))
-
-        trap_width = (-maximum, maximum)
-        return trap_width
+import csv
+import math
+import os
+import pathlib
+import time
+
+import numpy as np
+from scipy.interpolate import interp2d
+from scipy.misc import derivative
+from scipy.optimize import fmin
+
+
+class TrapFieldProfile:
+    def __init__(self, main_field, trap_current):
+
+        # TODO: May want to protect these variables with underscores?
+        # TODO: Would be nice to have an attribute be the relative trap depth.
+        # TODO: Add in trap radius as an attribute?
+        
+        self.trap_current = trap_current
+        self.main_field = main_field
+
+        self.field_strength = self.initialize_field_strength_interp()
+        self.trap_width = self.trap_width_calc()
+
+        # TODO: Actually test to be sure it is a trap.
+        self.is_trap = True
+
+        self.relative_depth = (main_field - self.field_strength(0, 0)) / main_field
+
+    def initialize_field_strength_interp(self):
+        """Document"""
+        # TODO: hmm I guess these need to be hardcoded for the moment.
+        waveguide_radius = 0.578e-2  # (m)
+        trap_zmax = 5.5e-2  # (m)
+
+        grid_edge_length = 4e-4  # (m), it was found that grid_edge_length = 5e-4 results in 1ppm agreement between field_stength and field_strength_interp
+
+        rho_array = np.arange(0, waveguide_radius, grid_edge_length)
+        z_array = np.arange(-trap_zmax, trap_zmax, grid_edge_length)
+
+        dir_path = pathlib.Path(__file__).parents[0]
+
+        pkl_path = (
+            dir_path
+            / "trap_field_profile_pkl/2021_trap_profile_mainfield_0T_trap_1A.csv"
+        )
+
+        try:
+            with open(pkl_path, "r") as pkl_file:
+                map_array = np.loadtxt(pkl_file)
+
+        except IOError as e:
+            print("Do you have a field map here: {} ".format(pkl_path))
+            raise e
+
+        # Adjust the field values so they align with the given trap configuration.
+        map_array = map_array * self.trap_current + self.main_field
+        # Now use the map_array to do the interpolation.
+        B_interp2d = interp2d(rho_array, z_array, map_array, kind="cubic")
+
+        # Making it vectorized, meaning float or np array can be inputs.
+        def B_interp(rho, z):
+            return B_interp2d(rho, z)[0]
+
+        return np.vectorize(B_interp)
+
+    def trap_width_calc(self):
+        """
+        Calculates the trap width of the object trap_profile.
+        """
+
+        field_func = self.field_strength
+
+        def func(z):
+            return -1 * field_func(0, z)
+
+        maximum = fmin(func, 0, xtol=1e-12)[0]
+        print("Trap width: ({},{})".format(-maximum, maximum))
+        print("Maximum Field: {}".format(-1 * func(maximum)))
+
+        trap_width = (-maximum, maximum)
+        return trap_width
```

### Comparing `he6_cres_spec_sims-0.1.5/he6_cres_spec_sims/spec_tools/trap_field_profile_pkl/2021_trap_profile_mainfield_0T_trap_1A.csv` & `he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims/spec_tools/trap_field_profile_pkl/2021_trap_profile_mainfield_0T_trap_1A.csv`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,275 +1,275 @@
-8.251458698098414505e-04 8.246769589162286380e-04 8.234039043558003196e-04 8.212721733606382973e-04 8.182668452132121385e-04 8.143671167745807592e-04 8.095464051753534099e-04 8.037725049410900406e-04 7.970078194015538459e-04 7.892096925689142447e-04 7.803308740403520080e-04 7.703201569929625861e-04 7.591232350217194278e-04 7.466838371619741220e-04 7.329451935972345266e-04
-8.666880077794763973e-04 8.662233891057375974e-04 8.649646829590024698e-04 8.628554233099085475e-04 8.598784929777047829e-04 8.560099491161493037e-04 8.512190619265760190e-04 8.454683908889397501e-04 8.387139200206762246e-04 8.309052812555254349e-04 8.219861031712825256e-04 8.118945323648632008e-04 8.005639841770494395e-04 7.879241971348899688e-04 7.739026658341767798e-04
-9.099008429463485183e-04 9.094454302024174630e-04 9.082147730035228066e-04 9.061508125134442107e-04 9.032342174087134743e-04 8.994378637587281721e-04 8.947267919680939544e-04 8.890581775678933025e-04 8.823813377885848710e-04 8.746378044582922388e-04 8.657615037154720505e-04 8.556790942608376652e-04 8.443105353375451524e-04 8.315699642328702994e-04 8.173669938254197803e-04
-9.547460132392979193e-04 9.543053468077052938e-04 9.531181691322979880e-04 9.511252652566476321e-04 9.483051417141248997e-04 9.446275501506826806e-04 9.400533448591558193e-04 9.345343231955019307e-04 9.280130695221833594e-04 9.204228324409187726e-04 9.116874764018822455e-04 9.017215614475613704e-04 8.904306313930435320e-04 8.777117991537690790e-04 8.634547656783294863e-04
-1.001164609950772532e-03 1.000744838966615823e-03 9.996182519631060560e-04 9.977250180730253687e-04 9.950416171605788295e-04 9.915348518661501812e-04 9.871615898314125160e-04 9.818684503338677427e-04 9.755914528085739930e-04 9.682556530332358906e-04 9.597748048030894496e-04 9.500510992923891316e-04 9.389750630632696547e-04 9.264257118302860481e-04 9.122711119770747284e-04
-1.049074973538484086e-03 1.048682814193480214e-03 1.047635494389912575e-03 1.045873215311582480e-03 1.043370661192264846e-03 1.040091998608721905e-03 1.035990490777310589e-03 1.031008011368883407e-03 1.025074469183329725e-03 1.018107162108353517e-03 1.010010089203796247e-03 1.000673268091927665e-03 9.899721247632539689e-04 9.777670602284787172e-04 9.639033430296588267e-04
-1.098370647900580180e-03 1.098013314820221655e-03 1.097065314351421562e-03 1.095467635479777666e-03 1.093193502428132851e-03 1.090204910532094167e-03 1.086452105614331854e-03 1.081872912983997863e-03 1.076391918421576313e-03 1.069919508289635546e-03 1.062350782531073460e-03 1.053564375250083283e-03 1.043421226055517943e-03 1.031763396749678461e-03 1.018413065308820765e-03
-1.148918591128879211e-03 1.148603699605396829e-03 1.147776175569215074e-03 1.146378654076584324e-03 1.144383343802659204e-03 1.141750693350404187e-03 1.138428736352133487e-03 1.134352233860187005e-03 1.129441604818144694e-03 1.123601636469013457e-03 1.116719967823146236e-03 1.108665358363047134e-03 1.099285750966683562e-03 1.088406192567250219e-03 1.075826704526137729e-03
-1.200557748484297211e-03 1.200293186708070291e-03 1.199608048116102476e-03 1.198447560028561556e-03 1.196783469951667733e-03 1.194575461647333012e-03 1.191770381163758307e-03 1.188301202856967232e-03 1.184085719853381416e-03 1.179024931080912544e-03 1.173001093718464751e-03 1.165875417662684630e-03 1.157485371566711625e-03 1.147641604785184415e-03 1.136124511314853596e-03
-1.253098096143418329e-03 1.252891868315510757e-03 1.252371337859033672e-03 1.251485349120837372e-03 1.250205834132558707e-03 1.248492641672240651e-03 1.246292660065379280e-03 1.243538634198036296e-03 1.240147647278242327e-03 1.236019218741851765e-03 1.231032960627075892e-03 1.225045725374593200e-03 1.217888166448511094e-03 1.209360636603841509e-03 1.199228353319265654e-03
-1.306320260728286537e-03 1.306180303998706518e-03 1.305846411595629588e-03 1.305272117103545076e-03 1.304430261920048670e-03 1.303281910828748679e-03 1.301775397719914318e-03 1.299845036926637089e-03 1.297409450057432747e-03 1.294369440293647103e-03 1.290605331084471695e-03 1.285973654625076519e-03 1.280303016797418271e-03 1.273389270978323102e-03 1.264988908632659658e-03
-1.359975808704555825e-03 1.359909789084633646e-03 1.359783806903593247e-03 1.359557165777019235e-03 1.359204401180540535e-03 1.358688926076052255e-03 1.357962046393332203e-03 1.356961622622503963e-03 1.355610317001121898e-03 1.353813341307849973e-03 1.351455600277676194e-03 1.348398074622721848e-03 1.344473260892519936e-03 1.339479411447671046e-03 1.333173252019167251e-03
-1.413788280847893576e-03 1.413803375417640919e-03 1.413905208787005286e-03 1.414059916270368669e-03 1.414244528898890877e-03 1.414425975250449379e-03 1.414560115701654023e-03 1.414590422818240130e-03 1.414446241740222867e-03 1.414040534913557981e-03 1.413266993447817761e-03 1.411996327975689356e-03 1.410071518898813828e-03 1.407301696540673788e-03 1.403454215296332137e-03
-1.467455020361010942e-03 1.467557694956730160e-03 1.467905264537987253e-03 1.468471694703994473e-03 1.469237294681922283e-03 1.470173652577304660e-03 1.471242741118637155e-03 1.472395691621981731e-03 1.473571170508245235e-03 1.474693262293995779e-03 1.475668737601112642e-03 1.476383512047740095e-03 1.476698057417306182e-03 1.476441401425265419e-03 1.475403213311188939e-03
-1.520649809946401617e-03 1.520845602833211570e-03 1.521454242068595629e-03 1.522458417443907537e-03 1.523842438986079770e-03 1.525583612813727992e-03 1.527651470015551098e-03 1.530006708236136825e-03 1.532599787746009856e-03 1.535369096163139054e-03 1.538238571069847158e-03 1.541114603149409002e-03 1.543881994573738890e-03 1.546398625001165665e-03 1.548488329449515186e-03
-1.573026295216811872e-03 1.573319617781321431e-03 1.574201517590846167e-03 1.575664158416537324e-03 1.577696473663376710e-03 1.580282400004270286e-03 1.583400274734963944e-03 1.587022010517392945e-03 1.591112003376060928e-03 1.595625708727786782e-03 1.600507800247186370e-03 1.605689774872599883e-03 1.611086826773961431e-03 1.616593714237170862e-03 1.622079217544768453e-03
-1.624222132061147860e-03 1.624616097152548544e-03 1.625779827705265811e-03 1.627715532915717913e-03 1.630417257235958770e-03 1.633876281372745667e-03 1.638080722355794629e-03 1.643014990972341662e-03 1.648659081921209418e-03 1.654987660128463085e-03 1.661968896389090771e-03 1.669562975117044488e-03 1.677720175887938711e-03 1.686378372281656986e-03 1.695459718557214670e-03
-1.673863757358857313e-03 1.674360044507218178e-03 1.675810180002196541e-03 1.678226785371286995e-03 1.681609342589853980e-03 1.685956950857529823e-03 1.691268148593946504e-03 1.697540681335326252e-03 1.704771212984126753e-03 1.712954977889893883e-03 1.722085371229575227e-03 1.732153471975712367e-03 1.743147496569791809e-03 1.755052175208482489e-03 1.767848041916845678e-03
-1.721571649257314226e-03 1.722170413696109134e-03 1.723907279629990821e-03 1.726805427182696862e-03 1.730869926320061786e-03 1.736107907652344098e-03 1.742528608559642265e-03 1.750143454230455994e-03 1.758966193053722793e-03 1.769013118357117128e-03 1.780303417094997436e-03 1.792859713584412425e-03 1.806708901767612807e-03 1.821883408961924274e-03 1.838423105591144389e-03
-1.766965918331123500e-03 1.767665747761376117e-03 1.769685301744785633e-03 1.773058239783686279e-03 1.777795192330759808e-03 1.783911270147216666e-03 1.791426319805287330e-03 1.800365295551183955e-03 1.810758786174753322e-03 1.822643757640557589e-03 1.836064591008958885e-03 1.851074542646884103e-03 1.867737802937030189e-03 1.886132418766625109e-03 1.906354475134612722e-03
-1.809672056753726518e-03 1.810469976433477140e-03 1.812763824172409794e-03 1.816597440546523397e-03 1.821986821851462584e-03 1.828954760692474328e-03 1.837531281344237290e-03 1.847754258610599144e-03 1.859670272244223158e-03 1.873335778609562952e-03 1.888818704333870098e-03 1.906200629441091301e-03 1.925579788269001901e-03 1.947075228509197176e-03 1.970832627818915831e-03
-1.849326670415565388e-03 1.850218193838873166e-03 1.852773732519716809e-03 1.857046807181638804e-03 1.863058440193090647e-03 1.870838594919444322e-03 1.880426750738993687e-03 1.891872709593812050e-03 1.905237692553480222e-03 1.920595817862651719e-03 1.938036075232759010e-03 1.957664979599794963e-03 1.979610148647779552e-03 2.004025162857414610e-03 2.031096222805339746e-03
-1.885583028627639242e-03 1.886562248144303764e-03 1.889362921268414753e-03 1.894047569729277909e-03 1.900641787271190953e-03 1.909182030928746479e-03 1.919716290025430235e-03 1.932305013572191811e-03 1.947022353415392730e-03 1.963957813310643775e-03 1.983218412362030940e-03 2.004931537870078065e-03 2.029248712453247429e-03 2.056350599860823532e-03 2.086453700160030914e-03
-1.918116286151698349e-03 1.919175995725268908e-03 1.922201637365450900e-03 1.927263905987400359e-03 1.934392431655961248e-03 1.943629375209783485e-03 1.955030145659780207e-03 1.968664382348139438e-03 1.984617251285630910e-03 2.002991134740733301e-03 2.023907802176880613e-03 2.047511209539727272e-03 2.073971104238593859e-03 2.103487686473634252e-03 2.136297658746102480e-03
-1.946628260168638963e-03 1.947760101276158453e-03 1.950987344405636552e-03 1.956387912742993569e-03 1.963994892076981018e-03 1.973855297655985417e-03 1.986030799610417549e-03 2.000598702051894183e-03 2.017653212348290322e-03 2.037307060701269885e-03 2.059693528848203538e-03 2.084968992581211211e-03 2.113316091190043430e-03 2.144947678882585911e-03 2.180111746132030494e-03
-1.970851676955009003e-03 1.972046298498980176e-03 1.975449021696814699e-03 1.981143966681413182e-03 1.989167080050726483e-03 1.999569369845228314e-03 2.012417607834316152e-03 2.027795261868410841e-03 2.045803678643034682e-03 2.066563554592200716e-03 2.090216718497967495e-03 2.116928283247282959e-03 2.146889209010560944e-03 2.180319333071353491e-03 2.217470911600913277e-03
-1.990553835765599463e-03 1.991801059719903143e-03 1.995350849010493754e-03 2.001292430324060675e-03 2.009664026398335322e-03 2.020519800902447795e-03 2.033930518121115655e-03 2.049984402333661099e-03 2.068788200525908168e-03 2.090468462404398899e-03 2.115173026855511011e-03 2.143072724861307034e-03 2.174363274478474141e-03 2.209267331966561880e-03 2.248036621017933823e-03
-2.005539667162678594e-03 2.006828653334513657e-03 2.010495260631411148e-03 2.016632695138896939e-03 2.025280897255648214e-03 2.036496396697536852e-03 2.050352922584332792e-03 2.066942182080880319e-03 2.086374795888889296e-03 2.108781383012384939e-03 2.134313753331580372e-03 2.163146176715345821e-03 2.195476647991373691e-03 2.231528037794875286e-03 2.271548956073307299e-03
-2.015654186925639000e-03 2.016973592397941061e-03 2.020725378208300740e-03 2.027005582416657129e-03 2.035855337429671921e-03 2.047332805639322413e-03 2.061513744528055588e-03 2.078492213792605941e-03 2.098381400555690470e-03 2.121314538079580470e-03 2.147445765415646659e-03 2.176951476486784810e-03 2.210030202192586439e-03 2.246903918692757032e-03 2.287817487002487531e-03
-2.020784362822819393e-03 2.022122494029662126e-03 2.025926848816993631e-03 2.032295140339129575e-03 2.041269198068017786e-03 2.052908135011531458e-03 2.067288881804483624e-03 2.084506845110233389e-03 2.104676658558048575e-03 2.127932990795242639e-03 2.154431330435694052e-03 2.184348665516483955e-03 2.217883909333648231e-03 2.255257877714510542e-03 2.296712541958686061e-03
-2.020860419191701941e-03 2.022205376841533248e-03 2.026029121821792175e-03 2.032429882145843879e-03 2.041449710903682577e-03 2.053148025149760612e-03 2.067602128989530410e-03 2.084907854776172145e-03 2.105180287943673144e-03 2.128554536341000208e-03 2.155186458742850905e-03 2.185253263512038427e-03 2.218953820715789237e-03 2.256508482283080177e-03 2.298158122377806471e-03
-2.015856603889891983e-03 2.017196422797203677e-03 2.021006196141092188e-03 2.027383506202150732e-03 2.036370163913169516e-03 2.048025256414798441e-03 2.062425681233793443e-03 2.079666804795963792e-03 2.099863213498809767e-03 2.123149521922308713e-03 2.149681157958517868e-03 2.179635042471190706e-03 2.213210015355597613e-03 2.250626813054844300e-03 2.292127321764030490e-03
-2.005791435208866165e-03 2.007114222298962605e-03 2.010876860098461619e-03 2.017175126127835564e-03 2.026050115640361162e-03 2.037559939188944048e-03 2.051780287905830263e-03 2.068805140850065935e-03 2.088747590490255390e-03 2.111740761735981121e-03 2.137938671950537998e-03 2.167517580440400486e-03 2.200675871009370125e-03 2.237635360731377900e-03 2.278640740073223370e-03
-1.990727435085318762e-03 1.992021509254041350e-03 1.995704431785053513e-03 2.001869020982320786e-03 2.010555161326400830e-03 2.021819304512202566e-03 2.035735079798836264e-03 2.052394072987227727e-03 2.071906762320368817e-03 2.094403603727299380e-03 2.120036223944011828e-03 2.148978690238794245e-03 2.181428776058709929e-03 2.217609112615274471e-03 2.257768053183481765e-03
-1.970770342195867289e-03 1.972024379289131525e-03 1.975595991928352085e-03 1.981573895431500143e-03 1.989996237626753296e-03 2.000917077664311674e-03 2.014407046053391746e-03 2.030554204492317130e-03 2.049465109127868515e-03 2.071266091211314969e-03 2.096104744290768450e-03 2.124151627948849940e-03 2.155602163688488497e-03 2.190678687049116106e-03 2.229632577902079110e-03
-1.946067787259117381e-03 1.947270972233699441e-03 1.950701087003350485e-03 1.956441621655351064e-03 1.964528428582713263e-03 1.975012384385245803e-03 1.987960092599978020e-03 2.003454816621003456e-03 2.021597663152793940e-03 2.042509053911526797e-03 2.066330509157636528e-03 2.093226800487376152e-03 2.123388515153039075e-03 2.157035087136731279e-03 2.194418340266112658e-03
-1.916807405905087509e-03 1.917949592384575377e-03 1.921209870900817719e-03 1.926665422113979769e-03 1.934349217929998187e-03 1.944308114701408588e-03 1.956603579187025932e-03 1.971312668338312014e-03 1.988529299408615253e-03 2.008365870508461992e-03 2.030955290424822732e-03 2.056453522392483624e-03 2.085042754919108621e-03 2.116935354711625868e-03 2.152378789647286725e-03
-1.883214364078713600e-03 1.884286239258943160e-03 1.887350651482812671e-03 1.892477448182766989e-03 1.899696125400118004e-03 1.909048656976860062e-03 1.920590212587321892e-03 1.934390140706961298e-03 1.950533265932545470e-03 1.969121579723994830e-03 1.990276412657982028e-03 2.014141235191183477e-03 2.040885264271593419e-03 2.070708126439874293e-03 2.103845909254500705e-03
-1.845548278614837388e-03 1.846541529083474669e-03 1.849386815531936859e-03 1.854145716148014123e-03 1.860843669966138819e-03 1.869516918162874176e-03 1.880213173787014663e-03 1.892992550094494937e-03 1.907928804832820539e-03 1.925110990646815290e-03 1.944645620040722379e-03 1.966659519932477222e-03 1.991303600659522811e-03 2.018757863844301143e-03 2.049238099795281515e-03
-1.804099531761965821e-03 1.805007003615737449e-03 1.807613122505003769e-03 1.811970379883382333e-03 1.818099622092930008e-03 1.826030566900103871e-03 1.835802379345589756e-03 1.847464479362165030e-03 1.861077639633489014e-03 1.876715465159661594e-03 1.894466369284661693e-03 1.914436229399032368e-03 1.936751966611542771e-03 1.961566408137799689e-03 1.989064947124056289e-03
-1.759185002327844213e-03 1.760000847309334086e-03 1.762351383389695750e-03 1.766279347976510610e-03 1.771800539303823195e-03 1.778937473635091400e-03 1.787719821562774305e-03 1.798185028070422827e-03 1.810379168411896823e-03 1.824358121485556740e-03 1.840189165441805759e-03 1.857953163009741851e-03 1.877747564836161273e-03 1.899690571164470423e-03 1.923926951246277125e-03
-1.711143265856406373e-03 1.711863064382343307e-03 1.713945573771701730e-03 1.717423289864138157e-03 1.722306622206089656e-03 1.728610373345002265e-03 1.736353995381663753e-03 1.745561963176420423e-03 1.756264302849554464e-03 1.768497336324611991e-03 1.782304721435648380e-03 1.797738914589028757e-03 1.814863232179411440e-03 1.833754776028884972e-03 1.854508618055040027e-03
-1.660329348971716209e-03 1.660950201058331022e-03 1.662756466726253825e-03 1.665770117008214110e-03 1.669995977214895014e-03 1.675440836609340661e-03 1.682113495697179538e-03 1.690024848755202879e-03 1.699188021032658601e-03 1.709618592611307237e-03 1.721334949519361503e-03 1.734358830187784483e-03 1.748716160717489433e-03 1.764438321904596629e-03 1.781564062303676779e-03
-1.607109155181324182e-03 1.607629731463947314e-03 1.609155907342714551e-03 1.611699066649055273e-03 1.615258421951132296e-03 1.619832696568901820e-03 1.625419947854159870e-03 1.632017336730821541e-03 1.639620840940176705e-03 1.648224909462619146e-03 1.657822055574659226e-03 1.668402382819162257e-03 1.679953041994911760e-03 1.692457611058567537e-03 1.705895388812125749e-03
-1.551853707293184264e-03 1.552274254496153073e-03 1.553520882266885058e-03 1.555594552190912123e-03 1.558489013454915275e-03 1.562195134810233886e-03 1.566700506050904820e-03 1.571988897252345630e-03 1.578039551116204153e-03 1.584826271856277840e-03 1.592316263779455397e-03 1.600468642333162427e-03 1.609232519290833361e-03 1.618544505540280400e-03 1.628325401803409683e-03
-1.494933371704918737e-03 1.495255669824021357e-03 1.496227560621062307e-03 1.497839971017554932e-03 1.500081512080902535e-03 1.502935670759257113e-03 1.506380208777550675e-03 1.510386339352835826e-03 1.514917637586363653e-03 1.519928619303704490e-03 1.525362903135399741e-03 1.531150819129831891e-03 1.537206286707214122e-03 1.543422685752415596e-03 1.549667319410873633e-03
-1.436712239518824841e-03 1.436939511304332348e-03 1.437645493957037147e-03 1.438811673974016046e-03 1.440422010645720429e-03 1.442453320745515225e-03 1.444874509086591964e-03 1.447645512256516944e-03 1.450715897297258404e-03 1.454023029489721246e-03 1.457489698474857993e-03 1.461021025323274792e-03 1.464500425269550351e-03 1.467784278220837834e-03 1.470694812369525420e-03
-1.377542837235524661e-03 1.377679613915289408e-03 1.378132160793373419e-03 1.378873298789222174e-03 1.379882956549467266e-03 1.381132191197253318e-03 1.382582295899973182e-03 1.384183576167301137e-03 1.385873729204013935e-03 1.387575730228747528e-03 1.389195104292300677e-03 1.390616389443650623e-03 1.391698552625942427e-03 1.392268994269549613e-03 1.392115640647335071e-03
-1.317761325589869928e-03 1.317813275760601347e-03 1.318028025705189881e-03 1.318370652156215230e-03 1.318817774151089276e-03 1.319335745458521990e-03 1.319879690804966763e-03 1.320392188792774259e-03 1.320801535357347132e-03 1.321019492105433108e-03 1.320938401801264586e-03 1.320427483861510423e-03 1.319328089728315093e-03 1.317447588154422103e-03 1.314551447331831040e-03
-1.257683320184494477e-03 1.257657051103659197e-03 1.257652255382961685e-03 1.257627294238009051e-03 1.257556258038178667e-03 1.257401938737838553e-03 1.257114847491131024e-03 1.256631878975900986e-03 1.255874561901204741e-03 1.254746810700376781e-03 1.253132073410955817e-03 1.250889719710844344e-03 1.247850486196950322e-03 1.243810722486782564e-03 1.238525116661686257e-03
-1.197600434397629249e-03 1.197503276306121148e-03 1.197299197426441924e-03 1.196940938000089346e-03 1.196400859370603349e-03 1.195639356553527231e-03 1.194603906256878163e-03 1.193227781162324976e-03 1.191428380339047601e-03 1.189105107748022073e-03 1.186136715755305030e-03 1.182377999025047447e-03 1.177655665185452834e-03 1.171763516009717522e-03 1.164455844788313092e-03
-1.137777606807366046e-03 1.137617391321166065e-03 1.137235686672057001e-03 1.136580728797407505e-03 1.135623932748514378e-03 1.134324426012956388e-03 1.132628173789673514e-03 1.130466799170929196e-03 1.127756068758447010e-03 1.124393995098857272e-03 1.120258498248184525e-03 1.115204559406922976e-03 1.109060787617758594e-03 1.101625326583991361e-03 1.092661025967496145e-03
-1.078451235604399290e-03 1.078236078682947956e-03 1.077699193033307976e-03 1.076785421604202963e-03 1.075465955867025347e-03 1.073699703801068647e-03 1.071432518576588989e-03 1.068596167982054047e-03 1.065107029027065073e-03 1.060864479841421059e-03 1.055748957704735411e-03 1.049619659789875628e-03 1.042311855615757907e-03 1.033633818950223555e-03 1.023363396283954877e-03
-1.019828104536592674e-03 1.019566203215448337e-03 1.018896805443319066e-03 1.017762428523536714e-03 1.016134683758807737e-03 1.013973186286451587e-03 1.011224903022049084e-03 1.007823298702722201e-03 1.003687270793935304e-03 9.987198651245274804e-04 9.928067653396685337e-04 9.858145682363746252e-04 9.775888541349534583e-04 9.679521172606573524e-04 9.567016415238794973e-04
-9.620850516426729957e-04 9.617845018533785484e-04 9.610049803238944390e-04 9.596876712287806489e-04 9.578051576341384309e-04 9.553185403094160543e-04 9.521769201413899470e-04 9.483167310409493928e-04 9.436609256758515373e-04 9.381180211776421517e-04 9.315810185546584713e-04 9.239262302301885820e-04 9.150120602441577395e-04 9.046778294481945884e-04 8.927427771850545649e-04
-9.053693054086738804e-04 9.050379460414595010e-04 9.041699723338392268e-04 9.027061439579851538e-04 9.006204575929677289e-04 8.978761204922604093e-04 8.944251680311189829e-04 8.902079816905769834e-04 8.851527188049897578e-04 8.791746725024526333e-04 8.721755906506078408e-04 8.640430005770801530e-04 8.546496090723368052e-04 8.438528764799577012e-04 8.314949193207842168e-04
-8.497993940898093288e-04 8.494446802417765160e-04 8.485088581960423216e-04 8.469330735810046964e-04 8.446930695156063635e-04 8.417546206610132574e-04 8.380732789082404131e-04 8.335940644548863084e-04 8.282511197393107065e-04 8.219673520015179395e-04 8.146541022904140372e-04 8.062108925005591559e-04 7.965253352310837451e-04 7.854732931066957810e-04 7.729194544071608291e-04
-7.954665230042112182e-04 7.950954293017368493e-04 7.941110266100921819e-04 7.924555538746014174e-04 7.901067287194884527e-04 7.870332020010236806e-04 7.831944190218434508e-04 7.785404646656672546e-04 7.730119131062580199e-04 7.665397118268190606e-04 7.590451410440107478e-04 7.504399016431731982e-04 7.406264161180226143e-04 7.294984192464360438e-04 7.169419933516427146e-04
-7.424363110640048134e-04 7.420552642031228493e-04 7.410400250195011123e-04 7.393345304352662599e-04 7.369186048997567297e-04 7.337639464667524260e-04 7.298340876400088084e-04 7.250843711711511862e-04 7.194619627536875516e-04 7.129059311365471040e-04 7.053474359190020073e-04 6.967100757745934301e-04 6.869104672987653244e-04 6.758591310557412460e-04 6.634618054990986920e-04
-6.907507806086690249e-04 6.903656189020747390e-04 6.893356511725398390e-04 6.876070189156834912e-04 6.851617020590673431e-04 6.819744978334363805e-04 6.780130636140720059e-04 6.732379984513303271e-04 6.676029848135132862e-04 6.610550196156128643e-04 6.535347713469783631e-04 6.449771131345744370e-04 6.353118823230551699e-04 6.244649475013102973e-04 6.123596564961263783e-04
-6.404305023389528706e-04 6.400464591139161732e-04 6.390161877883018988e-04 6.372884506734806994e-04 6.348473619586192341e-04 6.316707717250103675e-04 6.277303729845899998e-04 6.229918644088555148e-04 6.174151885794727400e-04 6.109548719647605198e-04 6.035604985275023213e-04 5.951773612377977149e-04 5.857473255083037568e-04 5.752099813500763164e-04 5.635041223529441189e-04
-5.914768083434077941e-04 5.910985155034153161e-04 5.900806913086614541e-04 5.883750545250177781e-04 5.859677767408342586e-04 5.828396372671271241e-04 5.789661775589388919e-04 5.743179223866309120e-04 5.688606851677967648e-04 5.625559799583659294e-04 5.553615666289822171e-04 5.472321658068702221e-04 5.381203668995364732e-04 5.279777921317748909e-04 5.167565359090661985e-04
-5.438739994238936349e-04 5.435055072816418311e-04 5.425112602468710066e-04 5.408461994402817725e-04 5.384984350463658956e-04 5.354514946564217738e-04 5.316845099706622030e-04 5.271724763472063766e-04 5.218865998337880513e-04 5.157947501279653603e-04 5.088620409363449251e-04 5.010515654288314391e-04 4.923253039941393773e-04 4.826452488971144780e-04 4.719747587418391646e-04
-4.975914869242597290e-04 4.972362964928813203e-04 4.962752236625273157e-04 4.946666393114258981e-04 4.924004439931790704e-04 4.894626932960435915e-04 4.858358038910168502e-04 4.814988344166489117e-04 4.764278533685720120e-04 4.705964078518263052e-04 4.639761118750245481e-04 4.565373682031870391e-04 4.482502459709036650e-04 4.390855333596682003e-04 4.290159773036692913e-04
-4.525858230454243261e-04 4.522469272582233901e-04 4.513272048257518563e-04 4.497886163377565042e-04 4.476226860108765276e-04 4.448177533640526398e-04 4.413591878548896847e-04 4.372296775070613284e-04 4.324096009525286522e-04 4.268774929043003146e-04 4.206106193914537351e-04 4.135856636984008221e-04 4.057795526260579710e-04 3.971704183928681693e-04 3.877387095157515374e-04
-4.088025864557237664e-04 4.084825171777391618e-04 4.076110284148096738e-04 4.061537962157800745e-04 4.041037841003404865e-04 4.014513688180819124e-04 3.981845273340137441e-04 3.942891364484272967e-04 3.897493336754723962e-04 3.845479656923953557e-04 3.786671346584129043e-04 3.720888360630756155e-04 3.647957187680574490e-04 3.567719481456676405e-04 3.480041862101205218e-04
-3.661781014089101759e-04 3.658789795868573592e-04 3.650614512606466006e-04 3.636949979930803383e-04 3.617738612968255480e-04 3.592901827011771147e-04 3.562342122291575655e-04 3.525945834125655104e-04 3.483586594824245627e-04 3.435129554201575672e-04 3.380436449638378731e-04 3.319371443429771089e-04 3.251807968642220150e-04 3.177636375810780349e-04 3.096772468923459330e-04
-3.246409782942680320e-04 3.243645650778387421e-04 3.236057064104186343e-04 3.223377690481936311e-04 3.205560899229093950e-04 3.182543348859602364e-04 3.154246963277513942e-04 3.120581519428746635e-04 3.081447874923173911e-04 3.036741867267053123e-04 2.986358927397488820e-04 2.930199352208979514e-04 2.868174373231752064e-04 2.800212851456496945e-04 2.726268631367378525e-04
-2.841134715040255563e-04 2.838612186431061142e-04 2.831648581724067549e-04 2.820017078697979198e-04 2.803680337459021465e-04 2.782587897622083536e-04 2.756678015377665540e-04 2.725880053521371766e-04 2.690117436651322312e-04 2.649311210802703098e-04 2.603384145864280543e-04 2.552265477837587816e-04 2.495896195977851729e-04 2.434234854189369157e-04 2.367263845588781055e-04
-2.445126567533678955e-04 2.442857550077232346e-04 2.436549718963621587e-04 2.426016376098950075e-04 2.411227916665758815e-04 2.392144562526556280e-04 2.368718042037406993e-04 2.340893763286715278e-04 2.308613479053047281e-04 2.271818496554213972e-04 2.230453272386655303e-04 2.184469634061331786e-04 2.133831338422876082e-04 2.078519070475758827e-04 2.018535754700970784e-04
-2.057514346839375288e-04 2.055508593539987503e-04 2.049881067211617165e-04 2.040485820436908546e-04 2.027299553395512993e-04 2.010291157159254782e-04 1.989423227816309529e-04 1.964654015708122714e-04 1.935939800541375505e-04 1.903237736254135952e-04 1.866508999053671130e-04 1.825722468359384208e-04 1.780858647206217131e-04 1.731913919432377961e-04 1.678905015707670638e-04
-1.677393709016404566e-04 1.675659239060235716e-04 1.670731426194220547e-04 1.662505761396521834e-04 1.650963954831956640e-04 1.636081750395667266e-04 1.617830272963269615e-04 1.596177755249909055e-04 1.571091631101663541e-04 1.542541024367952293e-04 1.510499488591195822e-04 1.474948176990055059e-04 1.435879192005602646e-04 1.393299183989850289e-04 1.347233083924795263e-04
-1.303833847869339255e-04 1.302377329604582034e-04 1.298164550147091979e-04 1.291133228796028103e-04 1.281268928697863253e-04 1.268552628879221695e-04 1.252961908583286000e-04 1.234472459478354474e-04 1.213059912462056055e-04 1.188701982495401078e-04 1.161380851384717308e-04 1.131085852862748106e-04 1.097816323532422905e-04 1.061584621964546481e-04 1.022419230582611731e-04
-9.358830066280916956e-05 9.347101014423866636e-05 9.312245128547386847e-05 9.254071151545681438e-05 9.172463037113417540e-05 9.067268694515995080e-05 8.938310276337222836e-05 8.785397229974948935e-05 8.608342270266527855e-05 8.406979260404763208e-05 8.181184167578380408e-05 7.930897381346432200e-05 7.656147842419969911e-05 7.357078202165191836e-05 7.033970448719742473e-05
-5.725727544112534307e-05 5.716884216268585273e-05 5.689398381046474726e-05 5.643521255392407122e-05 5.579156336524751362e-05 5.496176932857888778e-05 5.394436149864236484e-05 5.273776844719843835e-05 5.134046061299682039e-05 4.975109601418239557e-05 4.796870204775234212e-05 4.599286041134816294e-05 4.382390880331946831e-05 4.146314924551418725e-05 3.891305848935310924e-05
-2.129211686649679818e-05 2.123299325439570597e-05 2.103265404360041472e-05 2.069816439181894829e-05 2.022867587449354526e-05 1.962307633579908625e-05 1.888006453276198953e-05 1.799824381183061798e-05 1.697623917972999175e-05 1.581281930068229749e-05 1.450704933154879147e-05 1.305844391088600200e-05 1.146713387985012340e-05 9.734037234630945170e-06 7.861030643460562391e-06
--1.440649389465464988e-05 -1.443587583953417143e-05 -1.456097840369679018e-05 -1.477003415183902165e-05 -1.506383860549017611e-05 -1.544344250763266961e-05 -1.591008977484926562e-05 -1.646513967851507423e-05 -1.710997046960057008e-05 -1.784587771192213410e-05 -1.867394957512224718e-05 -1.959494103497409529e-05 -2.060913799107734769e-05 -2.171621851051804296e-05 -2.291511441405959997e-05
--4.993886218580856926e-05 -4.993807122629218665e-05 -4.998726841844141890e-05 -5.006981201852406076e-05 -5.018649865969006843e-05 -5.033839240359135557e-05 -5.052677434495561214e-05 -5.075307912515162809e-05 -5.101881875943348025e-05 -5.132549679816863044e-05 -5.167451150356616740e-05 -5.206705289335755553e-05 -5.250399421297087733e-05 -5.298578110360325420e-05 -5.351232143559763344e-05
--8.540620991632370525e-05 -8.537479913057319692e-05 -8.534742735364915338e-05 -8.530238235257302834e-05 -8.524050580114665699e-05 -8.516293579491766613e-05 -8.507106728196758057e-05 -8.496650218660608731e-05 -8.485099002423287119e-05 -8.472636003168834251e-05 -8.459444608352319846e-05 -8.445700593336045981e-05 -8.431563659504478039e-05 -8.417168796051261793e-05 -8.402617701758739472e-05
--1.209106641247415350e-04 -1.208481574785967376e-04 -1.207435227302769572e-04 -1.205697556782260257e-04 -1.203277775530263075e-04 -1.200188481634777398e-04 -1.196445370974342311e-04 -1.192066835515699440e-04 -1.187073583229396930e-04 -1.181488071321545500e-04 -1.175333977856873793e-04 -1.168635593509887403e-04 -1.161417189790768479e-04 -1.153702372764369035e-04 -1.145513439316296037e-04
--1.565552931869003839e-04 -1.564611749615053989e-04 -1.562785249007092527e-04 -1.559747991527104453e-04 -1.555510241587658373e-04 -1.550086165512229355e-04 -1.543493660843369938e-04 -1.535754022287723764e-04 -1.526891779206906194e-04 -1.516934234566749164e-04 -1.505911139146826950e-04 -1.493854269728713186e-04 -1.480796994452694606e-04 -1.466773824614752829e-04 -1.451819963618798605e-04
--1.924441804774647627e-04 -1.923178874260749079e-04 -1.920563906143199614e-04 -1.916213319951874726e-04 -1.910138604166166396e-04 -1.902355729499097356e-04 -1.892885095051310594e-04 -1.881751272032365847e-04 -1.868983007577532140e-04 -1.854612917905097962e-04 -1.838677327090856991e-04 -1.821216028743003271e-04 -1.802272037677303442e-04 -1.781891327570095797e-04 -1.760122559122367361e-04
--2.286825258493162564e-04 -2.285234420042491269e-04 -2.281821740092853659e-04 -2.276142478082074730e-04 -2.268209436347389787e-04 -2.258040528480134224e-04 -2.245658769211920491e-04 -2.231092252898448118e-04 -2.214374140849688973e-04 -2.195542619824468911e-04 -2.174640866034459894e-04 -2.151716991230857075e-04 -2.126823976298154479e-04 -2.100019589617819690e-04 -2.071366288614144840e-04
--2.653767657021930044e-04 -2.651842198079255647e-04 -2.647621559844883302e-04 -2.640596549626567828e-04 -2.630781291883877208e-04 -2.618195647629449011e-04 -2.602865297397267833e-04 -2.584821842514476863e-04 -2.564102920689146194e-04 -2.540752331115198699e-04 -2.514820163513785596e-04 -2.486362924860387484e-04 -2.455443656913148414e-04 -2.422132037165570986e-04 -2.386504455461522730e-04
--3.026347026527138212e-04 -3.024079682576613659e-04 -3.019039831593902843e-04 -3.010650264873046913e-04 -2.998926354531397144e-04 -2.983889808376167098e-04 -2.965568850579353719e-04 -2.943998445152318732e-04 -2.919220555610738230e-04 -2.891284432767083495e-04 -2.860246921161341640e-04 -2.826172773308741211e-04 -2.789134959670344681e-04 -2.749214961161055735e-04 -2.706503030087387520e-04
--3.405656358729197784e-04 -3.403039341765055990e-04 -3.397168076985176044e-04 -3.387393509855280869e-04 -3.373732099848444780e-04 -3.356207184348479781e-04 -3.334849256264767734e-04 -3.309696330567160117e-04 -3.280794343956229347e-04 -3.248197622845066298e-04 -3.211969378259900356e-04 -3.172182221473385808e-04 -3.128918681579036221e-04 -3.082271705795121600e-04 -3.032345121767072321e-04
--3.792804830288493004e-04 -3.789829886453808237e-04 -3.783114191474921495e-04 -3.771932759785042691e-04 -3.756302887037898312e-04 -3.736249207348329125e-04 -3.711804018027124469e-04 -3.683007929494976291e-04 -3.649910265246985642e-04 -3.612569824697356240e-04 -3.571055550671475495e-04 -3.525447271002323901e-04 -3.475836968448229431e-04 -3.422326899185270245e-04 -3.365035508570878497e-04
--4.188918844168176793e-04 -4.185577342820372571e-04 -4.178003590951156945e-04 -4.165392347458680934e-04 -4.147761395169799470e-04 -4.125136169012959286e-04 -4.097550228605415673e-04 -4.065046017838037473e-04 -4.027675480206621087e-04 -3.985501026247815137e-04 -3.938596425503853335e-04 -3.887047798184187935e-04 -3.830954621296316174e-04 -3.770430724053608156e-04 -3.705605237311815001e-04
--4.595142793559646357e-04 -4.591425850709772373e-04 -4.582980089399200886e-04 -4.568915471969563799e-04 -4.549249812746170062e-04 -4.524008719790186049e-04 -4.493226247888072711e-04 -4.456945716332864470e-04 -4.415220674660448683e-04 -4.368115995259932516e-04 -4.315709067330638932e-04 -4.258091062119345131e-04 -4.195368234750252324e-04 -4.127663223503715592e-04 -4.055116303242210958e-04
--5.012639441614780058e-04 -5.008538081328215092e-04 -4.999206402967601090e-04 -4.983664845571156559e-04 -4.961930682003514240e-04 -4.934028913321119496e-04 -4.899993071128970392e-04 -4.859866224864585840e-04 -4.813702175002875362e-04 -4.761566808177299776e-04 -4.703539584867845306e-04 -4.639715124727101354e-04 -4.570204848820745265e-04 -4.495138632334048055e-04 -4.414666415697609180e-04
--5.442589800938005436e-04 -5.438095158905484035e-04 -5.427864166390079792e-04 -5.410822866992421676e-04 -5.386987289647661523e-04 -5.356380860798680161e-04 -5.319035372441061017e-04 -5.274992200518876942e-04 -5.224303752887318915e-04 -5.167035120298511114e-04 -5.103265897568262394e-04 -5.033092135337492376e-04 -4.956628375701258981e-04 -4.874009717585456769e-04 -4.785393850808696372e-04
--5.886192385693523937e-04 -5.881295959732968153e-04 -5.870153336397407025e-04 -5.851591197961146778e-04 -5.825623483873710456e-04 -5.792270879159231063e-04 -5.751561965789818865e-04 -5.703534672463978286e-04 -5.648238024018151270e-04 -5.585734092369503507e-04 -5.516100229260051824e-04 -5.439431420960855147e-04 -5.355842782017480701e-04 -5.265472103000765460e-04 -5.168482385094203121e-04
--6.344661696494730517e-04 -6.339355649224986131e-04 -6.327290843774149463e-04 -6.307189606341019432e-04 -6.279062783715145483e-04 -6.242926932509107029e-04 -6.198805672233925583e-04 -6.146731390337669635e-04 -6.086747330290789718e-04 -6.018909872944546314e-04 -5.943291240451338596e-04 -5.859982308447088091e-04 -5.769095628613299344e-04 -5.670768539851009675e-04 -5.565166293829145556e-04
--6.819225784336617078e-04 -6.813503303535968546e-04 -6.800508341255804244e-04 -6.778853924309073556e-04 -6.748546649602350008e-04 -6.709597260826539056e-04 -6.662022406621802501e-04 -6.605846449839621569e-04 -6.541103975746718167e-04 -6.467842516681973153e-04 -6.386125691735295871e-04 -6.296036585785717322e-04 -6.197681370577810649e-04 -6.091193070542233901e-04 -5.976735384737868898e-04
--7.311122725026151072e-04 -7.304978447329681275e-04 -7.291048879068468469e-04 -7.267832953843212209e-04 -7.235331622360491929e-04 -7.193548023142451626e-04 -7.142489328471018743e-04 -7.082169014931267948e-04 -7.012609664811268913e-04 -6.933846195857863368e-04 -6.845929507172723036e-04 -6.748930487183934460e-04 -6.642944320610983311e-04 -6.528095011030007454e-04 -6.404540019631474630e-04
--7.821595820709651477e-04 -7.815026324079914254e-04 -7.800162324054497236e-04 -7.775384134916331130e-04 -7.740685509265831515e-04 -7.696059770242715198e-04 -7.641501873066571708e-04 -7.577011041697526324e-04 -7.502593965123272859e-04 -7.418268535447785934e-04 -7.324068078805063154e-04 -7.220046057083175355e-04 -7.106281150630812827e-04 -6.982882651245625287e-04 -6.849996053035431205e-04
--8.351887330872352850e-04 -8.344891700721811635e-04 -8.329099322939132431e-04 -8.302767775035648033e-04 -8.265881840920346474e-04 -8.218422541087995773e-04 -8.160369455416287363e-04 -8.091703706267402421e-04 -8.012411590010413455e-04 -7.922488870294244756e-04 -7.821945619801649310e-04 -7.710811714269939776e-04 -7.589142771623846959e-04 -7.457026539097435158e-04 -7.314589585507302611e-04
--8.903230522855976655e-04 -8.895810995613590141e-04 -8.879103596352793488e-04 -8.851239623065860086e-04 -8.812192899661812004e-04 -8.761929356067623418e-04 -8.700409615182904278e-04 -8.627592330434914573e-04 -8.543438270260163845e-04 -8.447915188076727221e-04 -8.341003334305695585e-04 -8.222701794998691239e-04 -8.093035388493397550e-04 -7.952062170328867956e-04 -7.799881388578919954e-04
--9.476839822867323682e-04 -9.469002509115904184e-04 -9.451402339229999150e-04 -9.422041557060750749e-04 -9.380880818218641790e-04 -9.327867860092501013e-04 -9.262940346080502903e-04 -9.186029553784550838e-04 -9.097064921006325217e-04 -8.995979480014934136e-04 -8.882716126521933474e-04 -8.757234804300150161e-04 -8.619520473457685040e-04 -8.469591852288912461e-04 -8.307510805981591301e-04
--1.007389884455910448e-03 -1.006565453138834896e-03 -1.004719449686087901e-03 -1.001639014675363920e-03 -9.973186552056300617e-04 -9.917509850846573018e-04 -9.849270329767973158e-04 -9.768366442906041818e-04 -9.674689802627237231e-04 -9.568131176593533318e-04 -9.448587519671319259e-04 -9.315970045375699098e-04 -9.170213337046479677e-04 -9.011285441597137718e-04 -8.839198862428168093e-04
--1.069554607558354008e-03 -1.068691110448379044e-03 -1.066763668640156350e-03 -1.063546284864507049e-03 -1.059031647384112889e-03 -1.053209841433969422e-03 -1.046068677391802414e-03 -1.037594121595960921e-03 -1.027770835545356977e-03 -1.016582829727048169e-03 -1.004014239632450289e-03 -9.900502228347575050e-04 -9.746779898046232116e-04 -9.578879571373759066e-04 -9.396750233618949427e-04
--1.134285801579867437e-03 -1.133385522802311850e-03 -1.131382654363903128e-03 -1.128038159785132869e-03 -1.123342632917214996e-03 -1.117283238380155407e-03 -1.109844053936129022e-03 -1.101006523378989096e-03 -1.090750028567656410e-03 -1.079052590198042831e-03 -1.065891710746070739e-03 -1.051245358089994203e-03 -1.035093116147835874e-03 -1.017417488068149758e-03 -9.982053610168985062e-04
--1.201682958682963234e-03 -1.200748932265083670e-03 -1.198678329726648659e-03 -1.195219360039624602e-03 -1.190360230859069824e-03 -1.184084784221481335e-03 -1.176372823550059492e-03 -1.167200588964102713e-03 -1.156541348806715795e-03 -1.144366135611977553e-03 -1.130644642915390723e-03 -1.115346289528628852e-03 -1.098441480597588116e-03 -1.079903062432074597e-03 -1.059707984343815019e-03
--1.271835167474458586e-03 -1.270871280634071777e-03 -1.268742541122806723e-03 -1.265184899372944101e-03 -1.260183901826850182e-03 -1.253719640735453771e-03 -1.245767096894664439e-03 -1.236296602151785474e-03 -1.225274438166922388e-03 -1.212663589988720531e-03 -1.198424677567156045e-03 -1.182517085066410846e-03 -1.164900315998644532e-03 -1.145535591838696150e-03 -1.124387711431283155e-03
--1.344818572892437277e-03 -1.343829669880021189e-03 -1.341654519337922343e-03 -1.338017569077234927e-03 -1.332901417849748126e-03 -1.326282007572661707e-03 -1.318128945945298879e-03 -1.308405948240874391e-03 -1.297071419077197758e-03 -1.284079198536280768e-03 -1.269379501610872147e-03 -1.252920085064399783e-03 -1.234647670427835601e-03 -1.214509665473686691e-03 -1.192456210609862174e-03
--1.420693542402156175e-03 -1.419685525204001557e-03 -1.417478034933622412e-03 -1.413785061107470297e-03 -1.408585994971531339e-03 -1.401852246374848780e-03 -1.393547528027137827e-03 -1.383628253439327278e-03 -1.372044072996906044e-03 -1.358738579333587573e-03 -1.343650218377425137e-03 -1.326713452014011488e-03 -1.307860210393880151e-03 -1.287021697826915565e-03 -1.264130595178342619e-03
--1.499501550082235493e-03 -1.498481471343512039e-03 -1.496258256714525165e-03 -1.492536809207093730e-03 -1.487293088485807649e-03 -1.480493637445637767e-03 -1.472095806612550928e-03 -1.462048079714714727e-03 -1.450290529023696940e-03 -1.436755437659481853e-03 -1.421368133600149934e-03 -1.404048092545703060e-03 -1.384710362227506821e-03 -1.363267394087839873e-03 -1.339631342525186581e-03
--1.581261803762250805e-03 -1.580237946324214915e-03 -1.578018335364547156e-03 -1.574300521914796585e-03 -1.569056863852237886e-03 -1.562248774957377588e-03 -1.553826864718202546e-03 -1.543731158568221714e-03 -1.531891430594953208e-03 -1.518227691295224221e-03 -1.502650883228551400e-03 -1.485063852053462733e-03 -1.465362664448669697e-03 -1.443438377866935237e-03 -1.419179349238618073e-03
--1.665967656658892161e-03 -1.664949593199806102e-03 -1.662755750806508680e-03 -1.659078457368157048e-03 -1.653886373082594577e-03 -1.647135622615083714e-03 -1.638769823187089881e-03 -1.628720162707499117e-03 -1.616905562088327350e-03 -1.603232968250078863e-03 -1.587597837397983257e-03 -1.569884885022253956e-03 -1.549969194619074979e-03 -1.527717804611506162e-03 -1.502991902347276289e-03
--1.753582863751015431e-03 -1.752581489276319997e-03 -1.750438481131449996e-03 -1.746843492653804997e-03 -1.741761486824598302e-03 -1.735143273516521686e-03 -1.726925397633922998e-03 -1.717030036098465611e-03 -1.705364937867261945e-03 -1.691823454962842858e-03 -1.676284728137798210e-03 -1.658614109354020292e-03 -1.638663933671058275e-03 -1.616274767311503624e-03 -1.591277313444451917e-03
--1.844037763956353016e-03 -1.843065293419792220e-03 -1.841001072651173368e-03 -1.837535065257331823e-03 -1.832628656337210050e-03 -1.826227482955346650e-03 -1.818261154820616883e-03 -1.808642931182912524e-03 -1.797269385340821094e-03 -1.784020102628733947e-03 -1.768757475185557060e-03 -1.751326676969032145e-03 -1.731555944887457846e-03 -1.709257301041702684e-03 -1.684227938450933880e-03
--1.937225491189089937e-03 -1.936295414482402163e-03 -1.934340713973852150e-03 -1.931055089016733535e-03 -1.926396606482861035e-03 -1.920306072547732675e-03 -1.912706561654660192e-03 -1.903502837564323077e-03 -1.892580691985063261e-03 -1.879806239542618522e-03 -1.865025226031607683e-03 -1.848062428078338110e-03 -1.828721271284844798e-03 -1.806783808272561034e-03 -1.782011299018774596e-03
--2.032998339367835753e-03 -2.032125326437783566e-03 -2.030313440786996482e-03 -2.027263972835591666e-03 -2.022932089558264306e-03 -2.017254336607579492e-03 -2.010147957176524128e-03 -2.001510028934971354e-03 -1.991216434443239276e-03 -1.979120691197210589e-03 -1.965052683160049482e-03 -1.948817360779776754e-03 -1.930193515303219335e-03 -1.908932773833564621e-03 -1.884759045952897911e-03
--2.131164426793603125e-03 -2.130364176854517618e-03 -2.128730620592202312e-03 -2.125976895571570369e-03 -2.122055858924796166e-03 -2.116900615657534186e-03 -2.110423618267582690e-03 -2.102515503193634009e-03 -2.093043665126807090e-03 -2.081850576590440430e-03 -2.068751870676508939e-03 -2.053534230827320888e-03 -2.035953155904061864e-03 -2.015730728047885299e-03 -1.992553578916056358e-03
--2.231484822044141683e-03 -2.230773852847447308e-03 -2.229355885882705005e-03 -2.226960512772907519e-03 -2.223539047802159437e-03 -2.219022234811946111e-03 -2.213319130758558979e-03 -2.206315642011486000e-03 -2.197872695911907981e-03 -2.187824030468876659e-03 -2.175973587036190808e-03 -2.162092514073354205e-03 -2.145915792346784947e-03 -2.127138562897038215e-03 -2.105412282496987256e-03
--2.333671304410873081e-03 -2.333066680339170376e-03 -2.331902698764937686e-03 -2.329930287628518681e-03 -2.327100160401359211e-03 -2.323342033135501663e-03 -2.318563315356633216e-03 -2.312647366360071326e-03 -2.305451285158477154e-03 -2.296803186614151254e-03 -2.286498908855453659e-03 -2.274298108417641302e-03 -2.259919683420944826e-03 -2.243036520149213099e-03 -2.223269579998095932e-03
--2.437384934659943964e-03 -2.436903935963018707e-03 -2.436032728205469317e-03 -2.434548646704651122e-03 -2.432402895254436731e-03 -2.429525729878097718e-03 -2.425824987415486217e-03 -2.421184107830918943e-03 -2.415459596558183503e-03 -2.408477847125298308e-03 -2.400031226900128847e-03 -2.389873317712804240e-03 -2.377713171126913470e-03 -2.363208455516487266e-03 -2.345957361278720558e-03
--2.542235604436069232e-03 -2.541895344046318089e-03 -2.541355236415348585e-03 -2.540424157871644904e-03 -2.539055021507415771e-03 -2.537180380219512116e-03 -2.534710845295354894e-03 -2.531532944571841717e-03 -2.527506346184033807e-03 -2.522460336885017085e-03 -2.516189416736799422e-03 -2.508447832681126328e-03 -2.498942825766979191e-03 -2.487326331174834725e-03 -2.473184812083767652e-03
--2.647782713377485990e-03 -2.647599712136925430e-03 -2.647427617851620934e-03 -2.647111910819773938e-03 -2.646608514165183466e-03 -2.645854162465774775e-03 -2.644764777923467799e-03 -2.643233257116491767e-03 -2.641126578503563346e-03 -2.638282094047505501e-03 -2.634502832450357716e-03 -2.629551573595349107e-03 -2.623143390422552450e-03 -2.614936260117641832e-03 -2.604519228732301347e-03
--2.753537091262175680e-03 -2.753526826649646368e-03 -2.753757236822049724e-03 -2.754115248174647188e-03 -2.754561121949290498e-03 -2.755037707041100258e-03 -2.755468852918205747e-03 -2.755757235410323351e-03 -2.755781497220940318e-03 -2.755392551110606974e-03 -2.754408852274647414e-03 -2.752610354710321398e-03 -2.749730790274934177e-03 -2.745447762285934280e-03 -2.739369967381878775e-03
--2.858964238686594224e-03 -2.859140685779366919e-03 -2.859804641850520295e-03 -2.860888947291428692e-03 -2.862359490587128730e-03 -2.864167123376801759e-03 -2.866246188950510431e-03 -2.868512508048242076e-03 -2.870860717048583956e-03 -2.873160806811282750e-03 -2.875253665745089622e-03 -2.876945327307253459e-03 -2.877999539279426679e-03 -2.878128090963568905e-03 -2.876978114014523604e-03
--2.963488905705875982e-03 -2.963864091635589823e-03 -2.964988192698943172e-03 -2.966843890948861386e-03 -2.969403896404342481e-03 -2.972628804740698287e-03 -2.976465829715451913e-03 -2.980847066136507739e-03 -2.985687190462770011e-03 -2.990880462967308601e-03 -2.996296854400116918e-03 -3.001777019581325888e-03 -3.007125761633465313e-03 -3.012103444723275483e-03 -3.016414584027568742e-03
--3.066500966728437534e-03 -3.067084560863539075e-03 -3.068690044113034626e-03 -3.071353192918362465e-03 -3.075054563833752499e-03 -3.079765997168827912e-03 -3.085449625993885725e-03 -3.092056520886407069e-03 -3.099524900079901439e-03 -3.107777800274289480e-03 -3.116720074229362581e-03 -3.126234495640563618e-03 -3.136176694606949283e-03 -3.146368488457358410e-03 -3.156588980528466249e-03
--3.167362486197706616e-03 -3.168161447401959298e-03 -3.170263401126237682e-03 -3.173759667294768876e-03 -3.178639452085888720e-03 -3.184887014215869328e-03 -3.192481005397918275e-03 -3.201393576261687534e-03 -3.211589207952302450e-03 -3.223023209968811642e-03 -3.235639810522076328e-03 -3.249369710915315981e-03 -3.264126950911505360e-03 -3.279804831862937354e-03 -3.296270533585701681e-03
--3.265415808477476183e-03 -3.266434107962291802e-03 -3.269040853048740987e-03 -3.273384455076129834e-03 -3.279463308850888697e-03 -3.287274874229534002e-03 -3.296815379191188680e-03 -3.308079431802622098e-03 -3.321059536651336987e-03 -3.335745508351565039e-03 -3.352123781627321716e-03 -3.370176594885984991e-03 -3.389881049174235401e-03 -3.411208014459348858e-03 -3.434120858011654488e-03
--3.359992452374316839e-03 -3.361230886053084843e-03 -3.364343558472963729e-03 -3.369536555538895067e-03 -3.376817711558031954e-03 -3.386198042807587755e-03 -3.397691817267848441e-03 -3.411316677893209623e-03 -3.427093850384104693e-03 -3.445048480899462213e-03 -3.465210175901131152e-03 -3.487613829518335182e-03 -3.512300895854811658e-03 -3.539321308470785160e-03 -3.568736367666102294e-03
--3.450422550919221565e-03 -3.451878649196864039e-03 -3.455491001378394999e-03 -3.461522959973480779e-03 -3.469991758063453984e-03 -3.480921891312166970e-03 -3.494345531279218365e-03 -3.510303125501646609e-03 -3.528844246052795491e-03 -3.550028778531960031e-03 -3.573928584883188410e-03 -3.600629820292173319e-03 -3.630236191113985107e-03 -3.662873549107028160e-03 -3.698696425531270825e-03
--3.536044554214848833e-03 -3.537712590439587561e-03 -3.541811014323783657e-03 -3.548659057154636073e-03 -3.558283035534972726e-03 -3.570720441914584237e-03 -3.586020654613635093e-03 -3.604245945445262288e-03 -3.625472868932352530e-03 -3.649794159032615677e-03 -3.677321308500797713e-03 -3.708188077455179272e-03 -3.742555302319705568e-03 -3.780617522985567618e-03 -3.822612200524892669e-03
--3.616214909408062717e-03 -3.618086001521568854e-03 -3.622649761011287762e-03 -3.630278976211813013e-03 -3.641008492610929743e-03 -3.654887965833172013e-03 -3.671982803789343094e-03 -3.692375487090972502e-03 -3.716167363298566399e-03 -3.743481057648623180e-03 -3.774463694244070255e-03 -3.809291202814791243e-03 -3.848174111763599890e-03 -3.891365382418605391e-03 -3.939171091560615852e-03
--3.690317447109191500e-03 -3.692379741120163476e-03 -3.697381388307788286e-03 -3.705745553468256341e-03 -3.717514865733410195e-03 -3.732750034446682443e-03 -3.751530949271928306e-03 -3.773958205349551599e-03 -3.800155148685664848e-03 -3.830270584486364458e-03 -3.864482335858935094e-03 -3.903001918942752314e-03 -3.946080711832649496e-03 -3.994018127301084825e-03 -4.047172510177153050e-03
--3.757772235666615064e-03 -3.760011155094086181e-03 -3.765417094574325871e-03 -3.774459652497049421e-03 -3.787188362181370758e-03 -3.803673687976466197e-03 -3.824008208196259979e-03 -3.848308236454538178e-03 -3.876715965709724623e-03 -3.909402261831422185e-03 -3.946570265556878510e-03 -3.988460029905547752e-03 -4.035354501263172140e-03 -4.087587249040744788e-03 -4.145552492213931337e-03
--3.818043709576097230e-03 -3.820442252414645024e-03 -3.826213412177122478e-03 -3.835868625162227197e-03 -3.849463372817254515e-03 -3.867076474361198432e-03 -3.888811284610138239e-03 -3.914797314500400791e-03 -3.945192339379350287e-03 -3.980185093596154931e-03 -4.019998667353383813e-03 -4.064894769613252787e-03 -4.115179070828758716e-03 -4.171207888373522875e-03 -4.233396549342624722e-03
--3.870647930654761652e-03 -3.873186994895524721e-03 -3.879279561168025910e-03 -3.889473768980591505e-03 -3.903830067909812816e-03 -3.922434210126622516e-03 -3.945398408947095939e-03 -3.972862882571834807e-03 -4.004997823140572788e-03 -4.042005855475676833e-03 -4.084125047798698241e-03 -4.131632566411666367e-03 -4.184849081269296014e-03 -4.244144034308373892e-03 -4.309941889696350739e-03
--3.915158894578164329e-03 -3.917817614793608037e-03 -3.924183791569738934e-03 -3.934836704472310931e-03 -3.949840809945859114e-03 -3.969287413152747419e-03 -3.993295751212529686e-03 -4.022014411027951229e-03 -4.055623095321939098e-03 -4.094334764421516358e-03 -4.138398160803895102e-03 -4.188100737425443781e-03 -4.243771991243707256e-03 -4.305787175171306436e-03 -4.374571317576437211e-03
--3.951213845338953645e-03 -3.953969925980027784e-03 -3.960558687063102899e-03 -3.971584658127891819e-03 -3.987115389192300192e-03 -4.007246443167297029e-03 -4.032102387623835889e-03 -4.061838066859761558e-03 -4.096640142756095490e-03 -4.136728896839999073e-03 -4.182360251488947273e-03 -4.233827965044411473e-03 -4.291465913328747217e-03 -4.355650313986010776e-03 -4.426801673504102488e-03
--3.978517601411007791e-03 -3.981347636766957403e-03 -3.988105447845251804e-03 -3.999414686035126024e-03 -4.015345143884096503e-03 -4.035995451086855923e-03 -4.061493977849424050e-03 -4.091999969255283483e-03 -4.127704877945784917e-03 -4.168833858291708799e-03 -4.215647339849594097e-03 -4.268442581808047816e-03 -4.327555051725536471e-03 -4.393359397493048352e-03 -4.466269686423395696e-03
--3.996845926590044881e-03 -3.999725702218169011e-03 -4.006597201389662521e-03 -4.018096906281088884e-03 -4.034296062832213106e-03 -4.055295277947816232e-03 -4.081225353928933861e-03 -4.112248316774928109e-03 -4.148558590460611067e-03 -4.190384259556340953e-03 -4.237988309801649436e-03 -4.291669711693532792e-03 -4.351764143702957673e-03 -4.418644066887359584e-03 -4.492717758788281578e-03
--4.006047994025191579e-03 -4.008952769249251626e-03 -4.015881405139431343e-03 -4.027476823099315588e-03 -4.043810982312316671e-03 -4.064985456633554879e-03 -4.091132231441243702e-03 -4.122414674479724268e-03 -4.159028624873180487e-03 -4.201203531895950603e-03 -4.249203343966070912e-03 -4.303328216950346938e-03 -4.363913147063741040e-03 -4.431329325395113976e-03 -4.505981677431570957e-03
--4.006047994025218467e-03 -4.008952769249252493e-03 -4.015881405139442618e-03 -4.027476823099325996e-03 -4.043810982312326212e-03 -4.064985456633565288e-03 -4.091132231441254978e-03 -4.122414674479732942e-03 -4.159028624873188293e-03 -4.201203531895961012e-03 -4.249203343966082187e-03 -4.303328216950359081e-03 -4.363913147063750581e-03 -4.431329325395128721e-03 -4.505981677431586570e-03
--3.996845926590046616e-03 -3.999725702218214982e-03 -4.006597201389706757e-03 -4.018096906281133120e-03 -4.034296062832253872e-03 -4.055295277947861335e-03 -4.081225353928979831e-03 -4.112248316774974946e-03 -4.148558590460656170e-03 -4.190384259556391260e-03 -4.237988309801703213e-03 -4.291669711693586568e-03 -4.351764143703014918e-03 -4.418644066887422034e-03 -4.492717758788345762e-03
--3.978517601411049424e-03 -3.981347636766996434e-03 -3.988105447845287366e-03 -3.999414686035158983e-03 -4.015345143884133799e-03 -4.035995451086891485e-03 -4.061493977849460479e-03 -4.091999969255321647e-03 -4.127704877945823948e-03 -4.168833858291749565e-03 -4.215647339849633128e-03 -4.268442581808089449e-03 -4.327555051725582441e-03 -4.393359397493097791e-03 -4.466269686423445136e-03
--3.951213845338979666e-03 -3.953969925980076357e-03 -3.960558687063154941e-03 -3.971584658127944728e-03 -3.987115389192353102e-03 -4.007246443167350805e-03 -4.032102387623890533e-03 -4.061838066859819671e-03 -4.096640142756154471e-03 -4.136728896840058921e-03 -4.182360251489010590e-03 -4.233827965044475658e-03 -4.291465913328815739e-03 -4.355650313986083634e-03 -4.426801673504175347e-03
--3.915158894578264943e-03 -3.917817614793667885e-03 -3.924183791569809190e-03 -3.934836704472379453e-03 -3.949840809945930238e-03 -3.969287413152819410e-03 -3.993295751212603412e-03 -4.022014411028027557e-03 -4.055623095322017160e-03 -4.094334764421598757e-03 -4.138398160803979237e-03 -4.188100737425531385e-03 -4.243771991243795727e-03 -4.305787175171400111e-03 -4.374571317576537825e-03
--3.870647930654848821e-03 -3.873186994895604519e-03 -3.879279561168105274e-03 -3.889473768980670435e-03 -3.903830067909892180e-03 -3.922434210126701445e-03 -3.945398408947179206e-03 -3.972862882571916339e-03 -4.004997823140660392e-03 -4.042005855475764436e-03 -4.084125047798787579e-03 -4.131632566411761777e-03 -4.184849081269398363e-03 -4.244144034308479710e-03 -4.309941889696457425e-03
--3.818043709576145802e-03 -3.820442252414734362e-03 -3.826213412177216586e-03 -3.835868625162322607e-03 -3.849463372817351226e-03 -3.867076474361296010e-03 -3.888811284610237985e-03 -3.914797314500504874e-03 -3.945192339379453503e-03 -3.980185093596265954e-03 -4.019998667353495703e-03 -4.064894769613371615e-03 -4.115179070828878412e-03 -4.171207888373650377e-03 -4.233396549342759163e-03
--3.757772235666672310e-03 -3.760011155094202841e-03 -3.765417094574447735e-03 -3.774459652497173454e-03 -3.787188362181498694e-03 -3.803673687976595000e-03 -3.824008208196390517e-03 -3.848308236454672186e-03 -3.876715965709865135e-03 -3.909402261831564432e-03 -3.946570265557027696e-03 -3.988460029905706479e-03 -4.035354501263336939e-03 -4.087587249040916526e-03 -4.145552492214111748e-03
--3.690317447109338952e-03 -3.692379741120303555e-03 -3.697381388307927064e-03 -3.705745553468395553e-03 -3.717514865733550708e-03 -3.732750034446823822e-03 -3.751530949272074457e-03 -3.773958205349701653e-03 -3.800155148685819672e-03 -3.830270584486521884e-03 -3.864482335859099893e-03 -3.903001918942927088e-03 -3.946080711832829040e-03 -3.994018127301275645e-03 -4.047172510177355145e-03
--3.616214909408176342e-03 -3.618086001521687682e-03 -3.622649761011414397e-03 -3.630278976211937913e-03 -3.641008492611058547e-03 -3.654887965833305587e-03 -3.671982803789476668e-03 -3.692375487091109545e-03 -3.716167363298706044e-03 -3.743481057648768030e-03 -3.774463694244220308e-03 -3.809291202814952572e-03 -3.848174111763760785e-03 -3.891365382418776261e-03 -3.939171091560794528e-03
--3.536044554214973733e-03 -3.537712590439737615e-03 -3.541811014323932409e-03 -3.548659057154774418e-03 -3.558283035535121045e-03 -3.570720441914734290e-03 -3.586020654613789917e-03 -3.604245945445433159e-03 -3.625472868932515594e-03 -3.649794159032792185e-03 -3.677321308500970751e-03 -3.708188077455363586e-03 -3.742555302319889882e-03 -3.780617522985764943e-03 -3.822612200525104739e-03
--3.450422550919344730e-03 -3.451878649197002383e-03 -3.455491001378535511e-03 -3.461522959973614786e-03 -3.469991758063596665e-03 -3.480921891312312687e-03 -3.494345531279364949e-03 -3.510303125501811408e-03 -3.528844246052952917e-03 -3.550028778532134371e-03 -3.573928584883358846e-03 -3.600629820292346791e-03 -3.630236191114153809e-03 -3.662873549107229822e-03 -3.698696425531485064e-03
--3.359992452374481204e-03 -3.361230886053239234e-03 -3.364343558473124191e-03 -3.369536555539047722e-03 -3.376817711558193283e-03 -3.386198042807753422e-03 -3.397691817268014974e-03 -3.411316677893390468e-03 -3.427093850384281635e-03 -3.445048480899653900e-03 -3.465210175901320671e-03 -3.487613829518529038e-03 -3.512300895855002911e-03 -3.539321308471010674e-03 -3.568736367666342120e-03
--3.265415808477598048e-03 -3.266434107962455299e-03 -3.269040853048905352e-03 -3.273384455076287693e-03 -3.279463308851057399e-03 -3.287274874229705306e-03 -3.296815379191363454e-03 -3.308079431802814652e-03 -3.321059536651525205e-03 -3.335745508351765400e-03 -3.352123781627520775e-03 -3.370176594886189255e-03 -3.389881049174436195e-03 -3.411208014459583913e-03 -3.434120858011903421e-03
--3.167362486197891364e-03 -3.168161447402119760e-03 -3.170263401126402480e-03 -3.173759667294927603e-03 -3.178639452086055688e-03 -3.184887014216036295e-03 -3.192481005398092615e-03 -3.201393576261875318e-03 -3.211589207952488933e-03 -3.223023209969011135e-03 -3.235639810522272786e-03 -3.249369710915517642e-03 -3.264126950911701384e-03 -3.279804831863169373e-03 -3.296270533585943241e-03
--3.066500966728616644e-03 -3.067084560863696501e-03 -3.068690044113195087e-03 -3.071353192918522493e-03 -3.075054563833920333e-03 -3.079765997168999216e-03 -3.085449625994055728e-03 -3.092056520886589215e-03 -3.099524900080083151e-03 -3.107777800274488106e-03 -3.116720074229552100e-03 -3.126234495640760943e-03 -3.136176694607150511e-03 -3.146368488457570479e-03 -3.156588980528686125e-03
--2.963488905706134890e-03 -2.963864091635747249e-03 -2.964988192699110139e-03 -2.966843890949015777e-03 -2.969403896404499473e-03 -2.972628804740861351e-03 -2.976465829715621483e-03 -2.980847066136677308e-03 -2.985687190462936111e-03 -2.990880462967487278e-03 -2.996296854400287788e-03 -3.001777019581501962e-03 -3.007125761633651796e-03 -3.012103444723481047e-03 -3.016414584027782547e-03
--2.858964238686720859e-03 -2.859140685779530417e-03 -2.859804641850689430e-03 -2.860888947291596093e-03 -2.862359490587304371e-03 -2.864167123376980869e-03 -2.866246188950689108e-03 -2.868512508048427258e-03 -2.870860717048765234e-03 -2.873160806811471835e-03 -2.875253665745285646e-03 -2.876945327307455121e-03 -2.877999539279633544e-03 -2.878128090963782710e-03 -2.876978114014749552e-03
--2.753537091262292340e-03 -2.753526826649796422e-03 -2.753757236822206717e-03 -2.754115248174799843e-03 -2.754561121949450093e-03 -2.755037707041265490e-03 -2.755468852918370980e-03 -2.755757235410492487e-03 -2.755781497221104683e-03 -2.755392551110780446e-03 -2.754408852274825223e-03 -2.752610354710503544e-03 -2.749730790275121961e-03 -2.745447762286130303e-03 -2.739369967382075232e-03
--2.647782713377612625e-03 -2.647599712137090229e-03 -2.647427617851800478e-03 -2.647111910819945242e-03 -2.646608514165365179e-03 -2.645854162465959957e-03 -2.644764777923652548e-03 -2.643233257116685189e-03 -2.641126578503747661e-03 -2.638282094047701958e-03 -2.634502832450558076e-03 -2.629551573595555539e-03 -2.623143390422758448e-03 -2.614936260117861275e-03 -2.604519228732524692e-03
--2.542235604436222755e-03 -2.541895344046499368e-03 -2.541355236415538538e-03 -2.540424157871827918e-03 -2.539055021507607458e-03 -2.537180380219705104e-03 -2.534710845295551785e-03 -2.531532944572042077e-03 -2.527506346184229397e-03 -2.522460336885222650e-03 -2.516189416737010624e-03 -2.508447832681343168e-03 -2.498942825767197767e-03 -2.487326331175065876e-03 -2.473184812083998804e-03
--2.437384934660126110e-03 -2.436903935963177434e-03 -2.436032728205644524e-03 -2.434548646704819391e-03 -2.432402895254608902e-03 -2.429525729878273359e-03 -2.425824987415658388e-03 -2.421184107831099355e-03 -2.415459596558358277e-03 -2.408477847125481755e-03 -2.400031226900314896e-03 -2.389873317712991590e-03 -2.377713171127107325e-03 -2.363208455516685024e-03 -2.345957361278920052e-03
--2.333671304411034410e-03 -2.333066680339348619e-03 -2.331902698765125903e-03 -2.329930287628695623e-03 -2.327100160401541790e-03 -2.323342033135693784e-03 -2.318563315356821000e-03 -2.312647366360264314e-03 -2.305451285158668408e-03 -2.296803186614349013e-03 -2.286498908855650984e-03 -2.274298108417842097e-03 -2.259919683421149957e-03 -2.243036520149430807e-03 -2.223269579998311471e-03
--2.231484822044282196e-03 -2.230773852847601265e-03 -2.229355885882878478e-03 -2.226960512773072751e-03 -2.223539047802332910e-03 -2.219022234812124787e-03 -2.213319130758734619e-03 -2.206315642011668146e-03 -2.197872695912079719e-03 -2.187824030469060106e-03 -2.175973587036376423e-03 -2.162092514073542422e-03 -2.145915792346967960e-03 -2.127138562897232070e-03 -2.105412282497182413e-03
--2.131164426793757949e-03 -2.130364176854669840e-03 -2.128730620592364075e-03 -2.125976895571725193e-03 -2.122055858924956628e-03 -2.116900615657701587e-03 -2.110423618267744019e-03 -2.102515503193801410e-03 -2.093043665126967118e-03 -2.081850576590610433e-03 -2.068751870676673304e-03 -2.053534230827488722e-03 -2.035953155904232301e-03 -2.015730728048060940e-03 -1.992553578916233300e-03
--2.032998339367991011e-03 -2.032125326437938390e-03 -2.030313440787165618e-03 -2.027263972835752562e-03 -2.022932089558433007e-03 -2.017254336607752097e-03 -2.010147957176694998e-03 -2.001510028935147428e-03 -1.991216434443404074e-03 -1.979120691197381893e-03 -1.965052683160225556e-03 -1.948817360779955430e-03 -1.930193515303400397e-03 -1.908932773833753056e-03 -1.884759045953078756e-03
--1.937225491189284443e-03 -1.936295414482542892e-03 -1.934340713974002637e-03 -1.931055089016884023e-03 -1.926396606483011739e-03 -1.920306072547890101e-03 -1.912706561654811763e-03 -1.903502837564480287e-03 -1.892580691985212664e-03 -1.879806239542774864e-03 -1.865025226031763158e-03 -1.848062428078492934e-03 -1.828721271284999188e-03 -1.806783808272721496e-03 -1.782011299018935275e-03
--1.844037763956505455e-03 -1.843065293419931866e-03 -1.841001072651321903e-03 -1.837535065257469083e-03 -1.832628656337349478e-03 -1.826227482955490632e-03 -1.818261154820758480e-03 -1.808642931183059325e-03 -1.797269385340959872e-03 -1.784020102628876194e-03 -1.768757475185699958e-03 -1.751326676969173959e-03 -1.731555944887597492e-03 -1.709257301041847751e-03 -1.684227938451073742e-03
--1.753582863751078748e-03 -1.752581489276460510e-03 -1.750438481131595279e-03 -1.746843492653946377e-03 -1.741761486824740116e-03 -1.735143273516665452e-03 -1.726925397634066547e-03 -1.717030036098613280e-03 -1.705364937867402675e-03 -1.691823454962986407e-03 -1.676284728137944578e-03 -1.658614109354166659e-03 -1.638663933671201823e-03 -1.616274767311649558e-03 -1.591277313444593080e-03
--1.665967656659078210e-03 -1.664949593199938158e-03 -1.662755750806644639e-03 -1.659078457368286935e-03 -1.653886373082726199e-03 -1.647135622615219239e-03 -1.638769823187222587e-03 -1.628720162707637895e-03 -1.616905562088458538e-03 -1.603232968250212003e-03 -1.587597837398115530e-03 -1.569884885022386012e-03 -1.549969194619203348e-03 -1.527717804611638652e-03 -1.502991902347400755e-03
--1.581261803762402593e-03 -1.580237946324343501e-03 -1.578018335364687885e-03 -1.574300521914929508e-03 -1.569056863852372327e-03 -1.562248774957519402e-03 -1.553826864718340674e-03 -1.543731158568362009e-03 -1.531891430595085698e-03 -1.518227691295361481e-03 -1.502650883228688877e-03 -1.485063852053601294e-03 -1.465362664448804355e-03 -1.443438377867073581e-03 -1.419179349238748611e-03
--1.499501550082323531e-03 -1.498481471343636722e-03 -1.496258256714649414e-03 -1.492536809207216895e-03 -1.487293088485928862e-03 -1.480493637445763535e-03 -1.472095806612671925e-03 -1.462048079714841796e-03 -1.450290529023814468e-03 -1.436755437659603717e-03 -1.421368133600267461e-03 -1.404048092545818202e-03 -1.384710362227620228e-03 -1.363267394087958918e-03 -1.339631342525301723e-03
--1.420693542402225997e-03 -1.419685525204116483e-03 -1.417478034933730832e-03 -1.413785061107579368e-03 -1.408585994971638024e-03 -1.401852246374960887e-03 -1.393547528027244513e-03 -1.383628253439438517e-03 -1.372044072997006658e-03 -1.358738579333692957e-03 -1.343650218377532039e-03 -1.326713452014111885e-03 -1.307860210393975995e-03 -1.287021697827010758e-03 -1.264130595178433909e-03
--1.344818572892578223e-03 -1.343829669880120935e-03 -1.341654519338040738e-03 -1.338017569077349853e-03 -1.332901417849865003e-03 -1.326282007572778150e-03 -1.318128945945413154e-03 -1.308405948240989967e-03 -1.297071419077311166e-03 -1.284079198536394609e-03 -1.269379501610981434e-03 -1.252920085064508204e-03 -1.234647670427946840e-03 -1.214509665473796846e-03 -1.192456210609970377e-03
--1.271835167474529276e-03 -1.270871280634179763e-03 -1.268742541122913408e-03 -1.265184899373045582e-03 -1.260183901826948628e-03 -1.253719640735559589e-03 -1.245767096894761150e-03 -1.236296602151893244e-03 -1.225274438167022568e-03 -1.212663589988817025e-03 -1.198424677567251889e-03 -1.182517085066500835e-03 -1.164900315998737773e-03 -1.145535591838791776e-03 -1.124387711431372493e-03
--1.201682958683055608e-03 -1.200748932265200764e-03 -1.198678329726764885e-03 -1.195219360039734323e-03 -1.190360230859178895e-03 -1.184084784221596477e-03 -1.176372823550170732e-03 -1.167200588964216338e-03 -1.156541348806823999e-03 -1.144366135612086624e-03 -1.130644642915500661e-03 -1.115346289528713853e-03 -1.098441480597698054e-03 -1.079903062432182367e-03 -1.059707984343896551e-03
--1.134285801579978242e-03 -1.133385522802426342e-03 -1.131382654364045592e-03 -1.128038159785250613e-03 -1.123342632917323633e-03 -1.117283238380296787e-03 -1.109844053936267366e-03 -1.101006523379100335e-03 -1.090750028567775455e-03 -1.079052590198144529e-03 -1.065891710746173521e-03 -1.051245358090089179e-03 -1.035093116147952534e-03 -1.017417488068272707e-03 -9.982053610169965181e-04
--1.069554607558473487e-03 -1.068691110448495270e-03 -1.066763668640294694e-03 -1.063546284864616553e-03 -1.059031647384209816e-03 -1.053209841434105381e-03 -1.046068677391936205e-03 -1.037594121596059800e-03 -1.027770835545469517e-03 -1.016582829727146831e-03 -1.004014239632545482e-03 -9.900502228348464096e-04 -9.746779898047400886e-04 -9.578879571374952773e-04 -9.396750233619860157e-04
--1.007389884455990679e-03 -1.006565453138923366e-03 -1.004719449686207163e-03 -1.001639014675458680e-03 -9.973186552057087748e-04 -9.917509850847737451e-04 -9.849270329769120244e-04 -9.768366442906880991e-04 -9.674689802628153382e-04 -9.568131176594309607e-04 -9.448587519672009896e-04 -9.315970045376392988e-04 -9.170213337047337281e-04 -9.011285441598086395e-04 -8.839198862428814278e-04
--9.476839822868025160e-04 -9.469002509116768293e-04 -9.451402339231094194e-04 -9.422041557061587753e-04 -9.380880818219303153e-04 -9.327867860093526668e-04 -9.262940346081568674e-04 -9.186029553785285927e-04 -9.097064921007158968e-04 -8.995979480015558636e-04 -8.882716126522533038e-04 -8.757234804300717199e-04 -8.619520473458365918e-04 -8.469591852289613939e-04 -8.307510805982074855e-04
--8.903230522856420094e-04 -8.895810995614577849e-04 -8.879103596353824564e-04 -8.851239623066770815e-04 -8.812192899662514567e-04 -8.761929356068748819e-04 -8.700409615184004743e-04 -8.627592330435637736e-04 -8.543438270261016028e-04 -8.447915188077408100e-04 -8.341003334306284307e-04 -8.222701794999287550e-04 -8.093035388494183597e-04 -7.952062170329688697e-04 -7.799881388579493497e-04
--8.351887330873533546e-04 -8.344891700722620450e-04 -8.329099322940080024e-04 -8.302767775036341922e-04 -8.265881840920869059e-04 -8.218422541088979145e-04 -8.160369455417237124e-04 -8.091703706267949943e-04 -8.012411590011069397e-04 -7.922488870294708795e-04 -7.821945619802077570e-04 -7.710811714270329005e-04 -7.589142771624515912e-04 -7.457026539098171331e-04 -7.314589585507538967e-04
--7.821595820710307420e-04 -7.815026324080796795e-04 -7.800162324055439408e-04 -7.775384134917095492e-04 -7.740685509266464689e-04 -7.696059770243692064e-04 -7.641501873067567006e-04 -7.577011041698069509e-04 -7.502593965124066495e-04 -7.418268535448338877e-04 -7.324068078805637781e-04 -7.220046057083678425e-04 -7.106281150631564179e-04 -6.982882651246320261e-04 -6.849996053035865970e-04
--7.311122725026915434e-04 -7.304978447330395764e-04 -7.291048879069307641e-04 -7.267832953843901761e-04 -7.235331622360977651e-04 -7.193548023143311399e-04 -7.142489328471960915e-04 -7.082169014931703798e-04 -7.012609664811886908e-04 -6.933846195858336080e-04 -6.845929507173066728e-04 -6.748930487184274900e-04 -6.642944320611530833e-04 -6.528095011030551724e-04 -6.404540019631755439e-04
--6.819225784337563587e-04 -6.813503303536915055e-04 -6.800508341256953498e-04 -6.778853924310068854e-04 -6.748546649603108950e-04 -6.709597260827717584e-04 -6.662022406622951755e-04 -6.605846449840330637e-04 -6.541103975747664676e-04 -6.467842516682694148e-04 -6.386125691736010360e-04 -6.296036585786376517e-04 -6.197681370578717042e-04 -6.091193070543158726e-04 -5.976735384738579050e-04
--6.344661696495458017e-04 -6.339355649225831809e-04 -6.327290843775139340e-04 -6.307189606341845594e-04 -6.279062783715837204e-04 -6.242926932510132684e-04 -6.198805672234960996e-04 -6.146731390338268115e-04 -6.086747330291606122e-04 -6.018909872945133951e-04 -5.943291240451870940e-04 -5.859982308447592245e-04 -5.769095628614078885e-04 -5.670768539851708985e-04 -5.565166293829636700e-04
--5.886192385693716925e-04 -5.881295959733982967e-04 -5.870153336398569290e-04 -5.851591197962051003e-04 -5.825623483874434703e-04 -5.792270879160282739e-04 -5.751561965790997393e-04 -5.703534672464700365e-04 -5.648238024019070673e-04 -5.585734092370199565e-04 -5.516100229260742461e-04 -5.439431420961489405e-04 -5.355842782018414199e-04 -5.265472103001638243e-04 -5.168482385094878579e-04
--5.442589800939208900e-04 -5.438095158906122630e-04 -5.427864166390825723e-04 -5.410822866993085208e-04 -5.386987289648140741e-04 -5.356380860799499818e-04 -5.319035372441941389e-04 -5.274992200519256413e-04 -5.224303752887910889e-04 -5.167035120298900342e-04 -5.103265897568618013e-04 -5.033092135337792700e-04 -4.956628375701784819e-04 -4.874009717585961465e-04 -4.785393850808986938e-04
--5.012639441615498884e-04 -5.008538081328975117e-04 -4.999206402968542177e-04 -4.983664845571914416e-04 -4.961930682004098625e-04 -4.934028913322069257e-04 -4.899993071129954848e-04 -4.859866224865034157e-04 -4.813702175003603404e-04 -4.761566808177817483e-04 -4.703539584868276276e-04 -4.639715124727493293e-04 -4.570204848821389824e-04 -4.495138632334708334e-04 -4.414666415698066714e-04
--4.595142793560014986e-04 -4.591425850710304174e-04 -4.582980089399852491e-04 -4.568915471970093974e-04 -4.549249812746479060e-04 -4.524008719790855544e-04 -4.493226247888770395e-04 -4.456945716333065590e-04 -4.415220674660926816e-04 -4.368115995260164535e-04 -4.315709067330757110e-04 -4.258091062119396088e-04 -4.195368234750575416e-04 -4.127663223503968753e-04 -4.055116303242194695e-04
--4.188918844169252863e-04 -4.185577342821148860e-04 -4.178003590952124053e-04 -4.165392347459481617e-04 -4.147761395170393071e-04 -4.125136169013914468e-04 -4.097550228606459217e-04 -4.065046017838647337e-04 -4.027675480207443997e-04 -3.985501026248353985e-04 -3.938596425504410073e-04 -3.887047798184674742e-04 -3.830954621297117399e-04 -3.770430724054411008e-04 -3.705605237312313734e-04
--3.792804830289472039e-04 -3.789829886454556336e-04 -3.783114191475872340e-04 -3.771932759785892163e-04 -3.756302887038526065e-04 -3.736249207349351528e-04 -3.711804018028201082e-04 -3.683007929495572060e-04 -3.649910265247866014e-04 -3.612569824698030072e-04 -3.571055550672030065e-04 -3.525447271002871965e-04 -3.475836968449047461e-04 -3.422326899186101828e-04 -3.365035508571560460e-04
--3.405656358729733922e-04 -3.403039341765820352e-04 -3.397168076986086774e-04 -3.387393509856057158e-04 -3.373732099849121322e-04 -3.356207184349508689e-04 -3.334849256265849226e-04 -3.309696330567753718e-04 -3.280794343957060388e-04 -3.248197622845663151e-04 -3.211969378260469020e-04 -3.172182221473917609e-04 -3.128918681579832568e-04 -3.082271705795923910e-04 -3.032345121767639358e-04
--3.026347026528157362e-04 -3.024079682577169854e-04 -3.019039831594671000e-04 -3.010650264873721829e-04 -2.998926354531938703e-04 -2.983889808376992176e-04 -2.965568850580203191e-04 -2.943998445152768676e-04 -2.919220555611349178e-04 -2.891284432767487903e-04 -2.860246921161718942e-04 -2.826172773309047499e-04 -2.789134959670924729e-04 -2.749214961161583742e-04 -2.706503030087689470e-04
--2.653767657022094301e-04 -2.651842198080171797e-04 -2.647621559845870468e-04 -2.640596549627388569e-04 -2.630781291884592239e-04 -2.618195647630463282e-04 -2.602865297398416003e-04 -2.584821842515103532e-04 -2.564102920689981572e-04 -2.540752331115862773e-04 -2.514820163514382449e-04 -2.486362924861006021e-04 -2.455443656914036376e-04 -2.422132037166483342e-04 -2.386504455462242370e-04
--2.286825258493388078e-04 -2.285234420043431272e-04 -2.281821740093804775e-04 -2.276142478082923389e-04 -2.268209436348089369e-04 -2.258040528481157711e-04 -2.245658769213001440e-04 -2.231092252899060150e-04 -2.214374140850560130e-04 -2.195542619825127835e-04 -2.174640866035053494e-04 -2.151716991231456639e-04 -2.126823976299026990e-04 -2.100019589618755899e-04 -2.071366288614814063e-04
--1.924441804775619343e-04 -1.923178874261406647e-04 -1.920563906143963706e-04 -1.916213319952455316e-04 -1.910138604166581374e-04 -1.902355729499901021e-04 -1.892885095052174432e-04 -1.881751272032748299e-04 -1.868983007578120590e-04 -1.854612917905531372e-04 -1.838677327091178186e-04 -1.821216028743284621e-04 -1.802272037677908156e-04 -1.781891327570682892e-04 -1.760122559122721895e-04
--1.565552931869531846e-04 -1.564611749616008629e-04 -1.562785249008071019e-04 -1.559747991527966936e-04 -1.555510241588373404e-04 -1.550086165513289704e-04 -1.543493660844537894e-04 -1.535754022288338778e-04 -1.526891779207790361e-04 -1.516934234567472056e-04 -1.505911139147425430e-04 -1.493854269729313292e-04 -1.480796994453595036e-04 -1.466773824615666541e-04 -1.451819963619547247e-04
--1.209106641247459802e-04 -1.208481574786645003e-04 -1.207435227303678676e-04 -1.205697556782948997e-04 -1.203277775530831061e-04 -1.200188481635659126e-04 -1.196445370975368237e-04 -1.192066835516263903e-04 -1.187073583230156956e-04 -1.181488071322143031e-04 -1.175333977857371441e-04 -1.168635593510359031e-04 -1.161417189791529047e-04 -1.153702372765133804e-04 -1.145513439316878795e-04
--8.540620991638820172e-05 -8.537479913062222996e-05 -8.534742735372683646e-05 -8.530238235263332353e-05 -8.524050580118857495e-05 -8.516293579499212372e-05 -8.507106728205041362e-05 -8.496650218664416991e-05 -8.485099002429391177e-05 -8.472636003172386368e-05 -8.459444608355796069e-05 -8.445700593338412252e-05 -8.431563659510601071e-05 -8.417168796056564897e-05 -8.402617701761509609e-05
--4.993886218588607616e-05 -4.993807122634710827e-05 -4.998726841850588149e-05 -5.006981201857566878e-05 -5.018649865971846775e-05 -5.033839240365273497e-05 -5.052677434503157405e-05 -5.075307912517131991e-05 -5.101881875947753952e-05 -5.132549679819455642e-05 -5.167451150358203741e-05 -5.206705289337494342e-05 -5.250399421300811290e-05 -5.298578110364072016e-05 -5.351232143560569719e-05
--1.440649389470921235e-05 -1.443587583957581157e-05 -1.456097840376360244e-05 -1.477003415188839859e-05 -1.506383860552231932e-05 -1.544344250770134704e-05 -1.591008977492192750e-05 -1.646513967854505581e-05 -1.710997046966688260e-05 -1.784587771194533603e-05 -1.867394957514207114e-05 -1.959494103498756650e-05 -2.060913799110014643e-05 -2.171621851057673218e-05 -2.291511441406603742e-05
-2.129211686639119689e-05 2.123299325434508051e-05 2.103265404354792917e-05 2.069816439176732671e-05 2.022867587444696861e-05 1.962307633574048851e-05 1.888006453270094217e-05 1.799824381179087858e-05 1.697623917968016588e-05 1.581281930063317296e-05 1.450704933151237414e-05 1.305844391084572727e-05 1.146713387980972162e-05 9.734037234588200499e-06 7.861030643412569505e-06
-5.725727544098659907e-05 5.716884216262741424e-05 5.689398381041434541e-05 5.643521255386786889e-05 5.579156336519544481e-05 5.496176932853069500e-05 5.394436149858637935e-05 5.273776844714751473e-05 5.134046061294219015e-05 4.975109601413263069e-05 4.796870204770790338e-05 4.599286041131100868e-05 4.382390880326703358e-05 4.146314924547653833e-05 3.891305848931745932e-05
-9.358830066279324534e-05 9.347101014414884021e-05 9.312245128540987344e-05 9.254071151539120660e-05 9.172463037106698197e-05 9.067268694509079225e-05 8.938310276329630710e-05 8.785397229968270249e-05 8.608342270260022642e-05 8.406979260397652197e-05 8.181184167572460664e-05 7.930897381340349826e-05 7.656147842413283094e-05 7.357078202157446567e-05 7.033970448712363122e-05
-1.303833847868369165e-04 1.302377329603673743e-04 1.298164550146288314e-04 1.291133228795305482e-04 1.281268928697113256e-04 1.268552628878315031e-04 1.252961908582439781e-04 1.234472459477588486e-04 1.213059912461359998e-04 1.188701982494646744e-04 1.161380851383991028e-04 1.131085852862010713e-04 1.097816323531601622e-04 1.061584621963684405e-04 1.022419230581831512e-04
-1.677393709015124394e-04 1.675659239059841066e-04 1.670731426193581681e-04 1.662505761396056983e-04 1.650963954831440560e-04 1.636081750395074479e-04 1.617830272962706914e-04 1.596177755249350420e-04 1.571091631101256695e-04 1.542541024367473888e-04 1.510499488590763767e-04 1.474948176989647128e-04 1.435879192005120718e-04 1.393299183989325806e-04 1.347233083924413623e-04
-2.057514346839201002e-04 2.055508593539513164e-04 2.049881067210997001e-04 2.040485820436407916e-04 2.027299553394957339e-04 2.010291157158658470e-04 1.989423227815715115e-04 1.964654015707494148e-04 1.935939800540938029e-04 1.903237736253615264e-04 1.866508999053186763e-04 1.825722468358903635e-04 1.780858647205720837e-04 1.731913919431826102e-04 1.678905015707220423e-04
-2.445126567532744915e-04 2.442857550076726566e-04 2.436549718963066475e-04 2.426016376098576025e-04 2.411227916665315105e-04 2.392144562526028815e-04 2.368718042036946749e-04 2.340893763286164232e-04 2.308613479052699252e-04 2.271818496553734213e-04 2.230453272386292637e-04 2.184469634060988365e-04 2.133831338422536184e-04 2.078519070475345204e-04 2.018535754700689975e-04
-2.841134715038249247e-04 2.838612186430499525e-04 2.831648581723679404e-04 2.820017078697660984e-04 2.803680337458632778e-04 2.782587897621604861e-04 2.756678015377250833e-04 2.725880053520892549e-04 2.690117436651027951e-04 2.649311210802322543e-04 2.603384145863961788e-04 2.552265477837283155e-04 2.495896195977550321e-04 2.434234854189066123e-04 2.367263845588558251e-04
-3.246409782942185924e-04 3.243645650777759125e-04 3.236057064103238208e-04 3.223377690481250553e-04 3.205560899228327961e-04 3.182543348858875949e-04 3.154246963276812464e-04 3.120581519427931315e-04 3.081447874922549953e-04 3.036741867266367365e-04 2.986358927396745599e-04 2.930199352208314898e-04 2.868174373231125937e-04 2.800212851455775409e-04 2.726268631366755108e-04
-3.661781014088232229e-04 3.658789795867687798e-04 3.650614512605686464e-04 3.636949979930172920e-04 3.617738612967524728e-04 3.592901827010894027e-04 3.562342122290866045e-04 3.525945834124888574e-04 3.483586594823643895e-04 3.435129554200808057e-04 3.380436449637675084e-04 3.319371443429039253e-04 3.251807968641513792e-04 3.177636375809928166e-04 3.096772468922749178e-04
-4.088025864557044676e-04 4.084825171776391983e-04 4.076110284147270576e-04 4.061537962157117697e-04 4.041037841002609061e-04 4.014513688179910020e-04 3.981845273339296100e-04 3.942891364483367116e-04 3.897493336753943879e-04 3.845479656923149621e-04 3.786671346583318060e-04 3.720888360629950051e-04 3.647957187679766217e-04 3.567719481455699539e-04 3.480041862100374177e-04
-4.525858230453858370e-04 4.522469272581638674e-04 4.513272048256862078e-04 4.497886163377000173e-04 4.476226860108281722e-04 4.448177533639898103e-04 4.413591878548323304e-04 4.372296775069973063e-04 4.324096009524851757e-04 4.268774929042405751e-04 4.206106193914015850e-04 4.135856636983516535e-04 4.057795526260102661e-04 3.971704183928066951e-04 3.877387095156992246e-04
-4.975914869242235167e-04 4.972362964928225566e-04 4.962752236624505542e-04 4.946666393113646407e-04 4.924004439931197645e-04 4.894626932959718173e-04 4.858358038909535871e-04 4.814988344165748065e-04 4.764278533685169887e-04 4.705964078517561574e-04 4.639761118749589539e-04 4.565373682031287090e-04 4.482502459708392092e-04 4.390855333596050455e-04 4.290159773036168701e-04
-5.438739994237118142e-04 5.435055072815508665e-04 5.425112602467858968e-04 5.408461994402075047e-04 5.384984350462920615e-04 5.354514946563359050e-04 5.316845099705878267e-04 5.271724763471259288e-04 5.218865998337174697e-04 5.157947501278841535e-04 5.088620409362704404e-04 5.010515654287581470e-04 4.923253039940632663e-04 4.826452488970275250e-04 4.719747587417634873e-04
-5.914768083433094570e-04 5.910985155033541671e-04 5.900806913086004135e-04 5.883750545249619417e-04 5.859677767407752780e-04 5.828396372670645656e-04 5.789661775588852239e-04 5.743179223865631493e-04 5.688606851677494936e-04 5.625559799583025036e-04 5.553615666289245375e-04 5.472321658068114584e-04 5.381203668994831305e-04 5.279777921317149346e-04 5.167565359090243483e-04
-6.404305023388424988e-04 6.400464591138151256e-04 6.390161877882032365e-04 6.372884506733861570e-04 6.348473619585295706e-04 6.316707717249051999e-04 6.277303729844919879e-04 6.229918644087579366e-04 6.174151885793744028e-04 6.109548719646532922e-04 6.035604985274046347e-04 5.951773612376931978e-04 5.857473255082113828e-04 5.752099813499561868e-04 5.635041223528319040e-04
-6.907507806085445585e-04 6.903656189019672946e-04 6.893356511724489828e-04 6.876070189155989235e-04 6.851617020589919910e-04 6.819744978333401033e-04 6.780130636139824508e-04 6.732379984512394709e-04 6.676029848134358742e-04 6.610550196155186471e-04 6.535347713468918438e-04 6.449771131344852072e-04 6.353118823229685422e-04 6.244649475012084908e-04 6.123596564960467978e-04
-7.424363110639263172e-04 7.420552642030200669e-04 7.410400250193875963e-04 7.393345304351722595e-04 7.369186048996567663e-04 7.337639464666476921e-04 7.298340876399101460e-04 7.250843711710461270e-04 7.194619627535912745e-04 7.129059311364307691e-04 7.053474359189058386e-04 6.967100757744820825e-04 6.869104672986728419e-04 6.758591310556321752e-04 6.634618054989966686e-04
-7.954665230040306985e-04 7.950954293016421984e-04 7.941110266099873395e-04 7.924555538745018876e-04 7.901067287193949944e-04 7.870332020009180793e-04 7.831944190217403432e-04 7.785404646655539555e-04 7.730119131061621764e-04 7.665397118267194224e-04 7.590451410439010265e-04 7.504399016430759453e-04 7.406264161179160373e-04 7.294984192463244794e-04 7.169419933515294155e-04
-8.497993940897636839e-04 8.494446802416487970e-04 8.485088581959106995e-04 8.469330735808934573e-04 8.446930695154898118e-04 8.417546206608877068e-04 8.380732789081229940e-04 8.335940644547611914e-04 8.282511197391929621e-04 8.219673520014023635e-04 8.146541022902907634e-04 8.062108925004302443e-04 7.965253352309501714e-04 7.854732931065484380e-04 7.729194544070187986e-04
-9.053693054086240071e-04 9.050379460413559597e-04 9.041699723337523822e-04 9.027061439579017786e-04 9.006204575928778485e-04 8.978761204921536154e-04 8.944251680310230310e-04 8.902079816904711652e-04 8.851527188048981427e-04 8.791746725023559224e-04 8.721755906505191530e-04 8.640430005769834422e-04 8.546496090722409617e-04 8.438528764798476547e-04 8.314949193206844702e-04
-9.620850516426366749e-04 9.617845018532866080e-04 9.610049803237853683e-04 9.596876712286764571e-04 9.578051576340312033e-04 9.553185403093021047e-04 9.521769201412776237e-04 9.483167310408299137e-04 9.436609256757508149e-04 9.381180211775292863e-04 9.315810185545449554e-04 9.239262302300722471e-04 9.150120602440450909e-04 9.046778294480712062e-04 8.927427771849449521e-04
-1.019828104536427225e-03 1.019566203215361601e-03 1.018896805443223223e-03 1.017762428523459085e-03 1.016134683758727723e-03 1.013973186286363766e-03 1.011224903021963649e-03 1.007823298702623105e-03 1.003687270793865265e-03 9.987198651244357569e-04 9.928067653395830985e-04 9.858145682362859374e-04 9.775888541348632527e-04 9.679521172605712667e-04 9.567016415237949295e-04
-1.078451235604301712e-03 1.078236078682866857e-03 1.077699193033213000e-03 1.076785421604129454e-03 1.075465955866938394e-03 1.073699703800969768e-03 1.071432518576497265e-03 1.068596167981960372e-03 1.065107029026979204e-03 1.060864479841324131e-03 1.055748957704640435e-03 1.049619659789777833e-03 1.042311855615659678e-03 1.033633818950116653e-03 1.023363396283861202e-03
-1.137777606807224666e-03 1.137617391321094290e-03 1.137235686671975035e-03 1.136580728797338550e-03 1.135623932748440002e-03 1.134324426012888083e-03 1.132628173789606727e-03 1.130466799170850266e-03 1.127756068758391499e-03 1.124393995098790702e-03 1.120258498248112317e-03 1.115204559406844263e-03 1.109060787617677062e-03 1.101625326583902673e-03 1.092661025967427190e-03
-1.197600434397516492e-03 1.197503276306042218e-03 1.197299197426328300e-03 1.196940937999985913e-03 1.196400859370493411e-03 1.195639356553409487e-03 1.194603906256766707e-03 1.193227781162208966e-03 1.191428380338945903e-03 1.189105107747905196e-03 1.186136715755185768e-03 1.182377999024918644e-03 1.177655665185332271e-03 1.171763516009581346e-03 1.164455844788192095e-03
-1.257683320184378034e-03 1.257657051103567908e-03 1.257652255382885357e-03 1.257627294237927519e-03 1.257556258038091930e-03 1.257401938737739890e-03 1.257114847491037348e-03 1.256631878975797336e-03 1.255874561901108247e-03 1.254746810700267494e-03 1.253132073410861492e-03 1.250889719710743947e-03 1.247850486196835831e-03 1.243810722486659399e-03 1.238525116661573283e-03
-1.317761325589789263e-03 1.317813275760511358e-03 1.318028025705066716e-03 1.318370652156117002e-03 1.318817774150986277e-03 1.319335745458418991e-03 1.319879690804863330e-03 1.320392188792655431e-03 1.320801535357243265e-03 1.321019492105325556e-03 1.320938401801144673e-03 1.320427483861390293e-03 1.319328089728195831e-03 1.317447588154293083e-03 1.314551447331703104e-03
-1.377542837235361164e-03 1.377679613915196166e-03 1.378132160793300127e-03 1.378873298789150183e-03 1.379882956549385083e-03 1.381132191197166799e-03 1.382582295899886663e-03 1.384183576167208763e-03 1.385873729203936089e-03 1.387575730228658624e-03 1.389195104292212206e-03 1.390616389443555647e-03 1.391698552625848968e-03 1.392268994269452251e-03 1.392115640647252888e-03
-1.436712239518718372e-03 1.436939511304274669e-03 1.437645493956956266e-03 1.438811673973945573e-03 1.440422010645646270e-03 1.442453320745415695e-03 1.444874509086494386e-03 1.447645512256422184e-03 1.450715897297177089e-03 1.454023029489613259e-03 1.457489698474776028e-03 1.461021025323194777e-03 1.464500425269463181e-03 1.467784278220729847e-03 1.470694812369419385e-03
-1.494933371704813569e-03 1.495255669823951968e-03 1.496227560620981209e-03 1.497839971017480556e-03 1.500081512080813848e-03 1.502935670759180135e-03 1.506380208777470010e-03 1.510386339352761016e-03 1.514917637586273881e-03 1.519928619303620790e-03 1.525362903135306283e-03 1.531150819129739517e-03 1.537206286707124350e-03 1.543422685752320620e-03 1.549667319410780826e-03
-1.551853707293095576e-03 1.552274254496055711e-03 1.553520882266766446e-03 1.555594552190812593e-03 1.558489013454818347e-03 1.562195134810128068e-03 1.566700506050796617e-03 1.571988897252240246e-03 1.578039551116103539e-03 1.584826271856157711e-03 1.592316263779347844e-03 1.600468642333039912e-03 1.609232519290700438e-03 1.618544505540142923e-03 1.628325401803269821e-03
-1.607109155181227905e-03 1.607629731463843881e-03 1.609155907342611986e-03 1.611699066648955309e-03 1.615258421951038404e-03 1.619832696568799905e-03 1.625419947854061208e-03 1.632017336730710085e-03 1.639620840940067418e-03 1.648224909462504221e-03 1.657822055574539747e-03 1.668402382819046898e-03 1.679953041994763658e-03 1.692457611058442854e-03 1.705895388811977430e-03
-1.660329348971636412e-03 1.660950201058192894e-03 1.662756466726136948e-03 1.665770117008108508e-03 1.669995977214778354e-03 1.675440836609228120e-03 1.682113495697065697e-03 1.690024848755089472e-03 1.699188021032543242e-03 1.709618592611194697e-03 1.721334949519225978e-03 1.734358830187652210e-03 1.748716160717355859e-03 1.764438321904456984e-03 1.781564062303522171e-03
-1.711143265856331346e-03 1.711863064382248547e-03 1.713945573771618464e-03 1.717423289864039278e-03 1.722306622206002703e-03 1.728610373344912059e-03 1.736353995381568344e-03 1.745561963176328266e-03 1.756264302849456019e-03 1.768497336324517449e-03 1.782304721435543646e-03 1.797738914588907543e-03 1.814863232179274831e-03 1.833754776028783057e-03 1.854508618054921416e-03
-1.759185002327732540e-03 1.760000847309254723e-03 1.762351383389618121e-03 1.766279347976419320e-03 1.771800539303735158e-03 1.778937473634999676e-03 1.787719821562691689e-03 1.798185028070354522e-03 1.810379168411815291e-03 1.824358121485483231e-03 1.840189165441715336e-03 1.857953163009643622e-03 1.877747564836039192e-03 1.899690571164378483e-03 1.923926951246184751e-03
-1.804099531761954329e-03 1.805007003615665025e-03 1.807613122504892747e-03 1.811970379883271528e-03 1.818099622092835899e-03 1.826030566900010412e-03 1.835802379345478734e-03 1.847464479362075909e-03 1.861077639633390568e-03 1.876715465159572473e-03 1.894466369284549369e-03 1.914436229398921345e-03 1.936751966611402476e-03 1.961566408137693437e-03 1.989064947123943099e-03
-1.845548278614710753e-03 1.846541529083385764e-03 1.849386815531844268e-03 1.854145716147896812e-03 1.860843669966047746e-03 1.869516918162784837e-03 1.880213173786910146e-03 1.892992550094415791e-03 1.907928804832717757e-03 1.925110990646725518e-03 1.944645620040595310e-03 1.966659519932360996e-03 1.991303600659377962e-03 2.018757863844197493e-03 2.049238099795162686e-03
-1.883214364078664811e-03 1.884286239258832355e-03 1.887350651482723766e-03 1.892477448182679602e-03 1.899696125400040158e-03 1.909048656976812790e-03 1.920590212587258141e-03 1.934390140706869141e-03 1.950533265932519016e-03 1.969121579723951028e-03 1.990276412657867970e-03 2.014141235191107583e-03 2.040885264271453774e-03 2.070708126439796664e-03 2.103845909254446495e-03
-1.916807405905026794e-03 1.917949592384525287e-03 1.921209870900758522e-03 1.926665422113896719e-03 1.934349217929925546e-03 1.944308114701372159e-03 1.956603579186990370e-03 1.971312668338266912e-03 1.988529299408551936e-03 2.008365870508360945e-03 2.030955290424741634e-03 2.056453522392366531e-03 2.085042754919002369e-03 2.116935354711606352e-03 2.152378789647163559e-03
-1.946067787259110442e-03 1.947270972233684262e-03 1.950701087003303214e-03 1.956441621655287313e-03 1.964528428582660788e-03 1.975012384385244069e-03 1.987960092599972816e-03 2.003454816620974833e-03 2.021597663152754475e-03 2.042509053911455239e-03 2.066330509157577981e-03 2.093226800487284645e-03 2.123388515152959278e-03 2.157035087136737351e-03 2.194418340266018549e-03
-1.970770342195820018e-03 1.972024379289112443e-03 1.975595991928296574e-03 1.981573895431432922e-03 1.989996237626697351e-03 2.000917077664307771e-03 2.014407046053377434e-03 2.030554204492287206e-03 2.049465109127814738e-03 2.071266091211242544e-03 2.096104744290711204e-03 2.124151627948751928e-03 2.155602163688396990e-03 2.190678687049118275e-03 2.229632577901976762e-03
-1.990727435085379478e-03 1.992021509254015763e-03 1.995704431784978486e-03 2.001869020982242724e-03 2.010555161326343585e-03 2.021819304512179581e-03 2.035735079798804605e-03 2.052394072987184358e-03 2.071906762320304199e-03 2.094403603727207006e-03 2.120036223943943306e-03 2.148978690238674983e-03 2.181428776058612351e-03 2.217609112615255822e-03 2.257768053183365538e-03
-2.005791435208882211e-03 2.007114222298937451e-03 2.010876860098385292e-03 2.017175126127749695e-03 2.026050115640301314e-03 2.037559939188916293e-03 2.051780287905799471e-03 2.068805140850025169e-03 2.088747590490189036e-03 2.111740761735888747e-03 2.137938671950462971e-03 2.167517580440285127e-03 2.200675871009270812e-03 2.237635360731352312e-03 2.278640740073100638e-03
-2.015856603889921907e-03 2.017196422797239239e-03 2.021006196141082213e-03 2.027383506202121675e-03 2.036370163913153904e-03 2.048025256414838340e-03 2.062425681233824235e-03 2.079666804795976803e-03 2.099863213498809333e-03 2.123149521922287897e-03 2.149681157958511363e-03 2.179635042471140833e-03 2.213210015355573327e-03 2.250626813054911520e-03 2.292127321763994929e-03
-2.020860419191692400e-03 2.022205376841554499e-03 2.026029121821783067e-03 2.032429882145821761e-03 2.041449710903676940e-03 2.053148025149787500e-03 2.067602128989554262e-03 2.084907854776184722e-03 2.105180287943669674e-03 2.128554536340980258e-03 2.155186458742839629e-03 2.185253263511987686e-03 2.218953820715758446e-03 2.256508482283145663e-03 2.298158122377772644e-03
-2.020784362822821562e-03 2.022122494029693351e-03 2.025926848816978453e-03 2.032295140339108758e-03 2.041269198068018653e-03 2.052908135011566153e-03 2.067288881804505742e-03 2.084506845110253338e-03 2.104676658558049442e-03 2.127932990795217052e-03 2.154431330435688848e-03 2.184348665516433214e-03 2.217883909333628716e-03 2.255257877714573859e-03 2.296712541958654836e-03
-2.015654186925650709e-03 2.016973592398041241e-03 2.020725378208333700e-03 2.027005582416672308e-03 2.035855337429695773e-03 2.047332805639400042e-03 2.061513744528119339e-03 2.078492213792656248e-03 2.098381400555727333e-03 2.121314538079601287e-03 2.147445765415674848e-03 2.176951476486779172e-03 2.210030202192599449e-03 2.246903918692858080e-03 2.287817487002505746e-03
-2.005539667162692039e-03 2.006828653334607332e-03 2.010495260631447578e-03 2.016632695138919924e-03 2.025280897255691149e-03 2.036496396697614914e-03 2.050352922584403915e-03 2.066942182080929759e-03 2.086374795888929629e-03 2.108781383012403587e-03 2.134313753331627209e-03 2.163146176715352326e-03 2.195476647991397110e-03 2.231528037794985007e-03 2.271548956073335054e-03
-1.990553835765705281e-03 1.991801059719990313e-03 1.995350849010544495e-03 2.001292430324092333e-03 2.009664026398380425e-03 2.020519800902541470e-03 2.033930518121191550e-03 2.049984402333732657e-03 2.068788200525959343e-03 2.090468462404434461e-03 2.115173026855558715e-03 2.143072724861311371e-03 2.174363274478522713e-03 2.209267331966693285e-03 2.248036621017975890e-03
-1.970851676955098341e-03 1.972046298499033085e-03 1.975449021696829011e-03 1.981143966681428795e-03 1.989167080050758575e-03 1.999569369845304641e-03 2.012417607834392913e-03 2.027795261868475894e-03 2.045803678643081519e-03 2.066563554592226303e-03 2.090216718498000888e-03 2.116928283247285995e-03 2.146889209010586531e-03 2.180319333071477524e-03 2.217470911600932359e-03
-1.946628260168658045e-03 1.947760101276254296e-03 1.950987344405690112e-03 1.956387912743036070e-03 1.963994892077033060e-03 1.973855297656071286e-03 1.986030799610500816e-03 2.000598702051964439e-03 2.017653212348344098e-03 2.037307060701299809e-03 2.059693528848265988e-03 2.084968992581225523e-03 2.113316091190091568e-03 2.144947678882726423e-03 2.180111746132067790e-03
-1.918116286151728273e-03 1.919175995725335912e-03 1.922201637365493184e-03 1.927263905987432668e-03 1.934392431656010471e-03 1.943629375209877594e-03 1.955030145659867376e-03 1.968664382348214031e-03 1.984617251285683819e-03 2.002991134740773633e-03 2.023907802176937425e-03 2.047511209539747221e-03 2.073971104238642432e-03 2.103487686473766525e-03 2.136297658746148451e-03
-1.885583028627598259e-03 1.886562248144374454e-03 1.889362921268441207e-03 1.894047569729317157e-03 1.900641787271237573e-03 1.909182030928836035e-03 1.919716290025519139e-03 1.932305013572267055e-03 1.947022353415449976e-03 1.963957813310691480e-03 1.983218412362080813e-03 2.004931537870103218e-03 2.029248712453284725e-03 2.056350599860963177e-03 2.086453700160068210e-03
-1.849326670415652992e-03 1.850218193838942555e-03 1.852773732519767550e-03 1.857046807181673065e-03 1.863058440193129679e-03 1.870838594919545369e-03 1.880426750739088012e-03 1.891872709593882306e-03 1.905237692553539636e-03 1.920595817862687281e-03 1.938036075232825147e-03 1.957664979599813612e-03 1.979610148647829859e-03 2.004025162857546449e-03 2.031096222805385716e-03
-1.809672056753794172e-03 1.810469976433557370e-03 1.812763824172440802e-03 1.816597440546551152e-03 1.821986821851509855e-03 1.828954760692557161e-03 1.837531281344320774e-03 1.847754258610670051e-03 1.859670272244283874e-03 1.873335778609594394e-03 1.888818704333929078e-03 1.906200629441115587e-03 1.925579788269053509e-03 1.947075228509317739e-03 1.970832627818953128e-03
-1.766965918331212188e-03 1.767665747761459818e-03 1.769685301744830085e-03 1.773058239783715769e-03 1.777795192330807730e-03 1.783911270147303402e-03 1.791426319805367344e-03 1.800365295551252260e-03 1.810758786174801026e-03 1.822643757640591200e-03 1.836064591009006590e-03 1.851074542646899716e-03 1.867737802937071605e-03 1.886132418766752828e-03 1.906354475134644597e-03
-1.721571649257334176e-03 1.722170413696245310e-03 1.723907279630076039e-03 1.726805427182761697e-03 1.730869926320147004e-03 1.736107907652478539e-03 1.742528608559774103e-03 1.750143454230565065e-03 1.758966193053816468e-03 1.769013118357207334e-03 1.780303417095106507e-03 1.792859713584480730e-03 1.806708901767706699e-03 1.821883408962114877e-03 1.838423105591241316e-03
-1.673863757358931906e-03 1.674360044507296674e-03 1.675810180002264413e-03 1.678226785371349878e-03 1.681609342589914478e-03 1.685956950857638460e-03 1.691268148594056659e-03 1.697540681335420578e-03 1.704771212984210887e-03 1.712954977889959152e-03 1.722085371229652639e-03 1.732153471975749663e-03 1.743147496569864233e-03 1.755052175208650107e-03 1.767848041916919404e-03
-1.624222132061287288e-03 1.624616097152689490e-03 1.625779827705342573e-03 1.627715532915799011e-03 1.630417257236061769e-03 1.633876281372894420e-03 1.638080722355928203e-03 1.643014990972472850e-03 1.648659081921323476e-03 1.654987660128559145e-03 1.661968896389213286e-03 1.669562975117127538e-03 1.677720175888056890e-03 1.686378372281860166e-03 1.695459718557335016e-03
-1.573026295216956505e-03 1.573319617781453053e-03 1.574201517590874139e-03 1.575664158416569850e-03 1.577696473663417693e-03 1.580282400004346614e-03 1.583400274735043524e-03 1.587022010517461900e-03 1.591112003376119691e-03 1.595625708727825597e-03 1.600507800247235810e-03 1.605689774872612894e-03 1.611086826773998728e-03 1.616593714237293811e-03 1.622079217544799244e-03
-1.520649809946502881e-03 1.520845602833363359e-03 1.521454242068689738e-03 1.522458417443999694e-03 1.523842438986176048e-03 1.525583612813869805e-03 1.527651470015686406e-03 1.530006708236261075e-03 1.532599787746124782e-03 1.535369096163242486e-03 1.538238571069977479e-03 1.541114603149511351e-03 1.543881994573841673e-03 1.546398625001371447e-03 1.548488329449638134e-03
-1.467455020360966273e-03 1.467557694956860264e-03 1.467905264538094806e-03 1.468471694704080776e-03 1.469237294682027668e-03 1.470173652577444305e-03 1.471242741118776801e-03 1.472395691622093838e-03 1.473571170508354306e-03 1.474693262294071456e-03 1.475668737601237759e-03 1.476383512047826181e-03 1.476698057417431299e-03 1.476441401425437373e-03 1.475403213311288469e-03
-1.413788280847963616e-03 1.413803375417792491e-03 1.413905208787123030e-03 1.414059916270485762e-03 1.414244528899009923e-03 1.414425975250609624e-03 1.414560115701807763e-03 1.414590422818377607e-03 1.414446241740353405e-03 1.414040534913655559e-03 1.413266993447962394e-03 1.411996327975799728e-03 1.410071518898965400e-03 1.407301696540881955e-03 1.403454215296445545e-03
-1.359975808704594639e-03 1.359909789084765269e-03 1.359783806903704702e-03 1.359557165777125487e-03 1.359204401180651774e-03 1.358688926076167180e-03 1.357962046393431299e-03 1.356961622622604793e-03 1.355610317001232270e-03 1.353813341307959260e-03 1.351455600277793505e-03 1.348398074622833304e-03 1.344473260892653510e-03 1.339479411447799199e-03 1.333173252019298656e-03
-1.306320260728363299e-03 1.306180303998780027e-03 1.305846411595717191e-03 1.305272117103632246e-03 1.304430261920148416e-03 1.303281910828846474e-03 1.301775397720006475e-03 1.299845036926735534e-03 1.297409450057528156e-03 1.294369440293752270e-03 1.290605331084569924e-03 1.285973654625181687e-03 1.280303016797533196e-03 1.273389270978430438e-03 1.264988908632775667e-03
-1.253098096143456710e-03 1.252891868315648667e-03 1.252371337859134503e-03 1.251485349120936685e-03 1.250205834132667561e-03 1.248492641672350805e-03 1.246292660065485749e-03 1.243538634198143849e-03 1.240147647278350314e-03 1.236019218741965606e-03 1.231032960627192335e-03 1.225045725374708343e-03 1.217888166448630356e-03 1.209360636603959470e-03 1.199228353319397710e-03
-1.200557748484452252e-03 1.200293186708089807e-03 1.199608048116126762e-03 1.198447560028591263e-03 1.196783469951694838e-03 1.194575461647364237e-03 1.191770381163783461e-03 1.188301202857000843e-03 1.184085719853400281e-03 1.179024931080938999e-03 1.173001093718489905e-03 1.165875417662698725e-03 1.157485371566721166e-03 1.147641604785196992e-03 1.136124511314864655e-03
-1.148918591128897425e-03 1.148603699605498527e-03 1.147776175569363176e-03 1.146378654076710092e-03 1.144383343802796681e-03 1.141750693350544049e-03 1.138428736352272699e-03 1.134352233860329469e-03 1.129441604818296700e-03 1.123601636469161559e-03 1.116719967823306915e-03 1.108665358363202826e-03 1.099285750966849011e-03 1.088406192567411548e-03 1.075826704526310984e-03
-1.098370647900735004e-03 1.098013314820270011e-03 1.097065314351484879e-03 1.095467635479840766e-03 1.093193502428194651e-03 1.090204910532144474e-03 1.086452105614386932e-03 1.081872912984057928e-03 1.076391918421630524e-03 1.069919508289684552e-03 1.062350782531134609e-03 1.053564375250138794e-03 1.043421226055573020e-03 1.031763396749733105e-03 1.018413065308869554e-03
-1.049074973538519214e-03 1.048682814193585382e-03 1.047635494390033572e-03 1.045873215311699574e-03 1.043370661192392782e-03 1.040091998608860683e-03 1.035990490777450234e-03 1.031008011369030208e-03 1.025074469183472840e-03 1.018107162108493812e-03 1.010010089203949336e-03 1.000673268092084007e-03 9.899721247634098772e-04 9.777670602286346255e-04 9.639033430298345759e-04
-1.001164609950819804e-03 1.000744838966681526e-03 9.996182519631585314e-04 9.977250180730834819e-04 9.950416171606267512e-04 9.915348518662072102e-04 9.871615898314656419e-04 9.818684503339169655e-04 9.755914528086318893e-04 9.682556530332948712e-04 9.597748048031389976e-04 9.500510992924426912e-04 9.389750630633232143e-04 9.264257118303388487e-04 9.122711119771103987e-04
-9.547460132393893175e-04 9.543053468078038478e-04 9.531181691323588117e-04 9.511252652567187557e-04 9.483051417141900603e-04 9.446275501507430707e-04 9.400533448592140410e-04 9.345343231955585261e-04 9.280130695222427737e-04 9.204228324409832827e-04 9.116874764019445871e-04 9.017215614476136289e-04 8.904306313931120535e-04 8.777117991538393353e-04 8.634547656784031036e-04
-9.099008429463824538e-04 9.094454302024490133e-04 9.082147730035609705e-04 9.061508125134910482e-04 9.032342174087716960e-04 8.994378637587847674e-04 8.947267919681494656e-04 8.890581775679442600e-04 8.823813377886336601e-04 8.746378044583467742e-04 8.657615037155299469e-04 8.556790942608809248e-04 8.443105353375904721e-04 8.315699642329165949e-04 8.173669938254621726e-04
-8.666880077795851428e-04 8.662233891058414639e-04 8.649646829591009153e-04 8.628554233099981026e-04 8.598784929778046380e-04 8.560099491162338715e-04 8.512190619266758740e-04 8.454683908890334252e-04 8.387139200207707670e-04 8.309052812556216036e-04 8.219861031713711049e-04 8.118945323649555748e-04 8.005639841771459335e-04 7.879241971349862459e-04 7.739026658342824895e-04
+8.251458698098414505e-04 8.246769589162286380e-04 8.234039043558003196e-04 8.212721733606382973e-04 8.182668452132121385e-04 8.143671167745807592e-04 8.095464051753534099e-04 8.037725049410900406e-04 7.970078194015538459e-04 7.892096925689142447e-04 7.803308740403520080e-04 7.703201569929625861e-04 7.591232350217194278e-04 7.466838371619741220e-04 7.329451935972345266e-04
+8.666880077794763973e-04 8.662233891057375974e-04 8.649646829590024698e-04 8.628554233099085475e-04 8.598784929777047829e-04 8.560099491161493037e-04 8.512190619265760190e-04 8.454683908889397501e-04 8.387139200206762246e-04 8.309052812555254349e-04 8.219861031712825256e-04 8.118945323648632008e-04 8.005639841770494395e-04 7.879241971348899688e-04 7.739026658341767798e-04
+9.099008429463485183e-04 9.094454302024174630e-04 9.082147730035228066e-04 9.061508125134442107e-04 9.032342174087134743e-04 8.994378637587281721e-04 8.947267919680939544e-04 8.890581775678933025e-04 8.823813377885848710e-04 8.746378044582922388e-04 8.657615037154720505e-04 8.556790942608376652e-04 8.443105353375451524e-04 8.315699642328702994e-04 8.173669938254197803e-04
+9.547460132392979193e-04 9.543053468077052938e-04 9.531181691322979880e-04 9.511252652566476321e-04 9.483051417141248997e-04 9.446275501506826806e-04 9.400533448591558193e-04 9.345343231955019307e-04 9.280130695221833594e-04 9.204228324409187726e-04 9.116874764018822455e-04 9.017215614475613704e-04 8.904306313930435320e-04 8.777117991537690790e-04 8.634547656783294863e-04
+1.001164609950772532e-03 1.000744838966615823e-03 9.996182519631060560e-04 9.977250180730253687e-04 9.950416171605788295e-04 9.915348518661501812e-04 9.871615898314125160e-04 9.818684503338677427e-04 9.755914528085739930e-04 9.682556530332358906e-04 9.597748048030894496e-04 9.500510992923891316e-04 9.389750630632696547e-04 9.264257118302860481e-04 9.122711119770747284e-04
+1.049074973538484086e-03 1.048682814193480214e-03 1.047635494389912575e-03 1.045873215311582480e-03 1.043370661192264846e-03 1.040091998608721905e-03 1.035990490777310589e-03 1.031008011368883407e-03 1.025074469183329725e-03 1.018107162108353517e-03 1.010010089203796247e-03 1.000673268091927665e-03 9.899721247632539689e-04 9.777670602284787172e-04 9.639033430296588267e-04
+1.098370647900580180e-03 1.098013314820221655e-03 1.097065314351421562e-03 1.095467635479777666e-03 1.093193502428132851e-03 1.090204910532094167e-03 1.086452105614331854e-03 1.081872912983997863e-03 1.076391918421576313e-03 1.069919508289635546e-03 1.062350782531073460e-03 1.053564375250083283e-03 1.043421226055517943e-03 1.031763396749678461e-03 1.018413065308820765e-03
+1.148918591128879211e-03 1.148603699605396829e-03 1.147776175569215074e-03 1.146378654076584324e-03 1.144383343802659204e-03 1.141750693350404187e-03 1.138428736352133487e-03 1.134352233860187005e-03 1.129441604818144694e-03 1.123601636469013457e-03 1.116719967823146236e-03 1.108665358363047134e-03 1.099285750966683562e-03 1.088406192567250219e-03 1.075826704526137729e-03
+1.200557748484297211e-03 1.200293186708070291e-03 1.199608048116102476e-03 1.198447560028561556e-03 1.196783469951667733e-03 1.194575461647333012e-03 1.191770381163758307e-03 1.188301202856967232e-03 1.184085719853381416e-03 1.179024931080912544e-03 1.173001093718464751e-03 1.165875417662684630e-03 1.157485371566711625e-03 1.147641604785184415e-03 1.136124511314853596e-03
+1.253098096143418329e-03 1.252891868315510757e-03 1.252371337859033672e-03 1.251485349120837372e-03 1.250205834132558707e-03 1.248492641672240651e-03 1.246292660065379280e-03 1.243538634198036296e-03 1.240147647278242327e-03 1.236019218741851765e-03 1.231032960627075892e-03 1.225045725374593200e-03 1.217888166448511094e-03 1.209360636603841509e-03 1.199228353319265654e-03
+1.306320260728286537e-03 1.306180303998706518e-03 1.305846411595629588e-03 1.305272117103545076e-03 1.304430261920048670e-03 1.303281910828748679e-03 1.301775397719914318e-03 1.299845036926637089e-03 1.297409450057432747e-03 1.294369440293647103e-03 1.290605331084471695e-03 1.285973654625076519e-03 1.280303016797418271e-03 1.273389270978323102e-03 1.264988908632659658e-03
+1.359975808704555825e-03 1.359909789084633646e-03 1.359783806903593247e-03 1.359557165777019235e-03 1.359204401180540535e-03 1.358688926076052255e-03 1.357962046393332203e-03 1.356961622622503963e-03 1.355610317001121898e-03 1.353813341307849973e-03 1.351455600277676194e-03 1.348398074622721848e-03 1.344473260892519936e-03 1.339479411447671046e-03 1.333173252019167251e-03
+1.413788280847893576e-03 1.413803375417640919e-03 1.413905208787005286e-03 1.414059916270368669e-03 1.414244528898890877e-03 1.414425975250449379e-03 1.414560115701654023e-03 1.414590422818240130e-03 1.414446241740222867e-03 1.414040534913557981e-03 1.413266993447817761e-03 1.411996327975689356e-03 1.410071518898813828e-03 1.407301696540673788e-03 1.403454215296332137e-03
+1.467455020361010942e-03 1.467557694956730160e-03 1.467905264537987253e-03 1.468471694703994473e-03 1.469237294681922283e-03 1.470173652577304660e-03 1.471242741118637155e-03 1.472395691621981731e-03 1.473571170508245235e-03 1.474693262293995779e-03 1.475668737601112642e-03 1.476383512047740095e-03 1.476698057417306182e-03 1.476441401425265419e-03 1.475403213311188939e-03
+1.520649809946401617e-03 1.520845602833211570e-03 1.521454242068595629e-03 1.522458417443907537e-03 1.523842438986079770e-03 1.525583612813727992e-03 1.527651470015551098e-03 1.530006708236136825e-03 1.532599787746009856e-03 1.535369096163139054e-03 1.538238571069847158e-03 1.541114603149409002e-03 1.543881994573738890e-03 1.546398625001165665e-03 1.548488329449515186e-03
+1.573026295216811872e-03 1.573319617781321431e-03 1.574201517590846167e-03 1.575664158416537324e-03 1.577696473663376710e-03 1.580282400004270286e-03 1.583400274734963944e-03 1.587022010517392945e-03 1.591112003376060928e-03 1.595625708727786782e-03 1.600507800247186370e-03 1.605689774872599883e-03 1.611086826773961431e-03 1.616593714237170862e-03 1.622079217544768453e-03
+1.624222132061147860e-03 1.624616097152548544e-03 1.625779827705265811e-03 1.627715532915717913e-03 1.630417257235958770e-03 1.633876281372745667e-03 1.638080722355794629e-03 1.643014990972341662e-03 1.648659081921209418e-03 1.654987660128463085e-03 1.661968896389090771e-03 1.669562975117044488e-03 1.677720175887938711e-03 1.686378372281656986e-03 1.695459718557214670e-03
+1.673863757358857313e-03 1.674360044507218178e-03 1.675810180002196541e-03 1.678226785371286995e-03 1.681609342589853980e-03 1.685956950857529823e-03 1.691268148593946504e-03 1.697540681335326252e-03 1.704771212984126753e-03 1.712954977889893883e-03 1.722085371229575227e-03 1.732153471975712367e-03 1.743147496569791809e-03 1.755052175208482489e-03 1.767848041916845678e-03
+1.721571649257314226e-03 1.722170413696109134e-03 1.723907279629990821e-03 1.726805427182696862e-03 1.730869926320061786e-03 1.736107907652344098e-03 1.742528608559642265e-03 1.750143454230455994e-03 1.758966193053722793e-03 1.769013118357117128e-03 1.780303417094997436e-03 1.792859713584412425e-03 1.806708901767612807e-03 1.821883408961924274e-03 1.838423105591144389e-03
+1.766965918331123500e-03 1.767665747761376117e-03 1.769685301744785633e-03 1.773058239783686279e-03 1.777795192330759808e-03 1.783911270147216666e-03 1.791426319805287330e-03 1.800365295551183955e-03 1.810758786174753322e-03 1.822643757640557589e-03 1.836064591008958885e-03 1.851074542646884103e-03 1.867737802937030189e-03 1.886132418766625109e-03 1.906354475134612722e-03
+1.809672056753726518e-03 1.810469976433477140e-03 1.812763824172409794e-03 1.816597440546523397e-03 1.821986821851462584e-03 1.828954760692474328e-03 1.837531281344237290e-03 1.847754258610599144e-03 1.859670272244223158e-03 1.873335778609562952e-03 1.888818704333870098e-03 1.906200629441091301e-03 1.925579788269001901e-03 1.947075228509197176e-03 1.970832627818915831e-03
+1.849326670415565388e-03 1.850218193838873166e-03 1.852773732519716809e-03 1.857046807181638804e-03 1.863058440193090647e-03 1.870838594919444322e-03 1.880426750738993687e-03 1.891872709593812050e-03 1.905237692553480222e-03 1.920595817862651719e-03 1.938036075232759010e-03 1.957664979599794963e-03 1.979610148647779552e-03 2.004025162857414610e-03 2.031096222805339746e-03
+1.885583028627639242e-03 1.886562248144303764e-03 1.889362921268414753e-03 1.894047569729277909e-03 1.900641787271190953e-03 1.909182030928746479e-03 1.919716290025430235e-03 1.932305013572191811e-03 1.947022353415392730e-03 1.963957813310643775e-03 1.983218412362030940e-03 2.004931537870078065e-03 2.029248712453247429e-03 2.056350599860823532e-03 2.086453700160030914e-03
+1.918116286151698349e-03 1.919175995725268908e-03 1.922201637365450900e-03 1.927263905987400359e-03 1.934392431655961248e-03 1.943629375209783485e-03 1.955030145659780207e-03 1.968664382348139438e-03 1.984617251285630910e-03 2.002991134740733301e-03 2.023907802176880613e-03 2.047511209539727272e-03 2.073971104238593859e-03 2.103487686473634252e-03 2.136297658746102480e-03
+1.946628260168638963e-03 1.947760101276158453e-03 1.950987344405636552e-03 1.956387912742993569e-03 1.963994892076981018e-03 1.973855297655985417e-03 1.986030799610417549e-03 2.000598702051894183e-03 2.017653212348290322e-03 2.037307060701269885e-03 2.059693528848203538e-03 2.084968992581211211e-03 2.113316091190043430e-03 2.144947678882585911e-03 2.180111746132030494e-03
+1.970851676955009003e-03 1.972046298498980176e-03 1.975449021696814699e-03 1.981143966681413182e-03 1.989167080050726483e-03 1.999569369845228314e-03 2.012417607834316152e-03 2.027795261868410841e-03 2.045803678643034682e-03 2.066563554592200716e-03 2.090216718497967495e-03 2.116928283247282959e-03 2.146889209010560944e-03 2.180319333071353491e-03 2.217470911600913277e-03
+1.990553835765599463e-03 1.991801059719903143e-03 1.995350849010493754e-03 2.001292430324060675e-03 2.009664026398335322e-03 2.020519800902447795e-03 2.033930518121115655e-03 2.049984402333661099e-03 2.068788200525908168e-03 2.090468462404398899e-03 2.115173026855511011e-03 2.143072724861307034e-03 2.174363274478474141e-03 2.209267331966561880e-03 2.248036621017933823e-03
+2.005539667162678594e-03 2.006828653334513657e-03 2.010495260631411148e-03 2.016632695138896939e-03 2.025280897255648214e-03 2.036496396697536852e-03 2.050352922584332792e-03 2.066942182080880319e-03 2.086374795888889296e-03 2.108781383012384939e-03 2.134313753331580372e-03 2.163146176715345821e-03 2.195476647991373691e-03 2.231528037794875286e-03 2.271548956073307299e-03
+2.015654186925639000e-03 2.016973592397941061e-03 2.020725378208300740e-03 2.027005582416657129e-03 2.035855337429671921e-03 2.047332805639322413e-03 2.061513744528055588e-03 2.078492213792605941e-03 2.098381400555690470e-03 2.121314538079580470e-03 2.147445765415646659e-03 2.176951476486784810e-03 2.210030202192586439e-03 2.246903918692757032e-03 2.287817487002487531e-03
+2.020784362822819393e-03 2.022122494029662126e-03 2.025926848816993631e-03 2.032295140339129575e-03 2.041269198068017786e-03 2.052908135011531458e-03 2.067288881804483624e-03 2.084506845110233389e-03 2.104676658558048575e-03 2.127932990795242639e-03 2.154431330435694052e-03 2.184348665516483955e-03 2.217883909333648231e-03 2.255257877714510542e-03 2.296712541958686061e-03
+2.020860419191701941e-03 2.022205376841533248e-03 2.026029121821792175e-03 2.032429882145843879e-03 2.041449710903682577e-03 2.053148025149760612e-03 2.067602128989530410e-03 2.084907854776172145e-03 2.105180287943673144e-03 2.128554536341000208e-03 2.155186458742850905e-03 2.185253263512038427e-03 2.218953820715789237e-03 2.256508482283080177e-03 2.298158122377806471e-03
+2.015856603889891983e-03 2.017196422797203677e-03 2.021006196141092188e-03 2.027383506202150732e-03 2.036370163913169516e-03 2.048025256414798441e-03 2.062425681233793443e-03 2.079666804795963792e-03 2.099863213498809767e-03 2.123149521922308713e-03 2.149681157958517868e-03 2.179635042471190706e-03 2.213210015355597613e-03 2.250626813054844300e-03 2.292127321764030490e-03
+2.005791435208866165e-03 2.007114222298962605e-03 2.010876860098461619e-03 2.017175126127835564e-03 2.026050115640361162e-03 2.037559939188944048e-03 2.051780287905830263e-03 2.068805140850065935e-03 2.088747590490255390e-03 2.111740761735981121e-03 2.137938671950537998e-03 2.167517580440400486e-03 2.200675871009370125e-03 2.237635360731377900e-03 2.278640740073223370e-03
+1.990727435085318762e-03 1.992021509254041350e-03 1.995704431785053513e-03 2.001869020982320786e-03 2.010555161326400830e-03 2.021819304512202566e-03 2.035735079798836264e-03 2.052394072987227727e-03 2.071906762320368817e-03 2.094403603727299380e-03 2.120036223944011828e-03 2.148978690238794245e-03 2.181428776058709929e-03 2.217609112615274471e-03 2.257768053183481765e-03
+1.970770342195867289e-03 1.972024379289131525e-03 1.975595991928352085e-03 1.981573895431500143e-03 1.989996237626753296e-03 2.000917077664311674e-03 2.014407046053391746e-03 2.030554204492317130e-03 2.049465109127868515e-03 2.071266091211314969e-03 2.096104744290768450e-03 2.124151627948849940e-03 2.155602163688488497e-03 2.190678687049116106e-03 2.229632577902079110e-03
+1.946067787259117381e-03 1.947270972233699441e-03 1.950701087003350485e-03 1.956441621655351064e-03 1.964528428582713263e-03 1.975012384385245803e-03 1.987960092599978020e-03 2.003454816621003456e-03 2.021597663152793940e-03 2.042509053911526797e-03 2.066330509157636528e-03 2.093226800487376152e-03 2.123388515153039075e-03 2.157035087136731279e-03 2.194418340266112658e-03
+1.916807405905087509e-03 1.917949592384575377e-03 1.921209870900817719e-03 1.926665422113979769e-03 1.934349217929998187e-03 1.944308114701408588e-03 1.956603579187025932e-03 1.971312668338312014e-03 1.988529299408615253e-03 2.008365870508461992e-03 2.030955290424822732e-03 2.056453522392483624e-03 2.085042754919108621e-03 2.116935354711625868e-03 2.152378789647286725e-03
+1.883214364078713600e-03 1.884286239258943160e-03 1.887350651482812671e-03 1.892477448182766989e-03 1.899696125400118004e-03 1.909048656976860062e-03 1.920590212587321892e-03 1.934390140706961298e-03 1.950533265932545470e-03 1.969121579723994830e-03 1.990276412657982028e-03 2.014141235191183477e-03 2.040885264271593419e-03 2.070708126439874293e-03 2.103845909254500705e-03
+1.845548278614837388e-03 1.846541529083474669e-03 1.849386815531936859e-03 1.854145716148014123e-03 1.860843669966138819e-03 1.869516918162874176e-03 1.880213173787014663e-03 1.892992550094494937e-03 1.907928804832820539e-03 1.925110990646815290e-03 1.944645620040722379e-03 1.966659519932477222e-03 1.991303600659522811e-03 2.018757863844301143e-03 2.049238099795281515e-03
+1.804099531761965821e-03 1.805007003615737449e-03 1.807613122505003769e-03 1.811970379883382333e-03 1.818099622092930008e-03 1.826030566900103871e-03 1.835802379345589756e-03 1.847464479362165030e-03 1.861077639633489014e-03 1.876715465159661594e-03 1.894466369284661693e-03 1.914436229399032368e-03 1.936751966611542771e-03 1.961566408137799689e-03 1.989064947124056289e-03
+1.759185002327844213e-03 1.760000847309334086e-03 1.762351383389695750e-03 1.766279347976510610e-03 1.771800539303823195e-03 1.778937473635091400e-03 1.787719821562774305e-03 1.798185028070422827e-03 1.810379168411896823e-03 1.824358121485556740e-03 1.840189165441805759e-03 1.857953163009741851e-03 1.877747564836161273e-03 1.899690571164470423e-03 1.923926951246277125e-03
+1.711143265856406373e-03 1.711863064382343307e-03 1.713945573771701730e-03 1.717423289864138157e-03 1.722306622206089656e-03 1.728610373345002265e-03 1.736353995381663753e-03 1.745561963176420423e-03 1.756264302849554464e-03 1.768497336324611991e-03 1.782304721435648380e-03 1.797738914589028757e-03 1.814863232179411440e-03 1.833754776028884972e-03 1.854508618055040027e-03
+1.660329348971716209e-03 1.660950201058331022e-03 1.662756466726253825e-03 1.665770117008214110e-03 1.669995977214895014e-03 1.675440836609340661e-03 1.682113495697179538e-03 1.690024848755202879e-03 1.699188021032658601e-03 1.709618592611307237e-03 1.721334949519361503e-03 1.734358830187784483e-03 1.748716160717489433e-03 1.764438321904596629e-03 1.781564062303676779e-03
+1.607109155181324182e-03 1.607629731463947314e-03 1.609155907342714551e-03 1.611699066649055273e-03 1.615258421951132296e-03 1.619832696568901820e-03 1.625419947854159870e-03 1.632017336730821541e-03 1.639620840940176705e-03 1.648224909462619146e-03 1.657822055574659226e-03 1.668402382819162257e-03 1.679953041994911760e-03 1.692457611058567537e-03 1.705895388812125749e-03
+1.551853707293184264e-03 1.552274254496153073e-03 1.553520882266885058e-03 1.555594552190912123e-03 1.558489013454915275e-03 1.562195134810233886e-03 1.566700506050904820e-03 1.571988897252345630e-03 1.578039551116204153e-03 1.584826271856277840e-03 1.592316263779455397e-03 1.600468642333162427e-03 1.609232519290833361e-03 1.618544505540280400e-03 1.628325401803409683e-03
+1.494933371704918737e-03 1.495255669824021357e-03 1.496227560621062307e-03 1.497839971017554932e-03 1.500081512080902535e-03 1.502935670759257113e-03 1.506380208777550675e-03 1.510386339352835826e-03 1.514917637586363653e-03 1.519928619303704490e-03 1.525362903135399741e-03 1.531150819129831891e-03 1.537206286707214122e-03 1.543422685752415596e-03 1.549667319410873633e-03
+1.436712239518824841e-03 1.436939511304332348e-03 1.437645493957037147e-03 1.438811673974016046e-03 1.440422010645720429e-03 1.442453320745515225e-03 1.444874509086591964e-03 1.447645512256516944e-03 1.450715897297258404e-03 1.454023029489721246e-03 1.457489698474857993e-03 1.461021025323274792e-03 1.464500425269550351e-03 1.467784278220837834e-03 1.470694812369525420e-03
+1.377542837235524661e-03 1.377679613915289408e-03 1.378132160793373419e-03 1.378873298789222174e-03 1.379882956549467266e-03 1.381132191197253318e-03 1.382582295899973182e-03 1.384183576167301137e-03 1.385873729204013935e-03 1.387575730228747528e-03 1.389195104292300677e-03 1.390616389443650623e-03 1.391698552625942427e-03 1.392268994269549613e-03 1.392115640647335071e-03
+1.317761325589869928e-03 1.317813275760601347e-03 1.318028025705189881e-03 1.318370652156215230e-03 1.318817774151089276e-03 1.319335745458521990e-03 1.319879690804966763e-03 1.320392188792774259e-03 1.320801535357347132e-03 1.321019492105433108e-03 1.320938401801264586e-03 1.320427483861510423e-03 1.319328089728315093e-03 1.317447588154422103e-03 1.314551447331831040e-03
+1.257683320184494477e-03 1.257657051103659197e-03 1.257652255382961685e-03 1.257627294238009051e-03 1.257556258038178667e-03 1.257401938737838553e-03 1.257114847491131024e-03 1.256631878975900986e-03 1.255874561901204741e-03 1.254746810700376781e-03 1.253132073410955817e-03 1.250889719710844344e-03 1.247850486196950322e-03 1.243810722486782564e-03 1.238525116661686257e-03
+1.197600434397629249e-03 1.197503276306121148e-03 1.197299197426441924e-03 1.196940938000089346e-03 1.196400859370603349e-03 1.195639356553527231e-03 1.194603906256878163e-03 1.193227781162324976e-03 1.191428380339047601e-03 1.189105107748022073e-03 1.186136715755305030e-03 1.182377999025047447e-03 1.177655665185452834e-03 1.171763516009717522e-03 1.164455844788313092e-03
+1.137777606807366046e-03 1.137617391321166065e-03 1.137235686672057001e-03 1.136580728797407505e-03 1.135623932748514378e-03 1.134324426012956388e-03 1.132628173789673514e-03 1.130466799170929196e-03 1.127756068758447010e-03 1.124393995098857272e-03 1.120258498248184525e-03 1.115204559406922976e-03 1.109060787617758594e-03 1.101625326583991361e-03 1.092661025967496145e-03
+1.078451235604399290e-03 1.078236078682947956e-03 1.077699193033307976e-03 1.076785421604202963e-03 1.075465955867025347e-03 1.073699703801068647e-03 1.071432518576588989e-03 1.068596167982054047e-03 1.065107029027065073e-03 1.060864479841421059e-03 1.055748957704735411e-03 1.049619659789875628e-03 1.042311855615757907e-03 1.033633818950223555e-03 1.023363396283954877e-03
+1.019828104536592674e-03 1.019566203215448337e-03 1.018896805443319066e-03 1.017762428523536714e-03 1.016134683758807737e-03 1.013973186286451587e-03 1.011224903022049084e-03 1.007823298702722201e-03 1.003687270793935304e-03 9.987198651245274804e-04 9.928067653396685337e-04 9.858145682363746252e-04 9.775888541349534583e-04 9.679521172606573524e-04 9.567016415238794973e-04
+9.620850516426729957e-04 9.617845018533785484e-04 9.610049803238944390e-04 9.596876712287806489e-04 9.578051576341384309e-04 9.553185403094160543e-04 9.521769201413899470e-04 9.483167310409493928e-04 9.436609256758515373e-04 9.381180211776421517e-04 9.315810185546584713e-04 9.239262302301885820e-04 9.150120602441577395e-04 9.046778294481945884e-04 8.927427771850545649e-04
+9.053693054086738804e-04 9.050379460414595010e-04 9.041699723338392268e-04 9.027061439579851538e-04 9.006204575929677289e-04 8.978761204922604093e-04 8.944251680311189829e-04 8.902079816905769834e-04 8.851527188049897578e-04 8.791746725024526333e-04 8.721755906506078408e-04 8.640430005770801530e-04 8.546496090723368052e-04 8.438528764799577012e-04 8.314949193207842168e-04
+8.497993940898093288e-04 8.494446802417765160e-04 8.485088581960423216e-04 8.469330735810046964e-04 8.446930695156063635e-04 8.417546206610132574e-04 8.380732789082404131e-04 8.335940644548863084e-04 8.282511197393107065e-04 8.219673520015179395e-04 8.146541022904140372e-04 8.062108925005591559e-04 7.965253352310837451e-04 7.854732931066957810e-04 7.729194544071608291e-04
+7.954665230042112182e-04 7.950954293017368493e-04 7.941110266100921819e-04 7.924555538746014174e-04 7.901067287194884527e-04 7.870332020010236806e-04 7.831944190218434508e-04 7.785404646656672546e-04 7.730119131062580199e-04 7.665397118268190606e-04 7.590451410440107478e-04 7.504399016431731982e-04 7.406264161180226143e-04 7.294984192464360438e-04 7.169419933516427146e-04
+7.424363110640048134e-04 7.420552642031228493e-04 7.410400250195011123e-04 7.393345304352662599e-04 7.369186048997567297e-04 7.337639464667524260e-04 7.298340876400088084e-04 7.250843711711511862e-04 7.194619627536875516e-04 7.129059311365471040e-04 7.053474359190020073e-04 6.967100757745934301e-04 6.869104672987653244e-04 6.758591310557412460e-04 6.634618054990986920e-04
+6.907507806086690249e-04 6.903656189020747390e-04 6.893356511725398390e-04 6.876070189156834912e-04 6.851617020590673431e-04 6.819744978334363805e-04 6.780130636140720059e-04 6.732379984513303271e-04 6.676029848135132862e-04 6.610550196156128643e-04 6.535347713469783631e-04 6.449771131345744370e-04 6.353118823230551699e-04 6.244649475013102973e-04 6.123596564961263783e-04
+6.404305023389528706e-04 6.400464591139161732e-04 6.390161877883018988e-04 6.372884506734806994e-04 6.348473619586192341e-04 6.316707717250103675e-04 6.277303729845899998e-04 6.229918644088555148e-04 6.174151885794727400e-04 6.109548719647605198e-04 6.035604985275023213e-04 5.951773612377977149e-04 5.857473255083037568e-04 5.752099813500763164e-04 5.635041223529441189e-04
+5.914768083434077941e-04 5.910985155034153161e-04 5.900806913086614541e-04 5.883750545250177781e-04 5.859677767408342586e-04 5.828396372671271241e-04 5.789661775589388919e-04 5.743179223866309120e-04 5.688606851677967648e-04 5.625559799583659294e-04 5.553615666289822171e-04 5.472321658068702221e-04 5.381203668995364732e-04 5.279777921317748909e-04 5.167565359090661985e-04
+5.438739994238936349e-04 5.435055072816418311e-04 5.425112602468710066e-04 5.408461994402817725e-04 5.384984350463658956e-04 5.354514946564217738e-04 5.316845099706622030e-04 5.271724763472063766e-04 5.218865998337880513e-04 5.157947501279653603e-04 5.088620409363449251e-04 5.010515654288314391e-04 4.923253039941393773e-04 4.826452488971144780e-04 4.719747587418391646e-04
+4.975914869242597290e-04 4.972362964928813203e-04 4.962752236625273157e-04 4.946666393114258981e-04 4.924004439931790704e-04 4.894626932960435915e-04 4.858358038910168502e-04 4.814988344166489117e-04 4.764278533685720120e-04 4.705964078518263052e-04 4.639761118750245481e-04 4.565373682031870391e-04 4.482502459709036650e-04 4.390855333596682003e-04 4.290159773036692913e-04
+4.525858230454243261e-04 4.522469272582233901e-04 4.513272048257518563e-04 4.497886163377565042e-04 4.476226860108765276e-04 4.448177533640526398e-04 4.413591878548896847e-04 4.372296775070613284e-04 4.324096009525286522e-04 4.268774929043003146e-04 4.206106193914537351e-04 4.135856636984008221e-04 4.057795526260579710e-04 3.971704183928681693e-04 3.877387095157515374e-04
+4.088025864557237664e-04 4.084825171777391618e-04 4.076110284148096738e-04 4.061537962157800745e-04 4.041037841003404865e-04 4.014513688180819124e-04 3.981845273340137441e-04 3.942891364484272967e-04 3.897493336754723962e-04 3.845479656923953557e-04 3.786671346584129043e-04 3.720888360630756155e-04 3.647957187680574490e-04 3.567719481456676405e-04 3.480041862101205218e-04
+3.661781014089101759e-04 3.658789795868573592e-04 3.650614512606466006e-04 3.636949979930803383e-04 3.617738612968255480e-04 3.592901827011771147e-04 3.562342122291575655e-04 3.525945834125655104e-04 3.483586594824245627e-04 3.435129554201575672e-04 3.380436449638378731e-04 3.319371443429771089e-04 3.251807968642220150e-04 3.177636375810780349e-04 3.096772468923459330e-04
+3.246409782942680320e-04 3.243645650778387421e-04 3.236057064104186343e-04 3.223377690481936311e-04 3.205560899229093950e-04 3.182543348859602364e-04 3.154246963277513942e-04 3.120581519428746635e-04 3.081447874923173911e-04 3.036741867267053123e-04 2.986358927397488820e-04 2.930199352208979514e-04 2.868174373231752064e-04 2.800212851456496945e-04 2.726268631367378525e-04
+2.841134715040255563e-04 2.838612186431061142e-04 2.831648581724067549e-04 2.820017078697979198e-04 2.803680337459021465e-04 2.782587897622083536e-04 2.756678015377665540e-04 2.725880053521371766e-04 2.690117436651322312e-04 2.649311210802703098e-04 2.603384145864280543e-04 2.552265477837587816e-04 2.495896195977851729e-04 2.434234854189369157e-04 2.367263845588781055e-04
+2.445126567533678955e-04 2.442857550077232346e-04 2.436549718963621587e-04 2.426016376098950075e-04 2.411227916665758815e-04 2.392144562526556280e-04 2.368718042037406993e-04 2.340893763286715278e-04 2.308613479053047281e-04 2.271818496554213972e-04 2.230453272386655303e-04 2.184469634061331786e-04 2.133831338422876082e-04 2.078519070475758827e-04 2.018535754700970784e-04
+2.057514346839375288e-04 2.055508593539987503e-04 2.049881067211617165e-04 2.040485820436908546e-04 2.027299553395512993e-04 2.010291157159254782e-04 1.989423227816309529e-04 1.964654015708122714e-04 1.935939800541375505e-04 1.903237736254135952e-04 1.866508999053671130e-04 1.825722468359384208e-04 1.780858647206217131e-04 1.731913919432377961e-04 1.678905015707670638e-04
+1.677393709016404566e-04 1.675659239060235716e-04 1.670731426194220547e-04 1.662505761396521834e-04 1.650963954831956640e-04 1.636081750395667266e-04 1.617830272963269615e-04 1.596177755249909055e-04 1.571091631101663541e-04 1.542541024367952293e-04 1.510499488591195822e-04 1.474948176990055059e-04 1.435879192005602646e-04 1.393299183989850289e-04 1.347233083924795263e-04
+1.303833847869339255e-04 1.302377329604582034e-04 1.298164550147091979e-04 1.291133228796028103e-04 1.281268928697863253e-04 1.268552628879221695e-04 1.252961908583286000e-04 1.234472459478354474e-04 1.213059912462056055e-04 1.188701982495401078e-04 1.161380851384717308e-04 1.131085852862748106e-04 1.097816323532422905e-04 1.061584621964546481e-04 1.022419230582611731e-04
+9.358830066280916956e-05 9.347101014423866636e-05 9.312245128547386847e-05 9.254071151545681438e-05 9.172463037113417540e-05 9.067268694515995080e-05 8.938310276337222836e-05 8.785397229974948935e-05 8.608342270266527855e-05 8.406979260404763208e-05 8.181184167578380408e-05 7.930897381346432200e-05 7.656147842419969911e-05 7.357078202165191836e-05 7.033970448719742473e-05
+5.725727544112534307e-05 5.716884216268585273e-05 5.689398381046474726e-05 5.643521255392407122e-05 5.579156336524751362e-05 5.496176932857888778e-05 5.394436149864236484e-05 5.273776844719843835e-05 5.134046061299682039e-05 4.975109601418239557e-05 4.796870204775234212e-05 4.599286041134816294e-05 4.382390880331946831e-05 4.146314924551418725e-05 3.891305848935310924e-05
+2.129211686649679818e-05 2.123299325439570597e-05 2.103265404360041472e-05 2.069816439181894829e-05 2.022867587449354526e-05 1.962307633579908625e-05 1.888006453276198953e-05 1.799824381183061798e-05 1.697623917972999175e-05 1.581281930068229749e-05 1.450704933154879147e-05 1.305844391088600200e-05 1.146713387985012340e-05 9.734037234630945170e-06 7.861030643460562391e-06
+-1.440649389465464988e-05 -1.443587583953417143e-05 -1.456097840369679018e-05 -1.477003415183902165e-05 -1.506383860549017611e-05 -1.544344250763266961e-05 -1.591008977484926562e-05 -1.646513967851507423e-05 -1.710997046960057008e-05 -1.784587771192213410e-05 -1.867394957512224718e-05 -1.959494103497409529e-05 -2.060913799107734769e-05 -2.171621851051804296e-05 -2.291511441405959997e-05
+-4.993886218580856926e-05 -4.993807122629218665e-05 -4.998726841844141890e-05 -5.006981201852406076e-05 -5.018649865969006843e-05 -5.033839240359135557e-05 -5.052677434495561214e-05 -5.075307912515162809e-05 -5.101881875943348025e-05 -5.132549679816863044e-05 -5.167451150356616740e-05 -5.206705289335755553e-05 -5.250399421297087733e-05 -5.298578110360325420e-05 -5.351232143559763344e-05
+-8.540620991632370525e-05 -8.537479913057319692e-05 -8.534742735364915338e-05 -8.530238235257302834e-05 -8.524050580114665699e-05 -8.516293579491766613e-05 -8.507106728196758057e-05 -8.496650218660608731e-05 -8.485099002423287119e-05 -8.472636003168834251e-05 -8.459444608352319846e-05 -8.445700593336045981e-05 -8.431563659504478039e-05 -8.417168796051261793e-05 -8.402617701758739472e-05
+-1.209106641247415350e-04 -1.208481574785967376e-04 -1.207435227302769572e-04 -1.205697556782260257e-04 -1.203277775530263075e-04 -1.200188481634777398e-04 -1.196445370974342311e-04 -1.192066835515699440e-04 -1.187073583229396930e-04 -1.181488071321545500e-04 -1.175333977856873793e-04 -1.168635593509887403e-04 -1.161417189790768479e-04 -1.153702372764369035e-04 -1.145513439316296037e-04
+-1.565552931869003839e-04 -1.564611749615053989e-04 -1.562785249007092527e-04 -1.559747991527104453e-04 -1.555510241587658373e-04 -1.550086165512229355e-04 -1.543493660843369938e-04 -1.535754022287723764e-04 -1.526891779206906194e-04 -1.516934234566749164e-04 -1.505911139146826950e-04 -1.493854269728713186e-04 -1.480796994452694606e-04 -1.466773824614752829e-04 -1.451819963618798605e-04
+-1.924441804774647627e-04 -1.923178874260749079e-04 -1.920563906143199614e-04 -1.916213319951874726e-04 -1.910138604166166396e-04 -1.902355729499097356e-04 -1.892885095051310594e-04 -1.881751272032365847e-04 -1.868983007577532140e-04 -1.854612917905097962e-04 -1.838677327090856991e-04 -1.821216028743003271e-04 -1.802272037677303442e-04 -1.781891327570095797e-04 -1.760122559122367361e-04
+-2.286825258493162564e-04 -2.285234420042491269e-04 -2.281821740092853659e-04 -2.276142478082074730e-04 -2.268209436347389787e-04 -2.258040528480134224e-04 -2.245658769211920491e-04 -2.231092252898448118e-04 -2.214374140849688973e-04 -2.195542619824468911e-04 -2.174640866034459894e-04 -2.151716991230857075e-04 -2.126823976298154479e-04 -2.100019589617819690e-04 -2.071366288614144840e-04
+-2.653767657021930044e-04 -2.651842198079255647e-04 -2.647621559844883302e-04 -2.640596549626567828e-04 -2.630781291883877208e-04 -2.618195647629449011e-04 -2.602865297397267833e-04 -2.584821842514476863e-04 -2.564102920689146194e-04 -2.540752331115198699e-04 -2.514820163513785596e-04 -2.486362924860387484e-04 -2.455443656913148414e-04 -2.422132037165570986e-04 -2.386504455461522730e-04
+-3.026347026527138212e-04 -3.024079682576613659e-04 -3.019039831593902843e-04 -3.010650264873046913e-04 -2.998926354531397144e-04 -2.983889808376167098e-04 -2.965568850579353719e-04 -2.943998445152318732e-04 -2.919220555610738230e-04 -2.891284432767083495e-04 -2.860246921161341640e-04 -2.826172773308741211e-04 -2.789134959670344681e-04 -2.749214961161055735e-04 -2.706503030087387520e-04
+-3.405656358729197784e-04 -3.403039341765055990e-04 -3.397168076985176044e-04 -3.387393509855280869e-04 -3.373732099848444780e-04 -3.356207184348479781e-04 -3.334849256264767734e-04 -3.309696330567160117e-04 -3.280794343956229347e-04 -3.248197622845066298e-04 -3.211969378259900356e-04 -3.172182221473385808e-04 -3.128918681579036221e-04 -3.082271705795121600e-04 -3.032345121767072321e-04
+-3.792804830288493004e-04 -3.789829886453808237e-04 -3.783114191474921495e-04 -3.771932759785042691e-04 -3.756302887037898312e-04 -3.736249207348329125e-04 -3.711804018027124469e-04 -3.683007929494976291e-04 -3.649910265246985642e-04 -3.612569824697356240e-04 -3.571055550671475495e-04 -3.525447271002323901e-04 -3.475836968448229431e-04 -3.422326899185270245e-04 -3.365035508570878497e-04
+-4.188918844168176793e-04 -4.185577342820372571e-04 -4.178003590951156945e-04 -4.165392347458680934e-04 -4.147761395169799470e-04 -4.125136169012959286e-04 -4.097550228605415673e-04 -4.065046017838037473e-04 -4.027675480206621087e-04 -3.985501026247815137e-04 -3.938596425503853335e-04 -3.887047798184187935e-04 -3.830954621296316174e-04 -3.770430724053608156e-04 -3.705605237311815001e-04
+-4.595142793559646357e-04 -4.591425850709772373e-04 -4.582980089399200886e-04 -4.568915471969563799e-04 -4.549249812746170062e-04 -4.524008719790186049e-04 -4.493226247888072711e-04 -4.456945716332864470e-04 -4.415220674660448683e-04 -4.368115995259932516e-04 -4.315709067330638932e-04 -4.258091062119345131e-04 -4.195368234750252324e-04 -4.127663223503715592e-04 -4.055116303242210958e-04
+-5.012639441614780058e-04 -5.008538081328215092e-04 -4.999206402967601090e-04 -4.983664845571156559e-04 -4.961930682003514240e-04 -4.934028913321119496e-04 -4.899993071128970392e-04 -4.859866224864585840e-04 -4.813702175002875362e-04 -4.761566808177299776e-04 -4.703539584867845306e-04 -4.639715124727101354e-04 -4.570204848820745265e-04 -4.495138632334048055e-04 -4.414666415697609180e-04
+-5.442589800938005436e-04 -5.438095158905484035e-04 -5.427864166390079792e-04 -5.410822866992421676e-04 -5.386987289647661523e-04 -5.356380860798680161e-04 -5.319035372441061017e-04 -5.274992200518876942e-04 -5.224303752887318915e-04 -5.167035120298511114e-04 -5.103265897568262394e-04 -5.033092135337492376e-04 -4.956628375701258981e-04 -4.874009717585456769e-04 -4.785393850808696372e-04
+-5.886192385693523937e-04 -5.881295959732968153e-04 -5.870153336397407025e-04 -5.851591197961146778e-04 -5.825623483873710456e-04 -5.792270879159231063e-04 -5.751561965789818865e-04 -5.703534672463978286e-04 -5.648238024018151270e-04 -5.585734092369503507e-04 -5.516100229260051824e-04 -5.439431420960855147e-04 -5.355842782017480701e-04 -5.265472103000765460e-04 -5.168482385094203121e-04
+-6.344661696494730517e-04 -6.339355649224986131e-04 -6.327290843774149463e-04 -6.307189606341019432e-04 -6.279062783715145483e-04 -6.242926932509107029e-04 -6.198805672233925583e-04 -6.146731390337669635e-04 -6.086747330290789718e-04 -6.018909872944546314e-04 -5.943291240451338596e-04 -5.859982308447088091e-04 -5.769095628613299344e-04 -5.670768539851009675e-04 -5.565166293829145556e-04
+-6.819225784336617078e-04 -6.813503303535968546e-04 -6.800508341255804244e-04 -6.778853924309073556e-04 -6.748546649602350008e-04 -6.709597260826539056e-04 -6.662022406621802501e-04 -6.605846449839621569e-04 -6.541103975746718167e-04 -6.467842516681973153e-04 -6.386125691735295871e-04 -6.296036585785717322e-04 -6.197681370577810649e-04 -6.091193070542233901e-04 -5.976735384737868898e-04
+-7.311122725026151072e-04 -7.304978447329681275e-04 -7.291048879068468469e-04 -7.267832953843212209e-04 -7.235331622360491929e-04 -7.193548023142451626e-04 -7.142489328471018743e-04 -7.082169014931267948e-04 -7.012609664811268913e-04 -6.933846195857863368e-04 -6.845929507172723036e-04 -6.748930487183934460e-04 -6.642944320610983311e-04 -6.528095011030007454e-04 -6.404540019631474630e-04
+-7.821595820709651477e-04 -7.815026324079914254e-04 -7.800162324054497236e-04 -7.775384134916331130e-04 -7.740685509265831515e-04 -7.696059770242715198e-04 -7.641501873066571708e-04 -7.577011041697526324e-04 -7.502593965123272859e-04 -7.418268535447785934e-04 -7.324068078805063154e-04 -7.220046057083175355e-04 -7.106281150630812827e-04 -6.982882651245625287e-04 -6.849996053035431205e-04
+-8.351887330872352850e-04 -8.344891700721811635e-04 -8.329099322939132431e-04 -8.302767775035648033e-04 -8.265881840920346474e-04 -8.218422541087995773e-04 -8.160369455416287363e-04 -8.091703706267402421e-04 -8.012411590010413455e-04 -7.922488870294244756e-04 -7.821945619801649310e-04 -7.710811714269939776e-04 -7.589142771623846959e-04 -7.457026539097435158e-04 -7.314589585507302611e-04
+-8.903230522855976655e-04 -8.895810995613590141e-04 -8.879103596352793488e-04 -8.851239623065860086e-04 -8.812192899661812004e-04 -8.761929356067623418e-04 -8.700409615182904278e-04 -8.627592330434914573e-04 -8.543438270260163845e-04 -8.447915188076727221e-04 -8.341003334305695585e-04 -8.222701794998691239e-04 -8.093035388493397550e-04 -7.952062170328867956e-04 -7.799881388578919954e-04
+-9.476839822867323682e-04 -9.469002509115904184e-04 -9.451402339229999150e-04 -9.422041557060750749e-04 -9.380880818218641790e-04 -9.327867860092501013e-04 -9.262940346080502903e-04 -9.186029553784550838e-04 -9.097064921006325217e-04 -8.995979480014934136e-04 -8.882716126521933474e-04 -8.757234804300150161e-04 -8.619520473457685040e-04 -8.469591852288912461e-04 -8.307510805981591301e-04
+-1.007389884455910448e-03 -1.006565453138834896e-03 -1.004719449686087901e-03 -1.001639014675363920e-03 -9.973186552056300617e-04 -9.917509850846573018e-04 -9.849270329767973158e-04 -9.768366442906041818e-04 -9.674689802627237231e-04 -9.568131176593533318e-04 -9.448587519671319259e-04 -9.315970045375699098e-04 -9.170213337046479677e-04 -9.011285441597137718e-04 -8.839198862428168093e-04
+-1.069554607558354008e-03 -1.068691110448379044e-03 -1.066763668640156350e-03 -1.063546284864507049e-03 -1.059031647384112889e-03 -1.053209841433969422e-03 -1.046068677391802414e-03 -1.037594121595960921e-03 -1.027770835545356977e-03 -1.016582829727048169e-03 -1.004014239632450289e-03 -9.900502228347575050e-04 -9.746779898046232116e-04 -9.578879571373759066e-04 -9.396750233618949427e-04
+-1.134285801579867437e-03 -1.133385522802311850e-03 -1.131382654363903128e-03 -1.128038159785132869e-03 -1.123342632917214996e-03 -1.117283238380155407e-03 -1.109844053936129022e-03 -1.101006523378989096e-03 -1.090750028567656410e-03 -1.079052590198042831e-03 -1.065891710746070739e-03 -1.051245358089994203e-03 -1.035093116147835874e-03 -1.017417488068149758e-03 -9.982053610168985062e-04
+-1.201682958682963234e-03 -1.200748932265083670e-03 -1.198678329726648659e-03 -1.195219360039624602e-03 -1.190360230859069824e-03 -1.184084784221481335e-03 -1.176372823550059492e-03 -1.167200588964102713e-03 -1.156541348806715795e-03 -1.144366135611977553e-03 -1.130644642915390723e-03 -1.115346289528628852e-03 -1.098441480597588116e-03 -1.079903062432074597e-03 -1.059707984343815019e-03
+-1.271835167474458586e-03 -1.270871280634071777e-03 -1.268742541122806723e-03 -1.265184899372944101e-03 -1.260183901826850182e-03 -1.253719640735453771e-03 -1.245767096894664439e-03 -1.236296602151785474e-03 -1.225274438166922388e-03 -1.212663589988720531e-03 -1.198424677567156045e-03 -1.182517085066410846e-03 -1.164900315998644532e-03 -1.145535591838696150e-03 -1.124387711431283155e-03
+-1.344818572892437277e-03 -1.343829669880021189e-03 -1.341654519337922343e-03 -1.338017569077234927e-03 -1.332901417849748126e-03 -1.326282007572661707e-03 -1.318128945945298879e-03 -1.308405948240874391e-03 -1.297071419077197758e-03 -1.284079198536280768e-03 -1.269379501610872147e-03 -1.252920085064399783e-03 -1.234647670427835601e-03 -1.214509665473686691e-03 -1.192456210609862174e-03
+-1.420693542402156175e-03 -1.419685525204001557e-03 -1.417478034933622412e-03 -1.413785061107470297e-03 -1.408585994971531339e-03 -1.401852246374848780e-03 -1.393547528027137827e-03 -1.383628253439327278e-03 -1.372044072996906044e-03 -1.358738579333587573e-03 -1.343650218377425137e-03 -1.326713452014011488e-03 -1.307860210393880151e-03 -1.287021697826915565e-03 -1.264130595178342619e-03
+-1.499501550082235493e-03 -1.498481471343512039e-03 -1.496258256714525165e-03 -1.492536809207093730e-03 -1.487293088485807649e-03 -1.480493637445637767e-03 -1.472095806612550928e-03 -1.462048079714714727e-03 -1.450290529023696940e-03 -1.436755437659481853e-03 -1.421368133600149934e-03 -1.404048092545703060e-03 -1.384710362227506821e-03 -1.363267394087839873e-03 -1.339631342525186581e-03
+-1.581261803762250805e-03 -1.580237946324214915e-03 -1.578018335364547156e-03 -1.574300521914796585e-03 -1.569056863852237886e-03 -1.562248774957377588e-03 -1.553826864718202546e-03 -1.543731158568221714e-03 -1.531891430594953208e-03 -1.518227691295224221e-03 -1.502650883228551400e-03 -1.485063852053462733e-03 -1.465362664448669697e-03 -1.443438377866935237e-03 -1.419179349238618073e-03
+-1.665967656658892161e-03 -1.664949593199806102e-03 -1.662755750806508680e-03 -1.659078457368157048e-03 -1.653886373082594577e-03 -1.647135622615083714e-03 -1.638769823187089881e-03 -1.628720162707499117e-03 -1.616905562088327350e-03 -1.603232968250078863e-03 -1.587597837397983257e-03 -1.569884885022253956e-03 -1.549969194619074979e-03 -1.527717804611506162e-03 -1.502991902347276289e-03
+-1.753582863751015431e-03 -1.752581489276319997e-03 -1.750438481131449996e-03 -1.746843492653804997e-03 -1.741761486824598302e-03 -1.735143273516521686e-03 -1.726925397633922998e-03 -1.717030036098465611e-03 -1.705364937867261945e-03 -1.691823454962842858e-03 -1.676284728137798210e-03 -1.658614109354020292e-03 -1.638663933671058275e-03 -1.616274767311503624e-03 -1.591277313444451917e-03
+-1.844037763956353016e-03 -1.843065293419792220e-03 -1.841001072651173368e-03 -1.837535065257331823e-03 -1.832628656337210050e-03 -1.826227482955346650e-03 -1.818261154820616883e-03 -1.808642931182912524e-03 -1.797269385340821094e-03 -1.784020102628733947e-03 -1.768757475185557060e-03 -1.751326676969032145e-03 -1.731555944887457846e-03 -1.709257301041702684e-03 -1.684227938450933880e-03
+-1.937225491189089937e-03 -1.936295414482402163e-03 -1.934340713973852150e-03 -1.931055089016733535e-03 -1.926396606482861035e-03 -1.920306072547732675e-03 -1.912706561654660192e-03 -1.903502837564323077e-03 -1.892580691985063261e-03 -1.879806239542618522e-03 -1.865025226031607683e-03 -1.848062428078338110e-03 -1.828721271284844798e-03 -1.806783808272561034e-03 -1.782011299018774596e-03
+-2.032998339367835753e-03 -2.032125326437783566e-03 -2.030313440786996482e-03 -2.027263972835591666e-03 -2.022932089558264306e-03 -2.017254336607579492e-03 -2.010147957176524128e-03 -2.001510028934971354e-03 -1.991216434443239276e-03 -1.979120691197210589e-03 -1.965052683160049482e-03 -1.948817360779776754e-03 -1.930193515303219335e-03 -1.908932773833564621e-03 -1.884759045952897911e-03
+-2.131164426793603125e-03 -2.130364176854517618e-03 -2.128730620592202312e-03 -2.125976895571570369e-03 -2.122055858924796166e-03 -2.116900615657534186e-03 -2.110423618267582690e-03 -2.102515503193634009e-03 -2.093043665126807090e-03 -2.081850576590440430e-03 -2.068751870676508939e-03 -2.053534230827320888e-03 -2.035953155904061864e-03 -2.015730728047885299e-03 -1.992553578916056358e-03
+-2.231484822044141683e-03 -2.230773852847447308e-03 -2.229355885882705005e-03 -2.226960512772907519e-03 -2.223539047802159437e-03 -2.219022234811946111e-03 -2.213319130758558979e-03 -2.206315642011486000e-03 -2.197872695911907981e-03 -2.187824030468876659e-03 -2.175973587036190808e-03 -2.162092514073354205e-03 -2.145915792346784947e-03 -2.127138562897038215e-03 -2.105412282496987256e-03
+-2.333671304410873081e-03 -2.333066680339170376e-03 -2.331902698764937686e-03 -2.329930287628518681e-03 -2.327100160401359211e-03 -2.323342033135501663e-03 -2.318563315356633216e-03 -2.312647366360071326e-03 -2.305451285158477154e-03 -2.296803186614151254e-03 -2.286498908855453659e-03 -2.274298108417641302e-03 -2.259919683420944826e-03 -2.243036520149213099e-03 -2.223269579998095932e-03
+-2.437384934659943964e-03 -2.436903935963018707e-03 -2.436032728205469317e-03 -2.434548646704651122e-03 -2.432402895254436731e-03 -2.429525729878097718e-03 -2.425824987415486217e-03 -2.421184107830918943e-03 -2.415459596558183503e-03 -2.408477847125298308e-03 -2.400031226900128847e-03 -2.389873317712804240e-03 -2.377713171126913470e-03 -2.363208455516487266e-03 -2.345957361278720558e-03
+-2.542235604436069232e-03 -2.541895344046318089e-03 -2.541355236415348585e-03 -2.540424157871644904e-03 -2.539055021507415771e-03 -2.537180380219512116e-03 -2.534710845295354894e-03 -2.531532944571841717e-03 -2.527506346184033807e-03 -2.522460336885017085e-03 -2.516189416736799422e-03 -2.508447832681126328e-03 -2.498942825766979191e-03 -2.487326331174834725e-03 -2.473184812083767652e-03
+-2.647782713377485990e-03 -2.647599712136925430e-03 -2.647427617851620934e-03 -2.647111910819773938e-03 -2.646608514165183466e-03 -2.645854162465774775e-03 -2.644764777923467799e-03 -2.643233257116491767e-03 -2.641126578503563346e-03 -2.638282094047505501e-03 -2.634502832450357716e-03 -2.629551573595349107e-03 -2.623143390422552450e-03 -2.614936260117641832e-03 -2.604519228732301347e-03
+-2.753537091262175680e-03 -2.753526826649646368e-03 -2.753757236822049724e-03 -2.754115248174647188e-03 -2.754561121949290498e-03 -2.755037707041100258e-03 -2.755468852918205747e-03 -2.755757235410323351e-03 -2.755781497220940318e-03 -2.755392551110606974e-03 -2.754408852274647414e-03 -2.752610354710321398e-03 -2.749730790274934177e-03 -2.745447762285934280e-03 -2.739369967381878775e-03
+-2.858964238686594224e-03 -2.859140685779366919e-03 -2.859804641850520295e-03 -2.860888947291428692e-03 -2.862359490587128730e-03 -2.864167123376801759e-03 -2.866246188950510431e-03 -2.868512508048242076e-03 -2.870860717048583956e-03 -2.873160806811282750e-03 -2.875253665745089622e-03 -2.876945327307253459e-03 -2.877999539279426679e-03 -2.878128090963568905e-03 -2.876978114014523604e-03
+-2.963488905705875982e-03 -2.963864091635589823e-03 -2.964988192698943172e-03 -2.966843890948861386e-03 -2.969403896404342481e-03 -2.972628804740698287e-03 -2.976465829715451913e-03 -2.980847066136507739e-03 -2.985687190462770011e-03 -2.990880462967308601e-03 -2.996296854400116918e-03 -3.001777019581325888e-03 -3.007125761633465313e-03 -3.012103444723275483e-03 -3.016414584027568742e-03
+-3.066500966728437534e-03 -3.067084560863539075e-03 -3.068690044113034626e-03 -3.071353192918362465e-03 -3.075054563833752499e-03 -3.079765997168827912e-03 -3.085449625993885725e-03 -3.092056520886407069e-03 -3.099524900079901439e-03 -3.107777800274289480e-03 -3.116720074229362581e-03 -3.126234495640563618e-03 -3.136176694606949283e-03 -3.146368488457358410e-03 -3.156588980528466249e-03
+-3.167362486197706616e-03 -3.168161447401959298e-03 -3.170263401126237682e-03 -3.173759667294768876e-03 -3.178639452085888720e-03 -3.184887014215869328e-03 -3.192481005397918275e-03 -3.201393576261687534e-03 -3.211589207952302450e-03 -3.223023209968811642e-03 -3.235639810522076328e-03 -3.249369710915315981e-03 -3.264126950911505360e-03 -3.279804831862937354e-03 -3.296270533585701681e-03
+-3.265415808477476183e-03 -3.266434107962291802e-03 -3.269040853048740987e-03 -3.273384455076129834e-03 -3.279463308850888697e-03 -3.287274874229534002e-03 -3.296815379191188680e-03 -3.308079431802622098e-03 -3.321059536651336987e-03 -3.335745508351565039e-03 -3.352123781627321716e-03 -3.370176594885984991e-03 -3.389881049174235401e-03 -3.411208014459348858e-03 -3.434120858011654488e-03
+-3.359992452374316839e-03 -3.361230886053084843e-03 -3.364343558472963729e-03 -3.369536555538895067e-03 -3.376817711558031954e-03 -3.386198042807587755e-03 -3.397691817267848441e-03 -3.411316677893209623e-03 -3.427093850384104693e-03 -3.445048480899462213e-03 -3.465210175901131152e-03 -3.487613829518335182e-03 -3.512300895854811658e-03 -3.539321308470785160e-03 -3.568736367666102294e-03
+-3.450422550919221565e-03 -3.451878649196864039e-03 -3.455491001378394999e-03 -3.461522959973480779e-03 -3.469991758063453984e-03 -3.480921891312166970e-03 -3.494345531279218365e-03 -3.510303125501646609e-03 -3.528844246052795491e-03 -3.550028778531960031e-03 -3.573928584883188410e-03 -3.600629820292173319e-03 -3.630236191113985107e-03 -3.662873549107028160e-03 -3.698696425531270825e-03
+-3.536044554214848833e-03 -3.537712590439587561e-03 -3.541811014323783657e-03 -3.548659057154636073e-03 -3.558283035534972726e-03 -3.570720441914584237e-03 -3.586020654613635093e-03 -3.604245945445262288e-03 -3.625472868932352530e-03 -3.649794159032615677e-03 -3.677321308500797713e-03 -3.708188077455179272e-03 -3.742555302319705568e-03 -3.780617522985567618e-03 -3.822612200524892669e-03
+-3.616214909408062717e-03 -3.618086001521568854e-03 -3.622649761011287762e-03 -3.630278976211813013e-03 -3.641008492610929743e-03 -3.654887965833172013e-03 -3.671982803789343094e-03 -3.692375487090972502e-03 -3.716167363298566399e-03 -3.743481057648623180e-03 -3.774463694244070255e-03 -3.809291202814791243e-03 -3.848174111763599890e-03 -3.891365382418605391e-03 -3.939171091560615852e-03
+-3.690317447109191500e-03 -3.692379741120163476e-03 -3.697381388307788286e-03 -3.705745553468256341e-03 -3.717514865733410195e-03 -3.732750034446682443e-03 -3.751530949271928306e-03 -3.773958205349551599e-03 -3.800155148685664848e-03 -3.830270584486364458e-03 -3.864482335858935094e-03 -3.903001918942752314e-03 -3.946080711832649496e-03 -3.994018127301084825e-03 -4.047172510177153050e-03
+-3.757772235666615064e-03 -3.760011155094086181e-03 -3.765417094574325871e-03 -3.774459652497049421e-03 -3.787188362181370758e-03 -3.803673687976466197e-03 -3.824008208196259979e-03 -3.848308236454538178e-03 -3.876715965709724623e-03 -3.909402261831422185e-03 -3.946570265556878510e-03 -3.988460029905547752e-03 -4.035354501263172140e-03 -4.087587249040744788e-03 -4.145552492213931337e-03
+-3.818043709576097230e-03 -3.820442252414645024e-03 -3.826213412177122478e-03 -3.835868625162227197e-03 -3.849463372817254515e-03 -3.867076474361198432e-03 -3.888811284610138239e-03 -3.914797314500400791e-03 -3.945192339379350287e-03 -3.980185093596154931e-03 -4.019998667353383813e-03 -4.064894769613252787e-03 -4.115179070828758716e-03 -4.171207888373522875e-03 -4.233396549342624722e-03
+-3.870647930654761652e-03 -3.873186994895524721e-03 -3.879279561168025910e-03 -3.889473768980591505e-03 -3.903830067909812816e-03 -3.922434210126622516e-03 -3.945398408947095939e-03 -3.972862882571834807e-03 -4.004997823140572788e-03 -4.042005855475676833e-03 -4.084125047798698241e-03 -4.131632566411666367e-03 -4.184849081269296014e-03 -4.244144034308373892e-03 -4.309941889696350739e-03
+-3.915158894578164329e-03 -3.917817614793608037e-03 -3.924183791569738934e-03 -3.934836704472310931e-03 -3.949840809945859114e-03 -3.969287413152747419e-03 -3.993295751212529686e-03 -4.022014411027951229e-03 -4.055623095321939098e-03 -4.094334764421516358e-03 -4.138398160803895102e-03 -4.188100737425443781e-03 -4.243771991243707256e-03 -4.305787175171306436e-03 -4.374571317576437211e-03
+-3.951213845338953645e-03 -3.953969925980027784e-03 -3.960558687063102899e-03 -3.971584658127891819e-03 -3.987115389192300192e-03 -4.007246443167297029e-03 -4.032102387623835889e-03 -4.061838066859761558e-03 -4.096640142756095490e-03 -4.136728896839999073e-03 -4.182360251488947273e-03 -4.233827965044411473e-03 -4.291465913328747217e-03 -4.355650313986010776e-03 -4.426801673504102488e-03
+-3.978517601411007791e-03 -3.981347636766957403e-03 -3.988105447845251804e-03 -3.999414686035126024e-03 -4.015345143884096503e-03 -4.035995451086855923e-03 -4.061493977849424050e-03 -4.091999969255283483e-03 -4.127704877945784917e-03 -4.168833858291708799e-03 -4.215647339849594097e-03 -4.268442581808047816e-03 -4.327555051725536471e-03 -4.393359397493048352e-03 -4.466269686423395696e-03
+-3.996845926590044881e-03 -3.999725702218169011e-03 -4.006597201389662521e-03 -4.018096906281088884e-03 -4.034296062832213106e-03 -4.055295277947816232e-03 -4.081225353928933861e-03 -4.112248316774928109e-03 -4.148558590460611067e-03 -4.190384259556340953e-03 -4.237988309801649436e-03 -4.291669711693532792e-03 -4.351764143702957673e-03 -4.418644066887359584e-03 -4.492717758788281578e-03
+-4.006047994025191579e-03 -4.008952769249251626e-03 -4.015881405139431343e-03 -4.027476823099315588e-03 -4.043810982312316671e-03 -4.064985456633554879e-03 -4.091132231441243702e-03 -4.122414674479724268e-03 -4.159028624873180487e-03 -4.201203531895950603e-03 -4.249203343966070912e-03 -4.303328216950346938e-03 -4.363913147063741040e-03 -4.431329325395113976e-03 -4.505981677431570957e-03
+-4.006047994025218467e-03 -4.008952769249252493e-03 -4.015881405139442618e-03 -4.027476823099325996e-03 -4.043810982312326212e-03 -4.064985456633565288e-03 -4.091132231441254978e-03 -4.122414674479732942e-03 -4.159028624873188293e-03 -4.201203531895961012e-03 -4.249203343966082187e-03 -4.303328216950359081e-03 -4.363913147063750581e-03 -4.431329325395128721e-03 -4.505981677431586570e-03
+-3.996845926590046616e-03 -3.999725702218214982e-03 -4.006597201389706757e-03 -4.018096906281133120e-03 -4.034296062832253872e-03 -4.055295277947861335e-03 -4.081225353928979831e-03 -4.112248316774974946e-03 -4.148558590460656170e-03 -4.190384259556391260e-03 -4.237988309801703213e-03 -4.291669711693586568e-03 -4.351764143703014918e-03 -4.418644066887422034e-03 -4.492717758788345762e-03
+-3.978517601411049424e-03 -3.981347636766996434e-03 -3.988105447845287366e-03 -3.999414686035158983e-03 -4.015345143884133799e-03 -4.035995451086891485e-03 -4.061493977849460479e-03 -4.091999969255321647e-03 -4.127704877945823948e-03 -4.168833858291749565e-03 -4.215647339849633128e-03 -4.268442581808089449e-03 -4.327555051725582441e-03 -4.393359397493097791e-03 -4.466269686423445136e-03
+-3.951213845338979666e-03 -3.953969925980076357e-03 -3.960558687063154941e-03 -3.971584658127944728e-03 -3.987115389192353102e-03 -4.007246443167350805e-03 -4.032102387623890533e-03 -4.061838066859819671e-03 -4.096640142756154471e-03 -4.136728896840058921e-03 -4.182360251489010590e-03 -4.233827965044475658e-03 -4.291465913328815739e-03 -4.355650313986083634e-03 -4.426801673504175347e-03
+-3.915158894578264943e-03 -3.917817614793667885e-03 -3.924183791569809190e-03 -3.934836704472379453e-03 -3.949840809945930238e-03 -3.969287413152819410e-03 -3.993295751212603412e-03 -4.022014411028027557e-03 -4.055623095322017160e-03 -4.094334764421598757e-03 -4.138398160803979237e-03 -4.188100737425531385e-03 -4.243771991243795727e-03 -4.305787175171400111e-03 -4.374571317576537825e-03
+-3.870647930654848821e-03 -3.873186994895604519e-03 -3.879279561168105274e-03 -3.889473768980670435e-03 -3.903830067909892180e-03 -3.922434210126701445e-03 -3.945398408947179206e-03 -3.972862882571916339e-03 -4.004997823140660392e-03 -4.042005855475764436e-03 -4.084125047798787579e-03 -4.131632566411761777e-03 -4.184849081269398363e-03 -4.244144034308479710e-03 -4.309941889696457425e-03
+-3.818043709576145802e-03 -3.820442252414734362e-03 -3.826213412177216586e-03 -3.835868625162322607e-03 -3.849463372817351226e-03 -3.867076474361296010e-03 -3.888811284610237985e-03 -3.914797314500504874e-03 -3.945192339379453503e-03 -3.980185093596265954e-03 -4.019998667353495703e-03 -4.064894769613371615e-03 -4.115179070828878412e-03 -4.171207888373650377e-03 -4.233396549342759163e-03
+-3.757772235666672310e-03 -3.760011155094202841e-03 -3.765417094574447735e-03 -3.774459652497173454e-03 -3.787188362181498694e-03 -3.803673687976595000e-03 -3.824008208196390517e-03 -3.848308236454672186e-03 -3.876715965709865135e-03 -3.909402261831564432e-03 -3.946570265557027696e-03 -3.988460029905706479e-03 -4.035354501263336939e-03 -4.087587249040916526e-03 -4.145552492214111748e-03
+-3.690317447109338952e-03 -3.692379741120303555e-03 -3.697381388307927064e-03 -3.705745553468395553e-03 -3.717514865733550708e-03 -3.732750034446823822e-03 -3.751530949272074457e-03 -3.773958205349701653e-03 -3.800155148685819672e-03 -3.830270584486521884e-03 -3.864482335859099893e-03 -3.903001918942927088e-03 -3.946080711832829040e-03 -3.994018127301275645e-03 -4.047172510177355145e-03
+-3.616214909408176342e-03 -3.618086001521687682e-03 -3.622649761011414397e-03 -3.630278976211937913e-03 -3.641008492611058547e-03 -3.654887965833305587e-03 -3.671982803789476668e-03 -3.692375487091109545e-03 -3.716167363298706044e-03 -3.743481057648768030e-03 -3.774463694244220308e-03 -3.809291202814952572e-03 -3.848174111763760785e-03 -3.891365382418776261e-03 -3.939171091560794528e-03
+-3.536044554214973733e-03 -3.537712590439737615e-03 -3.541811014323932409e-03 -3.548659057154774418e-03 -3.558283035535121045e-03 -3.570720441914734290e-03 -3.586020654613789917e-03 -3.604245945445433159e-03 -3.625472868932515594e-03 -3.649794159032792185e-03 -3.677321308500970751e-03 -3.708188077455363586e-03 -3.742555302319889882e-03 -3.780617522985764943e-03 -3.822612200525104739e-03
+-3.450422550919344730e-03 -3.451878649197002383e-03 -3.455491001378535511e-03 -3.461522959973614786e-03 -3.469991758063596665e-03 -3.480921891312312687e-03 -3.494345531279364949e-03 -3.510303125501811408e-03 -3.528844246052952917e-03 -3.550028778532134371e-03 -3.573928584883358846e-03 -3.600629820292346791e-03 -3.630236191114153809e-03 -3.662873549107229822e-03 -3.698696425531485064e-03
+-3.359992452374481204e-03 -3.361230886053239234e-03 -3.364343558473124191e-03 -3.369536555539047722e-03 -3.376817711558193283e-03 -3.386198042807753422e-03 -3.397691817268014974e-03 -3.411316677893390468e-03 -3.427093850384281635e-03 -3.445048480899653900e-03 -3.465210175901320671e-03 -3.487613829518529038e-03 -3.512300895855002911e-03 -3.539321308471010674e-03 -3.568736367666342120e-03
+-3.265415808477598048e-03 -3.266434107962455299e-03 -3.269040853048905352e-03 -3.273384455076287693e-03 -3.279463308851057399e-03 -3.287274874229705306e-03 -3.296815379191363454e-03 -3.308079431802814652e-03 -3.321059536651525205e-03 -3.335745508351765400e-03 -3.352123781627520775e-03 -3.370176594886189255e-03 -3.389881049174436195e-03 -3.411208014459583913e-03 -3.434120858011903421e-03
+-3.167362486197891364e-03 -3.168161447402119760e-03 -3.170263401126402480e-03 -3.173759667294927603e-03 -3.178639452086055688e-03 -3.184887014216036295e-03 -3.192481005398092615e-03 -3.201393576261875318e-03 -3.211589207952488933e-03 -3.223023209969011135e-03 -3.235639810522272786e-03 -3.249369710915517642e-03 -3.264126950911701384e-03 -3.279804831863169373e-03 -3.296270533585943241e-03
+-3.066500966728616644e-03 -3.067084560863696501e-03 -3.068690044113195087e-03 -3.071353192918522493e-03 -3.075054563833920333e-03 -3.079765997168999216e-03 -3.085449625994055728e-03 -3.092056520886589215e-03 -3.099524900080083151e-03 -3.107777800274488106e-03 -3.116720074229552100e-03 -3.126234495640760943e-03 -3.136176694607150511e-03 -3.146368488457570479e-03 -3.156588980528686125e-03
+-2.963488905706134890e-03 -2.963864091635747249e-03 -2.964988192699110139e-03 -2.966843890949015777e-03 -2.969403896404499473e-03 -2.972628804740861351e-03 -2.976465829715621483e-03 -2.980847066136677308e-03 -2.985687190462936111e-03 -2.990880462967487278e-03 -2.996296854400287788e-03 -3.001777019581501962e-03 -3.007125761633651796e-03 -3.012103444723481047e-03 -3.016414584027782547e-03
+-2.858964238686720859e-03 -2.859140685779530417e-03 -2.859804641850689430e-03 -2.860888947291596093e-03 -2.862359490587304371e-03 -2.864167123376980869e-03 -2.866246188950689108e-03 -2.868512508048427258e-03 -2.870860717048765234e-03 -2.873160806811471835e-03 -2.875253665745285646e-03 -2.876945327307455121e-03 -2.877999539279633544e-03 -2.878128090963782710e-03 -2.876978114014749552e-03
+-2.753537091262292340e-03 -2.753526826649796422e-03 -2.753757236822206717e-03 -2.754115248174799843e-03 -2.754561121949450093e-03 -2.755037707041265490e-03 -2.755468852918370980e-03 -2.755757235410492487e-03 -2.755781497221104683e-03 -2.755392551110780446e-03 -2.754408852274825223e-03 -2.752610354710503544e-03 -2.749730790275121961e-03 -2.745447762286130303e-03 -2.739369967382075232e-03
+-2.647782713377612625e-03 -2.647599712137090229e-03 -2.647427617851800478e-03 -2.647111910819945242e-03 -2.646608514165365179e-03 -2.645854162465959957e-03 -2.644764777923652548e-03 -2.643233257116685189e-03 -2.641126578503747661e-03 -2.638282094047701958e-03 -2.634502832450558076e-03 -2.629551573595555539e-03 -2.623143390422758448e-03 -2.614936260117861275e-03 -2.604519228732524692e-03
+-2.542235604436222755e-03 -2.541895344046499368e-03 -2.541355236415538538e-03 -2.540424157871827918e-03 -2.539055021507607458e-03 -2.537180380219705104e-03 -2.534710845295551785e-03 -2.531532944572042077e-03 -2.527506346184229397e-03 -2.522460336885222650e-03 -2.516189416737010624e-03 -2.508447832681343168e-03 -2.498942825767197767e-03 -2.487326331175065876e-03 -2.473184812083998804e-03
+-2.437384934660126110e-03 -2.436903935963177434e-03 -2.436032728205644524e-03 -2.434548646704819391e-03 -2.432402895254608902e-03 -2.429525729878273359e-03 -2.425824987415658388e-03 -2.421184107831099355e-03 -2.415459596558358277e-03 -2.408477847125481755e-03 -2.400031226900314896e-03 -2.389873317712991590e-03 -2.377713171127107325e-03 -2.363208455516685024e-03 -2.345957361278920052e-03
+-2.333671304411034410e-03 -2.333066680339348619e-03 -2.331902698765125903e-03 -2.329930287628695623e-03 -2.327100160401541790e-03 -2.323342033135693784e-03 -2.318563315356821000e-03 -2.312647366360264314e-03 -2.305451285158668408e-03 -2.296803186614349013e-03 -2.286498908855650984e-03 -2.274298108417842097e-03 -2.259919683421149957e-03 -2.243036520149430807e-03 -2.223269579998311471e-03
+-2.231484822044282196e-03 -2.230773852847601265e-03 -2.229355885882878478e-03 -2.226960512773072751e-03 -2.223539047802332910e-03 -2.219022234812124787e-03 -2.213319130758734619e-03 -2.206315642011668146e-03 -2.197872695912079719e-03 -2.187824030469060106e-03 -2.175973587036376423e-03 -2.162092514073542422e-03 -2.145915792346967960e-03 -2.127138562897232070e-03 -2.105412282497182413e-03
+-2.131164426793757949e-03 -2.130364176854669840e-03 -2.128730620592364075e-03 -2.125976895571725193e-03 -2.122055858924956628e-03 -2.116900615657701587e-03 -2.110423618267744019e-03 -2.102515503193801410e-03 -2.093043665126967118e-03 -2.081850576590610433e-03 -2.068751870676673304e-03 -2.053534230827488722e-03 -2.035953155904232301e-03 -2.015730728048060940e-03 -1.992553578916233300e-03
+-2.032998339367991011e-03 -2.032125326437938390e-03 -2.030313440787165618e-03 -2.027263972835752562e-03 -2.022932089558433007e-03 -2.017254336607752097e-03 -2.010147957176694998e-03 -2.001510028935147428e-03 -1.991216434443404074e-03 -1.979120691197381893e-03 -1.965052683160225556e-03 -1.948817360779955430e-03 -1.930193515303400397e-03 -1.908932773833753056e-03 -1.884759045953078756e-03
+-1.937225491189284443e-03 -1.936295414482542892e-03 -1.934340713974002637e-03 -1.931055089016884023e-03 -1.926396606483011739e-03 -1.920306072547890101e-03 -1.912706561654811763e-03 -1.903502837564480287e-03 -1.892580691985212664e-03 -1.879806239542774864e-03 -1.865025226031763158e-03 -1.848062428078492934e-03 -1.828721271284999188e-03 -1.806783808272721496e-03 -1.782011299018935275e-03
+-1.844037763956505455e-03 -1.843065293419931866e-03 -1.841001072651321903e-03 -1.837535065257469083e-03 -1.832628656337349478e-03 -1.826227482955490632e-03 -1.818261154820758480e-03 -1.808642931183059325e-03 -1.797269385340959872e-03 -1.784020102628876194e-03 -1.768757475185699958e-03 -1.751326676969173959e-03 -1.731555944887597492e-03 -1.709257301041847751e-03 -1.684227938451073742e-03
+-1.753582863751078748e-03 -1.752581489276460510e-03 -1.750438481131595279e-03 -1.746843492653946377e-03 -1.741761486824740116e-03 -1.735143273516665452e-03 -1.726925397634066547e-03 -1.717030036098613280e-03 -1.705364937867402675e-03 -1.691823454962986407e-03 -1.676284728137944578e-03 -1.658614109354166659e-03 -1.638663933671201823e-03 -1.616274767311649558e-03 -1.591277313444593080e-03
+-1.665967656659078210e-03 -1.664949593199938158e-03 -1.662755750806644639e-03 -1.659078457368286935e-03 -1.653886373082726199e-03 -1.647135622615219239e-03 -1.638769823187222587e-03 -1.628720162707637895e-03 -1.616905562088458538e-03 -1.603232968250212003e-03 -1.587597837398115530e-03 -1.569884885022386012e-03 -1.549969194619203348e-03 -1.527717804611638652e-03 -1.502991902347400755e-03
+-1.581261803762402593e-03 -1.580237946324343501e-03 -1.578018335364687885e-03 -1.574300521914929508e-03 -1.569056863852372327e-03 -1.562248774957519402e-03 -1.553826864718340674e-03 -1.543731158568362009e-03 -1.531891430595085698e-03 -1.518227691295361481e-03 -1.502650883228688877e-03 -1.485063852053601294e-03 -1.465362664448804355e-03 -1.443438377867073581e-03 -1.419179349238748611e-03
+-1.499501550082323531e-03 -1.498481471343636722e-03 -1.496258256714649414e-03 -1.492536809207216895e-03 -1.487293088485928862e-03 -1.480493637445763535e-03 -1.472095806612671925e-03 -1.462048079714841796e-03 -1.450290529023814468e-03 -1.436755437659603717e-03 -1.421368133600267461e-03 -1.404048092545818202e-03 -1.384710362227620228e-03 -1.363267394087958918e-03 -1.339631342525301723e-03
+-1.420693542402225997e-03 -1.419685525204116483e-03 -1.417478034933730832e-03 -1.413785061107579368e-03 -1.408585994971638024e-03 -1.401852246374960887e-03 -1.393547528027244513e-03 -1.383628253439438517e-03 -1.372044072997006658e-03 -1.358738579333692957e-03 -1.343650218377532039e-03 -1.326713452014111885e-03 -1.307860210393975995e-03 -1.287021697827010758e-03 -1.264130595178433909e-03
+-1.344818572892578223e-03 -1.343829669880120935e-03 -1.341654519338040738e-03 -1.338017569077349853e-03 -1.332901417849865003e-03 -1.326282007572778150e-03 -1.318128945945413154e-03 -1.308405948240989967e-03 -1.297071419077311166e-03 -1.284079198536394609e-03 -1.269379501610981434e-03 -1.252920085064508204e-03 -1.234647670427946840e-03 -1.214509665473796846e-03 -1.192456210609970377e-03
+-1.271835167474529276e-03 -1.270871280634179763e-03 -1.268742541122913408e-03 -1.265184899373045582e-03 -1.260183901826948628e-03 -1.253719640735559589e-03 -1.245767096894761150e-03 -1.236296602151893244e-03 -1.225274438167022568e-03 -1.212663589988817025e-03 -1.198424677567251889e-03 -1.182517085066500835e-03 -1.164900315998737773e-03 -1.145535591838791776e-03 -1.124387711431372493e-03
+-1.201682958683055608e-03 -1.200748932265200764e-03 -1.198678329726764885e-03 -1.195219360039734323e-03 -1.190360230859178895e-03 -1.184084784221596477e-03 -1.176372823550170732e-03 -1.167200588964216338e-03 -1.156541348806823999e-03 -1.144366135612086624e-03 -1.130644642915500661e-03 -1.115346289528713853e-03 -1.098441480597698054e-03 -1.079903062432182367e-03 -1.059707984343896551e-03
+-1.134285801579978242e-03 -1.133385522802426342e-03 -1.131382654364045592e-03 -1.128038159785250613e-03 -1.123342632917323633e-03 -1.117283238380296787e-03 -1.109844053936267366e-03 -1.101006523379100335e-03 -1.090750028567775455e-03 -1.079052590198144529e-03 -1.065891710746173521e-03 -1.051245358090089179e-03 -1.035093116147952534e-03 -1.017417488068272707e-03 -9.982053610169965181e-04
+-1.069554607558473487e-03 -1.068691110448495270e-03 -1.066763668640294694e-03 -1.063546284864616553e-03 -1.059031647384209816e-03 -1.053209841434105381e-03 -1.046068677391936205e-03 -1.037594121596059800e-03 -1.027770835545469517e-03 -1.016582829727146831e-03 -1.004014239632545482e-03 -9.900502228348464096e-04 -9.746779898047400886e-04 -9.578879571374952773e-04 -9.396750233619860157e-04
+-1.007389884455990679e-03 -1.006565453138923366e-03 -1.004719449686207163e-03 -1.001639014675458680e-03 -9.973186552057087748e-04 -9.917509850847737451e-04 -9.849270329769120244e-04 -9.768366442906880991e-04 -9.674689802628153382e-04 -9.568131176594309607e-04 -9.448587519672009896e-04 -9.315970045376392988e-04 -9.170213337047337281e-04 -9.011285441598086395e-04 -8.839198862428814278e-04
+-9.476839822868025160e-04 -9.469002509116768293e-04 -9.451402339231094194e-04 -9.422041557061587753e-04 -9.380880818219303153e-04 -9.327867860093526668e-04 -9.262940346081568674e-04 -9.186029553785285927e-04 -9.097064921007158968e-04 -8.995979480015558636e-04 -8.882716126522533038e-04 -8.757234804300717199e-04 -8.619520473458365918e-04 -8.469591852289613939e-04 -8.307510805982074855e-04
+-8.903230522856420094e-04 -8.895810995614577849e-04 -8.879103596353824564e-04 -8.851239623066770815e-04 -8.812192899662514567e-04 -8.761929356068748819e-04 -8.700409615184004743e-04 -8.627592330435637736e-04 -8.543438270261016028e-04 -8.447915188077408100e-04 -8.341003334306284307e-04 -8.222701794999287550e-04 -8.093035388494183597e-04 -7.952062170329688697e-04 -7.799881388579493497e-04
+-8.351887330873533546e-04 -8.344891700722620450e-04 -8.329099322940080024e-04 -8.302767775036341922e-04 -8.265881840920869059e-04 -8.218422541088979145e-04 -8.160369455417237124e-04 -8.091703706267949943e-04 -8.012411590011069397e-04 -7.922488870294708795e-04 -7.821945619802077570e-04 -7.710811714270329005e-04 -7.589142771624515912e-04 -7.457026539098171331e-04 -7.314589585507538967e-04
+-7.821595820710307420e-04 -7.815026324080796795e-04 -7.800162324055439408e-04 -7.775384134917095492e-04 -7.740685509266464689e-04 -7.696059770243692064e-04 -7.641501873067567006e-04 -7.577011041698069509e-04 -7.502593965124066495e-04 -7.418268535448338877e-04 -7.324068078805637781e-04 -7.220046057083678425e-04 -7.106281150631564179e-04 -6.982882651246320261e-04 -6.849996053035865970e-04
+-7.311122725026915434e-04 -7.304978447330395764e-04 -7.291048879069307641e-04 -7.267832953843901761e-04 -7.235331622360977651e-04 -7.193548023143311399e-04 -7.142489328471960915e-04 -7.082169014931703798e-04 -7.012609664811886908e-04 -6.933846195858336080e-04 -6.845929507173066728e-04 -6.748930487184274900e-04 -6.642944320611530833e-04 -6.528095011030551724e-04 -6.404540019631755439e-04
+-6.819225784337563587e-04 -6.813503303536915055e-04 -6.800508341256953498e-04 -6.778853924310068854e-04 -6.748546649603108950e-04 -6.709597260827717584e-04 -6.662022406622951755e-04 -6.605846449840330637e-04 -6.541103975747664676e-04 -6.467842516682694148e-04 -6.386125691736010360e-04 -6.296036585786376517e-04 -6.197681370578717042e-04 -6.091193070543158726e-04 -5.976735384738579050e-04
+-6.344661696495458017e-04 -6.339355649225831809e-04 -6.327290843775139340e-04 -6.307189606341845594e-04 -6.279062783715837204e-04 -6.242926932510132684e-04 -6.198805672234960996e-04 -6.146731390338268115e-04 -6.086747330291606122e-04 -6.018909872945133951e-04 -5.943291240451870940e-04 -5.859982308447592245e-04 -5.769095628614078885e-04 -5.670768539851708985e-04 -5.565166293829636700e-04
+-5.886192385693716925e-04 -5.881295959733982967e-04 -5.870153336398569290e-04 -5.851591197962051003e-04 -5.825623483874434703e-04 -5.792270879160282739e-04 -5.751561965790997393e-04 -5.703534672464700365e-04 -5.648238024019070673e-04 -5.585734092370199565e-04 -5.516100229260742461e-04 -5.439431420961489405e-04 -5.355842782018414199e-04 -5.265472103001638243e-04 -5.168482385094878579e-04
+-5.442589800939208900e-04 -5.438095158906122630e-04 -5.427864166390825723e-04 -5.410822866993085208e-04 -5.386987289648140741e-04 -5.356380860799499818e-04 -5.319035372441941389e-04 -5.274992200519256413e-04 -5.224303752887910889e-04 -5.167035120298900342e-04 -5.103265897568618013e-04 -5.033092135337792700e-04 -4.956628375701784819e-04 -4.874009717585961465e-04 -4.785393850808986938e-04
+-5.012639441615498884e-04 -5.008538081328975117e-04 -4.999206402968542177e-04 -4.983664845571914416e-04 -4.961930682004098625e-04 -4.934028913322069257e-04 -4.899993071129954848e-04 -4.859866224865034157e-04 -4.813702175003603404e-04 -4.761566808177817483e-04 -4.703539584868276276e-04 -4.639715124727493293e-04 -4.570204848821389824e-04 -4.495138632334708334e-04 -4.414666415698066714e-04
+-4.595142793560014986e-04 -4.591425850710304174e-04 -4.582980089399852491e-04 -4.568915471970093974e-04 -4.549249812746479060e-04 -4.524008719790855544e-04 -4.493226247888770395e-04 -4.456945716333065590e-04 -4.415220674660926816e-04 -4.368115995260164535e-04 -4.315709067330757110e-04 -4.258091062119396088e-04 -4.195368234750575416e-04 -4.127663223503968753e-04 -4.055116303242194695e-04
+-4.188918844169252863e-04 -4.185577342821148860e-04 -4.178003590952124053e-04 -4.165392347459481617e-04 -4.147761395170393071e-04 -4.125136169013914468e-04 -4.097550228606459217e-04 -4.065046017838647337e-04 -4.027675480207443997e-04 -3.985501026248353985e-04 -3.938596425504410073e-04 -3.887047798184674742e-04 -3.830954621297117399e-04 -3.770430724054411008e-04 -3.705605237312313734e-04
+-3.792804830289472039e-04 -3.789829886454556336e-04 -3.783114191475872340e-04 -3.771932759785892163e-04 -3.756302887038526065e-04 -3.736249207349351528e-04 -3.711804018028201082e-04 -3.683007929495572060e-04 -3.649910265247866014e-04 -3.612569824698030072e-04 -3.571055550672030065e-04 -3.525447271002871965e-04 -3.475836968449047461e-04 -3.422326899186101828e-04 -3.365035508571560460e-04
+-3.405656358729733922e-04 -3.403039341765820352e-04 -3.397168076986086774e-04 -3.387393509856057158e-04 -3.373732099849121322e-04 -3.356207184349508689e-04 -3.334849256265849226e-04 -3.309696330567753718e-04 -3.280794343957060388e-04 -3.248197622845663151e-04 -3.211969378260469020e-04 -3.172182221473917609e-04 -3.128918681579832568e-04 -3.082271705795923910e-04 -3.032345121767639358e-04
+-3.026347026528157362e-04 -3.024079682577169854e-04 -3.019039831594671000e-04 -3.010650264873721829e-04 -2.998926354531938703e-04 -2.983889808376992176e-04 -2.965568850580203191e-04 -2.943998445152768676e-04 -2.919220555611349178e-04 -2.891284432767487903e-04 -2.860246921161718942e-04 -2.826172773309047499e-04 -2.789134959670924729e-04 -2.749214961161583742e-04 -2.706503030087689470e-04
+-2.653767657022094301e-04 -2.651842198080171797e-04 -2.647621559845870468e-04 -2.640596549627388569e-04 -2.630781291884592239e-04 -2.618195647630463282e-04 -2.602865297398416003e-04 -2.584821842515103532e-04 -2.564102920689981572e-04 -2.540752331115862773e-04 -2.514820163514382449e-04 -2.486362924861006021e-04 -2.455443656914036376e-04 -2.422132037166483342e-04 -2.386504455462242370e-04
+-2.286825258493388078e-04 -2.285234420043431272e-04 -2.281821740093804775e-04 -2.276142478082923389e-04 -2.268209436348089369e-04 -2.258040528481157711e-04 -2.245658769213001440e-04 -2.231092252899060150e-04 -2.214374140850560130e-04 -2.195542619825127835e-04 -2.174640866035053494e-04 -2.151716991231456639e-04 -2.126823976299026990e-04 -2.100019589618755899e-04 -2.071366288614814063e-04
+-1.924441804775619343e-04 -1.923178874261406647e-04 -1.920563906143963706e-04 -1.916213319952455316e-04 -1.910138604166581374e-04 -1.902355729499901021e-04 -1.892885095052174432e-04 -1.881751272032748299e-04 -1.868983007578120590e-04 -1.854612917905531372e-04 -1.838677327091178186e-04 -1.821216028743284621e-04 -1.802272037677908156e-04 -1.781891327570682892e-04 -1.760122559122721895e-04
+-1.565552931869531846e-04 -1.564611749616008629e-04 -1.562785249008071019e-04 -1.559747991527966936e-04 -1.555510241588373404e-04 -1.550086165513289704e-04 -1.543493660844537894e-04 -1.535754022288338778e-04 -1.526891779207790361e-04 -1.516934234567472056e-04 -1.505911139147425430e-04 -1.493854269729313292e-04 -1.480796994453595036e-04 -1.466773824615666541e-04 -1.451819963619547247e-04
+-1.209106641247459802e-04 -1.208481574786645003e-04 -1.207435227303678676e-04 -1.205697556782948997e-04 -1.203277775530831061e-04 -1.200188481635659126e-04 -1.196445370975368237e-04 -1.192066835516263903e-04 -1.187073583230156956e-04 -1.181488071322143031e-04 -1.175333977857371441e-04 -1.168635593510359031e-04 -1.161417189791529047e-04 -1.153702372765133804e-04 -1.145513439316878795e-04
+-8.540620991638820172e-05 -8.537479913062222996e-05 -8.534742735372683646e-05 -8.530238235263332353e-05 -8.524050580118857495e-05 -8.516293579499212372e-05 -8.507106728205041362e-05 -8.496650218664416991e-05 -8.485099002429391177e-05 -8.472636003172386368e-05 -8.459444608355796069e-05 -8.445700593338412252e-05 -8.431563659510601071e-05 -8.417168796056564897e-05 -8.402617701761509609e-05
+-4.993886218588607616e-05 -4.993807122634710827e-05 -4.998726841850588149e-05 -5.006981201857566878e-05 -5.018649865971846775e-05 -5.033839240365273497e-05 -5.052677434503157405e-05 -5.075307912517131991e-05 -5.101881875947753952e-05 -5.132549679819455642e-05 -5.167451150358203741e-05 -5.206705289337494342e-05 -5.250399421300811290e-05 -5.298578110364072016e-05 -5.351232143560569719e-05
+-1.440649389470921235e-05 -1.443587583957581157e-05 -1.456097840376360244e-05 -1.477003415188839859e-05 -1.506383860552231932e-05 -1.544344250770134704e-05 -1.591008977492192750e-05 -1.646513967854505581e-05 -1.710997046966688260e-05 -1.784587771194533603e-05 -1.867394957514207114e-05 -1.959494103498756650e-05 -2.060913799110014643e-05 -2.171621851057673218e-05 -2.291511441406603742e-05
+2.129211686639119689e-05 2.123299325434508051e-05 2.103265404354792917e-05 2.069816439176732671e-05 2.022867587444696861e-05 1.962307633574048851e-05 1.888006453270094217e-05 1.799824381179087858e-05 1.697623917968016588e-05 1.581281930063317296e-05 1.450704933151237414e-05 1.305844391084572727e-05 1.146713387980972162e-05 9.734037234588200499e-06 7.861030643412569505e-06
+5.725727544098659907e-05 5.716884216262741424e-05 5.689398381041434541e-05 5.643521255386786889e-05 5.579156336519544481e-05 5.496176932853069500e-05 5.394436149858637935e-05 5.273776844714751473e-05 5.134046061294219015e-05 4.975109601413263069e-05 4.796870204770790338e-05 4.599286041131100868e-05 4.382390880326703358e-05 4.146314924547653833e-05 3.891305848931745932e-05
+9.358830066279324534e-05 9.347101014414884021e-05 9.312245128540987344e-05 9.254071151539120660e-05 9.172463037106698197e-05 9.067268694509079225e-05 8.938310276329630710e-05 8.785397229968270249e-05 8.608342270260022642e-05 8.406979260397652197e-05 8.181184167572460664e-05 7.930897381340349826e-05 7.656147842413283094e-05 7.357078202157446567e-05 7.033970448712363122e-05
+1.303833847868369165e-04 1.302377329603673743e-04 1.298164550146288314e-04 1.291133228795305482e-04 1.281268928697113256e-04 1.268552628878315031e-04 1.252961908582439781e-04 1.234472459477588486e-04 1.213059912461359998e-04 1.188701982494646744e-04 1.161380851383991028e-04 1.131085852862010713e-04 1.097816323531601622e-04 1.061584621963684405e-04 1.022419230581831512e-04
+1.677393709015124394e-04 1.675659239059841066e-04 1.670731426193581681e-04 1.662505761396056983e-04 1.650963954831440560e-04 1.636081750395074479e-04 1.617830272962706914e-04 1.596177755249350420e-04 1.571091631101256695e-04 1.542541024367473888e-04 1.510499488590763767e-04 1.474948176989647128e-04 1.435879192005120718e-04 1.393299183989325806e-04 1.347233083924413623e-04
+2.057514346839201002e-04 2.055508593539513164e-04 2.049881067210997001e-04 2.040485820436407916e-04 2.027299553394957339e-04 2.010291157158658470e-04 1.989423227815715115e-04 1.964654015707494148e-04 1.935939800540938029e-04 1.903237736253615264e-04 1.866508999053186763e-04 1.825722468358903635e-04 1.780858647205720837e-04 1.731913919431826102e-04 1.678905015707220423e-04
+2.445126567532744915e-04 2.442857550076726566e-04 2.436549718963066475e-04 2.426016376098576025e-04 2.411227916665315105e-04 2.392144562526028815e-04 2.368718042036946749e-04 2.340893763286164232e-04 2.308613479052699252e-04 2.271818496553734213e-04 2.230453272386292637e-04 2.184469634060988365e-04 2.133831338422536184e-04 2.078519070475345204e-04 2.018535754700689975e-04
+2.841134715038249247e-04 2.838612186430499525e-04 2.831648581723679404e-04 2.820017078697660984e-04 2.803680337458632778e-04 2.782587897621604861e-04 2.756678015377250833e-04 2.725880053520892549e-04 2.690117436651027951e-04 2.649311210802322543e-04 2.603384145863961788e-04 2.552265477837283155e-04 2.495896195977550321e-04 2.434234854189066123e-04 2.367263845588558251e-04
+3.246409782942185924e-04 3.243645650777759125e-04 3.236057064103238208e-04 3.223377690481250553e-04 3.205560899228327961e-04 3.182543348858875949e-04 3.154246963276812464e-04 3.120581519427931315e-04 3.081447874922549953e-04 3.036741867266367365e-04 2.986358927396745599e-04 2.930199352208314898e-04 2.868174373231125937e-04 2.800212851455775409e-04 2.726268631366755108e-04
+3.661781014088232229e-04 3.658789795867687798e-04 3.650614512605686464e-04 3.636949979930172920e-04 3.617738612967524728e-04 3.592901827010894027e-04 3.562342122290866045e-04 3.525945834124888574e-04 3.483586594823643895e-04 3.435129554200808057e-04 3.380436449637675084e-04 3.319371443429039253e-04 3.251807968641513792e-04 3.177636375809928166e-04 3.096772468922749178e-04
+4.088025864557044676e-04 4.084825171776391983e-04 4.076110284147270576e-04 4.061537962157117697e-04 4.041037841002609061e-04 4.014513688179910020e-04 3.981845273339296100e-04 3.942891364483367116e-04 3.897493336753943879e-04 3.845479656923149621e-04 3.786671346583318060e-04 3.720888360629950051e-04 3.647957187679766217e-04 3.567719481455699539e-04 3.480041862100374177e-04
+4.525858230453858370e-04 4.522469272581638674e-04 4.513272048256862078e-04 4.497886163377000173e-04 4.476226860108281722e-04 4.448177533639898103e-04 4.413591878548323304e-04 4.372296775069973063e-04 4.324096009524851757e-04 4.268774929042405751e-04 4.206106193914015850e-04 4.135856636983516535e-04 4.057795526260102661e-04 3.971704183928066951e-04 3.877387095156992246e-04
+4.975914869242235167e-04 4.972362964928225566e-04 4.962752236624505542e-04 4.946666393113646407e-04 4.924004439931197645e-04 4.894626932959718173e-04 4.858358038909535871e-04 4.814988344165748065e-04 4.764278533685169887e-04 4.705964078517561574e-04 4.639761118749589539e-04 4.565373682031287090e-04 4.482502459708392092e-04 4.390855333596050455e-04 4.290159773036168701e-04
+5.438739994237118142e-04 5.435055072815508665e-04 5.425112602467858968e-04 5.408461994402075047e-04 5.384984350462920615e-04 5.354514946563359050e-04 5.316845099705878267e-04 5.271724763471259288e-04 5.218865998337174697e-04 5.157947501278841535e-04 5.088620409362704404e-04 5.010515654287581470e-04 4.923253039940632663e-04 4.826452488970275250e-04 4.719747587417634873e-04
+5.914768083433094570e-04 5.910985155033541671e-04 5.900806913086004135e-04 5.883750545249619417e-04 5.859677767407752780e-04 5.828396372670645656e-04 5.789661775588852239e-04 5.743179223865631493e-04 5.688606851677494936e-04 5.625559799583025036e-04 5.553615666289245375e-04 5.472321658068114584e-04 5.381203668994831305e-04 5.279777921317149346e-04 5.167565359090243483e-04
+6.404305023388424988e-04 6.400464591138151256e-04 6.390161877882032365e-04 6.372884506733861570e-04 6.348473619585295706e-04 6.316707717249051999e-04 6.277303729844919879e-04 6.229918644087579366e-04 6.174151885793744028e-04 6.109548719646532922e-04 6.035604985274046347e-04 5.951773612376931978e-04 5.857473255082113828e-04 5.752099813499561868e-04 5.635041223528319040e-04
+6.907507806085445585e-04 6.903656189019672946e-04 6.893356511724489828e-04 6.876070189155989235e-04 6.851617020589919910e-04 6.819744978333401033e-04 6.780130636139824508e-04 6.732379984512394709e-04 6.676029848134358742e-04 6.610550196155186471e-04 6.535347713468918438e-04 6.449771131344852072e-04 6.353118823229685422e-04 6.244649475012084908e-04 6.123596564960467978e-04
+7.424363110639263172e-04 7.420552642030200669e-04 7.410400250193875963e-04 7.393345304351722595e-04 7.369186048996567663e-04 7.337639464666476921e-04 7.298340876399101460e-04 7.250843711710461270e-04 7.194619627535912745e-04 7.129059311364307691e-04 7.053474359189058386e-04 6.967100757744820825e-04 6.869104672986728419e-04 6.758591310556321752e-04 6.634618054989966686e-04
+7.954665230040306985e-04 7.950954293016421984e-04 7.941110266099873395e-04 7.924555538745018876e-04 7.901067287193949944e-04 7.870332020009180793e-04 7.831944190217403432e-04 7.785404646655539555e-04 7.730119131061621764e-04 7.665397118267194224e-04 7.590451410439010265e-04 7.504399016430759453e-04 7.406264161179160373e-04 7.294984192463244794e-04 7.169419933515294155e-04
+8.497993940897636839e-04 8.494446802416487970e-04 8.485088581959106995e-04 8.469330735808934573e-04 8.446930695154898118e-04 8.417546206608877068e-04 8.380732789081229940e-04 8.335940644547611914e-04 8.282511197391929621e-04 8.219673520014023635e-04 8.146541022902907634e-04 8.062108925004302443e-04 7.965253352309501714e-04 7.854732931065484380e-04 7.729194544070187986e-04
+9.053693054086240071e-04 9.050379460413559597e-04 9.041699723337523822e-04 9.027061439579017786e-04 9.006204575928778485e-04 8.978761204921536154e-04 8.944251680310230310e-04 8.902079816904711652e-04 8.851527188048981427e-04 8.791746725023559224e-04 8.721755906505191530e-04 8.640430005769834422e-04 8.546496090722409617e-04 8.438528764798476547e-04 8.314949193206844702e-04
+9.620850516426366749e-04 9.617845018532866080e-04 9.610049803237853683e-04 9.596876712286764571e-04 9.578051576340312033e-04 9.553185403093021047e-04 9.521769201412776237e-04 9.483167310408299137e-04 9.436609256757508149e-04 9.381180211775292863e-04 9.315810185545449554e-04 9.239262302300722471e-04 9.150120602440450909e-04 9.046778294480712062e-04 8.927427771849449521e-04
+1.019828104536427225e-03 1.019566203215361601e-03 1.018896805443223223e-03 1.017762428523459085e-03 1.016134683758727723e-03 1.013973186286363766e-03 1.011224903021963649e-03 1.007823298702623105e-03 1.003687270793865265e-03 9.987198651244357569e-04 9.928067653395830985e-04 9.858145682362859374e-04 9.775888541348632527e-04 9.679521172605712667e-04 9.567016415237949295e-04
+1.078451235604301712e-03 1.078236078682866857e-03 1.077699193033213000e-03 1.076785421604129454e-03 1.075465955866938394e-03 1.073699703800969768e-03 1.071432518576497265e-03 1.068596167981960372e-03 1.065107029026979204e-03 1.060864479841324131e-03 1.055748957704640435e-03 1.049619659789777833e-03 1.042311855615659678e-03 1.033633818950116653e-03 1.023363396283861202e-03
+1.137777606807224666e-03 1.137617391321094290e-03 1.137235686671975035e-03 1.136580728797338550e-03 1.135623932748440002e-03 1.134324426012888083e-03 1.132628173789606727e-03 1.130466799170850266e-03 1.127756068758391499e-03 1.124393995098790702e-03 1.120258498248112317e-03 1.115204559406844263e-03 1.109060787617677062e-03 1.101625326583902673e-03 1.092661025967427190e-03
+1.197600434397516492e-03 1.197503276306042218e-03 1.197299197426328300e-03 1.196940937999985913e-03 1.196400859370493411e-03 1.195639356553409487e-03 1.194603906256766707e-03 1.193227781162208966e-03 1.191428380338945903e-03 1.189105107747905196e-03 1.186136715755185768e-03 1.182377999024918644e-03 1.177655665185332271e-03 1.171763516009581346e-03 1.164455844788192095e-03
+1.257683320184378034e-03 1.257657051103567908e-03 1.257652255382885357e-03 1.257627294237927519e-03 1.257556258038091930e-03 1.257401938737739890e-03 1.257114847491037348e-03 1.256631878975797336e-03 1.255874561901108247e-03 1.254746810700267494e-03 1.253132073410861492e-03 1.250889719710743947e-03 1.247850486196835831e-03 1.243810722486659399e-03 1.238525116661573283e-03
+1.317761325589789263e-03 1.317813275760511358e-03 1.318028025705066716e-03 1.318370652156117002e-03 1.318817774150986277e-03 1.319335745458418991e-03 1.319879690804863330e-03 1.320392188792655431e-03 1.320801535357243265e-03 1.321019492105325556e-03 1.320938401801144673e-03 1.320427483861390293e-03 1.319328089728195831e-03 1.317447588154293083e-03 1.314551447331703104e-03
+1.377542837235361164e-03 1.377679613915196166e-03 1.378132160793300127e-03 1.378873298789150183e-03 1.379882956549385083e-03 1.381132191197166799e-03 1.382582295899886663e-03 1.384183576167208763e-03 1.385873729203936089e-03 1.387575730228658624e-03 1.389195104292212206e-03 1.390616389443555647e-03 1.391698552625848968e-03 1.392268994269452251e-03 1.392115640647252888e-03
+1.436712239518718372e-03 1.436939511304274669e-03 1.437645493956956266e-03 1.438811673973945573e-03 1.440422010645646270e-03 1.442453320745415695e-03 1.444874509086494386e-03 1.447645512256422184e-03 1.450715897297177089e-03 1.454023029489613259e-03 1.457489698474776028e-03 1.461021025323194777e-03 1.464500425269463181e-03 1.467784278220729847e-03 1.470694812369419385e-03
+1.494933371704813569e-03 1.495255669823951968e-03 1.496227560620981209e-03 1.497839971017480556e-03 1.500081512080813848e-03 1.502935670759180135e-03 1.506380208777470010e-03 1.510386339352761016e-03 1.514917637586273881e-03 1.519928619303620790e-03 1.525362903135306283e-03 1.531150819129739517e-03 1.537206286707124350e-03 1.543422685752320620e-03 1.549667319410780826e-03
+1.551853707293095576e-03 1.552274254496055711e-03 1.553520882266766446e-03 1.555594552190812593e-03 1.558489013454818347e-03 1.562195134810128068e-03 1.566700506050796617e-03 1.571988897252240246e-03 1.578039551116103539e-03 1.584826271856157711e-03 1.592316263779347844e-03 1.600468642333039912e-03 1.609232519290700438e-03 1.618544505540142923e-03 1.628325401803269821e-03
+1.607109155181227905e-03 1.607629731463843881e-03 1.609155907342611986e-03 1.611699066648955309e-03 1.615258421951038404e-03 1.619832696568799905e-03 1.625419947854061208e-03 1.632017336730710085e-03 1.639620840940067418e-03 1.648224909462504221e-03 1.657822055574539747e-03 1.668402382819046898e-03 1.679953041994763658e-03 1.692457611058442854e-03 1.705895388811977430e-03
+1.660329348971636412e-03 1.660950201058192894e-03 1.662756466726136948e-03 1.665770117008108508e-03 1.669995977214778354e-03 1.675440836609228120e-03 1.682113495697065697e-03 1.690024848755089472e-03 1.699188021032543242e-03 1.709618592611194697e-03 1.721334949519225978e-03 1.734358830187652210e-03 1.748716160717355859e-03 1.764438321904456984e-03 1.781564062303522171e-03
+1.711143265856331346e-03 1.711863064382248547e-03 1.713945573771618464e-03 1.717423289864039278e-03 1.722306622206002703e-03 1.728610373344912059e-03 1.736353995381568344e-03 1.745561963176328266e-03 1.756264302849456019e-03 1.768497336324517449e-03 1.782304721435543646e-03 1.797738914588907543e-03 1.814863232179274831e-03 1.833754776028783057e-03 1.854508618054921416e-03
+1.759185002327732540e-03 1.760000847309254723e-03 1.762351383389618121e-03 1.766279347976419320e-03 1.771800539303735158e-03 1.778937473634999676e-03 1.787719821562691689e-03 1.798185028070354522e-03 1.810379168411815291e-03 1.824358121485483231e-03 1.840189165441715336e-03 1.857953163009643622e-03 1.877747564836039192e-03 1.899690571164378483e-03 1.923926951246184751e-03
+1.804099531761954329e-03 1.805007003615665025e-03 1.807613122504892747e-03 1.811970379883271528e-03 1.818099622092835899e-03 1.826030566900010412e-03 1.835802379345478734e-03 1.847464479362075909e-03 1.861077639633390568e-03 1.876715465159572473e-03 1.894466369284549369e-03 1.914436229398921345e-03 1.936751966611402476e-03 1.961566408137693437e-03 1.989064947123943099e-03
+1.845548278614710753e-03 1.846541529083385764e-03 1.849386815531844268e-03 1.854145716147896812e-03 1.860843669966047746e-03 1.869516918162784837e-03 1.880213173786910146e-03 1.892992550094415791e-03 1.907928804832717757e-03 1.925110990646725518e-03 1.944645620040595310e-03 1.966659519932360996e-03 1.991303600659377962e-03 2.018757863844197493e-03 2.049238099795162686e-03
+1.883214364078664811e-03 1.884286239258832355e-03 1.887350651482723766e-03 1.892477448182679602e-03 1.899696125400040158e-03 1.909048656976812790e-03 1.920590212587258141e-03 1.934390140706869141e-03 1.950533265932519016e-03 1.969121579723951028e-03 1.990276412657867970e-03 2.014141235191107583e-03 2.040885264271453774e-03 2.070708126439796664e-03 2.103845909254446495e-03
+1.916807405905026794e-03 1.917949592384525287e-03 1.921209870900758522e-03 1.926665422113896719e-03 1.934349217929925546e-03 1.944308114701372159e-03 1.956603579186990370e-03 1.971312668338266912e-03 1.988529299408551936e-03 2.008365870508360945e-03 2.030955290424741634e-03 2.056453522392366531e-03 2.085042754919002369e-03 2.116935354711606352e-03 2.152378789647163559e-03
+1.946067787259110442e-03 1.947270972233684262e-03 1.950701087003303214e-03 1.956441621655287313e-03 1.964528428582660788e-03 1.975012384385244069e-03 1.987960092599972816e-03 2.003454816620974833e-03 2.021597663152754475e-03 2.042509053911455239e-03 2.066330509157577981e-03 2.093226800487284645e-03 2.123388515152959278e-03 2.157035087136737351e-03 2.194418340266018549e-03
+1.970770342195820018e-03 1.972024379289112443e-03 1.975595991928296574e-03 1.981573895431432922e-03 1.989996237626697351e-03 2.000917077664307771e-03 2.014407046053377434e-03 2.030554204492287206e-03 2.049465109127814738e-03 2.071266091211242544e-03 2.096104744290711204e-03 2.124151627948751928e-03 2.155602163688396990e-03 2.190678687049118275e-03 2.229632577901976762e-03
+1.990727435085379478e-03 1.992021509254015763e-03 1.995704431784978486e-03 2.001869020982242724e-03 2.010555161326343585e-03 2.021819304512179581e-03 2.035735079798804605e-03 2.052394072987184358e-03 2.071906762320304199e-03 2.094403603727207006e-03 2.120036223943943306e-03 2.148978690238674983e-03 2.181428776058612351e-03 2.217609112615255822e-03 2.257768053183365538e-03
+2.005791435208882211e-03 2.007114222298937451e-03 2.010876860098385292e-03 2.017175126127749695e-03 2.026050115640301314e-03 2.037559939188916293e-03 2.051780287905799471e-03 2.068805140850025169e-03 2.088747590490189036e-03 2.111740761735888747e-03 2.137938671950462971e-03 2.167517580440285127e-03 2.200675871009270812e-03 2.237635360731352312e-03 2.278640740073100638e-03
+2.015856603889921907e-03 2.017196422797239239e-03 2.021006196141082213e-03 2.027383506202121675e-03 2.036370163913153904e-03 2.048025256414838340e-03 2.062425681233824235e-03 2.079666804795976803e-03 2.099863213498809333e-03 2.123149521922287897e-03 2.149681157958511363e-03 2.179635042471140833e-03 2.213210015355573327e-03 2.250626813054911520e-03 2.292127321763994929e-03
+2.020860419191692400e-03 2.022205376841554499e-03 2.026029121821783067e-03 2.032429882145821761e-03 2.041449710903676940e-03 2.053148025149787500e-03 2.067602128989554262e-03 2.084907854776184722e-03 2.105180287943669674e-03 2.128554536340980258e-03 2.155186458742839629e-03 2.185253263511987686e-03 2.218953820715758446e-03 2.256508482283145663e-03 2.298158122377772644e-03
+2.020784362822821562e-03 2.022122494029693351e-03 2.025926848816978453e-03 2.032295140339108758e-03 2.041269198068018653e-03 2.052908135011566153e-03 2.067288881804505742e-03 2.084506845110253338e-03 2.104676658558049442e-03 2.127932990795217052e-03 2.154431330435688848e-03 2.184348665516433214e-03 2.217883909333628716e-03 2.255257877714573859e-03 2.296712541958654836e-03
+2.015654186925650709e-03 2.016973592398041241e-03 2.020725378208333700e-03 2.027005582416672308e-03 2.035855337429695773e-03 2.047332805639400042e-03 2.061513744528119339e-03 2.078492213792656248e-03 2.098381400555727333e-03 2.121314538079601287e-03 2.147445765415674848e-03 2.176951476486779172e-03 2.210030202192599449e-03 2.246903918692858080e-03 2.287817487002505746e-03
+2.005539667162692039e-03 2.006828653334607332e-03 2.010495260631447578e-03 2.016632695138919924e-03 2.025280897255691149e-03 2.036496396697614914e-03 2.050352922584403915e-03 2.066942182080929759e-03 2.086374795888929629e-03 2.108781383012403587e-03 2.134313753331627209e-03 2.163146176715352326e-03 2.195476647991397110e-03 2.231528037794985007e-03 2.271548956073335054e-03
+1.990553835765705281e-03 1.991801059719990313e-03 1.995350849010544495e-03 2.001292430324092333e-03 2.009664026398380425e-03 2.020519800902541470e-03 2.033930518121191550e-03 2.049984402333732657e-03 2.068788200525959343e-03 2.090468462404434461e-03 2.115173026855558715e-03 2.143072724861311371e-03 2.174363274478522713e-03 2.209267331966693285e-03 2.248036621017975890e-03
+1.970851676955098341e-03 1.972046298499033085e-03 1.975449021696829011e-03 1.981143966681428795e-03 1.989167080050758575e-03 1.999569369845304641e-03 2.012417607834392913e-03 2.027795261868475894e-03 2.045803678643081519e-03 2.066563554592226303e-03 2.090216718498000888e-03 2.116928283247285995e-03 2.146889209010586531e-03 2.180319333071477524e-03 2.217470911600932359e-03
+1.946628260168658045e-03 1.947760101276254296e-03 1.950987344405690112e-03 1.956387912743036070e-03 1.963994892077033060e-03 1.973855297656071286e-03 1.986030799610500816e-03 2.000598702051964439e-03 2.017653212348344098e-03 2.037307060701299809e-03 2.059693528848265988e-03 2.084968992581225523e-03 2.113316091190091568e-03 2.144947678882726423e-03 2.180111746132067790e-03
+1.918116286151728273e-03 1.919175995725335912e-03 1.922201637365493184e-03 1.927263905987432668e-03 1.934392431656010471e-03 1.943629375209877594e-03 1.955030145659867376e-03 1.968664382348214031e-03 1.984617251285683819e-03 2.002991134740773633e-03 2.023907802176937425e-03 2.047511209539747221e-03 2.073971104238642432e-03 2.103487686473766525e-03 2.136297658746148451e-03
+1.885583028627598259e-03 1.886562248144374454e-03 1.889362921268441207e-03 1.894047569729317157e-03 1.900641787271237573e-03 1.909182030928836035e-03 1.919716290025519139e-03 1.932305013572267055e-03 1.947022353415449976e-03 1.963957813310691480e-03 1.983218412362080813e-03 2.004931537870103218e-03 2.029248712453284725e-03 2.056350599860963177e-03 2.086453700160068210e-03
+1.849326670415652992e-03 1.850218193838942555e-03 1.852773732519767550e-03 1.857046807181673065e-03 1.863058440193129679e-03 1.870838594919545369e-03 1.880426750739088012e-03 1.891872709593882306e-03 1.905237692553539636e-03 1.920595817862687281e-03 1.938036075232825147e-03 1.957664979599813612e-03 1.979610148647829859e-03 2.004025162857546449e-03 2.031096222805385716e-03
+1.809672056753794172e-03 1.810469976433557370e-03 1.812763824172440802e-03 1.816597440546551152e-03 1.821986821851509855e-03 1.828954760692557161e-03 1.837531281344320774e-03 1.847754258610670051e-03 1.859670272244283874e-03 1.873335778609594394e-03 1.888818704333929078e-03 1.906200629441115587e-03 1.925579788269053509e-03 1.947075228509317739e-03 1.970832627818953128e-03
+1.766965918331212188e-03 1.767665747761459818e-03 1.769685301744830085e-03 1.773058239783715769e-03 1.777795192330807730e-03 1.783911270147303402e-03 1.791426319805367344e-03 1.800365295551252260e-03 1.810758786174801026e-03 1.822643757640591200e-03 1.836064591009006590e-03 1.851074542646899716e-03 1.867737802937071605e-03 1.886132418766752828e-03 1.906354475134644597e-03
+1.721571649257334176e-03 1.722170413696245310e-03 1.723907279630076039e-03 1.726805427182761697e-03 1.730869926320147004e-03 1.736107907652478539e-03 1.742528608559774103e-03 1.750143454230565065e-03 1.758966193053816468e-03 1.769013118357207334e-03 1.780303417095106507e-03 1.792859713584480730e-03 1.806708901767706699e-03 1.821883408962114877e-03 1.838423105591241316e-03
+1.673863757358931906e-03 1.674360044507296674e-03 1.675810180002264413e-03 1.678226785371349878e-03 1.681609342589914478e-03 1.685956950857638460e-03 1.691268148594056659e-03 1.697540681335420578e-03 1.704771212984210887e-03 1.712954977889959152e-03 1.722085371229652639e-03 1.732153471975749663e-03 1.743147496569864233e-03 1.755052175208650107e-03 1.767848041916919404e-03
+1.624222132061287288e-03 1.624616097152689490e-03 1.625779827705342573e-03 1.627715532915799011e-03 1.630417257236061769e-03 1.633876281372894420e-03 1.638080722355928203e-03 1.643014990972472850e-03 1.648659081921323476e-03 1.654987660128559145e-03 1.661968896389213286e-03 1.669562975117127538e-03 1.677720175888056890e-03 1.686378372281860166e-03 1.695459718557335016e-03
+1.573026295216956505e-03 1.573319617781453053e-03 1.574201517590874139e-03 1.575664158416569850e-03 1.577696473663417693e-03 1.580282400004346614e-03 1.583400274735043524e-03 1.587022010517461900e-03 1.591112003376119691e-03 1.595625708727825597e-03 1.600507800247235810e-03 1.605689774872612894e-03 1.611086826773998728e-03 1.616593714237293811e-03 1.622079217544799244e-03
+1.520649809946502881e-03 1.520845602833363359e-03 1.521454242068689738e-03 1.522458417443999694e-03 1.523842438986176048e-03 1.525583612813869805e-03 1.527651470015686406e-03 1.530006708236261075e-03 1.532599787746124782e-03 1.535369096163242486e-03 1.538238571069977479e-03 1.541114603149511351e-03 1.543881994573841673e-03 1.546398625001371447e-03 1.548488329449638134e-03
+1.467455020360966273e-03 1.467557694956860264e-03 1.467905264538094806e-03 1.468471694704080776e-03 1.469237294682027668e-03 1.470173652577444305e-03 1.471242741118776801e-03 1.472395691622093838e-03 1.473571170508354306e-03 1.474693262294071456e-03 1.475668737601237759e-03 1.476383512047826181e-03 1.476698057417431299e-03 1.476441401425437373e-03 1.475403213311288469e-03
+1.413788280847963616e-03 1.413803375417792491e-03 1.413905208787123030e-03 1.414059916270485762e-03 1.414244528899009923e-03 1.414425975250609624e-03 1.414560115701807763e-03 1.414590422818377607e-03 1.414446241740353405e-03 1.414040534913655559e-03 1.413266993447962394e-03 1.411996327975799728e-03 1.410071518898965400e-03 1.407301696540881955e-03 1.403454215296445545e-03
+1.359975808704594639e-03 1.359909789084765269e-03 1.359783806903704702e-03 1.359557165777125487e-03 1.359204401180651774e-03 1.358688926076167180e-03 1.357962046393431299e-03 1.356961622622604793e-03 1.355610317001232270e-03 1.353813341307959260e-03 1.351455600277793505e-03 1.348398074622833304e-03 1.344473260892653510e-03 1.339479411447799199e-03 1.333173252019298656e-03
+1.306320260728363299e-03 1.306180303998780027e-03 1.305846411595717191e-03 1.305272117103632246e-03 1.304430261920148416e-03 1.303281910828846474e-03 1.301775397720006475e-03 1.299845036926735534e-03 1.297409450057528156e-03 1.294369440293752270e-03 1.290605331084569924e-03 1.285973654625181687e-03 1.280303016797533196e-03 1.273389270978430438e-03 1.264988908632775667e-03
+1.253098096143456710e-03 1.252891868315648667e-03 1.252371337859134503e-03 1.251485349120936685e-03 1.250205834132667561e-03 1.248492641672350805e-03 1.246292660065485749e-03 1.243538634198143849e-03 1.240147647278350314e-03 1.236019218741965606e-03 1.231032960627192335e-03 1.225045725374708343e-03 1.217888166448630356e-03 1.209360636603959470e-03 1.199228353319397710e-03
+1.200557748484452252e-03 1.200293186708089807e-03 1.199608048116126762e-03 1.198447560028591263e-03 1.196783469951694838e-03 1.194575461647364237e-03 1.191770381163783461e-03 1.188301202857000843e-03 1.184085719853400281e-03 1.179024931080938999e-03 1.173001093718489905e-03 1.165875417662698725e-03 1.157485371566721166e-03 1.147641604785196992e-03 1.136124511314864655e-03
+1.148918591128897425e-03 1.148603699605498527e-03 1.147776175569363176e-03 1.146378654076710092e-03 1.144383343802796681e-03 1.141750693350544049e-03 1.138428736352272699e-03 1.134352233860329469e-03 1.129441604818296700e-03 1.123601636469161559e-03 1.116719967823306915e-03 1.108665358363202826e-03 1.099285750966849011e-03 1.088406192567411548e-03 1.075826704526310984e-03
+1.098370647900735004e-03 1.098013314820270011e-03 1.097065314351484879e-03 1.095467635479840766e-03 1.093193502428194651e-03 1.090204910532144474e-03 1.086452105614386932e-03 1.081872912984057928e-03 1.076391918421630524e-03 1.069919508289684552e-03 1.062350782531134609e-03 1.053564375250138794e-03 1.043421226055573020e-03 1.031763396749733105e-03 1.018413065308869554e-03
+1.049074973538519214e-03 1.048682814193585382e-03 1.047635494390033572e-03 1.045873215311699574e-03 1.043370661192392782e-03 1.040091998608860683e-03 1.035990490777450234e-03 1.031008011369030208e-03 1.025074469183472840e-03 1.018107162108493812e-03 1.010010089203949336e-03 1.000673268092084007e-03 9.899721247634098772e-04 9.777670602286346255e-04 9.639033430298345759e-04
+1.001164609950819804e-03 1.000744838966681526e-03 9.996182519631585314e-04 9.977250180730834819e-04 9.950416171606267512e-04 9.915348518662072102e-04 9.871615898314656419e-04 9.818684503339169655e-04 9.755914528086318893e-04 9.682556530332948712e-04 9.597748048031389976e-04 9.500510992924426912e-04 9.389750630633232143e-04 9.264257118303388487e-04 9.122711119771103987e-04
+9.547460132393893175e-04 9.543053468078038478e-04 9.531181691323588117e-04 9.511252652567187557e-04 9.483051417141900603e-04 9.446275501507430707e-04 9.400533448592140410e-04 9.345343231955585261e-04 9.280130695222427737e-04 9.204228324409832827e-04 9.116874764019445871e-04 9.017215614476136289e-04 8.904306313931120535e-04 8.777117991538393353e-04 8.634547656784031036e-04
+9.099008429463824538e-04 9.094454302024490133e-04 9.082147730035609705e-04 9.061508125134910482e-04 9.032342174087716960e-04 8.994378637587847674e-04 8.947267919681494656e-04 8.890581775679442600e-04 8.823813377886336601e-04 8.746378044583467742e-04 8.657615037155299469e-04 8.556790942608809248e-04 8.443105353375904721e-04 8.315699642329165949e-04 8.173669938254621726e-04
+8.666880077795851428e-04 8.662233891058414639e-04 8.649646829591009153e-04 8.628554233099981026e-04 8.598784929778046380e-04 8.560099491162338715e-04 8.512190619266758740e-04 8.454683908890334252e-04 8.387139200207707670e-04 8.309052812556216036e-04 8.219861031713711049e-04 8.118945323649555748e-04 8.005639841771459335e-04 7.879241971349862459e-04 7.739026658342824895e-04
```

### Comparing `he6_cres_spec_sims-0.1.5/he6_cres_spec_sims.egg-info/SOURCES.txt` & `he6_cres_spec_sims-0.2.0/src/he6_cres_spec_sims.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,61 @@
+LICENSE
 MANIFEST.in
 README.md
-setup.py
-he6_cres_spec_sims/__init__.py
-he6_cres_spec_sims/experiment.py
-he6_cres_spec_sims/simulation.py
-he6_cres_spec_sims/simulation_blocks.py
-he6_cres_spec_sims.egg-info/PKG-INFO
-he6_cres_spec_sims.egg-info/SOURCES.txt
-he6_cres_spec_sims.egg-info/dependency_links.txt
-he6_cres_spec_sims.egg-info/requires.txt
-he6_cres_spec_sims.egg-info/top_level.txt
-he6_cres_spec_sims/daq/__init__.py
-he6_cres_spec_sims/daq/frequency_domain_packet.py
-he6_cres_spec_sims/daq/example_spec/example_spec_file.spec
-he6_cres_spec_sims/daq/gain_noise_measurements/gain.csv
-he6_cres_spec_sims/daq/gain_noise_measurements/noise.csv
-he6_cres_spec_sims/spec_tools/__init__.py
-he6_cres_spec_sims/spec_tools/load_field_profile.py
-he6_cres_spec_sims/spec_tools/trap_field_profile.py
-he6_cres_spec_sims/spec_tools/beta_source/__init__.py
-he6_cres_spec_sims/spec_tools/beta_source/beta_source.py
-he6_cres_spec_sims/spec_tools/beta_source/beta_spectrum.py
-he6_cres_spec_sims/spec_tools/creating_trap_geometries/__init__.py
-he6_cres_spec_sims/spec_tools/creating_trap_geometries/load_default_field_profiles.py
-he6_cres_spec_sims/spec_tools/creating_trap_geometries/load_field_profile.py
-he6_cres_spec_sims/spec_tools/creating_trap_geometries/coil_classes/__init__.py
-he6_cres_spec_sims/spec_tools/creating_trap_geometries/coil_classes/coil_form.py
-he6_cres_spec_sims/spec_tools/creating_trap_geometries/coil_classes/field_profile.py
-he6_cres_spec_sims/spec_tools/creating_trap_geometries/coil_classes/trap_profile.py
-he6_cres_spec_sims/spec_tools/spec_calc/__init__.py
-he6_cres_spec_sims/spec_tools/spec_calc/power_calc.py
-he6_cres_spec_sims/spec_tools/spec_calc/spec_calc.py
-he6_cres_spec_sims/spec_tools/trap_field_profile_pkl/2021_trap_profile_mainfield_0T_trap_1A.csv
-he6_cres_spec_sims/spec_tools/trap_field_profile_pkl/__init__.py
-test/__init__.py
-test/conftest.py
+pyproject.toml
+run_local_experiment.py
+config_files/local_base_config_example.yaml
+config_files/local_exp_config_example.json
+config_files/rocks_base_config_example.yaml
+config_files/rocks_exp_config_example.json
+config_files/spec_example.json
+config_files/spec_example.yaml
+demo/local_sim_experiment_demo.ipynb
+demo/rocks_sim_experiment_demo.ipynb
+demo/readme_imgs/he6-cres_logo.png
+demo/readme_imgs/make_plot.png
+demo/readme_imgs/make_plot_1.png
+demo/readme_imgs/plot_stuff.png
+demo/readme_imgs/plot_stuff_1.png
+src/he6_cres_spec_sims/__init__.py
+src/he6_cres_spec_sims/constants.py
+src/he6_cres_spec_sims/experiment.py
+src/he6_cres_spec_sims/run_simulation.py
+src/he6_cres_spec_sims/simulation.py
+src/he6_cres_spec_sims.egg-info/PKG-INFO
+src/he6_cres_spec_sims.egg-info/SOURCES.txt
+src/he6_cres_spec_sims.egg-info/dependency_links.txt
+src/he6_cres_spec_sims.egg-info/requires.txt
+src/he6_cres_spec_sims.egg-info/top_level.txt
+src/he6_cres_spec_sims/daq/__init__.py
+src/he6_cres_spec_sims/daq/frequency_domain_packet.py
+src/he6_cres_spec_sims/simulation_blocks/DAQ.py
+src/he6_cres_spec_sims/simulation_blocks/__init__.py
+src/he6_cres_spec_sims/simulation_blocks/bandBuilder.py
+src/he6_cres_spec_sims/simulation_blocks/config.py
+src/he6_cres_spec_sims/simulation_blocks/dmTrackBuilder.py
+src/he6_cres_spec_sims/simulation_blocks/eventBuilder.py
+src/he6_cres_spec_sims/simulation_blocks/physics.py
+src/he6_cres_spec_sims/simulation_blocks/segmentBuilder.py
+src/he6_cres_spec_sims/simulation_blocks/trackBuilder.py
+src/he6_cres_spec_sims/spec_tools/__init__.py
+src/he6_cres_spec_sims/spec_tools/load_field_profile.py
+src/he6_cres_spec_sims/spec_tools/trap_field_profile.py
+src/he6_cres_spec_sims/spec_tools/beta_source/__init__.py
+src/he6_cres_spec_sims/spec_tools/beta_source/beta_source.py
+src/he6_cres_spec_sims/spec_tools/beta_source/beta_spectrum.py
+src/he6_cres_spec_sims/spec_tools/beta_source/beta_spectrum_alej_OLD.py
+src/he6_cres_spec_sims/spec_tools/beta_source/pickled_spectra/He6.json
+src/he6_cres_spec_sims/spec_tools/beta_source/pickled_spectra/Ne19.json
+src/he6_cres_spec_sims/spec_tools/creating_trap_geometries/__init__.py
+src/he6_cres_spec_sims/spec_tools/creating_trap_geometries/load_default_field_profiles.py
+src/he6_cres_spec_sims/spec_tools/creating_trap_geometries/load_field_profile.py
+src/he6_cres_spec_sims/spec_tools/creating_trap_geometries/coil_classes/__init__.py
+src/he6_cres_spec_sims/spec_tools/creating_trap_geometries/coil_classes/coil_form.py
+src/he6_cres_spec_sims/spec_tools/creating_trap_geometries/coil_classes/field_profile.py
+src/he6_cres_spec_sims/spec_tools/creating_trap_geometries/coil_classes/trap_profile.py
+src/he6_cres_spec_sims/spec_tools/spec_calc/__init__.py
+src/he6_cres_spec_sims/spec_tools/spec_calc/power_calc.py
+src/he6_cres_spec_sims/spec_tools/spec_calc/spec_calc.py
+src/he6_cres_spec_sims/spec_tools/trap_field_profile_pkl/2021_trap_profile_mainfield_0T_trap_1A.csv
+src/he6_cres_spec_sims/spec_tools/trap_field_profile_pkl/__init__.py
 test/test_simulation_blocks.py
```

