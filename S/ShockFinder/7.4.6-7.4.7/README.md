# Comparing `tmp/ShockFinder-7.4.6.tar.gz` & `tmp/ShockFinder-7.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ShockFinder-7.4.6.tar", last modified: Tue Mar 19 11:25:28 2024, max compression
+gzip compressed data, was "ShockFinder-7.4.7.tar", last modified: Mon May 20 07:23:04 2024, max compression
```

## Comparing `ShockFinder-7.4.6.tar` & `ShockFinder-7.4.7.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 11:25:28.716802 ShockFinder-7.4.6/
--rw-rw-rw-   0        0        0     1722 2023-07-11 13:12:33.000000 ShockFinder-7.4.6/LICENSE.txt
--rw-rw-rw-   0        0        0    17597 2024-03-19 11:25:28.715802 ShockFinder-7.4.6/PKG-INFO
--rw-rw-rw-   0        0        0    16996 2024-03-01 16:26:07.000000 ShockFinder-7.4.6/README.md
-drwxrwxrwx   0        0        0        0 2024-03-19 11:25:28.571769 ShockFinder-7.4.6/ShockFinder/
-drwxrwxrwx   0        0        0        0 2024-03-19 11:25:28.586773 ShockFinder-7.4.6/ShockFinder/Addon/
-drwxrwxrwx   0        0        0        0 2024-03-19 11:25:28.634784 ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/
--rw-rw-rw-   0        0        0     2949 2023-11-13 15:05:28.000000 ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/AnalysisToolModel.py
--rw-rw-rw-   0        0        0      351 2023-11-13 15:05:28.000000 ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/Basic.py
--rw-rw-rw-   0        0        0     2847 2023-11-13 15:05:28.000000 ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/Bremsstrahlung.py
--rw-rw-rw-   0        0        0     2655 2023-11-20 21:59:49.000000 ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/BruntVaisalaFrequency.py
--rw-rw-rw-   0        0        0     4669 2023-11-13 15:07:30.000000 ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/Config.py
--rw-rw-rw-   0        0        0    38927 2023-11-20 00:25:52.000000 ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/Differential.py
--rw-rw-rw-   0        0        0     2592 2023-11-13 15:05:28.000000 ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/Entropy.py
--rw-rw-rw-   0        0        0     4023 2023-11-20 13:07:39.000000 ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/Equilibrium.py
--rw-rw-rw-   0        0        0      626 2023-11-16 22:00:32.000000 ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/FastFourierTransform.py
--rw-rw-rw-   0        0        0     3444 2023-11-13 15:05:28.000000 ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/Harmonic.py
--rw-rw-rw-   0        0        0     2346 2023-12-15 14:44:40.000000 ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/KHI.py
--rw-rw-rw-   0        0        0     2925 2023-11-13 15:05:28.000000 ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/MachNumber.py
--rw-rw-rw-   0        0        0     1164 2023-11-13 15:05:28.000000 ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/MassFlux.py
--rw-rw-rw-   0        0        0     4282 2023-11-13 15:05:28.000000 ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/Mean.py
--rw-rw-rw-   0        0        0     2329 2023-11-20 21:59:35.000000 ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/RMI.py
--rw-rw-rw-   0        0        0     2978 2023-11-13 15:05:28.000000 ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/Radial.py
--rw-rw-rw-   0        0        0     2354 2023-11-20 21:59:28.000000 ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/ScalingSlope.py
--rw-rw-rw-   0        0        0     7191 2023-11-21 15:45:05.000000 ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/Shocks.py
--rw-rw-rw-   0        0        0     2627 2023-11-20 11:58:32.000000 ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/SoundSpeed.py
--rw-rw-rw-   0        0        0     2740 2023-11-20 12:09:09.000000 ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/Temperature.py
--rw-rw-rw-   0        0        0     2270 2023-11-13 15:05:28.000000 ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/TestData.py
--rw-rw-rw-   0        0        0      975 2023-11-13 15:05:28.000000 ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/Velocity.py
--rw-rw-rw-   0        0        0        0 2023-11-13 15:05:28.000000 ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/__init__.py
--rw-rw-rw-   0        0        0     1816 2024-03-01 08:43:18.000000 ShockFinder-7.4.6/ShockFinder/Addon/ConfigReader.py
-drwxrwxrwx   0        0        0        0 2024-03-19 11:25:28.640785 ShockFinder-7.4.6/ShockFinder/Addon/GUI/
--rw-rw-rw-   0        0        0      598 2023-10-23 22:22:13.000000 ShockFinder-7.4.6/ShockFinder/Addon/GUI/Config.py
--rw-rw-rw-   0        0        0     3201 2023-10-20 16:58:02.000000 ShockFinder-7.4.6/ShockFinder/Addon/GUI/XUI.py
-drwxrwxrwx   0        0        0        0 2024-03-19 11:25:28.646787 ShockFinder-7.4.6/ShockFinder/Addon/GUI/XUIlib/
--rw-rw-rw-   0        0        0    11875 2023-10-23 18:42:12.000000 ShockFinder-7.4.6/ShockFinder/Addon/GUI/XUIlib/ShockFinderFiguresHDF5.py
--rw-rw-rw-   0        0        0      503 2023-10-22 06:55:09.000000 ShockFinder-7.4.6/ShockFinder/Addon/GUI/XUIlib/XUIConfig.py
--rw-rw-rw-   0        0        0        0 2023-01-27 18:20:45.000000 ShockFinder-7.4.6/ShockFinder/Addon/GUI/XUIlib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 11:25:28.652788 ShockFinder-7.4.6/ShockFinder/Addon/GUI/XUIlib/image/
--rw-rw-rw-   0        0        0    96442 2024-03-01 16:15:33.000000 ShockFinder-7.4.6/ShockFinder/Addon/GUI/XUIlib/image/Main_logo.py
--rw-rw-rw-   0        0        0        0 2023-10-20 02:15:05.000000 ShockFinder-7.4.6/ShockFinder/Addon/GUI/XUIlib/image/__init__.py
--rw-rw-rw-   0        0        0      563 2023-10-20 16:52:36.000000 ShockFinder-7.4.6/ShockFinder/Addon/GUI/XUIlib/image/config.py
-drwxrwxrwx   0        0        0        0 2024-03-19 11:25:28.663791 ShockFinder-7.4.6/ShockFinder/Addon/GUI/XUIlib/pages/
--rw-rw-rw-   0        0        0    33969 2024-03-19 10:17:53.000000 ShockFinder-7.4.6/ShockFinder/Addon/GUI/XUIlib/pages/Analyze.py
--rw-rw-rw-   0        0        0   166605 2024-03-19 11:19:33.000000 ShockFinder-7.4.6/ShockFinder/Addon/GUI/XUIlib/pages/Figure.py
--rw-rw-rw-   0        0        0     1723 2023-11-13 15:05:29.000000 ShockFinder-7.4.6/ShockFinder/Addon/GUI/XUIlib/pages/Help.py
--rw-rw-rw-   0        0        0        0 2023-07-09 06:49:01.000000 ShockFinder-7.4.6/ShockFinder/Addon/GUI/XUIlib/pages/__init__.py
--rw-rw-rw-   0        0        0      732 2023-11-13 15:05:29.000000 ShockFinder-7.4.6/ShockFinder/Addon/GUI/XUIlib/pages/page_model.py
--rw-rw-rw-   0        0        0        0 2023-01-27 18:20:45.000000 ShockFinder-7.4.6/ShockFinder/Addon/GUI/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 11:25:28.672792 ShockFinder-7.4.6/ShockFinder/Addon/IO/
--rw-rw-rw-   0        0        0      598 2023-10-23 22:22:13.000000 ShockFinder-7.4.6/ShockFinder/Addon/IO/Config.py
--rw-rw-rw-   0        0        0     4005 2024-03-19 11:00:34.000000 ShockFinder-7.4.6/ShockFinder/Addon/IO/HDF5.py
--rw-rw-rw-   0        0        0     7449 2023-07-04 23:32:54.000000 ShockFinder-7.4.6/ShockFinder/Addon/IO/MySQL.py
--rw-rw-rw-   0        0        0        0 2023-07-03 20:09:39.000000 ShockFinder-7.4.6/ShockFinder/Addon/IO/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 11:25:28.684795 ShockFinder-7.4.6/ShockFinder/Addon/Loader/
--rw-rw-rw-   0        0        0      633 2023-10-23 22:22:13.000000 ShockFinder-7.4.6/ShockFinder/Addon/Loader/Config.py
--rw-rw-rw-   0        0        0      545 2023-09-12 20:20:45.000000 ShockFinder-7.4.6/ShockFinder/Addon/Loader/FileNamePreProcess.py
--rw-rw-rw-   0        0        0      798 2024-03-19 10:21:43.000000 ShockFinder-7.4.6/ShockFinder/Addon/Loader/FilesPreProcess.py
--rw-rw-rw-   0        0        0     1828 2023-07-08 11:49:23.000000 ShockFinder-7.4.6/ShockFinder/Addon/Loader/LoaderModel.py
--rw-rw-rw-   0        0        0     1581 2023-09-12 20:08:47.000000 ShockFinder-7.4.6/ShockFinder/Addon/Loader/Pluto.py
-drwxrwxrwx   0        0        0        0 2024-03-19 11:25:28.691797 ShockFinder-7.4.6/ShockFinder/Addon/Loader/Pluto_lib/
--rw-rw-rw-   0        0        0    14345 2021-05-30 02:54:20.000000 ShockFinder-7.4.6/ShockFinder/Addon/Loader/Pluto_lib/Tools.py
--rw-rw-rw-   0        0        0        0 2023-01-27 18:20:45.000000 ShockFinder-7.4.6/ShockFinder/Addon/Loader/Pluto_lib/__init__.py
--rw-rw-rw-   0        0        0    20616 2023-09-12 19:44:35.000000 ShockFinder-7.4.6/ShockFinder/Addon/Loader/Pluto_lib/pload.py
--rw-rw-rw-   0        0        0        0 2023-01-27 18:20:45.000000 ShockFinder-7.4.6/ShockFinder/Addon/Loader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 11:25:28.697798 ShockFinder-7.4.6/ShockFinder/Addon/MultiprocessEngine/
--rw-rw-rw-   0        0        0      704 2023-10-23 22:22:13.000000 ShockFinder-7.4.6/ShockFinder/Addon/MultiprocessEngine/Config.py
--rw-rw-rw-   0        0        0       65 2023-10-21 22:32:43.000000 ShockFinder-7.4.6/ShockFinder/Addon/MultiprocessEngine/XME.py
--rw-rw-rw-   0        0        0        0 2023-07-03 20:03:27.000000 ShockFinder-7.4.6/ShockFinder/Addon/MultiprocessEngine/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 11:25:28.713801 ShockFinder-7.4.6/ShockFinder/Addon/Painter/
--rw-rw-rw-   0        0        0     8861 2023-11-16 16:13:44.000000 ShockFinder-7.4.6/ShockFinder/Addon/Painter/Basic.py
--rw-rw-rw-   0        0        0     2058 2023-11-13 15:07:30.000000 ShockFinder-7.4.6/ShockFinder/Addon/Painter/Config.py
--rw-rw-rw-   0        0        0     6935 2023-11-20 13:51:45.000000 ShockFinder-7.4.6/ShockFinder/Addon/Painter/Line.py
--rw-rw-rw-   0        0        0     7012 2023-12-14 16:05:21.000000 ShockFinder-7.4.6/ShockFinder/Addon/Painter/P2D.py
--rw-rw-rw-   0        0        0     2840 2023-11-15 22:41:05.000000 ShockFinder-7.4.6/ShockFinder/Addon/Painter/P3D.py
--rw-rw-rw-   0        0        0      830 2023-11-13 15:05:29.000000 ShockFinder-7.4.6/ShockFinder/Addon/Painter/Scatter.py
--rw-rw-rw-   0        0        0     2321 2023-11-13 15:05:29.000000 ShockFinder-7.4.6/ShockFinder/Addon/Painter/Surface.py
--rw-rw-rw-   0        0        0        0 2023-07-02 10:54:39.000000 ShockFinder-7.4.6/ShockFinder/Addon/Painter/__init__.py
--rw-rw-rw-   0        0        0      257 2023-07-05 00:06:42.000000 ShockFinder-7.4.6/ShockFinder/Addon/Time.py
--rw-rw-rw-   0        0        0        0 2023-01-27 18:20:45.000000 ShockFinder-7.4.6/ShockFinder/Addon/__init__.py
--rw-rw-rw-   0        0        0     4474 2024-03-19 11:25:08.000000 ShockFinder-7.4.6/ShockFinder/Config.py
--rw-rw-rw-   0        0        0      271 2023-07-03 20:50:22.000000 ShockFinder-7.4.6/ShockFinder/Data.py
--rw-rw-rw-   0        0        0     5254 2023-11-13 10:16:46.000000 ShockFinder-7.4.6/ShockFinder/DataBase.py
--rw-rw-rw-   0        0        0      325 2023-06-30 17:59:11.000000 ShockFinder-7.4.6/ShockFinder/Loader.py
--rw-rw-rw-   0        0        0     3495 2023-10-21 21:08:01.000000 ShockFinder-7.4.6/ShockFinder/Update.py
--rw-rw-rw-   0        0        0    10216 2024-03-19 10:22:33.000000 ShockFinder-7.4.6/ShockFinder/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 11:25:28.580772 ShockFinder-7.4.6/ShockFinder.egg-info/
--rw-rw-rw-   0        0        0    17597 2024-03-19 11:25:28.000000 ShockFinder-7.4.6/ShockFinder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2938 2024-03-19 11:25:28.000000 ShockFinder-7.4.6/ShockFinder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 11:25:28.000000 ShockFinder-7.4.6/ShockFinder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-03-19 11:25:28.000000 ShockFinder-7.4.6/ShockFinder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-19 11:25:28.716802 ShockFinder-7.4.6/setup.cfg
--rw-rw-rw-   0        0        0      841 2024-03-19 11:25:15.000000 ShockFinder-7.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:23:04.724849 ShockFinder-7.4.7/
+-rw-rw-rw-   0        0        0     1722 2023-07-11 13:12:33.000000 ShockFinder-7.4.7/LICENSE.txt
+-rw-rw-rw-   0        0        0    17597 2024-05-20 07:23:04.723848 ShockFinder-7.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0    16996 2024-03-01 16:26:07.000000 ShockFinder-7.4.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 07:23:04.524803 ShockFinder-7.4.7/ShockFinder/
+drwxrwxrwx   0        0        0        0 2024-05-20 07:23:04.544808 ShockFinder-7.4.7/ShockFinder/Addon/
+drwxrwxrwx   0        0        0        0 2024-05-20 07:23:04.611823 ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/
+-rw-rw-rw-   0        0        0     2949 2023-11-13 15:05:28.000000 ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/AnalysisToolModel.py
+-rw-rw-rw-   0        0        0      351 2023-11-13 15:05:28.000000 ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/Basic.py
+-rw-rw-rw-   0        0        0     2847 2023-11-13 15:05:28.000000 ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/Bremsstrahlung.py
+-rw-rw-rw-   0        0        0     2655 2023-11-20 21:59:49.000000 ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/BruntVaisalaFrequency.py
+-rw-rw-rw-   0        0        0     4669 2023-11-13 15:07:30.000000 ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/Config.py
+-rw-rw-rw-   0        0        0    38927 2023-11-20 00:25:52.000000 ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/Differential.py
+-rw-rw-rw-   0        0        0     2592 2023-11-13 15:05:28.000000 ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/Entropy.py
+-rw-rw-rw-   0        0        0     4023 2023-11-20 13:07:39.000000 ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/Equilibrium.py
+-rw-rw-rw-   0        0        0      626 2023-11-16 22:00:32.000000 ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/FastFourierTransform.py
+-rw-rw-rw-   0        0        0     3444 2023-11-13 15:05:28.000000 ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/Harmonic.py
+-rw-rw-rw-   0        0        0     2346 2023-12-15 14:44:40.000000 ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/KHI.py
+-rw-rw-rw-   0        0        0     2925 2023-11-13 15:05:28.000000 ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/MachNumber.py
+-rw-rw-rw-   0        0        0     1164 2023-11-13 15:05:28.000000 ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/MassFlux.py
+-rw-rw-rw-   0        0        0     4282 2023-11-13 15:05:28.000000 ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/Mean.py
+-rw-rw-rw-   0        0        0     2329 2023-11-20 21:59:35.000000 ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/RMI.py
+-rw-rw-rw-   0        0        0     2978 2023-11-13 15:05:28.000000 ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/Radial.py
+-rw-rw-rw-   0        0        0     2354 2023-11-20 21:59:28.000000 ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/ScalingSlope.py
+-rw-rw-rw-   0        0        0     7191 2023-11-21 15:45:05.000000 ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/Shocks.py
+-rw-rw-rw-   0        0        0     2627 2023-11-20 11:58:32.000000 ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/SoundSpeed.py
+-rw-rw-rw-   0        0        0     2740 2023-11-20 12:09:09.000000 ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/Temperature.py
+-rw-rw-rw-   0        0        0     2270 2023-11-13 15:05:28.000000 ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/TestData.py
+-rw-rw-rw-   0        0        0      975 2023-11-13 15:05:28.000000 ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/Velocity.py
+-rw-rw-rw-   0        0        0        0 2023-11-13 15:05:28.000000 ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/__init__.py
+-rw-rw-rw-   0        0        0     1816 2024-03-01 08:43:18.000000 ShockFinder-7.4.7/ShockFinder/Addon/ConfigReader.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:23:04.620825 ShockFinder-7.4.7/ShockFinder/Addon/GUI/
+-rw-rw-rw-   0        0        0      598 2023-10-23 22:22:13.000000 ShockFinder-7.4.7/ShockFinder/Addon/GUI/Config.py
+-rw-rw-rw-   0        0        0     3201 2023-10-20 16:58:02.000000 ShockFinder-7.4.7/ShockFinder/Addon/GUI/XUI.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:23:04.629827 ShockFinder-7.4.7/ShockFinder/Addon/GUI/XUIlib/
+-rw-rw-rw-   0        0        0    11875 2023-10-23 18:42:12.000000 ShockFinder-7.4.7/ShockFinder/Addon/GUI/XUIlib/ShockFinderFiguresHDF5.py
+-rw-rw-rw-   0        0        0      503 2023-10-22 06:55:09.000000 ShockFinder-7.4.7/ShockFinder/Addon/GUI/XUIlib/XUIConfig.py
+-rw-rw-rw-   0        0        0        0 2023-01-27 18:20:45.000000 ShockFinder-7.4.7/ShockFinder/Addon/GUI/XUIlib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:23:04.638829 ShockFinder-7.4.7/ShockFinder/Addon/GUI/XUIlib/image/
+-rw-rw-rw-   0        0        0    96442 2024-03-01 16:15:33.000000 ShockFinder-7.4.7/ShockFinder/Addon/GUI/XUIlib/image/Main_logo.py
+-rw-rw-rw-   0        0        0        0 2023-10-20 02:15:05.000000 ShockFinder-7.4.7/ShockFinder/Addon/GUI/XUIlib/image/__init__.py
+-rw-rw-rw-   0        0        0      563 2023-10-20 16:52:36.000000 ShockFinder-7.4.7/ShockFinder/Addon/GUI/XUIlib/image/config.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:23:04.653833 ShockFinder-7.4.7/ShockFinder/Addon/GUI/XUIlib/pages/
+-rw-rw-rw-   0        0        0    33969 2024-03-19 10:17:53.000000 ShockFinder-7.4.7/ShockFinder/Addon/GUI/XUIlib/pages/Analyze.py
+-rw-rw-rw-   0        0        0   166605 2024-03-19 11:19:33.000000 ShockFinder-7.4.7/ShockFinder/Addon/GUI/XUIlib/pages/Figure.py
+-rw-rw-rw-   0        0        0     1723 2023-11-13 15:05:29.000000 ShockFinder-7.4.7/ShockFinder/Addon/GUI/XUIlib/pages/Help.py
+-rw-rw-rw-   0        0        0        0 2023-07-09 06:49:01.000000 ShockFinder-7.4.7/ShockFinder/Addon/GUI/XUIlib/pages/__init__.py
+-rw-rw-rw-   0        0        0      732 2023-11-13 15:05:29.000000 ShockFinder-7.4.7/ShockFinder/Addon/GUI/XUIlib/pages/page_model.py
+-rw-rw-rw-   0        0        0        0 2023-01-27 18:20:45.000000 ShockFinder-7.4.7/ShockFinder/Addon/GUI/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:23:04.663835 ShockFinder-7.4.7/ShockFinder/Addon/IO/
+-rw-rw-rw-   0        0        0      598 2023-10-23 22:22:13.000000 ShockFinder-7.4.7/ShockFinder/Addon/IO/Config.py
+-rw-rw-rw-   0        0        0     4005 2024-03-19 11:00:34.000000 ShockFinder-7.4.7/ShockFinder/Addon/IO/HDF5.py
+-rw-rw-rw-   0        0        0     7449 2023-07-04 23:32:54.000000 ShockFinder-7.4.7/ShockFinder/Addon/IO/MySQL.py
+-rw-rw-rw-   0        0        0        0 2023-07-03 20:09:39.000000 ShockFinder-7.4.7/ShockFinder/Addon/IO/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:23:04.680838 ShockFinder-7.4.7/ShockFinder/Addon/Loader/
+-rw-rw-rw-   0        0        0      633 2023-10-23 22:22:13.000000 ShockFinder-7.4.7/ShockFinder/Addon/Loader/Config.py
+-rw-rw-rw-   0        0        0      545 2023-09-12 20:20:45.000000 ShockFinder-7.4.7/ShockFinder/Addon/Loader/FileNamePreProcess.py
+-rw-rw-rw-   0        0        0      798 2024-03-19 10:21:43.000000 ShockFinder-7.4.7/ShockFinder/Addon/Loader/FilesPreProcess.py
+-rw-rw-rw-   0        0        0     1828 2023-07-08 11:49:23.000000 ShockFinder-7.4.7/ShockFinder/Addon/Loader/LoaderModel.py
+-rw-rw-rw-   0        0        0     1581 2023-09-12 20:08:47.000000 ShockFinder-7.4.7/ShockFinder/Addon/Loader/Pluto.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:23:04.690841 ShockFinder-7.4.7/ShockFinder/Addon/Loader/Pluto_lib/
+-rw-rw-rw-   0        0        0    14345 2021-05-30 02:54:20.000000 ShockFinder-7.4.7/ShockFinder/Addon/Loader/Pluto_lib/Tools.py
+-rw-rw-rw-   0        0        0        0 2023-01-27 18:20:45.000000 ShockFinder-7.4.7/ShockFinder/Addon/Loader/Pluto_lib/__init__.py
+-rw-rw-rw-   0        0        0    20616 2023-09-12 19:44:35.000000 ShockFinder-7.4.7/ShockFinder/Addon/Loader/Pluto_lib/pload.py
+-rw-rw-rw-   0        0        0        0 2023-01-27 18:20:45.000000 ShockFinder-7.4.7/ShockFinder/Addon/Loader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:23:04.698843 ShockFinder-7.4.7/ShockFinder/Addon/MultiprocessEngine/
+-rw-rw-rw-   0        0        0      704 2023-10-23 22:22:13.000000 ShockFinder-7.4.7/ShockFinder/Addon/MultiprocessEngine/Config.py
+-rw-rw-rw-   0        0        0       65 2023-10-21 22:32:43.000000 ShockFinder-7.4.7/ShockFinder/Addon/MultiprocessEngine/XME.py
+-rw-rw-rw-   0        0        0        0 2023-07-03 20:03:27.000000 ShockFinder-7.4.7/ShockFinder/Addon/MultiprocessEngine/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:23:04.721848 ShockFinder-7.4.7/ShockFinder/Addon/Painter/
+-rw-rw-rw-   0        0        0     8861 2023-11-16 16:13:44.000000 ShockFinder-7.4.7/ShockFinder/Addon/Painter/Basic.py
+-rw-rw-rw-   0        0        0     2058 2023-11-13 15:07:30.000000 ShockFinder-7.4.7/ShockFinder/Addon/Painter/Config.py
+-rw-rw-rw-   0        0        0     6935 2023-11-20 13:51:45.000000 ShockFinder-7.4.7/ShockFinder/Addon/Painter/Line.py
+-rw-rw-rw-   0        0        0     7012 2023-12-14 16:05:21.000000 ShockFinder-7.4.7/ShockFinder/Addon/Painter/P2D.py
+-rw-rw-rw-   0        0        0     2840 2023-11-15 22:41:05.000000 ShockFinder-7.4.7/ShockFinder/Addon/Painter/P3D.py
+-rw-rw-rw-   0        0        0      830 2023-11-13 15:05:29.000000 ShockFinder-7.4.7/ShockFinder/Addon/Painter/Scatter.py
+-rw-rw-rw-   0        0        0     2321 2023-11-13 15:05:29.000000 ShockFinder-7.4.7/ShockFinder/Addon/Painter/Surface.py
+-rw-rw-rw-   0        0        0        0 2023-07-02 10:54:39.000000 ShockFinder-7.4.7/ShockFinder/Addon/Painter/__init__.py
+-rw-rw-rw-   0        0        0      257 2023-07-05 00:06:42.000000 ShockFinder-7.4.7/ShockFinder/Addon/Time.py
+-rw-rw-rw-   0        0        0        0 2023-01-27 18:20:45.000000 ShockFinder-7.4.7/ShockFinder/Addon/__init__.py
+-rw-rw-rw-   0        0        0     4472 2024-05-20 07:17:10.000000 ShockFinder-7.4.7/ShockFinder/Config.py
+-rw-rw-rw-   0        0        0      271 2023-07-03 20:50:22.000000 ShockFinder-7.4.7/ShockFinder/Data.py
+-rw-rw-rw-   0        0        0     5254 2023-11-13 10:16:46.000000 ShockFinder-7.4.7/ShockFinder/DataBase.py
+-rw-rw-rw-   0        0        0      325 2023-06-30 17:59:11.000000 ShockFinder-7.4.7/ShockFinder/Loader.py
+-rw-rw-rw-   0        0        0     3495 2023-10-21 21:08:01.000000 ShockFinder-7.4.7/ShockFinder/Update.py
+-rw-rw-rw-   0        0        0    10216 2024-03-19 10:22:33.000000 ShockFinder-7.4.7/ShockFinder/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 07:23:04.535806 ShockFinder-7.4.7/ShockFinder.egg-info/
+-rw-rw-rw-   0        0        0    17597 2024-05-20 07:23:04.000000 ShockFinder-7.4.7/ShockFinder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2938 2024-05-20 07:23:04.000000 ShockFinder-7.4.7/ShockFinder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 07:23:04.000000 ShockFinder-7.4.7/ShockFinder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-20 07:23:04.000000 ShockFinder-7.4.7/ShockFinder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 07:23:04.724849 ShockFinder-7.4.7/setup.cfg
+-rw-rw-rw-   0        0        0      841 2024-05-20 07:17:31.000000 ShockFinder-7.4.7/setup.py
```

### Comparing `ShockFinder-7.4.6/LICENSE.txt` & `ShockFinder-7.4.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/PKG-INFO` & `ShockFinder-7.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShockFinder
-Version: 7.4.6
+Version: 7.4.7
 Summary: ShockFinder is an interactive scientic simulation data analysis software based on python and supports multi-process, multi-mode, I/O access and drawing.
 Home-page: https://github.com/wacmkxiaoyi/Shockfinder
 Author: Junxiang H. & C. B. Singh
 Author-email: huangjunxiang@mail.ynu.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ShockFinder-7.4.6/README.md` & `ShockFinder-7.4.7/README.md`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/AnalysisToolModel.py` & `ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/AnalysisToolModel.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/Bremsstrahlung.py` & `ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/Bremsstrahlung.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/BruntVaisalaFrequency.py` & `ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/BruntVaisalaFrequency.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/Config.py` & `ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/Config.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/Differential.py` & `ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/Differential.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/Entropy.py` & `ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/Entropy.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/Equilibrium.py` & `ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/Equilibrium.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/FastFourierTransform.py` & `ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/FastFourierTransform.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/Harmonic.py` & `ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/Harmonic.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/KHI.py` & `ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/KHI.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/MachNumber.py` & `ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/MachNumber.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/MassFlux.py` & `ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/MassFlux.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/Mean.py` & `ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/Mean.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/RMI.py` & `ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/RMI.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/Radial.py` & `ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/Radial.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/ScalingSlope.py` & `ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/ScalingSlope.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/Shocks.py` & `ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/Shocks.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/SoundSpeed.py` & `ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/SoundSpeed.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/Temperature.py` & `ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/Temperature.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/TestData.py` & `ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/TestData.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/AnalysisTool/Velocity.py` & `ShockFinder-7.4.7/ShockFinder/Addon/AnalysisTool/Velocity.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/ConfigReader.py` & `ShockFinder-7.4.7/ShockFinder/Addon/ConfigReader.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/GUI/Config.py` & `ShockFinder-7.4.7/ShockFinder/Addon/GUI/Config.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/GUI/XUI.py` & `ShockFinder-7.4.7/ShockFinder/Addon/GUI/XUI.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/GUI/XUIlib/ShockFinderFiguresHDF5.py` & `ShockFinder-7.4.7/ShockFinder/Addon/GUI/XUIlib/ShockFinderFiguresHDF5.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/GUI/XUIlib/image/Main_logo.py` & `ShockFinder-7.4.7/ShockFinder/Addon/GUI/XUIlib/image/Main_logo.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/GUI/XUIlib/image/config.py` & `ShockFinder-7.4.7/ShockFinder/Addon/GUI/XUIlib/image/config.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/GUI/XUIlib/pages/Analyze.py` & `ShockFinder-7.4.7/ShockFinder/Addon/GUI/XUIlib/pages/Analyze.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/GUI/XUIlib/pages/Figure.py` & `ShockFinder-7.4.7/ShockFinder/Addon/GUI/XUIlib/pages/Figure.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/GUI/XUIlib/pages/Help.py` & `ShockFinder-7.4.7/ShockFinder/Addon/GUI/XUIlib/pages/Help.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/GUI/XUIlib/pages/page_model.py` & `ShockFinder-7.4.7/ShockFinder/Addon/GUI/XUIlib/pages/page_model.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/IO/Config.py` & `ShockFinder-7.4.7/ShockFinder/Addon/IO/Config.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/IO/HDF5.py` & `ShockFinder-7.4.7/ShockFinder/Addon/IO/HDF5.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/IO/MySQL.py` & `ShockFinder-7.4.7/ShockFinder/Addon/IO/MySQL.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/Loader/Config.py` & `ShockFinder-7.4.7/ShockFinder/Addon/Loader/Config.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/Loader/FileNamePreProcess.py` & `ShockFinder-7.4.7/ShockFinder/Addon/Loader/FileNamePreProcess.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/Loader/FilesPreProcess.py` & `ShockFinder-7.4.7/ShockFinder/Addon/Loader/FilesPreProcess.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/Loader/LoaderModel.py` & `ShockFinder-7.4.7/ShockFinder/Addon/Loader/LoaderModel.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/Loader/Pluto.py` & `ShockFinder-7.4.7/ShockFinder/Addon/Loader/Pluto.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/Loader/Pluto_lib/Tools.py` & `ShockFinder-7.4.7/ShockFinder/Addon/Loader/Pluto_lib/Tools.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/Loader/Pluto_lib/pload.py` & `ShockFinder-7.4.7/ShockFinder/Addon/Loader/Pluto_lib/pload.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/MultiprocessEngine/Config.py` & `ShockFinder-7.4.7/ShockFinder/Addon/MultiprocessEngine/Config.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/Painter/Basic.py` & `ShockFinder-7.4.7/ShockFinder/Addon/Painter/Basic.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/Painter/Config.py` & `ShockFinder-7.4.7/ShockFinder/Addon/Painter/Config.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/Painter/Line.py` & `ShockFinder-7.4.7/ShockFinder/Addon/Painter/Line.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/Painter/P2D.py` & `ShockFinder-7.4.7/ShockFinder/Addon/Painter/P2D.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/Painter/P3D.py` & `ShockFinder-7.4.7/ShockFinder/Addon/Painter/P3D.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/Painter/Scatter.py` & `ShockFinder-7.4.7/ShockFinder/Addon/Painter/Scatter.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Addon/Painter/Surface.py` & `ShockFinder-7.4.7/ShockFinder/Addon/Painter/Surface.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Config.py` & `ShockFinder-7.4.7/ShockFinder/Config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #File type: Basic Default Value and libraries, please modify with the situation
 #By Junxiang H., 2023/07/1
 #wacmk.com/cn Tech. Supp.
 
 import os
-ShockFinderVersion=7.4.6
+ShockFinderVersion=7.4
 ShockFinderDir=os.path.join(__file__.rsplit("ShockFinder",1)[0],"ShockFinder")
 ShockFinderHeader=(
 		'■■■■■■■■■■■□■■■■■■■■■■■■■■■■■■■■',
 		'■■■■■■■■■■□■■■■■■■■■■■■■■■■■■■■■',
 		'■■■■■■■■■□△■■■■■■■■■■■■■■■■■■■■■',
 		'■■■■■■■■□■△■◁■■■■■■■ShockFinder v'+str(ShockFinderVersion)+'■■■■',
 		'■■■■■■■□■■△■■■■■■■■■■■■■■■■■■■■■',
```

### Comparing `ShockFinder-7.4.6/ShockFinder/DataBase.py` & `ShockFinder-7.4.7/ShockFinder/DataBase.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/Update.py` & `ShockFinder-7.4.7/ShockFinder/Update.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder/__init__.py` & `ShockFinder-7.4.7/ShockFinder/__init__.py`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/ShockFinder.egg-info/PKG-INFO` & `ShockFinder-7.4.7/ShockFinder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShockFinder
-Version: 7.4.6
+Version: 7.4.7
 Summary: ShockFinder is an interactive scientic simulation data analysis software based on python and supports multi-process, multi-mode, I/O access and drawing.
 Home-page: https://github.com/wacmkxiaoyi/Shockfinder
 Author: Junxiang H. & C. B. Singh
 Author-email: huangjunxiang@mail.ynu.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ShockFinder-7.4.6/ShockFinder.egg-info/SOURCES.txt` & `ShockFinder-7.4.7/ShockFinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ShockFinder-7.4.6/setup.py` & `ShockFinder-7.4.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="ShockFinder",
-    version="7.4.6",
+    version="7.4.7",
     author="Junxiang H. & C. B. Singh",
     author_email="huangjunxiang@mail.ynu.edu.cn",
     description="ShockFinder is an interactive scientic simulation data analysis software based on python and supports multi-process, multi-mode, I/O access and drawing.",
     long_description=long_description, 
     long_description_content_type="text/markdown",
     url="https://github.com/wacmkxiaoyi/Shockfinder", 
     packages=setuptools.find_packages(),
```

