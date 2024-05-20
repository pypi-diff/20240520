# Comparing `tmp/calc_ultra-1.3.6.tar.gz` & `tmp/calc_ultra-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calc_ultra-1.3.6.tar", last modified: Wed May 15 12:23:00 2024, max compression
+gzip compressed data, was "calc_ultra-1.3.7.tar", last modified: Mon May 20 14:17:02 2024, max compression
```

## Comparing `calc_ultra-1.3.6.tar` & `calc_ultra-1.3.7.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-05-15 12:23:00.161177 calc_ultra-1.3.6/
--rw-r--r--   0 Huatao     (502) staff       (20)     1068 2023-12-31 12:50:35.000000 calc_ultra-1.3.6/LICENSE
--rw-r--r--   0 Huatao     (502) staff       (20)       21 2023-12-09 18:58:14.000000 calc_ultra-1.3.6/MANIFEST.in
--rw-r--r--   0 Huatao     (502) staff       (20)     4203 2024-05-15 12:23:00.160963 calc_ultra-1.3.6/PKG-INFO
--rw-r--r--   0 Huatao     (502) staff       (20)     3434 2024-05-14 14:05:23.000000 calc_ultra-1.3.6/README.md
--rw-r--r--   0 Huatao     (502) staff       (20)      892 2024-05-14 13:18:36.000000 calc_ultra-1.3.6/pyproject.toml
--rw-r--r--   0 Huatao     (502) staff       (20)       38 2024-05-15 12:23:00.161224 calc_ultra-1.3.6/setup.cfg
-drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-05-15 12:23:00.157391 calc_ultra-1.3.6/src/
--rw-r--r--   0 Huatao     (502) staff       (20)     6148 2024-05-15 12:22:16.000000 calc_ultra-1.3.6/src/.DS_Store
-drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-05-15 12:23:00.158212 calc_ultra-1.3.6/src/calc_ultra/
--rw-r--r--   0 Huatao     (502) staff       (20)     6148 2024-05-15 11:24:35.000000 calc_ultra-1.3.6/src/calc_ultra/.DS_Store
--rw-r--r--   0 Huatao     (502) staff       (20)      128 2024-02-05 08:04:02.000000 calc_ultra-1.3.6/src/calc_ultra/__init__.py
--rw-r--r--   0 Huatao     (502) staff       (20)    46616 2024-05-15 11:27:19.000000 calc_ultra-1.3.6/src/calc_ultra/main.py
-drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-05-15 12:23:00.160464 calc_ultra-1.3.6/src/calc_ultra/texts/
--rw-r--r--   0 Huatao     (502) staff       (20)        0 2023-12-09 18:58:14.000000 calc_ultra-1.3.6/src/calc_ultra/texts/__init__.py
--rw-r--r--   0 Huatao     (502) staff       (20)      546 2024-03-19 08:27:24.000000 calc_ultra-1.3.6/src/calc_ultra/texts/algcalc.txt
--rw-r--r--   0 Huatao     (502) staff       (20)      740 2024-03-06 07:59:13.000000 calc_ultra-1.3.6/src/calc_ultra/texts/derivacalc.txt
--rw-r--r--   0 Huatao     (502) staff       (20)      761 2024-04-14 10:36:05.000000 calc_ultra-1.3.6/src/calc_ultra/texts/intecalc.txt
--rw-r--r--   0 Huatao     (502) staff       (20)      531 2024-03-06 07:59:34.000000 calc_ultra-1.3.6/src/calc_ultra/texts/limcalc.txt
--rw-r--r--   0 Huatao     (502) staff       (20)      706 2024-05-01 04:38:23.000000 calc_ultra-1.3.6/src/calc_ultra/texts/main_screen.txt
--rw-r--r--   0 Huatao     (502) staff       (20)      232 2024-04-14 10:37:09.000000 calc_ultra-1.3.6/src/calc_ultra/texts/settings.txt
-drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-05-15 12:23:00.160718 calc_ultra-1.3.6/src/calc_ultra.egg-info/
--rw-r--r--   0 Huatao     (502) staff       (20)     4203 2024-05-15 12:23:00.000000 calc_ultra-1.3.6/src/calc_ultra.egg-info/PKG-INFO
--rw-r--r--   0 Huatao     (502) staff       (20)      562 2024-05-15 12:23:00.000000 calc_ultra-1.3.6/src/calc_ultra.egg-info/SOURCES.txt
--rw-r--r--   0 Huatao     (502) staff       (20)        1 2024-05-15 12:23:00.000000 calc_ultra-1.3.6/src/calc_ultra.egg-info/dependency_links.txt
--rw-r--r--   0 Huatao     (502) staff       (20)       94 2024-05-15 12:23:00.000000 calc_ultra-1.3.6/src/calc_ultra.egg-info/requires.txt
--rw-r--r--   0 Huatao     (502) staff       (20)       11 2024-05-15 12:23:00.000000 calc_ultra-1.3.6/src/calc_ultra.egg-info/top_level.txt
+drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-05-20 14:17:02.063856 calc_ultra-1.3.7/
+-rw-r--r--   0 Huatao     (502) staff       (20)     1068 2023-12-31 12:50:35.000000 calc_ultra-1.3.7/LICENSE
+-rw-r--r--   0 Huatao     (502) staff       (20)       21 2023-12-09 18:58:14.000000 calc_ultra-1.3.7/MANIFEST.in
+-rw-r--r--   0 Huatao     (502) staff       (20)     4568 2024-05-20 14:17:02.063654 calc_ultra-1.3.7/PKG-INFO
+-rw-r--r--   0 Huatao     (502) staff       (20)     3799 2024-05-20 14:11:12.000000 calc_ultra-1.3.7/README.md
+-rw-r--r--   0 Huatao     (502) staff       (20)      892 2024-05-20 14:15:40.000000 calc_ultra-1.3.7/pyproject.toml
+-rw-r--r--   0 Huatao     (502) staff       (20)       38 2024-05-20 14:17:02.063905 calc_ultra-1.3.7/setup.cfg
+drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-05-20 14:17:02.061020 calc_ultra-1.3.7/src/
+-rw-r--r--   0 Huatao     (502) staff       (20)     6148 2024-05-20 14:15:15.000000 calc_ultra-1.3.7/src/.DS_Store
+drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-05-20 14:17:02.061713 calc_ultra-1.3.7/src/calc_ultra/
+-rw-r--r--   0 Huatao     (502) staff       (20)     6148 2024-05-20 12:07:01.000000 calc_ultra-1.3.7/src/calc_ultra/.DS_Store
+-rw-r--r--   0 Huatao     (502) staff       (20)       97 2024-05-20 14:05:35.000000 calc_ultra-1.3.7/src/calc_ultra/__init__.py
+-rw-r--r--   0 Huatao     (502) staff       (20)      297 2024-05-18 10:40:15.000000 calc_ultra-1.3.7/src/calc_ultra/example.py
+-rw-r--r--   0 Huatao     (502) staff       (20)    49474 2024-05-20 14:06:23.000000 calc_ultra-1.3.7/src/calc_ultra/main.py
+drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-05-20 14:17:02.063218 calc_ultra-1.3.7/src/calc_ultra/texts/
+-rw-r--r--   0 Huatao     (502) staff       (20)        0 2023-12-09 18:58:14.000000 calc_ultra-1.3.7/src/calc_ultra/texts/__init__.py
+-rw-r--r--   0 Huatao     (502) staff       (20)     2124 2024-05-20 10:20:17.000000 calc_ultra-1.3.7/src/calc_ultra/texts/algcalc.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)     2903 2024-05-19 07:18:42.000000 calc_ultra-1.3.7/src/calc_ultra/texts/derivacalc.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)     2375 2024-05-19 07:13:56.000000 calc_ultra-1.3.7/src/calc_ultra/texts/intecalc.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)     2050 2024-05-19 07:17:00.000000 calc_ultra-1.3.7/src/calc_ultra/texts/limcalc.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)     2774 2024-05-19 07:18:30.000000 calc_ultra-1.3.7/src/calc_ultra/texts/main_screen.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)      235 2024-05-19 07:14:41.000000 calc_ultra-1.3.7/src/calc_ultra/texts/settings.txt
+drwxr-xr-x   0 Huatao     (502) staff       (20)        0 2024-05-20 14:17:02.063416 calc_ultra-1.3.7/src/calc_ultra.egg-info/
+-rw-r--r--   0 Huatao     (502) staff       (20)     4568 2024-05-20 14:17:02.000000 calc_ultra-1.3.7/src/calc_ultra.egg-info/PKG-INFO
+-rw-r--r--   0 Huatao     (502) staff       (20)      588 2024-05-20 14:17:02.000000 calc_ultra-1.3.7/src/calc_ultra.egg-info/SOURCES.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)        1 2024-05-20 14:17:02.000000 calc_ultra-1.3.7/src/calc_ultra.egg-info/dependency_links.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)       94 2024-05-20 14:17:02.000000 calc_ultra-1.3.7/src/calc_ultra.egg-info/requires.txt
+-rw-r--r--   0 Huatao     (502) staff       (20)       11 2024-05-20 14:17:02.000000 calc_ultra-1.3.7/src/calc_ultra.egg-info/top_level.txt
```

### Comparing `calc_ultra-1.3.6/LICENSE` & `calc_ultra-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `calc_ultra-1.3.6/PKG-INFO` & `calc_ultra-1.3.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calc_ultra
-Version: 1.3.6
+Version: 1.3.7
 Summary: A calculus calculator with a menu-based interface.
 Author-email: Huatao <huatao.xue@outlook.com>
 Maintainer-email: Huatao <huatao.xue@outlook.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/sudoer-Huatao/calc_ultra
 Project-URL: Issues, https://github.com/sudoer-Huatao/calc_ultra/issues
 Keywords: calculus,calculator
@@ -16,50 +16,55 @@
 Requires-Dist: sympy>=1.12
 Requires-Dist: numpy>=1.26.2
 Requires-Dist: matplotlib>=3.8.4
 Requires-Dist: rich>=13.7.1
 Requires-Dist: scipy>=1.13.0
 Requires-Dist: prompt_toolkit>=3.0.43
 
-# calc-ultra
+# Calc-Ultra
 
-[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) [![Version](https://img.shields.io/badge/Version-1.3.6-blue.svg)](https://github.com/sudoer-Huatao/calc_ultra)
+[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) [![Version](https://img.shields.io/badge/Version-1.3.7-blue.svg)](https://pypi.org/project/calc-ultra/)
 
 > **Calculus made easy**
 
 (Turn on dark mode for a better aesthetic) 📲
 
-Calc-Ultra is a multi-functional calculator that uses command line interfaces. Little Python background knowledge is needed to use the calculator!
+Calc-Ultra (styled as CALC ULTRA) is a multi-functional calculator that uses a command-line/menu-based interface. Little Python background knowledge is needed to use this calculator!
 
 Supports:
 
+- Simple calculations (complex numbers supported!)
 - Derivatives
 - Partials
 - Implicit differentiation
 - Limits
 - Antiderivatives
 - Definite integrals
 - Improper integrals
 - Double integrals
 - Solving (sets) of equation(s)
 - Vector/matrix operations
 - **A perfect interface to do calculations!**  
 
 ## Chinese version
 
-Want to check out the Chinese version? Visit <https://github.com/sudoer-Huatao/calc_ultra-chinese>! 🇨🇳
+Want to check out the Chinese version? Visit the Chinese version [here](https://github.com/sudoer-Huatao/calc_ultra-chinese)! 🇨🇳
 
 ## Installation and Running
 
 > Run the calculus calculator with a single line of code
 
-Use the following command to download Calc-Ultra (pip should be installed):
+Use the following command to install Calc-Ultra:
 
 `pip3 install calc-ultra`
 
+or
+
+`python3 -m pip install calc-ultra` if you have lower versions of pip.
+
 Due to Python import identifiers restrictions, please import Calc-Ultra as "calc_ultra" and not "calc-ultra".
 
 Import Calc-Ultra like so to use:
 
 `from calc_ultra import main`
 
 Please make sure you have the latest version installed. To update calc-ultra, run the following command:
@@ -73,47 +78,50 @@
 - `sympy`
 - `numpy`
 - `matplotlib`
 - `scipy`
 - `rich`
 - `prompt-toolkit`
 
-If you do not have them installed, no need to worry! These modules should be installed automatically if you don't have them. Other required modules are built into most Python IDEs as well.
+If you do not have them installed, no need to worry! These modules should be installed automatically if you don't have them.
 
 ## Acknowledgements
 
 > Without them, this would be impossible
 
 A big thank-you to all GitHub users who gave feedback and/or starred this repository. ⭐️ Your encouragement is our motivation.
 The following contributors deserve a SPECIAL THANK-YOU 👍❤️:
 
-- @Haobot for troubleshooting and feedback!
-- Fanbo for feedback and ideas for improvement!
+- [@Haobot](https://github.com/Haobot) for troubleshooting and feedback!
+- [@FanboFB](https://github.com/FanboFB) for feedback and ideas for improvement!
 
 This program was made using `sympy` for calculation and `numpy`, `scipy`, and `matplotlib` for graphing.
 
 ## Gallery (Demos)
 
+Simple calculation screen demo:
+![simple_calculation_screen_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/9df15b7e-e239-4f99-8966-db684ff36b68 "simple_calculation_demo")
+
 DerivaCalc derivative with graph demo:
-![derivacalc_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/3d99a51d-2e46-414c-8929-fa16016a856a "derivacalc_demo")
+![derivacalc_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/d0491f48-1a4f-4538-be7e-0bf793815eff "derivacalc_demo")
 
 InteCalc antiderivative with graph demo:
-![intecalc_demo_1](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/f61d44ae-cebf-4972-b63f-7f08ee6655b5 "intecalc_demo_1")
+![intecalc_demo_1](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/2375f351-46ae-4bfd-ad25-af599a26bbce "intecalc_demo_1")
 
 InteCalc definite integral with graph demo:
-![intecalc_demo_2](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/b8294186-92f5-4df3-a000-d63f6fff93b0 "intecalc_demo_2")
+![intecalc_demo_2](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/0af601a5-3d4c-4db5-a2aa-dff4b6bdd4b5 "intecalc_demo_2")
 
-LimCalc limit demo:
-![limcalc_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/12db6a7b-a836-43ce-8cef-7bcf707051f7 "limcalc_demo")
+LimCalc limit and one-sided limit demo:
+![limcalc_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/bdecb164-b28c-4b4c-9f0a-cf9c44dfad90 "limcalc_demo")
 
 AlgCalc equation solver demo:
-![algcalc_demo_1](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/e4cfa016-52bf-43b5-a839-af9f42546468 "algcalc_demo_1")
+![algcalc_demo_1](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/74beffa8-7c82-4499-a114-8278e9929cdb "algcalc_demo_1")
 
 AlgCalc vector operation demo:
-![algcalc_demo_2](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/7f043cb2-6b0a-4460-ab35-30f09632b1c3 "algcalc_demo_2")
+![algcalc_demo_2](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/48b9624f-ab32-4f4c-99f7-1860dfd487a0 "algcalc_demo_2")
 
 AlgCalc matrix operation demo:
-![algcalc_demo_3](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/a9a5d56e-424a-4ef8-beb9-a9b64ce1a3f5 "algcalc_demo_3")
+![algcalc_demo_3](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/dee6cc8e-765d-4c41-b322-03f3ee501aac "algcalc_demo_3")
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

### Comparing `calc_ultra-1.3.6/README.md` & `calc_ultra-1.3.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,48 @@
-# calc-ultra
+# Calc-Ultra
 
-[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) [![Version](https://img.shields.io/badge/Version-1.3.6-blue.svg)](https://github.com/sudoer-Huatao/calc_ultra)
+[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) [![Version](https://img.shields.io/badge/Version-1.3.7-blue.svg)](https://pypi.org/project/calc-ultra/)
 
 > **Calculus made easy**
 
 (Turn on dark mode for a better aesthetic) 📲
 
-Calc-Ultra is a multi-functional calculator that uses command line interfaces. Little Python background knowledge is needed to use the calculator!
+Calc-Ultra (styled as CALC ULTRA) is a multi-functional calculator that uses a command-line/menu-based interface. Little Python background knowledge is needed to use this calculator!
 
 Supports:
 
+- Simple calculations (complex numbers supported!)
 - Derivatives
 - Partials
 - Implicit differentiation
 - Limits
 - Antiderivatives
 - Definite integrals
 - Improper integrals
 - Double integrals
 - Solving (sets) of equation(s)
 - Vector/matrix operations
 - **A perfect interface to do calculations!**  
 
 ## Chinese version
 
-Want to check out the Chinese version? Visit <https://github.com/sudoer-Huatao/calc_ultra-chinese>! 🇨🇳
+Want to check out the Chinese version? Visit the Chinese version [here](https://github.com/sudoer-Huatao/calc_ultra-chinese)! 🇨🇳
 
 ## Installation and Running
 
 > Run the calculus calculator with a single line of code
 
-Use the following command to download Calc-Ultra (pip should be installed):
+Use the following command to install Calc-Ultra:
 
 `pip3 install calc-ultra`
 
+or
+
+`python3 -m pip install calc-ultra` if you have lower versions of pip.
+
 Due to Python import identifiers restrictions, please import Calc-Ultra as "calc_ultra" and not "calc-ultra".
 
 Import Calc-Ultra like so to use:
 
 `from calc_ultra import main`
 
 Please make sure you have the latest version installed. To update calc-ultra, run the following command:
@@ -51,47 +56,50 @@
 - `sympy`
 - `numpy`
 - `matplotlib`
 - `scipy`
 - `rich`
 - `prompt-toolkit`
 
-If you do not have them installed, no need to worry! These modules should be installed automatically if you don't have them. Other required modules are built into most Python IDEs as well.
+If you do not have them installed, no need to worry! These modules should be installed automatically if you don't have them.
 
 ## Acknowledgements
 
 > Without them, this would be impossible
 
 A big thank-you to all GitHub users who gave feedback and/or starred this repository. ⭐️ Your encouragement is our motivation.
 The following contributors deserve a SPECIAL THANK-YOU 👍❤️:
 
-- @Haobot for troubleshooting and feedback!
-- Fanbo for feedback and ideas for improvement!
+- [@Haobot](https://github.com/Haobot) for troubleshooting and feedback!
+- [@FanboFB](https://github.com/FanboFB) for feedback and ideas for improvement!
 
 This program was made using `sympy` for calculation and `numpy`, `scipy`, and `matplotlib` for graphing.
 
 ## Gallery (Demos)
 
+Simple calculation screen demo:
+![simple_calculation_screen_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/9df15b7e-e239-4f99-8966-db684ff36b68 "simple_calculation_demo")
+
 DerivaCalc derivative with graph demo:
-![derivacalc_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/3d99a51d-2e46-414c-8929-fa16016a856a "derivacalc_demo")
+![derivacalc_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/d0491f48-1a4f-4538-be7e-0bf793815eff "derivacalc_demo")
 
 InteCalc antiderivative with graph demo:
-![intecalc_demo_1](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/f61d44ae-cebf-4972-b63f-7f08ee6655b5 "intecalc_demo_1")
+![intecalc_demo_1](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/2375f351-46ae-4bfd-ad25-af599a26bbce "intecalc_demo_1")
 
 InteCalc definite integral with graph demo:
-![intecalc_demo_2](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/b8294186-92f5-4df3-a000-d63f6fff93b0 "intecalc_demo_2")
+![intecalc_demo_2](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/0af601a5-3d4c-4db5-a2aa-dff4b6bdd4b5 "intecalc_demo_2")
 
-LimCalc limit demo:
-![limcalc_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/12db6a7b-a836-43ce-8cef-7bcf707051f7 "limcalc_demo")
+LimCalc limit and one-sided limit demo:
+![limcalc_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/bdecb164-b28c-4b4c-9f0a-cf9c44dfad90 "limcalc_demo")
 
 AlgCalc equation solver demo:
-![algcalc_demo_1](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/e4cfa016-52bf-43b5-a839-af9f42546468 "algcalc_demo_1")
+![algcalc_demo_1](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/74beffa8-7c82-4499-a114-8278e9929cdb "algcalc_demo_1")
 
 AlgCalc vector operation demo:
-![algcalc_demo_2](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/7f043cb2-6b0a-4460-ab35-30f09632b1c3 "algcalc_demo_2")
+![algcalc_demo_2](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/48b9624f-ab32-4f4c-99f7-1860dfd487a0 "algcalc_demo_2")
 
 AlgCalc matrix operation demo:
-![algcalc_demo_3](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/a9a5d56e-424a-4ef8-beb9-a9b64ce1a3f5 "algcalc_demo_3")
+![algcalc_demo_3](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/dee6cc8e-765d-4c41-b322-03f3ee501aac "algcalc_demo_3")
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

### Comparing `calc_ultra-1.3.6/pyproject.toml` & `calc_ultra-1.3.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [wheel]
 supported_platforms = ["macos"]
 
 [project]
 name = "calc_ultra"
-version = "1.3.6"
+version = "1.3.7"
 dependencies = [
   "sympy >= 1.12",
   "numpy >= 1.26.2",
   "matplotlib >= 3.8.4",
   "rich >= 13.7.1",
   "scipy >= 1.13.0",
   "prompt_toolkit >= 3.0.43"
```

### Comparing `calc_ultra-1.3.6/src/.DS_Store` & `calc_ultra-1.3.7/src/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 00000230: 6270 6c69 7374 3030 d601 0203 0405 0607  bplist00........
 00000240: 0807 080b 085d 5368 6f77 5374 6174 7573  .....]ShowStatus
 00000250: 4261 725b 5368 6f77 546f 6f6c 6261 725b  Bar[ShowToolbar[
 00000260: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
 00000270: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
 00000280: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
 00000290: 5368 6f77 5369 6465 6261 7208 0908 095f  ShowSidebar...._
-000002a0: 1018 7b7b 3433 302c 2034 3434 7d2c 207b  ..{{430, 444}, {
+000002a0: 1018 7b7b 3436 322c 2034 3233 7d2c 207b  ..{{462, 423}, {
 000002b0: 3835 352c 2034 3339 7d7d 0908 1523 2f3b  855, 439}}...#/;
 000002c0: 525f 6b6c 6d6e 6f8a 0000 0000 0000 0101  R_klmno.........
 000002d0: 0000 0000 0000 000d 0000 0000 0000 0000  ................
 000002e0: 0000 0000 0000 008b 0000 000a 0063 0061  .............c.a
 000002f0: 006c 0063 005f 0075 006c 0074 0072 0061  .l.c._.u.l.t.r.a
 00000300: 7653 726e 6c6f 6e67 0000 0001 0000 0000  vSrnlong........
 00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `calc_ultra-1.3.6/src/calc_ultra/.DS_Store` & `calc_ultra-1.3.7/src/calc_ultra/.DS_Store`

 * *Files 23% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 00000120: 6f62 0000 00b8 6270 6c69 7374 3030 d601  ob....bplist00..
 00000130: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
 00000140: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
 00000150: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
 00000160: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
 00000170: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
 00000180: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00000190: 7208 0908 095f 1018 7b7b 3436 382c 2032  r...._..{{468, 2
-000001a0: 3734 7d2c 207b 3835 352c 2034 3339 7d7d  74}, {855, 439}}
+00000190: 7208 0908 095f 1018 7b7b 3436 322c 2034  r...._..{{462, 4
+000001a0: 3233 7d2c 207b 3835 352c 2034 3339 7d7d  23}, {855, 439}}
 000001b0: 0908 1523 2f3b 525f 6b6c 6d6e 6f8a 0000  ...#/;R_klmno...
 000001c0: 0000 0000 0101 0000 0000 0000 000d 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 008b 0000  ................
 000001e0: 0005 0074 0065 0078 0074 0073 7653 726e  ...t.e.x.t.svSrn
 000001f0: 6c6f 6e67 0000 0001 0000 0000 0000 0000  long............
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `calc_ultra-1.3.6/src/calc_ultra/main.py` & `calc_ultra-1.3.7/src/calc_ultra/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     sinh,
     cosh,
     tanh,
     arcsinh,
     arccosh,
     arctanh,
     array,
-    array_equal,
     cross,
 )
 from numpy.linalg import norm, det
 from sympy import (
     diff,
     idiff,
     Integral,
@@ -44,73 +43,82 @@
     simplify,
     symbols,
     gamma,
     lowergamma,
     uppergamma,
     zeta,
 )
+from sympy.core.numbers import pi, E, I, oo
+import scipy.special as ss
 from scipy.special import polygamma, gammainc, gammaincc, erf, erfc
 from rich.progress import (
     Progress,
     SpinnerColumn,
     BarColumn,
     MofNCompleteColumn,
     TimeElapsedColumn,
     TextColumn,
 )
-from sympy.core.numbers import pi, E, oo, I
+import matplotlib.pyplot as plt
+from logging import warning, error
 from math import floor, ceil
-import scipy.special as ss
+from os.path import dirname, abspath, exists
 from prompt_toolkit import prompt
 from prompt_toolkit.key_binding import KeyBindings
-import matplotlib.pyplot as plt
-import datetime, logging, random, readline, os, time, warnings
+from random import randint
+from readline import parse_and_bind
+from time import sleep
+from warnings import filterwarnings
+import datetime
 
 
 ###########
 # Presets #
 ###########
 
-warnings.filterwarnings("ignore")
+filterwarnings("ignore")
 
-readline.parse_and_bind("tab: complete")
+parse_and_bind("tab: complete")
 
 x, y, z, t, m = symbols("x, y, z, t, m")
 
 history = [""]  # Stores calculation history
 
-input = prompt
-
 key_bindings = KeyBindings()
 
 idx = 1
 
+save_path = dirname(abspath(__file__)) + "/fig.pdf"
+
 expr_replace = [
+    ("E", "E1"),
+    ("e", "E1"),
+    # The extra 1 at the end is to recognize whether the "e"
+    # is part of an expression or a constant on it's own.
+    ("i", "I"),
     ("^", "**"),
     ("E1**", "exp"),
     ("E1xp", "exp"),
     ("E1r", "er"),
     ("sIn", "sin"),
     ("pI", "pi"),
     ("Ia", "ia"),
     ("ln", "log"),
     ("arc", "a"),
-    ("abs", "Abs"),
     ("pi", "3.141592653589793"),
     ("E1", "2.718281828459045"),
 ]
 
 graph_replace = [
     ("asin", "arcsin"),
     ("acos", "arccos"),
     ("atan", "arctan"),
     ("csc", "1/sin"),
     ("sec", "1/cos"),
     ("cot", "1/tan"),
-    ("Abs", "fabs"),
     ("gamma", "ss.gamma"),
     ("polyss.gamma", "polygamma"),
     ("lowergamma", "gammainc"),
     ("uppergamma", "gammaincc"),
 ]
 
 
@@ -156,132 +164,134 @@
             buffer.text = history[idx]
             buffer.cursor_position = len(buffer.text)
 
     except:
         pass
 
 
+# Control + C to clear history
+
+
 @key_bindings.add("c-c")
 def _(event):
+    global history
     history = [""]
 
 
 #####################
 # Calculation funcs #
 #####################
 
 
 def simp():
     print(
-        '\n[bold bright_green](Current Screen: Simple Calculation Screen)[/bold bright_green]\n("q" to quit)\nEnter any expression:\n'
+        '\n[bold bright_green](Current Screen: Simple Calculation Screen)[/bold bright_green]\n\n("q" to quit)\n\nEnter any expression:\n'
     )
 
     while True:
-        expr = input(key_bindings=key_bindings)
+        expr = prompt(key_bindings=key_bindings)
 
         try:
             if expr != "q":
                 # Easy to exit unlike VIM ;)
                 expr = expr.replace(" ", "")
 
                 if "?=" in expr:
-                    left = replace_graph(
-                        str(simplify(replace_expr(expr[: expr.find("?=")])).evalf())
-                    ).lstrip("0*x+")
-
-                    right = replace_graph(
-                        str(simplify(replace_expr(expr[expr.find("?=") + 2 :])).evalf())
-                    ).lstrip("0*x+")
-
-                    try:
-                        if "I" in left:
-                            left = left.replace(" ", "")
-                            imag = eval((left[left.find("+") + 1 :]).rstrip("*I"))
-
-                            if imag < 0.000001 and imag > -0.000001:
-                                left = left[: left.find("+")]
+                    left = replace_expr(expr[: expr.find("?=")])
+                    right = replace_expr(expr[expr.find("?=") + 2 :])
 
-                        elif left < 0.000001 and left > -0.000001:
-                            left = 0
+                    if "x" in left or "x" in right:
+                        equals = "True."
 
-                        if "I" in right:
-                            right = right.replace(" ", "")
-                            imag = eval((right[right.find("+") + 1 :]).rstrip("*I"))
-
-                            if imag < 0.000001 and imag > -0.000001:
-                                right = right[: right.find("+")]
-
-                        elif right < 0.000001 and right > -0.000001:
-                            right = 0
-
-                    except:
-                        pass
-
-                    if str(left).endswith("0") and left != 0:
-                        left = str(left).rstrip("0")
-
-                    if str(right).endswith("0") and right != 0:
-                        right = str(right).rstrip("0")
-
-                    if "x" in left and "x" in right:
-                        equals = "True"
+                        left = str(left)
+                        right = str(right)
 
                         for i in range(-100, 100):
-                            left_result = str(eval(left.replace("x", str(i))))
-                            right_result = str(eval(right.replace("x", str(i))))
-
-                            if left_result != right_result:
+                            left_result = simplify(
+                                left.replace("x", str(i)).replace("e" + str(i), "ex")
+                            ).evalf()
+                            right_result = simplify(right.replace("x", str(i))).evalf()
+
+                            if (
+                                "I" not in str(left_result)
+                                and left_result < 0.000001
+                                and left_result > -0.000001
+                            ):
+                                left_result = 0
+
+                            if (
+                                "I" not in str(right_result)
+                                and right_result < 0.000001
+                                and right_result > -0.000001
+                            ):
+                                right_result = 0
+
+                            if str(left_result).rstrip("*I") != str(
+                                right_result
+                            ).rstrip("*I"):
                                 equals = "False."
+                                print(left_result, right_result)
                                 break
 
-                        print("\n" + equals + "\n")
+                        print(f"\n{equals}\n")
 
                     else:
-                        print(left)
-                        print(right)
+                        left = replace_calc(left)
+                        right = replace_calc(right)
+
+                        if str(left).endswith("0") and left != 0:
+                            left = str(left).rstrip("0")
+
+                        if str(right).endswith("0") and right != 0:
+                            right = str(right).rstrip("0")
+
                         if left == right:
                             print("\nTrue.\n")
+
                         else:
-                            print("\nFalse.\n")
+                            print(
+                                "\nFalse.\n\nLeft side: "
+                                + left
+                                + ". Right side: "
+                                + right
+                                + ".\n"
+                            )
 
                 else:
-                    result = simplify(replace_expr(expr)).evalf()
+                    result = replace_expr(expr)
 
-                    try:
-                        if "I" in str(result):
-                            result = str(result).replace(" ", "")
-                            imag = eval((result[result.find("+") + 1 :]).rstrip("*I"))
+                    result = replace_calc(result)
 
-                            if imag < 0.000001 and imag > -0.000001:
-                                result = result[: result.find("+")]
+                    if result == None:
+                        error("Could not complete calculation.")
 
-                        elif result < 0.000001 and result > -0.000001:
-                            result = 0
-
-                    except:
-                        pass
+                    else:
+                        if str(result).endswith("0") and result != 0:
+                            result = eval(str(result).rstrip("0"))
 
-                    if str(result).endswith("0") and result != 0:
-                        result = eval(str(result).rstrip("0"))
+                        if history[len(history) - 1] != str(result) and result != None:
+                            history.append(str(result))
 
-                    history.append(str(result))
-                    print("\n[bright_yellow]Result: [/bright_yellow]", end="")
-                    pprint(result)
-                    print()
+                        print("\n[bright_yellow]Result: [/bright_yellow]", end="")
+                        pprint(result)
+                        print()
 
             else:
                 break
 
         except:
             print()
-            logging.error(f'Could not parse: "{expr}".\n')
+            error(f'Could not parse: "{expr}".\n')
 
 
 def derive(function: str, order: str):
-    """Calculates the derivative of a function.
+    r"""Calculates the derivative of a function.
+
+    Explanation
+    ===========
 
     Takes a function and an order of differentiation and
     returns the derivative of the function with the given order.
     Graph option available.
     """
 
     calc = replace_expr(function)
@@ -294,15 +304,17 @@
     print(
         f"\nDerivative of [bright_magenta]{replace_graph(function)}[/bright_magenta] with order {order} is:\n"
     )
     print_expr(df)
 
     df = replace_expr(str(df))
     check_simp(df)
-    history.append(df)
+
+    if history[len(history) - 1] != df:
+        history.append(df)
 
     df = replace_graph(df)
 
     print("\n[bright_yellow]Show graph of area? (y/n)[/bright_yellow]")
     show = input("(Exit the graph window when you are finished to continue) ")
 
     if show == "y":
@@ -315,15 +327,15 @@
                 TimeElapsedColumn(),
                 transient=False,
             ) as progress:
                 task = progress.add_task("", total=100)
 
                 while not progress.finished:
                     progress.update(task, advance=2)
-                    time.sleep(random.randint(2, 5) / 1000)
+                    sleep(randint(2, 5) / 1000)
 
             x_arr = linspace(-100, 100, 200000)
 
             def f(x: array):
                 return eval(replace_graph(calc))
 
             def dif(x: array):
@@ -338,29 +350,31 @@
             plt.axis([-7.5, 7.5, -7.5, 7.5])
             plt.legend(loc="lower left")
             plt.grid()
 
             download = input("Download graph? (y/n) ")
 
             if download == "y":
-                plt.savefig(df + ".pdf")
+                plt.savefig(save_path)
                 print("\nDownloaded graph.")
 
             plt.show()
-            print("\nExited graph.\n")
+            print("\nExited graph.")
 
         except:
             plt.close()
-            print("\n")
-            logging.warning("Could not graph function.")
+            warning("Could not graph function.")
             print("\nExited graph.")
 
 
 def partial_derive(function: str, var: str, order: str):
-    """Calculates the partial derivative of a function.
+    r"""Calculates the partial derivative of a function.
+
+    Explanation
+    ===========
 
     Takes a function, a variable, and an order of differentiation and
     returns the partial derivative of the function in respect
     to the variable with the order.
     """
 
     calc = replace_expr(function)
@@ -372,19 +386,24 @@
     print(
         f"\nPartial derivative of [bright_magenta]{replace_graph(function)}[/bright_magenta] in respect to {var} of order {order} is:\n"
     )
     print_expr(df)
 
     df = replace_expr(str(df))
     check_simp(df)
-    history.append(df)
+
+    if history[len(history) - 1] != df:
+        history.append(df)
 
 
 def implicit_derive(circ: str, order: str):
-    """Calculates the implicit derivative of an equation.
+    r"""Calculates the implicit derivative of an equation.
+
+    Explanation
+    ===========
 
     Takes an equation and an order of differentiation and
     returns the implicit derivative of an equation with the given order.
     """
 
     calc = replace_expr(circ)
     left = eval(calc[: calc.find("=")])
@@ -397,43 +416,50 @@
     print(
         f"\nDerivative of [bright_magenta]{circ}[/bright_magenta] with order {order} is:\n"
     )
     print_expr(df)
 
     df = replace_expr(str(df))
     check_simp(df)
-    history.append(df)
+
+    if history[len(history) - 1] != df:
+        history.append(df)
 
 
 def antiderive(function: str):
-    """Calculates the antiderivative of a function.
+    r"""Calculates the antiderivative of a function.
+
+    Explanation
+    ===========
 
     Takes a function and returns the antiderivative of the function.
     Graph option available.
     """
 
     calc = replace_expr(function)
     F = Integral(calc, x).doit()
 
     if "Integral" in str(F):
-        logging.warning("Cannot compute integral.\n")
+        warning("Cannot compute integral.\n")
         return ""
 
     print(
         f"\nAntiderivative of [bright_magenta]{replace_graph(function)}[/bright_magenta] is:\n"
     )
     print_expr(F)
 
     F = replace_expr(str(F))
     check_simp(F)
-    history.append(F)
+
+    if history[len(history) - 1] != F:
+        history.append(F)
 
     F = replace_graph(F)
 
-    print("\n[bold]Don't forget to add a constant![/bold]\n")
+    print("\n[bold]Don't forget to add a constant![/bold]")
 
     print("\n[bright_yellow]Show graph of area? (y/n)[/bright_yellow]")
     show = input("(Exit the graph window when you are finished to continue) ")
 
     if show == "y":
         try:
             print()
@@ -444,15 +470,15 @@
                 TimeElapsedColumn(),
                 transient=False,
             ) as progress:
                 task = progress.add_task("", total=100)
 
                 while not progress.finished:
                     progress.update(task, advance=2)
-                    time.sleep(random.randint(2, 5) / 1000)
+                    sleep(randint(2, 5) / 1000)
 
             x_arr = linspace(-100, 100, 200000)
 
             def f(x: array):
                 return eval(replace_graph(calc))
 
             def af(x: array):
@@ -466,30 +492,32 @@
             plt.plot(x_arr, af(x_arr), color="blue", label="Antiderivative")
             plt.axis([-7.5, 7.5, -7.5, 7.5])
             plt.legend(loc="lower left")
             plt.grid()
             download = input("Download graph? (y/n) ")
 
             if download == "y":
-                plt.savefig(df.replace("0 * x +", "") + ".pdf")
+                plt.savefig(save_path)
                 print("\nDownloaded graph.")
 
             plt.show()
 
-            print("\nExited graph.\n")
+            print("\nExited graph.")
 
         except:
             plt.close()
-            print("\n")
-            logging.warning("Could not graph function.")
-            print("\nExited graph.\n")
+            warning("Could not graph function.")
+            print("\nExited graph.")
 
 
 def def_int(function: str, low: str, up: str):
-    """Calculates the definite integral of a function.
+    r"""Calculates the definite integral of a function.
+
+    Explanation
+    ===========
 
     Takes a function and a lower and upper bound and
     returns the definite integral from the lower bound to
     the upper bound of the function.
     Graph option available.
     """
 
@@ -513,29 +541,31 @@
     # so calc-ultra is equipped with both symbolic and numerical answers.
 
     if (
         (str(result) == "nan")
         or ("i" in str(result))
         and ("Integral" not in str(result))
     ):
-        logging.warning("Cannot compute integral because integral does not converge.")
+        warning("Cannot compute integral because integral does not converge.")
         return ""
 
     if "Integral" not in str(result):
         print(
             f"\nCalculated integral of [bright_magenta]{replace_graph(function)}[/bright_magenta] from {low} to {up}. Final area is:\n"
         )
         print_expr(result)
         result = replace_expr(str(result))
-        history.append(result)
+
+        if history[len(history) - 1] != result:
+            history.append(result)
 
     else:
         print("\nCannot express result symbolically.")
 
-    nprint("\nNumeral evaluation/approximation:\n")
+    print("\nNumeral evaluation/approximation:\n")
     print_expr(num_result)
 
     print("\n[bright_yellow]Show graph of area? (y/n)[/bright_yellow]")
 
     show = input("(Exit the graph window when you are finished to continue) ")
 
     if show == "y":
@@ -548,15 +578,15 @@
                 TimeElapsedColumn(),
                 transient=False,
             ) as progress:
                 task = progress.add_task("", total=100)
 
                 while not progress.finished:
                     progress.update(task, advance=2)
-                    time.sleep(random.randint(2, 5) / 1000)
+                    sleep(randint(2, 5) / 1000)
 
             x_arr = linspace(-100, 100, 200000)
 
             if "log" in function:
                 x_arr = linspace(
                     0.0001,
                     100,
@@ -633,33 +663,35 @@
 
             plt.legend(loc="lower left")
             plt.grid()
 
             download = input("Download graph? (y/n) ")
 
             if download == "y":
-                plt.savefig(df.replace("0 * x +", "") + ".pdf")
+                plt.savefig(save_path)
                 print("\nDownloaded graph.")
 
             plt.show()
 
-            return "\nExited graph.\n"
+            return "\nExited graph."
 
         except:
             plt.close()
-            print("\n")
-            logging.warning("Could not graph function.")
-            return "\nExited graph.\n"
+            warning("Could not graph function.")
+            return "\nExited graph."
 
     else:
-        return "\n[bright_yellow]Exiting Definite Integral Screen ... ... ...[/bright_yellow]\n"
+        return "\n[bright_yellow]Exiting Definite Integral Screen ... ... ...[/bright_yellow]"
 
 
 def improp_int(function: str, low: str, up: str):
-    """Calculates the improper integral of a function.
+    r"""Calculates the improper integral of a function.
+
+    Explanation
+    ===========
 
     Takes a function and a lower and upper bound (can be inf)
     and returns the improper integral from the lower bound to
     the upper bound of the function. Uses Cauchy principal value
     for integrals with infinite bounds and standard integration
     for integrals with singularities.
     """
@@ -676,43 +708,50 @@
 
     try:
         improper_area = Integral(
             function, (x, calc_low, calc_up)
         ).principal_value()  # Cauchy Principal Value
 
         if "Integral" in str(improper_area):
-            logging.warning("Cannot compute improper integral.\n")
+            warning("Cannot compute improper integral.\n")
             return ""
 
         print(
             f"\nCalculated improper integral of [bright_magenta]{function}[/bright_magenta] from {low} to {up}. Final area is:\n"
         )
         print_expr(improper_area)
         improper_area = replace_expr(str(improper_area))
-        history.append(improper_area)
+
+        if history[len(history) - 1] != improper_area:
+            history.append(improper_area)
 
     except ValueError:
         improper_area = integrate(function, (x, calc_low, calc_up))
 
         if "Integral" in str(improper_area):
-            logging.warning("Cannot compute improper integral.\n")
+            warning("Cannot compute improper integral.\n")
             return ""
 
         print(
             f"\nCalculated improper integral of [bright_magenta]{function}[/bright_magenta] from {low} to {up}. Final area is:\n"
         )
         print_expr(improper_area)
         improper_area = replace_expr(str(improper_area))
-        history.append(improper_area)
+
+        if history[len(history) - 1] != improper_area:
+            history.append(improper_area)
 
     print()
 
 
 def double_int(function: str, out_low: str, out_up: str, in_low: str, in_up: str):
-    """Calculates the double integral of a function over region R.
+    r"""Calculates the double integral of a function over region R.
+
+    Explanation
+    ===========
 
     Takes a function and outer lower and upper and
     inner lower and upper bounds (that define region R)
     and returns the integral of the function over R.
     """
 
     function = replace_expr(function)
@@ -733,67 +772,77 @@
     out_low = eval(replace_expr(str(out_low)))
     in_up = eval(replace_expr(str(in_up)))
     in_low = eval(replace_expr(str(in_low)))
 
     result = integrate(function, (y, in_low, in_up), (x, out_low, out_up))
 
     if "Integral" in str(result):
-        logging.warning("Cannot compute integral.\n")
+        warning("Cannot compute integral.\n")
         return ""
 
     print(
         f"\nDouble integral of [bright_magenta]{function}[/bright_magenta] with inner bounds [bright_cyan]{in_low}[/bright_cyan] and [bright_cyan]{in_up}[/bright_cyan] and outer bounds {out_low} and {out_up} is:\n"
     )
     print_expr(result)
     result = replace_expr(str(result))
-    history.append(result)
-    print("")
+
+    if history[len(history) - 1] != result:
+        history.append(result)
+    print()
 
 
 def lim(function: str, value: str):
-    """Calculates limit of a function at a value.
+    r"""Calculates limit of a function at a value.
 
-    Takes a function and a value and
-    returns the limit of the function at the point.
+    Explanation
+    ===========
+
+    Takes a function and a value and returns the
+    limit of the function at the point.
     """
 
     function = replace_expr(function)
 
     check_num(value)
 
     value = float(eval(replace_expr(value)))
 
     l = limit(function, x, value)
 
     if "Limit" in str(l):
-        logging.warning("Cannot compute limit.")
+        warning("Cannot compute limit.")
         return ""
 
     if limit(function, x, value, "+") != limit(function, x, value, "-"):
-        logging.warning(
+        warning(
             "\nThe limit does not exist (the limit approaching from the right does not equal the limit approaching from the left)."
         )
         print(
             "[bright_red]Use one-side limit calculation to calculate the limit from one direction.[/bright_red]\n"
         )
         return ""
 
     print(
         f"\nLimit of [bright_magenta]{function}[/bright_magenta] as x approaches {value} is:\n"
     )
     print_expr(l)
     l = replace_expr(str(l))
-    history.append(l)
+
+    if history[len(history) - 1] != l:
+        history.append(l)
 
 
 def side_lim(function: str, value: str, direction: str):
-    """Calculates limit of a function at a value.
+    r"""Calculates limit of a function at a value.
 
-    Takes a function and a value and
-    returns the limit of the function at the point.
+    Explanation
+    ===========
+
+    Takes a function and a value and returns the
+    limit of the function at the point.
     """
     function = replace_expr(function)
 
     check_num(value)
 
     value = float(eval(replace_expr(value)))
 
@@ -801,53 +850,62 @@
         direction_sign = "-"
 
     elif direction == "right" or direction == "Right":
         direction_sign = "+"
 
     else:
         print()
-        logging.error("\nDirection is neither right or left.")
+        error("\nDirection is neither right or left.")
         return ""
 
     l = limit(function, x, value, dir=direction_sign)
 
     if "Limit" in str(l):
-        logging.warning("\nCannot compute limit.")
+        warning("\nCannot compute limit.")
         return ""
 
     print(
         f"\nLimit of [bright_magenta]{function}[/bright_magenta] as x approaches {value} from the [bright_cyan]{direction}[/bright_cyan] is:\n"
     )
     print_expr(l)
     l = replace_expr(str(l))
-    history.append(l)
+
+    if history[len(history) - 1] != l:
+        history.append(l)
 
 
 def eq_solve(mode: str):
-    """Solves an/a set of equation(s).
+    r"""Solves an/a set of equation(s).
+
+    Explanation
+    ===========
 
     Takes a mode to determine the number of equations
     to solve (1 to 3) and returns the values of the variables.
     """
 
     eq_list = []
 
     if mode == "1":
         eq1 = input("\nEnter equation: ")
         left = eval(eq1[: eq1.find("=")])
         right = eval(eq1[eq1.find("=") + 1 :])
         eq_set = solve(left - right)
         if len(eq_set) == 0:
             print()
-            logging.error("Cannot solve equation")
+            error("Cannot solve equation")
         else:
             print("\nx:\n")
             for i in range(0, len(eq_set)):
                 pprint(eq_set[i])
-                history.append(replace_expr(str(eq_set[i])))
+                sol = replace_expr(str(eq_set[i]))
+
+                if history[len(history) - 1] != sol:
+                    history.append(sol)
+
                 print()
 
     elif mode == "2":
         eq1 = input("Enter first equation: ")
         left1 = eval(eq1[: eq1.find("=")])
         right1 = eval(eq1[eq1.find("=") + 1 :])
 
@@ -896,15 +954,18 @@
 ################
 
 
 # These assistant functions sanatize inputs and prevent errors
 
 
 def check_simp(expr: str) -> bool:
-    """Check for simplification of an expression.
+    r"""Check for simplification of an expression.
+
+    Explanation
+    ===========
 
     Takes an expression and simplifies/rewrites it
     if possible. Otherwise returns boolean value False.
     """
 
     try:
         if str(simplify(expr, evaluate=False)) != expr:
@@ -915,123 +976,182 @@
             return False
 
     except:
         pass
 
 
 def check_order(order: str):
-    """Check if the order of differentiation is valid.
+    r"""Check if the order of differentiation is valid.
+
+    Explanation
+    ===========
 
     Takes the order of differentiation and gives an error
     if it is invalid.
     """
 
     if ("." in order) or (order.isnumeric() == False):
         print()
-        logging.error("Invalid order of differentiation.")
+        error("Invalid order of differentiation.")
 
 
 def check_num(num: str):
-    """Checks if a string is numerical (valid).
+    r"""Checks if a string is numerical (valid).
 
-    Takes a numerical valid string and gives an error
-    if it is invalid.
+    Explanation
+    ===========
+
+    Takes a string and checks if it is numerical valid
+    or containing a symbol. It gives an error if it
+    is invalid.
     """
 
     if (
         (num.isnumeric() is False)
         and ("pi" not in num)
         and ("e" not in num)
         and ("E" not in num)
         and ("-" not in num)
         and ("." not in num)
         and ("sqrt" not in num)
         and ("oo" not in num)
         and ("/" not in num)
+        and ("x" not in num)
+        and ("y" not in num)
+        and ("z" not in num)
+        and ("t" not in num)
+        and ("m" not in num)
     ):
         print()
-        logging.error("Invalid integration bound/numerical expression.")
+        error("Invalid integration bound/numerical expression.")
 
 
 def replace_expr(expr: str) -> str:
-    """Sanatizes an expression from input.
+    r"""Sanatizes an expression from input.
+
+    Explanation
+    ===========
 
     Takes a string and sanatizes input for calculation.
     """
 
-    expr = expr.strip()
-
-    # The extra 1 at the end is to recognize whether the "e"
-    # is part of an expression or a constant on it's own.
-
-    if "E" in expr:
-        expr = expr.replace("E", "E1")
-
-    if "e" in expr:
-        expr = expr.replace("e", "E1")
-
-    if "i" in expr:
-        expr = expr.replace("i", "I")
+    expr = expr.replace(" ", "")
 
     for r in expr_replace:
         expr = expr.replace(*r)
 
     return expr
 
 
 def replace_graph(function: str) -> str:
-    """Replaces an expression (function) for graphing.
+    r"""Replaces an expression (function) for graphing.
+
+    Explanation
+    ===========
 
     Takes a string and sanatizes it for graphing.
     This replacement includes changing prefixes of trig
     functions (since Sympy and Numpy trig functions uses
     different prefixes) and an implementation of csc, sec,
     cot, etc. (since Numpy does not provide them).
     """
 
-    if "log" in function and ",x)" in function:
-        function = function.replace("log", "mt.log")
-
     # Graph constant functions
 
     if "x" not in function:
         function = "0*x+" + function
 
     for r in graph_replace:
         function = function.replace(*r)
 
     return function
 
 
+def replace_calc(expr: str):
+    r"""Replaces an expression for calculation.
+
+    Explanation
+    ===========
+
+    Takes a string and sanatizes it for simple calculation
+    (i.e., calculation without calculus operations). This
+    replacement algorithm mainly deals with results that
+    should be 0 but instead outputs an answer near 0 (and is
+    simply changed to just 0), and complex numbers with an
+    imaginary part close to 0 (changed to 0). e.g., exp(i*pi)
+    gives a -1.0 * (a really small number). Using replace_calc
+    changes it to just -1.0.
+    """
+
+    try:
+        expr = simplify(expr.replace(" ", "").replace("ss.gamma", "gamma")).evalf()
+
+        if "I" not in str(expr):
+            if eval(str(expr)) < 0.000001 and eval(str(expr)) > -0.000001:
+                expr = 0
+
+        else:
+            expr = str(expr)
+            if "+" in str(expr):
+                imag = simplify(expr[expr.find("+") + 1 :].rstrip("*I")).evalf()
+                if imag < 0.000001 and imag > -0.000001:
+                    expr = simplify(expr[: expr.find("+")].rstrip("*I")).evalf()
+
+                else:
+                    expr = simplify(expr).evalf()
+
+            else:
+                if (
+                    simplify(expr.rstrip("*I")).evalf() < 0.000001
+                    and simplify(expr.rstrip("*I")).evalf() > -0.000001
+                ):
+                    expr = 0
+
+                else:
+                    expr = simplify(expr).evalf()
+
+        return expr
+
+    except:
+        pass
+
+
 def print_expr(text: str):
-    """Selects printing method.
+    r"""Selects printing method.
+
+    Explanation
+    ===========
 
     Linked to the printing settings option in settings.
     Chooses either normal print or Sympy pretty print.
+    Default setting in Sympy pprint.
     """
 
     printing_methods = {"p": lambda t: pprint(text), "n": lambda t: print(text)}
 
     try:
         printing_methods[print_option](text)
 
     except NameError:
         printing_methods["p"](text)
 
 
 def factorial(x):
-    """Simple implementation of a factorial function."""
+    r"""
+    Simple implementation of a factorial function,
+    using the gamma function as the expansion of
+    the factorial.
+    """
 
-    # Define our own factorial
     return ss.gamma(x + 1)
 
 
 def nprint(text: str):
     print(text)
-    time.sleep(0.04)
+    sleep(0.04)
 
 
 ####################
 # Driving programs #
 ####################
 
 
@@ -1044,39 +1164,34 @@
         TimeElapsedColumn(),
         transient=False,
     ) as progress:
         task = progress.add_task("", total=50)
 
         while not progress.finished:
             progress.update(task, advance=1)
-            time.sleep(random.randint(2, 5) / 100)
+            sleep(randint(2, 5) / 100)
 
-    global x, y, z, t, m, history, expr_replace, graph_replace
+    global x, y, z, t, m, history, expr_replace, graph_replace, save_path
 
     while True:
         instruct_path = (
-            os.path.dirname(os.path.abspath(__file__))
+            dirname(abspath(__file__))
             + "/texts/main_screen.txt"
             # TODO: make the PATH compatible with Windows
         )
         main = open(instruct_path, mode="r")
+
         for line in main.readlines():
             line = line.rstrip()
-            if ("---" in line) or ("|" in line):
-                nprint("[gold1]" + line + " [/gold1]")
+            if line.startswith(" "):
+                nprint(f"[gold1]{line}[/gold1]")
             else:
                 nprint(line)
 
-        try:
-            if date_option == "1":
-                now = (datetime.datetime.now()).strftime("%Y/%m/%d")
-            elif date_option == "2":
-                now = (datetime.datetime.now()).strftime("%Y/%m/%d %H:%M:%S")
-        except:
-            now = (datetime.datetime.now()).strftime("%Y/%m/%d %H:%M:%S")
+        now = (datetime.datetime.now()).strftime("%Y/%m/%d %H:%M:%S")
 
         print(f"\n(Time now is: {now})\n")
         print("[bold bright_green](Current Screen: Main Screen)[/bold bright_green]\n")
         print("[purple]Enter Command: [/purple]", end="")
         cmd = input()
 
         if cmd == "1":
@@ -1094,434 +1209,485 @@
         elif cmd == "5":
             algcalc()
 
         elif cmd == "6":
             settings()
 
         elif cmd == "7":
-            nprint("\n[bright_yellow]Exiting Calc-ULTRA ... ... ...[/bright_yellow]\n")
+            print("\n[bright_yellow]Exiting Calc-ULTRA ... ... ...[/bright_yellow]\n")
             break
 
         else:
-            print("\n")
-            logging.warning(f'Invalid command:"{cmd}"\n')
+            print()
+            warning(f'Invalid command:"{cmd}"\n')
 
 
 """
 If you find this message, type 'hi' in the general discussions - sudoer-Huatao
 """
 
 
 def derivacalc():
-    instruct_path = os.path.dirname(os.path.abspath(__file__)) + "/texts/derivacalc.txt"
-    derivacalc = open(instruct_path, mode="r")
-    for line in derivacalc.readlines():
-        line = line.rstrip()
-        if ("---" in line) or ("|" in line):
-            nprint("[gold1]" + line + " [/gold1]")
-        else:
-            nprint(line)
-    print()
-
     while True:
+        instruct_path = dirname(abspath(__file__)) + "/texts/derivacalc.txt"
+        derivacalc = open(instruct_path, mode="r")
+
+        for line in derivacalc.readlines():
+            line = line.rstrip()
+            if line.startswith(" "):
+                nprint(f"[gold1]{line}[/gold1]")
+            else:
+                nprint(line)
+
+        print()
+
         try:
-            nprint(
-                "\n[bold bright_green](Current Screen: DerivaCalc Main Screen)[/bold bright_green]\n"
+            print(
+                "[bold bright_green](Current Screen: DerivaCalc Main Screen)[/bold bright_green]\n"
             )
             print("[purple]Enter Command: [/purple]", end="")
             cmd = input()
 
             if cmd == "1":
-                nprint(
+                print(
                     "\n[bold bright_green](Current Screen: Derivative Screen)[/bold bright_green]\n"
                 )
-                function = input("Enter a function: ", key_bindings=key_bindings)
-                order = input(
+                function = prompt("Enter a function: ", key_bindings=key_bindings)
+                order = prompt(
                     "Enter order of derivative calculation: ", key_bindings=key_bindings
                 )
+
                 derive(function, order)
 
+                input("\nPress any key to continue: ")
+
             elif cmd == "2":
-                nprint(
+                print(
                     "\n[bold bright_green](Current Screen: Partial Derivative Screen)[/bold bright_green]\n"
                 )
-                function = input(
+                function = prompt(
                     "Enter a function containing x and y or x and y and z: ",
                     key_bindings=key_bindings,
                 )
-                var = input(
+                var = prompt(
                     "Enter variable to differentiate in respect to: ",
                     key_bindings=key_bindings,
                 )
+
                 if var != "x" and var != "y" and var != "z":
                     print()
-                    logging.error("Invalid variable to differentite in respect to.")
+                    error("Invalid variable to differentite in respect to.")
+
                 else:
-                    order = input(
+                    order = prompt(
                         "Enter the order of partial derivative calculation: ",
                         key_bindings=key_bindings,
                     )
+
                     partial_derive(function, var, order)
 
+                    input("\nPress any key to continue: ")
+
             elif cmd == "3":
-                nprint(
+                print(
                     "\n[bold bright_green](Current Screen: Implicit Derivative Screen)[/bold bright_green]\n"
                 )
-                circ = input(
+                circ = prompt(
                     "Enter an equation containing x and y:", key_bindings=key_bindings
                 )
-                order = input(
+                order = prompt(
                     "Enter order of implicit derivative calculation: ",
                     key_bindings=key_bindings,
                 )
+
                 implicit_derive(circ, order)
 
+                input("\nPress any key to continue: ")
+
             elif cmd == "4":
                 print("\n[bright_yellow]Exiting DerivaCalc ...[/bright_yellow]")
                 break
 
             else:
-                print("\n")
-                logging.warning(f'Invalid command:"{cmd}"')
+                print()
+                warning(f'Invalid command:"{cmd}"')
+                print()
+
         except:
-            print("\n")
-            logging.error("An unknown error occured.")
-            nprint("[bold bright_red]Check if your input is valid.[/bold bright_red]\n")
+            print()
+            error("An unknown error occured.")
+            print("[bold bright_red]Check if your input is valid.[/bold bright_red]\n")
 
 
 def intecalc():
-    instruct_path = os.path.dirname(os.path.abspath(__file__)) + "/texts/intecalc.txt"
-    intecalc = open(instruct_path, mode="r")
-    for line in intecalc.readlines():
-        line = line.rstrip()
-        if ("---" in line) or ("|" in line):
-            nprint("[gold1]" + line + " [/gold1]")
-        else:
-            nprint(line)
-    print()
-
     while True:
+        instruct_path = dirname((__file__)) + "/texts/intecalc.txt"
+        intecalc = open(instruct_path, mode="r")
+
+        for line in intecalc.readlines():
+            line = line.rstrip()
+            if line.startswith(" "):
+                nprint(f"[gold1]{line}[/gold1]")
+            else:
+                nprint(line)
+
+        print()
+
         try:
-            nprint(
+            print(
                 "[bold bright_green](Current Screen: InteCalc Main Screen)[/bold bright_green]\n"
             )
             print("[purple]Enter Command: [/purple]", end="")
             cmd = input()
 
             if cmd == "1":
-                nprint(
+                print(
                     "\n[bold bright_green](Current Screen: Antiderivative Screen)[/bold bright_green]\n"
                 )
-                function = input("Enter a function: ", key_bindings=key_bindings)
+                function = prompt("Enter a function: ", key_bindings=key_bindings)
+
                 antiderive(function)
 
+                input("\nPress any key to continue: ")
+
             elif cmd == "2":
-                nprint(
+                print(
                     "\n[bold bright_green](Current Screen: Definite Integral Screen)[/bold bright_green]\n"
                 )
-                function = input("Enter a function: ", key_bindings=key_bindings)
-                lower_bound = input(
+                function = prompt("Enter a function: ", key_bindings=key_bindings)
+                lower_bound = prompt(
                     "\nEnter the lower bound: ", key_bindings=key_bindings
                 )
-                upper_bound = input(
+                upper_bound = prompt(
                     "Enter the upper bound: ", key_bindings=key_bindings
                 )
+
                 print(def_int(function, lower_bound, upper_bound))
 
+                input("\nPress any key to continue: ")
+
             elif cmd == "3":
-                nprint(
+                print(
                     "\n[bold bright_green](Current Screen: Improper Integral Screen)[/bold bright_green]\n"
                 )
-                function = input("Enter a function: ", key_bindings=key_bindings)
-                lower_bound = input(
+                function = prompt("Enter a function: ", key_bindings=key_bindings)
+                lower_bound = prompt(
                     "\nEnter the lower bound: ", key_bindings=key_bindings
                 )
-                upper_bound = input(
+                upper_bound = prompt(
                     "Enter the upper bound: ", key_bindings=key_bindings
                 )
+
                 improp_int(function, lower_bound, upper_bound)
 
+                input("\nPress any key to continue: ")
+
             elif cmd == "4":
-                nprint(
+                print(
                     "\n[bold bright_green](Current Screen: Double Integral Screen)[/bold bright_green]\n"
                 )
-                function = input("Enter a function: ")
-                outer_low = input(
+                function = prompt("Enter a function: ", key_bindings=key_bindings)
+                outer_low = prompt(
                     "\nEnter the lower outer bound: ", key_bindings=key_bindings
                 )
-                outer_up = input(
+                outer_up = prompt(
                     "Enter the upper outer bound: ", key_bindings=key_bindings
                 )
-                inner_low = input(
+                inner_low = prompt(
                     "\nEnter the lower inner bound: ", key_bindings=key_bindings
                 )
-                inner_up = input(
+                inner_up = prompt(
                     "Enter the upper inner bound: ", key_bindings=key_bindings
                 )
+
                 double_int(function, outer_low, outer_up, inner_low, inner_up)
 
+                input("\nPress any key to continue: ")
+
             elif cmd == "5":
                 print("\n[bright_yellow]Exiting InteCalc ...[/bright_yellow]")
                 break
 
             else:
-                print("\n")
-                logging.warning(f'Invalid command: "{cmd}"')
+                print()
+                warning(f'Invalid command: "{cmd}"')
+
         except:
-            print("\n")
-            logging.error("An unknown error occured.")
-            nprint("[bold bright_red]Check if your input is valid.[/bold bright_red]\n")
+            print()
+            error("An unknown error occured.")
+            print("[bold bright_red]Check if your input is valid.[/bold bright_red]\n")
 
 
 def limcalc():
-    instruct_path = os.path.dirname(os.path.abspath(__file__)) + "/texts/limcalc.txt"
-    limcalc = open(instruct_path, mode="r")
-    for line in limcalc.readlines():
-        line = line.rstrip()
-        if ("---" in line) or ("|" in line):
-            nprint("[gold1]" + line + " [/gold1]")
-        else:
-            nprint(line)
-    print()
-
     while True:
+        instruct_path = dirname(abspath(__file__)) + "/texts/limcalc.txt"
+        limcalc = open(instruct_path, mode="r")
+
+        for line in limcalc.readlines():
+            line = line.rstrip()
+            if line.startswith(" "):
+                nprint(f"[gold1]{line}[/gold1]")
+            else:
+                nprint(line)
+
+        print()
+
         try:
-            nprint(
+            print(
                 "\n[bold bright_green](Current Screen: LimCalc Main Screen)[/bold bright_green]\n"
             )
             print("[purple]Enter Command: [/purple]", end="")
             cmd = input()
 
             if cmd == "1":
-                nprint(
+                print(
                     "\n[bold bright_green](Current screen: Limit Screen)[/bold bright_green]\n"
                 )
-                expr = input("Enter an expression: ", key_bindings=key_bindings)
-                value = input("Enter point of evaluation: ", key_bindings=key_bindings)
+                expr = prompt("Enter an expression: ", key_bindings=key_bindings)
+                value = prompt("Enter point of evaluation: ", key_bindings=key_bindings)
+
                 lim(expr, value)
 
+                input("\nPress any key to continue: ")
+
             elif cmd == "2":
-                nprint(
+                print(
                     "\n[bold bright_green](Current screen: One-sided Limit Screen)[/bold bright_green]\n"
                 )
-                expr = input("Enter an expression: ", key_bindings=key_bindings)
-                value = input("Enter point of evaluation: ", key_bindings=key_bindings)
+                expr = prompt("Enter an expression: ", key_bindings=key_bindings)
+                value = prompt("Enter point of evaluation: ", key_bindings=key_bindings)
                 direction = input("Enter direction of limit ('left' or 'right'): ")
+
                 side_lim(expr, value, direction)
 
+                input("\nPress any key to continue: ")
+
             elif cmd == "3":
                 print("\n[bright_yellow]Exiting LimCalc ...[/bright_yellow]")
                 break
 
             else:
-                print("\n")
-                logging.warning(f'Invalid command: "{cmd}"')
+                print()
+                warning(f'Invalid command: "{cmd}"')
 
         except:
-            print("\n")
-            logging.error("An unknown error occured.")
-            nprint("[bold bright_red]Check if your input is valid.[/bold bright_red]\n")
+            print()
+            error("An unknown error occured.")
+            print("[bold bright_red]Check if your input is valid.[/bold bright_red]\n")
 
 
 def algcalc():
-    instruct_path = os.path.dirname(os.path.abspath(__file__)) + "/texts/algcalc.txt"
-    algcalc = open(instruct_path, mode="r")
-    for line in algcalc.readlines():
-        line = line.rstrip()
-        if ("---" in line) or ("|" in line):
-            nprint("[gold1]" + line + " [/gold1]")
-        else:
-            nprint(line)
-    print()
-
     while True:
+        instruct_path = dirname(abspath(__file__)) + "/texts/algcalc.txt"
+        algcalc = open(instruct_path, mode="r")
+
+        for line in algcalc.readlines():
+            line = line.rstrip()
+            if line.startswith(" "):
+                nprint(f"[gold1]{line}[/gold1]")
+            else:
+                nprint(line)
+
+        print()
         try:
-            nprint(
+            print(
                 "\n[bold bright_green](Current Screen: AlgCalc Main Screen)[/bold bright_green]\n"
             )
             print("[purple]Enter Command: [/purple]", end="")
             cmd = input()
 
             if cmd == "1":
-                nprint(
+                print(
                     "\n[bold bright_green](Current screen: Equation Solver Screen)[/bold bright_green]\n"
                 )
                 mode = ""
 
                 while mode != "q":
                     print(
                         'Enter mode: 1 for one set equation, 2 for two, and 3 for three ("q" to quit): ',
                         end="",
                     )
                     mode = input()
                     eq_solve(mode)
 
             elif cmd == "2":
-                nprint(
+                print(
                     "\n[bold bright_green](Current screen: Vector Calculation Screen)[/bold bright_green]\n"
                 )
 
                 print("Write a vector like [1, 2, 3], then perform operations!")
                 print(
                     "\n- Use [bright_magenta]@[/bright_magenta] to calculate the dot product"
                 )
                 print("- cross(smth, smth) to calculate the cross product")
                 print(
                     "- A pair of [bright_magenta]< >[/bright_magenta]s encasing a vector to calculate it's norm!"
                 )
                 print('Enter any expression to start ("q" to quit):\n')
 
                 while True:
-                    expr = input(key_bindings=key_bindings)
+                    expr = prompt(key_bindings=key_bindings)
                     try:
                         if expr != "q":
                             expr = (
                                 (
                                     (
                                         (expr.replace("[", "array([")).replace(
                                             "]", "])"
                                         )
                                     ).replace("<", "norm(")
                                 ).replace(">", ")")
-                            ).strip(" ")
+                            ).replace(" ", "")
                             result = eval(replace_graph(expr))
                             print("\n[bright_yellow]Result: [/bright_yellow]", end="")
                             pprint(result)
                             print()
 
                         else:
                             break
                     except:
-                        logging.error(f'Could not parse: "{expr}"\n')
+                        error(f'Could not parse: "{expr}"\n')
 
                 print()
 
             elif cmd == "3":
-                nprint(
+                print(
                     "\n[bold bright_green](Current screen: Matrix Calculation Screen)[/bold bright_green]\n"
                 )
 
                 print("Write a matrix like [[1, 2], [3, 4]], then perform operations!")
                 print(
                     "- Use [bright_magenta]@[/bright_magenta] to calculate the dot product"
                 )
                 print(
                     "- A pair of [bright_magenta]| |[/bright_magenta] to calculate the determinant."
                 )
                 print('Enter any expression to start ("q" to quit):\n')
 
                 while True:
-                    expr = input(key_bindings=key_bindings)
+                    expr = prompt(key_bindings=key_bindings)
                     try:
                         if expr != "q":
                             expr = (
                                 (
                                     (
                                         (expr.replace("[[", "array([[")).replace(
                                             "]]", "]])"
                                         )
                                     ).replace("|a", "det(a")
                                 ).replace(")|", "))")
-                            ).strip(" ")
+                            ).replace(" ", "")
                             result = eval(replace_graph(expr))
                             print("\n[bright_yellow]Result: [/bright_yellow]\n")
                             pprint(result)
                             print()
 
                         else:
                             break
                     except:
-                        print("\n")
-                        logging.error(f'Could not parse: "{expr}"\n')
+                        print()
+                        error(f'Could not parse: "{expr}"\n')
 
             elif cmd == "4":
                 print("\n[bright_yellow]Exiting AlgCalc ...[/bright_yellow]")
                 break
 
             else:
-                print("\n")
-                logging.warning(f'Invalid command: "{cmd}"')
+                print()
+                warning(f'Invalid command: "{cmd}"')
 
         except:
-            print("\n")
-            logging.error("An unknown error occured.")
-            nprint("[bold bright_red]Check if your input is valid.[/bold bright_red]\n")
+            print()
+            error("An unknown error occured.")
+            print("[bold bright_red]Check if your input is valid.[/bold bright_red]\n")
 
 
 def settings():
     while True:
-        settings_path = (
-            os.path.dirname(os.path.abspath(__file__)) + "/texts/settings.txt"
-        )
+        settings_path = dirname(abspath(__file__)) + "/texts/settings.txt"
         settings = open(settings_path, mode="r")
 
         for line in settings.readlines():
             line = line.rstrip()
-            if ("---" in line) or ("|" in line):
-                nprint("[gold1]" + line + " [/gold1]")
+            if line.startswith(" "):
+                nprint(f"[gold1]{line}[/gold1]")
             else:
                 nprint(line)
+
         print("\n[bold green](Current Screen: Settings Screen)[/bold green]\n")
         print("[purple]Enter Command: [/purple]", end="")
         cmd = input()
 
         if cmd == "print":
             print(
                 "\n[bold bright_green](Current Screen: Print Settings Screen)[/bold bright_green]\n"
             )
 
             global print_option
+
             print_option = input(
                 'Set print mode: "p" (Sympy Pretty Print) or "n" (Normal Print): '
             )
             print(f'\nPrinting mode set to: "{print_option}"')
 
         elif cmd == "graph":
             print(
                 "\n[bold bright_green](Current Screen: Graph Settings Screen)[/bold bright_green]\n"
             )
 
             global graph_option
+
             graph_option = input(
                 'Set graph mode: "f" (Fixed graph view) or "a" (Adjusted graph view): '
             )
             print(f'\nGraph mode set to: "{graph_option}"')
 
-        elif cmd == "date":
-            print(
-                "\n[bold bright_green](Current Screen: Date Settings Screen)[/bold bright_green]\n"
-            )
-
-            global date_option
-            date_option = input(
-                'Set date mode: "1" (YY/MM/DD) or "2" (YY/MM/DD/HH/MM/SS): '
-            )
-            print(f'\nDate mode set to: "{date_option}"')
-
         elif cmd == "style":
             print(
                 "\n[bold bright_green](Current Screen: Graph Style Settings Screen)[/bold bright_green]\n"
             )
 
             print("You currently have these available styles:\n")
 
             style_list = plt.style.available
-            styles = ", ".join(style_list)
-            nprint("[bright_yellow]" + styles + " [/bright_yellow]")
+            styles = "  ,  ".join(style_list)
+            nprint(f"[bright_yellow]{styles}[/bright_yellow]")
 
             style = input('\nChoose a style to apply (type "default" to reset): ')
 
             plt.style.use(style)
 
             print(f'Graph style set to "{style}".')
 
+        elif cmd == "path":
+            print(
+                "\n[bold bright_green](Current Screen: Graph Save Path Screen)[/bold bright_green]\n"
+            )
+
+            global save_path
+
+            print(f"The current path where graphs will be saved to is: {save_path}.\n")
+
+            path = input(
+                'Enter a new absolute path for the graph to be saved in (e.g. /Users/spam/eggs), or exit ("q"): '
+            )
+
+            if path != "q":
+                if exists(path):
+                    save_path = path + "/fig.pdf"
+                    print(f"\nPath saved to: {save_path}.")
+
+                else:
+                    warning("\nThe path you specificied does not exist.")
+
         elif cmd == "exit":
             print("\n[bright_yellow]Exiting settings ... ... ...[/bright_yellow]")
             break
 
         else:
-            print("\n")
-            logging.warning(f'Invalid command:"{cmd}"')
+            print()
+            warning(f'Invalid command:"{cmd}"')
 
 
-main()
+if __name__ != "__main__":
+    main()
 # You've reached the end of the file!
```

### Comparing `calc_ultra-1.3.6/src/calc_ultra.egg-info/PKG-INFO` & `calc_ultra-1.3.7/src/calc_ultra.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calc_ultra
-Version: 1.3.6
+Version: 1.3.7
 Summary: A calculus calculator with a menu-based interface.
 Author-email: Huatao <huatao.xue@outlook.com>
 Maintainer-email: Huatao <huatao.xue@outlook.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/sudoer-Huatao/calc_ultra
 Project-URL: Issues, https://github.com/sudoer-Huatao/calc_ultra/issues
 Keywords: calculus,calculator
@@ -16,50 +16,55 @@
 Requires-Dist: sympy>=1.12
 Requires-Dist: numpy>=1.26.2
 Requires-Dist: matplotlib>=3.8.4
 Requires-Dist: rich>=13.7.1
 Requires-Dist: scipy>=1.13.0
 Requires-Dist: prompt_toolkit>=3.0.43
 
-# calc-ultra
+# Calc-Ultra
 
-[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) [![Version](https://img.shields.io/badge/Version-1.3.6-blue.svg)](https://github.com/sudoer-Huatao/calc_ultra)
+[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) [![Version](https://img.shields.io/badge/Version-1.3.7-blue.svg)](https://pypi.org/project/calc-ultra/)
 
 > **Calculus made easy**
 
 (Turn on dark mode for a better aesthetic) 📲
 
-Calc-Ultra is a multi-functional calculator that uses command line interfaces. Little Python background knowledge is needed to use the calculator!
+Calc-Ultra (styled as CALC ULTRA) is a multi-functional calculator that uses a command-line/menu-based interface. Little Python background knowledge is needed to use this calculator!
 
 Supports:
 
+- Simple calculations (complex numbers supported!)
 - Derivatives
 - Partials
 - Implicit differentiation
 - Limits
 - Antiderivatives
 - Definite integrals
 - Improper integrals
 - Double integrals
 - Solving (sets) of equation(s)
 - Vector/matrix operations
 - **A perfect interface to do calculations!**  
 
 ## Chinese version
 
-Want to check out the Chinese version? Visit <https://github.com/sudoer-Huatao/calc_ultra-chinese>! 🇨🇳
+Want to check out the Chinese version? Visit the Chinese version [here](https://github.com/sudoer-Huatao/calc_ultra-chinese)! 🇨🇳
 
 ## Installation and Running
 
 > Run the calculus calculator with a single line of code
 
-Use the following command to download Calc-Ultra (pip should be installed):
+Use the following command to install Calc-Ultra:
 
 `pip3 install calc-ultra`
 
+or
+
+`python3 -m pip install calc-ultra` if you have lower versions of pip.
+
 Due to Python import identifiers restrictions, please import Calc-Ultra as "calc_ultra" and not "calc-ultra".
 
 Import Calc-Ultra like so to use:
 
 `from calc_ultra import main`
 
 Please make sure you have the latest version installed. To update calc-ultra, run the following command:
@@ -73,47 +78,50 @@
 - `sympy`
 - `numpy`
 - `matplotlib`
 - `scipy`
 - `rich`
 - `prompt-toolkit`
 
-If you do not have them installed, no need to worry! These modules should be installed automatically if you don't have them. Other required modules are built into most Python IDEs as well.
+If you do not have them installed, no need to worry! These modules should be installed automatically if you don't have them.
 
 ## Acknowledgements
 
 > Without them, this would be impossible
 
 A big thank-you to all GitHub users who gave feedback and/or starred this repository. ⭐️ Your encouragement is our motivation.
 The following contributors deserve a SPECIAL THANK-YOU 👍❤️:
 
-- @Haobot for troubleshooting and feedback!
-- Fanbo for feedback and ideas for improvement!
+- [@Haobot](https://github.com/Haobot) for troubleshooting and feedback!
+- [@FanboFB](https://github.com/FanboFB) for feedback and ideas for improvement!
 
 This program was made using `sympy` for calculation and `numpy`, `scipy`, and `matplotlib` for graphing.
 
 ## Gallery (Demos)
 
+Simple calculation screen demo:
+![simple_calculation_screen_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/9df15b7e-e239-4f99-8966-db684ff36b68 "simple_calculation_demo")
+
 DerivaCalc derivative with graph demo:
-![derivacalc_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/3d99a51d-2e46-414c-8929-fa16016a856a "derivacalc_demo")
+![derivacalc_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/d0491f48-1a4f-4538-be7e-0bf793815eff "derivacalc_demo")
 
 InteCalc antiderivative with graph demo:
-![intecalc_demo_1](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/f61d44ae-cebf-4972-b63f-7f08ee6655b5 "intecalc_demo_1")
+![intecalc_demo_1](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/2375f351-46ae-4bfd-ad25-af599a26bbce "intecalc_demo_1")
 
 InteCalc definite integral with graph demo:
-![intecalc_demo_2](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/b8294186-92f5-4df3-a000-d63f6fff93b0 "intecalc_demo_2")
+![intecalc_demo_2](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/0af601a5-3d4c-4db5-a2aa-dff4b6bdd4b5 "intecalc_demo_2")
 
-LimCalc limit demo:
-![limcalc_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/12db6a7b-a836-43ce-8cef-7bcf707051f7 "limcalc_demo")
+LimCalc limit and one-sided limit demo:
+![limcalc_demo](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/bdecb164-b28c-4b4c-9f0a-cf9c44dfad90 "limcalc_demo")
 
 AlgCalc equation solver demo:
-![algcalc_demo_1](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/e4cfa016-52bf-43b5-a839-af9f42546468 "algcalc_demo_1")
+![algcalc_demo_1](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/74beffa8-7c82-4499-a114-8278e9929cdb "algcalc_demo_1")
 
 AlgCalc vector operation demo:
-![algcalc_demo_2](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/7f043cb2-6b0a-4460-ab35-30f09632b1c3 "algcalc_demo_2")
+![algcalc_demo_2](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/48b9624f-ab32-4f4c-99f7-1860dfd487a0 "algcalc_demo_2")
 
 AlgCalc matrix operation demo:
-![algcalc_demo_3](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/a9a5d56e-424a-4ef8-beb9-a9b64ce1a3f5 "algcalc_demo_3")
+![algcalc_demo_3](https://github.com/sudoer-Huatao/calc_ultra/assets/135504586/dee6cc8e-765d-4c41-b322-03f3ee501aac "algcalc_demo_3")
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

### Comparing `calc_ultra-1.3.6/src/calc_ultra.egg-info/SOURCES.txt` & `calc_ultra-1.3.7/src/calc_ultra.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 src/.DS_Store
 src/calc_ultra/.DS_Store
 src/calc_ultra/__init__.py
+src/calc_ultra/example.py
 src/calc_ultra/main.py
 src/calc_ultra.egg-info/PKG-INFO
 src/calc_ultra.egg-info/SOURCES.txt
 src/calc_ultra.egg-info/dependency_links.txt
 src/calc_ultra.egg-info/requires.txt
 src/calc_ultra.egg-info/top_level.txt
 src/calc_ultra/texts/__init__.py
```

