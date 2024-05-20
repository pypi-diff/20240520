# Comparing `tmp/vieworca-0.2.1.tar.gz` & `tmp/vieworca-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vieworca-0.2.1.tar", last modified: Tue May 14 13:13:49 2024, max compression
+gzip compressed data, was "vieworca-0.2.2.tar", last modified: Mon May 20 04:17:14 2024, max compression
```

## Comparing `vieworca-0.2.1.tar` & `vieworca-0.2.2.tar`

### file list

```diff
@@ -1,51 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:13:49.562180 vieworca-0.2.1/
--rwxr-xr-x   0 runner    (1001) docker     (127)    35129 2024-05-14 13:13:45.000000 vieworca-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-14 13:13:49.562180 vieworca-0.2.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2354 2024-05-14 13:13:45.000000 vieworca-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:13:49.558180 vieworca-0.2.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)       64 2024-05-14 13:13:45.000000 vieworca-0.2.1/bin/viewORCA
--rwxr-xr-x   0 runner    (1001) docker     (127)       89 2024-05-14 13:13:45.000000 vieworca-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:13:49.562180 vieworca-0.2.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3078 2024-05-14 13:13:45.000000 vieworca-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:13:49.558180 vieworca-0.2.1/viewORCA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:13:49.558180 vieworca-0.2.1/viewORCA/Programs/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4914 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/get_multiplicity.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6148 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewIRC.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:13:49.558180 vieworca-0.2.1/viewORCA/Programs/viewIRC_methods/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1982 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewIRC_methods/get_ORCA_IRC_images.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2050 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewIRC_methods/get_trajectory_filename.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6018 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewNEB.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:13:49.562180 vieworca-0.2.1/viewORCA/Programs/viewNEB_methods/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2057 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewNEB_methods/get_MEP_trajectory_filename.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2176 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewNEB_methods/get_ORCA_NEB_images.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6078 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewNEB_snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:13:49.562180 vieworca-0.2.1/viewORCA/Programs/viewNEB_snapshot_methods/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2141 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewNEB_snapshot_methods/get_interpolation_filename.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2955 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewNEB_snapshot_methods/plot_neb.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5394 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewNEB_snapshot_methods/read_orca_interpolation_file.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6056 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewOPT.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:13:49.562180 vieworca-0.2.1/viewORCA/Programs/viewOPT_methods/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2179 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewOPT_methods/get_ORCA_OPT_images.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1987 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewOPT_methods/get_trajectory_filename.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5006 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewSCAN.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:13:49.562180 vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4165 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3510 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_from_SCAN_folders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:13:49.562180 vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_method/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3652 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_method/assign_energies_to_SCAN_images.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1962 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_method/get_ORCA_SCAN_images.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:13:49.562180 vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/utility_methods/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4038 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/utility_methods/does_contain_SCAN_files.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2563 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/utility_methods/does_contain_SCAN_folders.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2029 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/utility_methods/get_trajectory_filename.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      617 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9059 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/check_prerequisites.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:13:49.562180 vieworca-0.2.1/viewORCA/cli/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4189 2024-05-14 13:13:45.000000 vieworca-0.2.1/viewORCA/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:13:49.562180 vieworca-0.2.1/viewORCA.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-14 13:13:49.000000 vieworca-0.2.1/viewORCA.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-14 13:13:49.000000 vieworca-0.2.1/viewORCA.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:13:49.000000 vieworca-0.2.1/viewORCA.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:13:49.000000 vieworca-0.2.1/viewORCA.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 13:13:49.000000 vieworca-0.2.1/viewORCA.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-14 13:13:49.000000 vieworca-0.2.1/viewORCA.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:17:14.759418 vieworca-0.2.2/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35129 2024-05-20 04:16:56.000000 vieworca-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-20 04:17:14.759418 vieworca-0.2.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2354 2024-05-20 04:16:56.000000 vieworca-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:17:14.751418 vieworca-0.2.2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       64 2024-05-20 04:16:56.000000 vieworca-0.2.2/bin/viewORCA
+-rwxr-xr-x   0 runner    (1001) docker     (127)       89 2024-05-20 04:16:56.000000 vieworca-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 04:17:14.759418 vieworca-0.2.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3078 2024-05-20 04:16:56.000000 vieworca-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:17:14.751418 vieworca-0.2.2/viewORCA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:17:14.755418 vieworca-0.2.2/viewORCA/Programs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3635 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/Programs/combine_systems_together.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4915 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/Programs/get_multiplicity.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5760 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/Programs/move_centre_of_mass.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6148 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/Programs/viewIRC.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:17:14.755418 vieworca-0.2.2/viewORCA/Programs/viewIRC_methods/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2178 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/Programs/viewIRC_methods/get_ORCA_IRC_images.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2050 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/Programs/viewIRC_methods/get_trajectory_filename.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6018 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/Programs/viewNEB.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9068 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/Programs/viewNEB_interpolate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:17:14.755418 vieworca-0.2.2/viewORCA/Programs/viewNEB_methods/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2057 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/Programs/viewNEB_methods/get_MEP_trajectory_filename.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2372 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/Programs/viewNEB_methods/get_ORCA_NEB_images.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6078 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/Programs/viewNEB_snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:17:14.755418 vieworca-0.2.2/viewORCA/Programs/viewNEB_snapshot_methods/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2141 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/Programs/viewNEB_snapshot_methods/get_interpolation_filename.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2955 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/Programs/viewNEB_snapshot_methods/plot_neb.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5394 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/Programs/viewNEB_snapshot_methods/read_orca_interpolation_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6056 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/Programs/viewOPT.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:17:14.755418 vieworca-0.2.2/viewORCA/Programs/viewOPT_methods/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2375 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/Programs/viewOPT_methods/get_ORCA_OPT_images.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1987 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/Programs/viewOPT_methods/get_trajectory_filename.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5006 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/Programs/viewSCAN.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:17:14.755418 vieworca-0.2.2/viewORCA/Programs/viewSCAN_methods/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4165 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3510 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_from_SCAN_folders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:17:14.759418 vieworca-0.2.2/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_method/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3848 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_method/assign_energies_to_SCAN_images.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1997 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_method/get_ORCA_SCAN_images.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:17:14.759418 vieworca-0.2.2/viewORCA/Programs/viewSCAN_methods/utility_methods/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4038 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/Programs/viewSCAN_methods/utility_methods/does_contain_SCAN_files.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2563 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/Programs/viewSCAN_methods/utility_methods/does_contain_SCAN_folders.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2029 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/Programs/viewSCAN_methods/utility_methods/get_trajectory_filename.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      617 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9059 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/check_prerequisites.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:17:14.759418 vieworca-0.2.2/viewORCA/cli/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4434 2024-05-20 04:16:56.000000 vieworca-0.2.2/viewORCA/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:17:14.759418 vieworca-0.2.2/viewORCA.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-20 04:17:14.000000 vieworca-0.2.2/viewORCA.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-20 04:17:14.000000 vieworca-0.2.2/viewORCA.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 04:17:14.000000 vieworca-0.2.2/viewORCA.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 04:17:14.000000 vieworca-0.2.2/viewORCA.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-20 04:17:14.000000 vieworca-0.2.2/viewORCA.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-20 04:17:14.000000 vieworca-0.2.2/viewORCA.egg-info/top_level.txt
```

### Comparing `vieworca-0.2.1/LICENSE` & `vieworca-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vieworca-0.2.1/PKG-INFO` & `vieworca-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: viewORCA
-Version: 0.2.1
+Version: 0.2.2
 Summary: This program is designed to allow the user to inspect calculations from ORCA. This is to be used along side the ORCA Reaction Mechanism Tutorial.
 Home-page: https://geoffreyweal.github.io/ORCA_Mechanism_Procedure/
-Download-URL: https://github.com/geoffreyweal/viewORCA/archive/v0.2.1.tar.gz
+Download-URL: https://github.com/geoffreyweal/viewORCA/archive/v0.2.2.tar.gz
 Author: Dr. Geoffrey R. Weal
 Author-email: geoffrey.weal@gmail.ac.nz
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Keywords: computational-chemistry,DFT,atomic-simulation-environment,ORCA
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `vieworca-0.2.1/README.md` & `vieworca-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `vieworca-0.2.1/setup.py` & `vieworca-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.2.1/viewORCA/Programs/get_multiplicity.py` & `vieworca-0.2.2/viewORCA/Programs/get_multiplicity.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 	# Third, make sure that charge is a digit
 	try:
 		charge = int(charge)
 	except Exception as exception:
 		raise Exception(f'Error: charge must be an integer. charge = {charge}')
 
 	# - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 
-	# Part II: Obtan the number of electrons in the molecule. 
+	# Part II: Obtain the number of electrons in the molecule. 
 
 	# Fourth, obtain the system from the filepath.
 	system = read(filepath)
 
 	# Fifth, get the atomic numbers of the atoms in the system. This is equivalent to the number of electrons in the neutrally charged system. 
 	total_number_of_electrons_in_neutral_system = int(sum(system.get_atomic_numbers()))
```

### Comparing `vieworca-0.2.1/viewORCA/Programs/viewIRC.py` & `vieworca-0.2.2/viewORCA/Programs/viewIRC.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.2.1/viewORCA/Programs/viewIRC_methods/get_ORCA_IRC_images.py` & `vieworca-0.2.2/viewORCA/Programs/viewIRC_methods/get_ORCA_IRC_images.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 get_ORCA_IRC_images.py, Geoffrey Weal, 23/4/24
 
 This method is designed to obtain the images and energies from the ORCA IRC file.
 """
+import warnings
 from ase    import Atoms, Atom
 from ase.io import read
 
 def get_ORCA_IRC_images(path_to_orca_IRC_trj_xyz):
 	"""
 	This method is designed to obtain the images and energies from the ORCA IRC file.
 
@@ -59,10 +60,10 @@
 
 				elif len(system) > number_of_atoms:
 					# 3.5: Something weird happened to get to this point.
 					raise Exception('Error: More atoms than should have.')
 
 	# Fourth: Check that all the entries in neb_images_energies are energies
 	if any([(energy is None) for energy in neb_images_energies]):
-		raise Exception('Error: Energy not given')
+		warnings.warn('Warning: Some of your molecules may not have an energy value assigned to it. This may be because your optimisation is still running or did not complete fully. Will continue running viewORCA, but be warned.')
 
 	return neb_images, neb_images_energies
```

### Comparing `vieworca-0.2.1/viewORCA/Programs/viewIRC_methods/get_trajectory_filename.py` & `vieworca-0.2.2/viewORCA/Programs/viewIRC_methods/get_trajectory_filename.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.2.1/viewORCA/Programs/viewNEB.py` & `vieworca-0.2.2/viewORCA/Programs/viewNEB.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.2.1/viewORCA/Programs/viewNEB_methods/get_MEP_trajectory_filename.py` & `vieworca-0.2.2/viewORCA/Programs/viewNEB_methods/get_MEP_trajectory_filename.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.2.1/viewORCA/Programs/viewNEB_methods/get_ORCA_NEB_images.py` & `vieworca-0.2.2/viewORCA/Programs/viewNEB_methods/get_ORCA_NEB_images.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 get_ORCA_NEB_images.py, Geoffrey Weal, 23/4/24
 
 This method is designed to obtain the images and energies from the ORCA NEB file.
 """
+import warnings
 from ase                         import Atoms, Atom
 from ase.io                      import read
 
 def get_ORCA_NEB_images(path_to_orca_NEB_trj_xyz):
 	"""
 	This method is designed to obtain the images and energies from the ORCA NEB file.
 
@@ -60,11 +61,11 @@
 
 				elif len(system) > number_of_atoms:
 					# 4.5: Something weird happened to get to this point.
 					raise Exception('Error: More atoms than should have.')
 
 	# Fifth, check that all the entries in neb_images_energies are energies
 	if any([(energy is None) for energy in neb_images_energies]):
-		raise Exception('Error: Energy not given')
+		warnings.warn('Warning: Some of your molecules may not have an energy value assigned to it. This may be because your optimisation is still running or did not complete fully. Will continue running viewORCA, but be warned.')
 
 	# Sixth, return neb_images and neb_images_energies
 	return neb_images, neb_images_energies
```

### Comparing `vieworca-0.2.1/viewORCA/Programs/viewNEB_snapshot.py` & `vieworca-0.2.2/viewORCA/Programs/viewNEB_snapshot.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.2.1/viewORCA/Programs/viewNEB_snapshot_methods/get_interpolation_filename.py` & `vieworca-0.2.2/viewORCA/Programs/viewNEB_snapshot_methods/get_interpolation_filename.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.2.1/viewORCA/Programs/viewNEB_snapshot_methods/plot_neb.py` & `vieworca-0.2.2/viewORCA/Programs/viewNEB_snapshot_methods/plot_neb.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.2.1/viewORCA/Programs/viewNEB_snapshot_methods/read_orca_interpolation_file.py` & `vieworca-0.2.2/viewORCA/Programs/viewNEB_snapshot_methods/read_orca_interpolation_file.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.2.1/viewORCA/Programs/viewOPT.py` & `vieworca-0.2.2/viewORCA/Programs/viewOPT.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.2.1/viewORCA/Programs/viewOPT_methods/get_ORCA_OPT_images.py` & `vieworca-0.2.2/viewORCA/Programs/viewOPT_methods/get_ORCA_OPT_images.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 get_ORCA_OPT_images.py, Geoffrey Weal, 23/4/24
 
 This method is designed to obtain the images and energies from the ORCA geometry optimisation file.
 """
+import warnings
 from ase    import Atoms, Atom
 from ase.io import read
 
 def get_ORCA_OPT_images(path_to_orca_OPT_trj_xyz):
 	"""
 	This method is designed to obtain the images and energies from the ORCA geometry optimisation file.
 
@@ -60,11 +61,11 @@
 
 				elif len(system) > number_of_atoms:
 					# 4.5: Something weird happened to get to this point.
 					raise Exception('Error: More atoms than should have.')
 
 	# Fifth, check that all the entries in opt_images_energies are energies
 	if any([(energy is None) for energy in opt_images_energies]):
-		raise Exception('Error: Energy not given')
+		warnings.warn('Warning: Some of your molecules may not have an energy value assigned to it. This may be because your optimisation is still running or did not complete fully. Will continue running viewORCA, but be warned.')
 
 	# Sixth, return opt_images and opt_images_energies
 	return opt_images, opt_images_energies
```

### Comparing `vieworca-0.2.1/viewORCA/Programs/viewOPT_methods/get_trajectory_filename.py` & `vieworca-0.2.2/viewORCA/Programs/viewOPT_methods/get_trajectory_filename.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.2.1/viewORCA/Programs/viewSCAN.py` & `vieworca-0.2.2/viewORCA/Programs/viewSCAN.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information.py` & `vieworca-0.2.2/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_from_SCAN_folders.py` & `vieworca-0.2.2/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_from_SCAN_folders.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_method/assign_energies_to_SCAN_images.py` & `vieworca-0.2.2/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_method/assign_energies_to_SCAN_images.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 assign_energies_to_SCAN_images.py, Geoffrey Weal, 18/4/24
 
 This method is designed to assign energies from the orca trajectory file to the xyz files for the SCAN images.
 """
+import warnings
 from ase import Atoms, Atom
 
 def assign_energies_to_SCAN_images(path_to_orca_trj_xyz, scan_images=[]):
 	"""
 	This method is designed to assign energies from the orca trajectory file to the xyz files for the SCAN images.
 
 	Parameters
@@ -62,15 +63,15 @@
 
 				elif len(system) > number_of_atoms:
 					# 4.5: Something weird happened to get to this point.
 					raise Exception('Error: More atoms than should have.')
 
 	# Fifth, check that all the entries in scan_images_energies are energies
 	if any([(energy is None) for energy in scan_images_energies]):
-		raise Exception('Error: Energy not given')
+		warnings.warn('Warning: Some of your molecules may not have an energy value assigned to it. This may be because your optimisation is still running or did not complete fully. Will continue running viewORCA, but be warned.')
 
 	# Sixth, return scan_images_energies
 	return scan_images_energies
 
 # ------------------------------------------------------------------------------
 
 def get_distance(position1, position2):
```

### Comparing `vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_method/get_ORCA_SCAN_images.py` & `vieworca-0.2.2/viewORCA/Programs/viewSCAN_methods/obtain_SCAN_information_method/get_ORCA_SCAN_images.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,13 +50,13 @@
 
 	# Third, sort SCAN_images by image number
 	SCAN_images.sort()
 
 	# Fourth, check that the component numbers in SCAN_images are consecutive
 	component_numbers = [component_number for (component_number, system) in SCAN_images]
 	if not (component_numbers == list(range(1,len(component_numbers)+1))):
-		raise Exception('Error')
+		raise Exception('Error: There may be a missing component?')
 
 	# Fifth, return SCAN_images, but just the ase.Atoms components
 	return [system for (component_number, system) in SCAN_images]
 
 # ------------------------------------------------------------------------------
```

### Comparing `vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/utility_methods/does_contain_SCAN_files.py` & `vieworca-0.2.2/viewORCA/Programs/viewSCAN_methods/utility_methods/does_contain_SCAN_files.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/utility_methods/does_contain_SCAN_folders.py` & `vieworca-0.2.2/viewORCA/Programs/viewSCAN_methods/utility_methods/does_contain_SCAN_folders.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.2.1/viewORCA/Programs/viewSCAN_methods/utility_methods/get_trajectory_filename.py` & `vieworca-0.2.2/viewORCA/Programs/viewSCAN_methods/utility_methods/get_trajectory_filename.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.2.1/viewORCA/__init__.py` & `vieworca-0.2.2/viewORCA/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # The information about the viewORCA program
 from viewORCA.check_prerequisites import check_prerequisites
 
 __name__    = 'viewORCA'
-__version__ = '0.2.1'
+__version__ = '0.2.2'
 __author__  = 'Dr. Geoffrey Weal'
 check_prerequisites(__version__)
 __author_email__ = 'geoffrey.weal@vuw.ac.nz'
 __license__ = 'GNU AFFERO GENERAL PUBLIC LICENSE'
 __url__ = 'https://github.com/geoffreyweal/viewORCA'
 __doc__ = 'See https://geoffreyweal.github.io/ORCA_Mechanism_Procedure for the documentation on this program'
```

### Comparing `vieworca-0.2.1/viewORCA/check_prerequisites.py` & `vieworca-0.2.2/viewORCA/check_prerequisites.py`

 * *Files identical despite different names*

### Comparing `vieworca-0.2.1/viewORCA/cli/main.py` & `vieworca-0.2.2/viewORCA/cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,20 +9,23 @@
     A subcommand may raise this.  The message will be forwarded to
     the error() method of the argument parser."""
 
 
 # Important: Following any change to command-line parameters, use
 # python3 -m ase.cli.completion to update autocompletion.
 commands = [
-    ('multi',    'viewORCA.Programs.get_multiplicity'),
-    ('opt',      'viewORCA.Programs.viewOPT'),
-    ('scan',     'viewORCA.Programs.viewSCAN'),
-    ('neb',      'viewORCA.Programs.viewNEB'),
-    ('neb_snap', 'viewORCA.Programs.viewNEB_snapshot'),
-    ('irc',      'viewORCA.Programs.viewIRC'),
+    ('opt',             'viewORCA.Programs.viewOPT'),
+    ('scan',            'viewORCA.Programs.viewSCAN'),
+    ('neb',             'viewORCA.Programs.viewNEB'),
+    ('neb_snap',        'viewORCA.Programs.viewNEB_snapshot'),
+    ('irc',             'viewORCA.Programs.viewIRC'),
+    ('multi',           'viewORCA.Programs.get_multiplicity'),
+    ('move_com',        'viewORCA.Programs.move_centre_of_mass'),
+    ('combine',         'viewORCA.Programs.combine_systems_together'),
+    ('neb_interpolate', 'viewORCA.Programs.viewNEB_interpolate'),
 ]
 
 def main(prog='viewORCA', description='Program for viewing jobs from ORCA', commands=commands, hook=None, args=None):
     """
     This method is designed to allow the user to view jobs performed by ORCA to study organic mechanisms. 
     """
     #check_prerequisites(__version__)
```

### Comparing `vieworca-0.2.1/viewORCA.egg-info/PKG-INFO` & `vieworca-0.2.2/viewORCA.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: viewORCA
-Version: 0.2.1
+Version: 0.2.2
 Summary: This program is designed to allow the user to inspect calculations from ORCA. This is to be used along side the ORCA Reaction Mechanism Tutorial.
 Home-page: https://geoffreyweal.github.io/ORCA_Mechanism_Procedure/
-Download-URL: https://github.com/geoffreyweal/viewORCA/archive/v0.2.1.tar.gz
+Download-URL: https://github.com/geoffreyweal/viewORCA/archive/v0.2.2.tar.gz
 Author: Dr. Geoffrey R. Weal
 Author-email: geoffrey.weal@gmail.ac.nz
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Keywords: computational-chemistry,DFT,atomic-simulation-environment,ORCA
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `vieworca-0.2.1/viewORCA.egg-info/SOURCES.txt` & `vieworca-0.2.2/viewORCA.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 viewORCA/check_prerequisites.py
 viewORCA.egg-info/PKG-INFO
 viewORCA.egg-info/SOURCES.txt
 viewORCA.egg-info/dependency_links.txt
 viewORCA.egg-info/not-zip-safe
 viewORCA.egg-info/requires.txt
 viewORCA.egg-info/top_level.txt
+viewORCA/Programs/combine_systems_together.py
 viewORCA/Programs/get_multiplicity.py
+viewORCA/Programs/move_centre_of_mass.py
 viewORCA/Programs/viewIRC.py
 viewORCA/Programs/viewNEB.py
+viewORCA/Programs/viewNEB_interpolate.py
 viewORCA/Programs/viewNEB_snapshot.py
 viewORCA/Programs/viewOPT.py
 viewORCA/Programs/viewSCAN.py
 viewORCA/Programs/viewIRC_methods/get_ORCA_IRC_images.py
 viewORCA/Programs/viewIRC_methods/get_trajectory_filename.py
 viewORCA/Programs/viewNEB_methods/get_MEP_trajectory_filename.py
 viewORCA/Programs/viewNEB_methods/get_ORCA_NEB_images.py
```

