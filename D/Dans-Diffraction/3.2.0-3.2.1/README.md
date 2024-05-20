# Comparing `tmp/Dans_Diffraction-3.2.0.tar.gz` & `tmp/dans_diffraction-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Dans_Diffraction-3.2.0.tar", last modified: Sun May 19 07:09:06 2024, max compression
+gzip compressed data, was "dans_diffraction-3.2.1.tar", last modified: Mon May 20 06:26:29 2024, max compression
```

## Comparing `Dans_Diffraction-3.2.0.tar` & `dans_diffraction-3.2.1.tar`

### file list

```diff
@@ -1,133 +1,135 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 07:09:06.573392 Dans_Diffraction-3.2.0/
-drwxrwxrwx   0        0        0        0 2024-05-19 07:09:05.976489 Dans_Diffraction-3.2.0/Dans_Diffraction/
-drwxrwxrwx   0        0        0        0 2024-05-19 07:09:06.111949 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/
--rw-rw-rw-   0        0        0     4217 2016-08-03 08:31:31.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Aluminium.cif
--rw-rw-rw-   0        0        0     2503 2017-07-31 08:37:44.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/BCC.cif
--rw-rw-rw-   0        0        0     1188 2015-08-03 13:46:33.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Beryllium.cif
--rw-rw-rw-   0        0        0     2250 2018-03-01 19:54:35.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Ca2RuO4.cif
--rw-rw-rw-   0        0        0     3878 2016-11-10 08:23:42.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Ca3CoMnO6.mcif
--rw-rw-rw-   0        0        0     1226 2017-07-31 09:00:59.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Cobalt.cif
--rw-rw-rw-   0        0        0     4214 2015-08-03 13:23:49.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Copper.cif
--rw-rw-rw-   0        0        0     1671 2016-09-15 10:40:04.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Cubic.cif
--rw-rw-rw-   0        0        0     4714 2016-12-06 14:03:28.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Diamond.cif
--rw-rw-rw-   0        0        0     4214 2015-08-03 13:23:49.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/FCC.cif
--rw-rw-rw-   0        0        0     4212 2018-02-14 08:14:18.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Gold.cif
--rw-rw-rw-   0        0        0     2243 2017-04-12 13:11:25.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Graphite.cif
--rw-rw-rw-   0        0        0     1226 2017-07-31 09:00:59.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/HCP.cif
--rw-rw-rw-   0        0        0     2503 2017-07-31 08:37:44.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Iron.cif
--rw-rw-rw-   0        0        0     4325 2017-07-09 15:12:00.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/KCl.cif
--rw-rw-rw-   0        0        0     3082 2020-04-17 07:58:01.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/LaMnO3.mcif
--rw-rw-rw-   0        0        0     1987 2016-05-31 12:37:29.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/LiCoO2.cif
--rw-rw-rw-   0        0        0     2067 2015-05-15 09:42:35.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Na0.8CoO2_P63mmc.cif
--rw-rw-rw-   0        0        0    17159 2023-05-08 11:29:37.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/NaCoO2_stripe_supercell.cif
--rw-rw-rw-   0        0        0     2507 2016-08-03 08:28:38.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Niobium.cif
--rw-rw-rw-   0        0        0     1901 2016-12-06 14:29:29.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Ruby.cif
--rw-rw-rw-   0        0        0     1191 2016-03-07 11:53:11.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Ruthenium.cif
--rw-rw-rw-   0        0        0     1927 2019-05-03 14:32:02.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Sapphire.cif
--rw-rw-rw-   0        0        0     4739 2015-08-04 14:43:40.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Silicon.cif
--rw-rw-rw-   0        0        0     4315 2017-09-05 12:52:37.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Silver.cif
--rw-rw-rw-   0        0        0    83448 2020-03-26 10:12:50.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Sr3LiRuO6.cif
--rw-rw-rw-   0        0        0     4568 2020-02-24 07:33:16.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Sr3LiRuO6_C2'c'.mcif
--rw-rw-rw-   0        0        0     2532 2019-04-03 13:35:10.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Vanadium.cif
--rw-rw-rw-   0        0        0     2468 2020-02-17 08:59:33.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/ZnO.cif
--rw-rw-rw-   0        0        0     9450 2024-05-19 06:53:14.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/__init__.py
--rw-rw-rw-   0        0        0     1101 2023-04-26 10:54:53.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/__main__.py
--rw-rw-rw-   0        0        0    92680 2024-05-02 07:03:04.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/classes_crystal.py
--rw-rw-rw-   0        0        0    51728 2024-05-02 07:03:04.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/classes_fdmnes.py
--rw-rw-rw-   0        0        0     9899 2022-07-23 11:12:54.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/classes_multicrystal.py
--rw-rw-rw-   0        0        0    19043 2023-07-16 14:24:15.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/classes_orbitals.py
--rw-rw-rw-   0        0        0    10482 2023-01-06 13:55:56.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/classes_orientation.py
--rw-rw-rw-   0        0        0    93613 2024-05-19 06:53:14.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/classes_plotting.py
--rw-rw-rw-   0        0        0    37527 2024-03-28 13:31:10.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/classes_properties.py
--rw-rw-rw-   0        0        0   139952 2024-05-19 06:32:45.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/classes_scattering.py
--rw-rw-rw-   0        0        0     2867 2023-08-18 10:11:48.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/classes_structures.py
-drwxrwxrwx   0        0        0        0 2024-05-19 07:09:06.220819 Dans_Diffraction-3.2.0/Dans_Diffraction/data/
--rw-rw-rw-   0        0        0    54010 2020-05-02 16:39:54.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/data/Dans Element Properties.txt
--rw-rw-rw-   0        0        0    43658 2019-12-13 07:38:09.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/data/Dans Element Properties_old.txt
--rw-rw-rw-   0        0        0     4719 2019-07-31 18:31:45.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/data/Element_OxidationStates.txt
--rw-rw-rw-   0        0        0    58645 2021-03-31 11:01:14.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/data/PointGroups.json
--rw-rw-rw-   0        0        0   997216 2020-04-22 21:04:44.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/data/SpaceGroups.json
--rw-rw-rw-   0        0        0  8319520 2020-05-26 14:42:44.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/data/SpaceGroupsMagnetic.json
--rw-rw-rw-   0        0        0    30113 2016-12-01 11:30:15.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/data/XRayEdges.dat
--rw-rw-rw-   0        0        0  2779670 2020-05-06 09:22:05.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/data/XRayMassAtten_muenp.dat
--rw-rw-rw-   0        0        0  2779670 2020-05-06 09:22:05.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/data/XRayMassAtten_mup.dat
--rw-rw-rw-   0        0        0  1317778 2021-01-21 09:28:34.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/data/atomic_scattering_factors.npy
--rw-rw-rw-   0        0        0    43385 2021-06-08 07:44:54.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/data/f0_WaasKirf.dat
--rw-rw-rw-   0        0        0    25892 2023-05-06 11:12:54.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/data/peng.dat
--rw-rw-rw-   0        0        0   152719 2024-05-18 09:47:05.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/functions_crystallography.py
--rw-rw-rw-   0        0        0    47409 2024-05-15 19:15:56.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/functions_general.py
--rw-rw-rw-   0        0        0    34608 2024-05-19 06:39:03.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/functions_plotting.py
--rw-rw-rw-   0        0        0    44417 2023-05-07 14:24:07.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/functions_scattering.py
--rw-rw-rw-   0        0        0    27095 2020-10-15 13:27:33.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/multiple_scattering.py
--rw-rw-rw-   0        0        0   192479 2023-01-06 14:04:42.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tensor_scattering.py
-drwxrwxrwx   0        0        0        0 2024-05-19 07:09:06.266292 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/
--rw-rw-rw-   0        0        0     1570 2024-03-28 13:17:42.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/__init__.py
--rw-rw-rw-   0        0        0    14834 2023-07-16 12:26:55.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/basic_widgets.py
--rw-rw-rw-   0        0        0    16665 2023-10-19 11:03:24.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/converter.py
--rw-rw-rw-   0        0        0    50929 2024-03-28 16:28:00.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/crystal.py
--rw-rw-rw-   0        0        0    73139 2023-10-19 09:23:59.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/diffractometer.py
--rw-rw-rw-   0        0        0    26672 2023-07-20 05:54:00.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/fdmnes.py
--rw-rw-rw-   0        0        0     9934 2024-03-28 15:58:36.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/multi_crystal.py
--rw-rw-rw-   0        0        0     7072 2023-07-14 09:21:27.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/multiple_scattering.py
--rw-rw-rw-   0        0        0    10826 2023-05-16 16:30:28.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/periodic_table.py
--rw-rw-rw-   0        0        0    30256 2023-08-14 07:29:38.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/properties.py
--rw-rw-rw-   0        0        0    94783 2024-05-18 09:36:05.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/scattering.py
--rw-rw-rw-   0        0        0    14775 2023-05-22 06:11:38.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/spacegroups.py
--rw-rw-rw-   0        0        0    13686 2020-02-20 13:50:35.000000 Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/tensor_scattering.py
-drwxrwxrwx   0        0        0        0 2024-05-19 07:09:05.999499 Dans_Diffraction-3.2.0/Dans_Diffraction.egg-info/
--rw-rw-rw-   0        0        0    14849 2024-05-19 07:09:05.000000 Dans_Diffraction-3.2.0/Dans_Diffraction.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4390 2024-05-19 07:09:05.000000 Dans_Diffraction-3.2.0/Dans_Diffraction.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 07:09:05.000000 Dans_Diffraction-3.2.0/Dans_Diffraction.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-19 07:09:05.000000 Dans_Diffraction-3.2.0/Dans_Diffraction.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-19 07:09:05.000000 Dans_Diffraction-3.2.0/Dans_Diffraction.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11558 2020-04-19 15:46:17.000000 Dans_Diffraction-3.2.0/LICENSE
--rw-rw-rw-   0        0        0    14849 2024-05-19 07:09:06.570107 Dans_Diffraction-3.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    14048 2024-05-17 08:01:40.000000 Dans_Diffraction-3.2.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-19 07:09:06.573892 Dans_Diffraction-3.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1255 2024-05-19 06:53:14.000000 Dans_Diffraction-3.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-19 07:09:06.567029 Dans_Diffraction-3.2.0/test/
--rw-rw-rw-   0        0        0     2282 2018-02-13 15:38:28.000000 Dans_Diffraction-3.2.0/test/test_LS_magnetic_components.py
--rw-rw-rw-   0        0        0     8939 2021-06-10 16:58:04.000000 Dans_Diffraction-3.2.0/test/test_WaasKirf_xray_factors.py
--rw-rw-rw-   0        0        0     2197 2020-04-30 13:31:49.000000 Dans_Diffraction-3.2.0/test/test_atom_properties.py
--rw-rw-rw-   0        0        0     1170 2020-05-06 08:27:47.000000 Dans_Diffraction-3.2.0/test/test_attenuation.py
--rw-rw-rw-   0        0        0     1910 2021-01-25 17:53:20.000000 Dans_Diffraction-3.2.0/test/test_attenuation_length.py
--rw-rw-rw-   0        0        0     2002 2020-11-12 13:20:39.000000 Dans_Diffraction-3.2.0/test/test_bmatrix.py
--rw-rw-rw-   0        0        0     1704 2023-08-16 11:18:50.000000 Dans_Diffraction-3.2.0/test/test_check_append_vs_unique.py
--rw-rw-rw-   0        0        0     1562 2020-10-19 07:41:46.000000 Dans_Diffraction-3.2.0/test/test_cif_files.py
--rw-rw-rw-   0        0        0     6312 2021-07-19 15:51:46.000000 Dans_Diffraction-3.2.0/test/test_coherent_diffraction.py
--rw-rw-rw-   0        0        0     3230 2021-07-17 05:26:09.000000 Dans_Diffraction-3.2.0/test/test_coherent_diffraction2.py
--rw-rw-rw-   0        0        0     1859 2019-12-12 20:20:59.000000 Dans_Diffraction-3.2.0/test/test_compare_intensity.py
--rw-rw-rw-   0        0        0     8480 2020-10-26 14:50:52.000000 Dans_Diffraction-3.2.0/test/test_compare_intensity_calculation.py
--rw-rw-rw-   0        0        0     4552 2020-05-12 07:18:31.000000 Dans_Diffraction-3.2.0/test/test_compound_name.py
--rw-rw-rw-   0        0        0     2740 2022-03-11 16:54:13.000000 Dans_Diffraction-3.2.0/test/test_convolve2d.py
--rw-rw-rw-   0        0        0      289 2020-10-20 19:46:18.000000 Dans_Diffraction-3.2.0/test/test_detector.py
--rw-rw-rw-   0        0        0     2902 2020-05-15 15:03:16.000000 Dans_Diffraction-3.2.0/test/test_electron_density.py
--rw-rw-rw-   0        0        0     5008 2020-10-19 07:41:46.000000 Dans_Diffraction-3.2.0/test/test_exchange_path.py
--rw-rw-rw-   0        0        0     4144 2020-10-19 07:41:46.000000 Dans_Diffraction-3.2.0/test/test_exchange_path2.py
--rw-rw-rw-   0        0        0      149 2018-06-08 14:18:49.000000 Dans_Diffraction-3.2.0/test/test_files.py
--rw-rw-rw-   0        0        0     5627 2021-07-15 05:41:12.000000 Dans_Diffraction-3.2.0/test/test_functions_scattering.py
--rw-rw-rw-   0        0        0     1152 2021-07-15 16:03:30.000000 Dans_Diffraction-3.2.0/test/test_functions_scattering_dispersion.py
--rw-rw-rw-   0        0        0     3320 2021-07-14 17:11:38.000000 Dans_Diffraction-3.2.0/test/test_functions_scattering_new.py
--rw-rw-rw-   0        0        0     4726 2021-07-13 13:13:30.000000 Dans_Diffraction-3.2.0/test/test_functions_scattering_pol.py
--rw-rw-rw-   0        0        0     3102 2021-07-13 14:17:38.000000 Dans_Diffraction-3.2.0/test/test_functions_scattering_xrm.py
--rw-rw-rw-   0        0        0     1691 2020-03-27 07:59:19.000000 Dans_Diffraction-3.2.0/test/test_gaussian.py
--rw-rw-rw-   0        0        0    17556 2020-06-09 08:44:11.000000 Dans_Diffraction-3.2.0/test/test_gen_sym_mat.py
--rw-rw-rw-   0        0        0      256 2020-03-31 13:19:32.000000 Dans_Diffraction-3.2.0/test/test_gui_multicrystal.py
--rw-rw-rw-   0        0        0     3193 2020-11-22 19:46:51.000000 Dans_Diffraction-3.2.0/test/test_i16_azimuth.py
--rw-rw-rw-   0        0        0      552 2020-03-27 16:10:17.000000 Dans_Diffraction-3.2.0/test/test_intensity_grid.py
--rw-rw-rw-   0        0        0     1196 2020-03-27 08:15:40.000000 Dans_Diffraction-3.2.0/test/test_isincell.py
--rw-rw-rw-   0        0        0     2536 2021-10-04 20:22:07.000000 Dans_Diffraction-3.2.0/test/test_laue_backscatter.py
--rw-rw-rw-   0        0        0     3864 2019-02-22 16:52:35.000000 Dans_Diffraction-3.2.0/test/test_nonresonant.py
--rw-rw-rw-   0        0        0     5702 2019-01-21 13:30:00.000000 Dans_Diffraction-3.2.0/test/test_nonresonant_plot.py
--rw-rw-rw-   0        0        0     3092 2019-01-21 13:25:46.000000 Dans_Diffraction-3.2.0/test/test_nonresonant_sergio.py
--rw-rw-rw-   0        0        0      453 2021-09-26 16:50:06.000000 Dans_Diffraction-3.2.0/test/test_orientation.py
--rw-rw-rw-   0        0        0     1044 2017-11-26 15:52:58.000000 Dans_Diffraction-3.2.0/test/test_parameter_plot.py
--rw-rw-rw-   0        0        0     4428 2020-11-22 20:40:03.000000 Dans_Diffraction-3.2.0/test/test_plot_orbitals.py
--rw-rw-rw-   0        0        0     1956 2017-08-22 12:09:50.000000 Dans_Diffraction-3.2.0/test/test_plotintensity.py
--rw-rw-rw-   0        0        0     2890 2017-08-22 15:29:48.000000 Dans_Diffraction-3.2.0/test/test_plotintensity2.py
--rw-rw-rw-   0        0        0     2593 2020-05-05 08:27:58.000000 Dans_Diffraction-3.2.0/test/test_readstfm.py
--rw-rw-rw-   0        0        0      327 2023-07-19 15:10:57.000000 Dans_Diffraction-3.2.0/test/test_reflection_selector.py
--rw-rw-rw-   0        0        0      988 2021-01-26 07:46:04.000000 Dans_Diffraction-3.2.0/test/test_refractive_index.py
--rw-rw-rw-   0        0        0     1843 2017-10-30 14:29:08.000000 Dans_Diffraction-3.2.0/test/test_scattering.py
--rw-rw-rw-   0        0        0     2649 2017-11-09 11:24:34.000000 Dans_Diffraction-3.2.0/test/test_supercell.py
--rw-rw-rw-   0        0        0     9400 2020-06-09 13:06:44.000000 Dans_Diffraction-3.2.0/test/test_symmetry_ops2magnetic.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:26:29.109241 dans_diffraction-3.2.1/
+drwxrwxrwx   0        0        0        0 2024-05-20 06:26:28.478042 dans_diffraction-3.2.1/Dans_Diffraction/
+drwxrwxrwx   0        0        0        0 2024-05-20 06:26:28.604691 dans_diffraction-3.2.1/Dans_Diffraction/Structures/
+-rw-rw-rw-   0        0        0     4217 2016-08-03 08:31:31.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/Aluminium.cif
+-rw-rw-rw-   0        0        0     2503 2017-07-31 08:37:44.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/BCC.cif
+-rw-rw-rw-   0        0        0     1188 2015-08-03 13:46:33.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/Beryllium.cif
+-rw-rw-rw-   0        0        0     2250 2018-03-01 19:54:35.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/Ca2RuO4.cif
+-rw-rw-rw-   0        0        0     3878 2016-11-10 08:23:42.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/Ca3CoMnO6.mcif
+-rw-rw-rw-   0        0        0     1226 2017-07-31 09:00:59.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/Cobalt.cif
+-rw-rw-rw-   0        0        0     4214 2015-08-03 13:23:49.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/Copper.cif
+-rw-rw-rw-   0        0        0     1671 2016-09-15 10:40:04.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/Cubic.cif
+-rw-rw-rw-   0        0        0     4714 2016-12-06 14:03:28.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/Diamond.cif
+-rw-rw-rw-   0        0        0     4214 2015-08-03 13:23:49.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/FCC.cif
+-rw-rw-rw-   0        0        0     4212 2018-02-14 08:14:18.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/Gold.cif
+-rw-rw-rw-   0        0        0     2243 2017-04-12 13:11:25.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/Graphite.cif
+-rw-rw-rw-   0        0        0     1226 2017-07-31 09:00:59.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/HCP.cif
+-rw-rw-rw-   0        0        0     2503 2017-07-31 08:37:44.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/Iron.cif
+-rw-rw-rw-   0        0        0     4325 2017-07-09 15:12:00.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/KCl.cif
+-rw-rw-rw-   0        0        0     3082 2020-04-17 07:58:01.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/LaMnO3.mcif
+-rw-rw-rw-   0        0        0     1987 2016-05-31 12:37:29.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/LiCoO2.cif
+-rw-rw-rw-   0        0        0     2067 2015-05-15 09:42:35.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/Na0.8CoO2_P63mmc.cif
+-rw-rw-rw-   0        0        0    17159 2023-05-08 11:29:37.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/NaCoO2_stripe_supercell.cif
+-rw-rw-rw-   0        0        0     2507 2016-08-03 08:28:38.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/Niobium.cif
+-rw-rw-rw-   0        0        0     1901 2016-12-06 14:29:29.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/Ruby.cif
+-rw-rw-rw-   0        0        0     1191 2016-03-07 11:53:11.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/Ruthenium.cif
+-rw-rw-rw-   0        0        0     1927 2019-05-03 14:32:02.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/Sapphire.cif
+-rw-rw-rw-   0        0        0     4739 2015-08-04 14:43:40.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/Silicon.cif
+-rw-rw-rw-   0        0        0     4315 2017-09-05 12:52:37.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/Silver.cif
+-rw-rw-rw-   0        0        0    83448 2020-03-26 10:12:50.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/Sr3LiRuO6.cif
+-rw-rw-rw-   0        0        0     4568 2020-02-24 07:33:16.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/Sr3LiRuO6_C2'c'.mcif
+-rw-rw-rw-   0        0        0     2532 2019-04-03 13:35:10.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/Vanadium.cif
+-rw-rw-rw-   0        0        0     2468 2020-02-17 08:59:33.000000 dans_diffraction-3.2.1/Dans_Diffraction/Structures/ZnO.cif
+-rw-rw-rw-   0        0        0     9635 2024-05-20 06:24:54.000000 dans_diffraction-3.2.1/Dans_Diffraction/__init__.py
+-rw-rw-rw-   0        0        0     1101 2023-04-26 10:54:53.000000 dans_diffraction-3.2.1/Dans_Diffraction/__main__.py
+-rw-rw-rw-   0        0        0    96185 2024-05-20 05:50:04.000000 dans_diffraction-3.2.1/Dans_Diffraction/classes_crystal.py
+-rw-rw-rw-   0        0        0    51728 2024-05-02 07:03:04.000000 dans_diffraction-3.2.1/Dans_Diffraction/classes_fdmnes.py
+-rw-rw-rw-   0        0        0     9899 2022-07-23 11:12:54.000000 dans_diffraction-3.2.1/Dans_Diffraction/classes_multicrystal.py
+-rw-rw-rw-   0        0        0    19043 2023-07-16 14:24:15.000000 dans_diffraction-3.2.1/Dans_Diffraction/classes_orbitals.py
+-rw-rw-rw-   0        0        0    10482 2023-01-06 13:55:56.000000 dans_diffraction-3.2.1/Dans_Diffraction/classes_orientation.py
+-rw-rw-rw-   0        0        0    95148 2024-05-20 05:50:04.000000 dans_diffraction-3.2.1/Dans_Diffraction/classes_plotting.py
+-rw-rw-rw-   0        0        0    37527 2024-03-28 13:31:10.000000 dans_diffraction-3.2.1/Dans_Diffraction/classes_properties.py
+-rw-rw-rw-   0        0        0   139952 2024-05-19 06:32:45.000000 dans_diffraction-3.2.1/Dans_Diffraction/classes_scattering.py
+-rw-rw-rw-   0        0        0     2867 2023-08-18 10:11:48.000000 dans_diffraction-3.2.1/Dans_Diffraction/classes_structures.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:26:28.694551 dans_diffraction-3.2.1/Dans_Diffraction/data/
+-rw-rw-rw-   0        0        0    54010 2020-05-02 16:39:54.000000 dans_diffraction-3.2.1/Dans_Diffraction/data/Dans Element Properties.txt
+-rw-rw-rw-   0        0        0    43658 2019-12-13 07:38:09.000000 dans_diffraction-3.2.1/Dans_Diffraction/data/Dans Element Properties_old.txt
+-rw-rw-rw-   0        0        0     4719 2019-07-31 18:31:45.000000 dans_diffraction-3.2.1/Dans_Diffraction/data/Element_OxidationStates.txt
+-rw-rw-rw-   0        0        0    58645 2021-03-31 11:01:14.000000 dans_diffraction-3.2.1/Dans_Diffraction/data/PointGroups.json
+-rw-rw-rw-   0        0        0   997216 2020-04-22 21:04:44.000000 dans_diffraction-3.2.1/Dans_Diffraction/data/SpaceGroups.json
+-rw-rw-rw-   0        0        0  8319520 2020-05-26 14:42:44.000000 dans_diffraction-3.2.1/Dans_Diffraction/data/SpaceGroupsMagnetic.json
+-rw-rw-rw-   0        0        0    30113 2016-12-01 11:30:15.000000 dans_diffraction-3.2.1/Dans_Diffraction/data/XRayEdges.dat
+-rw-rw-rw-   0        0        0  2779670 2020-05-06 09:22:05.000000 dans_diffraction-3.2.1/Dans_Diffraction/data/XRayMassAtten_muenp.dat
+-rw-rw-rw-   0        0        0  2779670 2020-05-06 09:22:05.000000 dans_diffraction-3.2.1/Dans_Diffraction/data/XRayMassAtten_mup.dat
+-rw-rw-rw-   0        0        0  1317778 2021-01-21 09:28:34.000000 dans_diffraction-3.2.1/Dans_Diffraction/data/atomic_scattering_factors.npy
+-rw-rw-rw-   0        0        0    43385 2021-06-08 07:44:54.000000 dans_diffraction-3.2.1/Dans_Diffraction/data/f0_WaasKirf.dat
+-rw-rw-rw-   0        0        0    25892 2023-05-06 11:12:54.000000 dans_diffraction-3.2.1/Dans_Diffraction/data/peng.dat
+-rw-rw-rw-   0        0        0   152719 2024-05-18 09:47:05.000000 dans_diffraction-3.2.1/Dans_Diffraction/functions_crystallography.py
+-rw-rw-rw-   0        0        0    48088 2024-05-20 05:50:04.000000 dans_diffraction-3.2.1/Dans_Diffraction/functions_general.py
+-rw-rw-rw-   0        0        0    34608 2024-05-19 06:39:03.000000 dans_diffraction-3.2.1/Dans_Diffraction/functions_plotting.py
+-rw-rw-rw-   0        0        0    44417 2023-05-07 14:24:07.000000 dans_diffraction-3.2.1/Dans_Diffraction/functions_scattering.py
+-rw-rw-rw-   0        0        0    27095 2020-10-15 13:27:33.000000 dans_diffraction-3.2.1/Dans_Diffraction/multiple_scattering.py
+-rw-rw-rw-   0        0        0   192479 2023-01-06 14:04:42.000000 dans_diffraction-3.2.1/Dans_Diffraction/tensor_scattering.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:26:28.754001 dans_diffraction-3.2.1/Dans_Diffraction/tkgui/
+-rw-rw-rw-   0        0        0     1570 2024-03-28 13:17:42.000000 dans_diffraction-3.2.1/Dans_Diffraction/tkgui/__init__.py
+-rw-rw-rw-   0        0        0    14834 2023-07-16 12:26:55.000000 dans_diffraction-3.2.1/Dans_Diffraction/tkgui/basic_widgets.py
+-rw-rw-rw-   0        0        0    16665 2023-10-19 11:03:24.000000 dans_diffraction-3.2.1/Dans_Diffraction/tkgui/converter.py
+-rw-rw-rw-   0        0        0    50929 2024-03-28 16:28:00.000000 dans_diffraction-3.2.1/Dans_Diffraction/tkgui/crystal.py
+-rw-rw-rw-   0        0        0    73139 2023-10-19 09:23:59.000000 dans_diffraction-3.2.1/Dans_Diffraction/tkgui/diffractometer.py
+-rw-rw-rw-   0        0        0    26672 2023-07-20 05:54:00.000000 dans_diffraction-3.2.1/Dans_Diffraction/tkgui/fdmnes.py
+-rw-rw-rw-   0        0        0     9934 2024-03-28 15:58:36.000000 dans_diffraction-3.2.1/Dans_Diffraction/tkgui/multi_crystal.py
+-rw-rw-rw-   0        0        0     7072 2023-07-14 09:21:27.000000 dans_diffraction-3.2.1/Dans_Diffraction/tkgui/multiple_scattering.py
+-rw-rw-rw-   0        0        0    10826 2023-05-16 16:30:28.000000 dans_diffraction-3.2.1/Dans_Diffraction/tkgui/periodic_table.py
+-rw-rw-rw-   0        0        0    30256 2023-08-14 07:29:38.000000 dans_diffraction-3.2.1/Dans_Diffraction/tkgui/properties.py
+-rw-rw-rw-   0        0        0    94783 2024-05-18 09:36:05.000000 dans_diffraction-3.2.1/Dans_Diffraction/tkgui/scattering.py
+-rw-rw-rw-   0        0        0    14775 2023-05-22 06:11:38.000000 dans_diffraction-3.2.1/Dans_Diffraction/tkgui/spacegroups.py
+-rw-rw-rw-   0        0        0    13686 2020-02-20 13:50:35.000000 dans_diffraction-3.2.1/Dans_Diffraction/tkgui/tensor_scattering.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:26:29.094861 dans_diffraction-3.2.1/Dans_Diffraction.egg-info/
+-rw-rw-rw-   0        0        0    28722 2024-05-20 06:26:28.000000 dans_diffraction-3.2.1/Dans_Diffraction.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4448 2024-05-20 06:26:28.000000 dans_diffraction-3.2.1/Dans_Diffraction.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 06:26:28.000000 dans_diffraction-3.2.1/Dans_Diffraction.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2024-05-20 06:26:28.000000 dans_diffraction-3.2.1/Dans_Diffraction.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-05-20 06:26:28.000000 dans_diffraction-3.2.1/Dans_Diffraction.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-20 06:26:28.000000 dans_diffraction-3.2.1/Dans_Diffraction.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2020-04-19 15:46:17.000000 dans_diffraction-3.2.1/LICENSE
+-rw-rw-rw-   0        0        0    28722 2024-05-20 06:26:29.105062 dans_diffraction-3.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    14265 2024-05-20 05:46:18.000000 dans_diffraction-3.2.1/README.md
+-rw-rw-rw-   0        0        0     1528 2024-05-20 06:24:54.000000 dans_diffraction-3.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-20 06:26:29.109740 dans_diffraction-3.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1255 2024-05-20 06:24:54.000000 dans_diffraction-3.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 06:26:29.081891 dans_diffraction-3.2.1/test/
+-rw-rw-rw-   0        0        0     2282 2018-02-13 15:38:28.000000 dans_diffraction-3.2.1/test/test_LS_magnetic_components.py
+-rw-rw-rw-   0        0        0     8939 2021-06-10 16:58:04.000000 dans_diffraction-3.2.1/test/test_WaasKirf_xray_factors.py
+-rw-rw-rw-   0        0        0     2197 2020-04-30 13:31:49.000000 dans_diffraction-3.2.1/test/test_atom_properties.py
+-rw-rw-rw-   0        0        0     1170 2020-05-06 08:27:47.000000 dans_diffraction-3.2.1/test/test_attenuation.py
+-rw-rw-rw-   0        0        0     1910 2021-01-25 17:53:20.000000 dans_diffraction-3.2.1/test/test_attenuation_length.py
+-rw-rw-rw-   0        0        0     2002 2020-11-12 13:20:39.000000 dans_diffraction-3.2.1/test/test_bmatrix.py
+-rw-rw-rw-   0        0        0     1704 2023-08-16 11:18:50.000000 dans_diffraction-3.2.1/test/test_check_append_vs_unique.py
+-rw-rw-rw-   0        0        0     1562 2020-10-19 07:41:46.000000 dans_diffraction-3.2.1/test/test_cif_files.py
+-rw-rw-rw-   0        0        0     6312 2021-07-19 15:51:46.000000 dans_diffraction-3.2.1/test/test_coherent_diffraction.py
+-rw-rw-rw-   0        0        0     3230 2021-07-17 05:26:09.000000 dans_diffraction-3.2.1/test/test_coherent_diffraction2.py
+-rw-rw-rw-   0        0        0     1859 2019-12-12 20:20:59.000000 dans_diffraction-3.2.1/test/test_compare_intensity.py
+-rw-rw-rw-   0        0        0     8480 2020-10-26 14:50:52.000000 dans_diffraction-3.2.1/test/test_compare_intensity_calculation.py
+-rw-rw-rw-   0        0        0     4552 2020-05-12 07:18:31.000000 dans_diffraction-3.2.1/test/test_compound_name.py
+-rw-rw-rw-   0        0        0     2740 2022-03-11 16:54:13.000000 dans_diffraction-3.2.1/test/test_convolve2d.py
+-rw-rw-rw-   0        0        0      289 2020-10-20 19:46:18.000000 dans_diffraction-3.2.1/test/test_detector.py
+-rw-rw-rw-   0        0        0     2902 2020-05-15 15:03:16.000000 dans_diffraction-3.2.1/test/test_electron_density.py
+-rw-rw-rw-   0        0        0     5008 2020-10-19 07:41:46.000000 dans_diffraction-3.2.1/test/test_exchange_path.py
+-rw-rw-rw-   0        0        0     4144 2020-10-19 07:41:46.000000 dans_diffraction-3.2.1/test/test_exchange_path2.py
+-rw-rw-rw-   0        0        0      149 2018-06-08 14:18:49.000000 dans_diffraction-3.2.1/test/test_files.py
+-rw-rw-rw-   0        0        0     5627 2021-07-15 05:41:12.000000 dans_diffraction-3.2.1/test/test_functions_scattering.py
+-rw-rw-rw-   0        0        0     1152 2021-07-15 16:03:30.000000 dans_diffraction-3.2.1/test/test_functions_scattering_dispersion.py
+-rw-rw-rw-   0        0        0     3320 2021-07-14 17:11:38.000000 dans_diffraction-3.2.1/test/test_functions_scattering_new.py
+-rw-rw-rw-   0        0        0     4726 2021-07-13 13:13:30.000000 dans_diffraction-3.2.1/test/test_functions_scattering_pol.py
+-rw-rw-rw-   0        0        0     3102 2021-07-13 14:17:38.000000 dans_diffraction-3.2.1/test/test_functions_scattering_xrm.py
+-rw-rw-rw-   0        0        0     1691 2020-03-27 07:59:19.000000 dans_diffraction-3.2.1/test/test_gaussian.py
+-rw-rw-rw-   0        0        0    17556 2020-06-09 08:44:11.000000 dans_diffraction-3.2.1/test/test_gen_sym_mat.py
+-rw-rw-rw-   0        0        0      256 2020-03-31 13:19:32.000000 dans_diffraction-3.2.1/test/test_gui_multicrystal.py
+-rw-rw-rw-   0        0        0     3193 2020-11-22 19:46:51.000000 dans_diffraction-3.2.1/test/test_i16_azimuth.py
+-rw-rw-rw-   0        0        0      552 2020-03-27 16:10:17.000000 dans_diffraction-3.2.1/test/test_intensity_grid.py
+-rw-rw-rw-   0        0        0     1196 2020-03-27 08:15:40.000000 dans_diffraction-3.2.1/test/test_isincell.py
+-rw-rw-rw-   0        0        0     2536 2021-10-04 20:22:07.000000 dans_diffraction-3.2.1/test/test_laue_backscatter.py
+-rw-rw-rw-   0        0        0     3864 2019-02-22 16:52:35.000000 dans_diffraction-3.2.1/test/test_nonresonant.py
+-rw-rw-rw-   0        0        0     5702 2019-01-21 13:30:00.000000 dans_diffraction-3.2.1/test/test_nonresonant_plot.py
+-rw-rw-rw-   0        0        0     3092 2019-01-21 13:25:46.000000 dans_diffraction-3.2.1/test/test_nonresonant_sergio.py
+-rw-rw-rw-   0        0        0      453 2021-09-26 16:50:06.000000 dans_diffraction-3.2.1/test/test_orientation.py
+-rw-rw-rw-   0        0        0     1044 2017-11-26 15:52:58.000000 dans_diffraction-3.2.1/test/test_parameter_plot.py
+-rw-rw-rw-   0        0        0     4428 2020-11-22 20:40:03.000000 dans_diffraction-3.2.1/test/test_plot_orbitals.py
+-rw-rw-rw-   0        0        0     1956 2017-08-22 12:09:50.000000 dans_diffraction-3.2.1/test/test_plotintensity.py
+-rw-rw-rw-   0        0        0     2890 2017-08-22 15:29:48.000000 dans_diffraction-3.2.1/test/test_plotintensity2.py
+-rw-rw-rw-   0        0        0     2593 2020-05-05 08:27:58.000000 dans_diffraction-3.2.1/test/test_readstfm.py
+-rw-rw-rw-   0        0        0      327 2023-07-19 15:10:57.000000 dans_diffraction-3.2.1/test/test_reflection_selector.py
+-rw-rw-rw-   0        0        0      988 2021-01-26 07:46:04.000000 dans_diffraction-3.2.1/test/test_refractive_index.py
+-rw-rw-rw-   0        0        0     1843 2017-10-30 14:29:08.000000 dans_diffraction-3.2.1/test/test_scattering.py
+-rw-rw-rw-   0        0        0     2649 2017-11-09 11:24:34.000000 dans_diffraction-3.2.1/test/test_supercell.py
+-rw-rw-rw-   0        0        0     9400 2020-06-09 13:06:44.000000 dans_diffraction-3.2.1/test/test_symmetry_ops2magnetic.py
```

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Aluminium.cif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/Aluminium.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/BCC.cif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/BCC.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Beryllium.cif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/Beryllium.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Ca2RuO4.cif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/Ca2RuO4.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Ca3CoMnO6.mcif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/Ca3CoMnO6.mcif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Cobalt.cif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/Cobalt.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Copper.cif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/Copper.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Cubic.cif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/Cubic.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Diamond.cif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/Diamond.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/FCC.cif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/FCC.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Gold.cif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/Gold.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Graphite.cif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/Graphite.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/HCP.cif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/HCP.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Iron.cif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/Iron.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/KCl.cif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/KCl.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/LaMnO3.mcif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/LaMnO3.mcif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/LiCoO2.cif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/LiCoO2.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Na0.8CoO2_P63mmc.cif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/Na0.8CoO2_P63mmc.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/NaCoO2_stripe_supercell.cif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/NaCoO2_stripe_supercell.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Niobium.cif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/Niobium.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Ruby.cif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/Ruby.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Ruthenium.cif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/Ruthenium.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Sapphire.cif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/Sapphire.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Silicon.cif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/Silicon.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Silver.cif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/Silver.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Sr3LiRuO6.cif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/Sr3LiRuO6.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Sr3LiRuO6_C2'c'.mcif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/Sr3LiRuO6_C2'c'.mcif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/Vanadium.cif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/Vanadium.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/Structures/ZnO.cif` & `dans_diffraction-3.2.1/Dans_Diffraction/Structures/ZnO.cif`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/__init__.py` & `dans_diffraction-3.2.1/Dans_Diffraction/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 GitHub Repo: https://github.com/DanPorter/Dans_Diffraction
 Citation DOI: https://doi.org/10.5281/zenodo.8106031
 
 By Dan Porter, PhD
 Diamond
 2017
 
-Version 3.2.0
-Last updated: 19/05/24
+Version 3.2.1
+Last updated: 20/05/24
 
 Version History:
 02/03/18 1.0    Version History started.
 30/05/18 1.1    Fdmnes added
 08/06/18 1.2    Python3 now fully supported
 23/02/19 1.3    Graphical user intrface and magnetic x-ray scattering now implemented
 13/07/19 1.4    FDMNES GUI functionality added
@@ -72,14 +72,15 @@
 20/07/23 3.1.0  Refactored FDMNES wrapper with new methods and new defaults. Thanks YvesJoly!
 26/09/23 3.1.1  Minor changes and improvments. Added hkl1, hkl2 = xtl.scatter.orientation_reflections()
 19/10/23 3.1.2  xray_resonant() now works with non-cubic systems, fixed scaling issue in diffractometer.py
 25/10/23 3.1.3  Fixed error with powder plot for Neutrons. Thanks Cyril!
 28/03/24 3.1.4  Fixed error with site symmetries having spaces in AtomsGui, added Properties.relative_positions()
 10/05/24 3.1.5  Fixed SyntaxWarnings from Unrecognized escape sequences in Python 3.12, various fixes to scattering
 15/05/24 3.2.0  Added "save" and "load" methods to structure factor calculation, improved powder for large calculations
+20/05/24 3.2.1  Added pyproject.toml file for installation, including dansdiffraction script
 
 Acknoledgements:
     2018        Thanks to Hepesu for help with Python3 support and ideas about breaking up calculations
     Dec 2019    Thanks to Gareth Nisbet for allowing me to inlude his multiple scattering siumulation
     April 2020  Thanks to ChunHai Wang for helpful suggestions in readcif!
     May 2020    Thanks to AndreEbel for helpful suggestions on citations
     Dec 2020    Thanks to Chris Drozdowski for suggestions about reflection families
@@ -91,14 +92,15 @@
     Jan 2023    Thanks to Andreas Rosnes for testing the installation in jupyterlab
     May 2023    Thanks to Carmelo Prestipino for adding electron scattering factors
     June 2023   Thanks to Sergio I. Rincon for pointing out the rounding error in Scatter.powder
     July 2023   Thanks to asteppke for suggested update to Arrow3D for matplotlib V>3.4
     July 2023   Thanks to Yves Joly for helpful suggestions on FDMNES wrapper
     Oct 2023    Thanks to asteppke for pointing out scaling issue in diffractometer gui
     Oct 2023    Thanks to Cyril Cayron for pointing out the error with plotting neutron power spectra
+    Jan 2024    Thanks to Carmelo Prestipino for adding search_distance and plot_distance
     May 2024    Thanks to Innbig for spotting some errors in large liquid crystal powder patterns
     May 2024    Thanks to paul-cares pointing out a silly spelling error in the title!
 
 -----------------------------------------------------------------------------
    Copyright 2024 Diamond Light Source Ltd.
 
    Licensed under the Apache License, Version 2.0 (the "License");
@@ -142,16 +144,16 @@
 from .classes_crystal import Crystal
 from .classes_multicrystal import MultiCrystal
 from .classes_structures import Structures
 from .classes_fdmnes import fdmnes_checker, Fdmnes, FdmnesAnalysis
 from .functions_crystallography import readcif
 
 
-__version__ = '3.2.0'
-__date__ = '19/05/24'
+__version__ = '3.2.1'
+__date__ = '20/05/24'
 
 
 # Build
 structure_list = Structures()
 
 
 def version_info():
```

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/__main__.py` & `dans_diffraction-3.2.1/Dans_Diffraction/__main__.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/classes_crystal.py` & `dans_diffraction-3.2.1/Dans_Diffraction/classes_crystal.py`

 * *Files 2% similar despite different names*

```diff
@@ -361,14 +361,104 @@
         """
         try:
             from .tkgui import CrystalGui
             CrystalGui(self)
         except ImportError:
             print('Sorry, you need to install tkinter!')
 
+    def search_distances(self, min_d=0.65, max_d=3.20, c_ele=None, elems=None,
+                         labels=None, simple=True):
+        """
+        Calculated atoms interatomic distances form each label.
+        :param c_ele (list,string): only sites with noted elements
+                                    if None all site
+        :param elems (list,string): only distances with noted elements
+                                    if None all site
+        :param min_d: minimum distance 
+        :param max_d: maximum distance
+        :return dictionary: 
+
+        """
+        xyz = self.Cell.calculateR(self.Atoms.uvw())
+        UVstar = self.Cell.UVstar()
+        UV = self.Cell.UV()
+        Lpar = self.Cell.lp()[:3]
+
+        Lran = np.array([0, 0, 0, 0, 0, 0])
+
+        for i in range(3):
+            Lran[i] = min(fg.distance2plane([0, 0, 0], UVstar[i], xyz))
+        for i in range(3):
+            Lran[3 + i] = min(fg.distance2plane(UV[i], UVstar[i] + UV[i], xyz))
+        for i, L in enumerate(Lran):
+            Lran[i] = np.ceil(max_d / Lpar[i % 3]) if L < max_d else 0
+
+        IntRes = self.Structure.generate_lattice(U=Lran[0] + Lran[3],
+                                                 V=Lran[1] + Lran[4],
+                                                 W=Lran[2] + Lran[5],
+                                                 centred=False)[:3]
+        B_uvw, B_Ele, B_label = IntRes
+        B_label, B_Ele = np.asarray(B_label), np.asarray(B_Ele)
+
+        B_uvw -= np.array(Lran[:3])
+        B_xyz = self.Cell.calculateR(B_uvw)
+
+        if c_ele is None:
+            c_ele = set(self.Atoms.type)
+        elif isinstance(c_ele, str):
+            c_ele = [c_ele]
+
+        if elems is None:
+            elems = set(self.Atoms.type)
+        elif isinstance(elems, str):
+            elems = [elems]
+
+        if labels is None:
+            labels = self.Atoms.label
+        elif isinstance(labels, str):
+            labels = [labels]
+
+        distances = {}
+        for i, atom in enumerate(xyz):
+            if not self.Atoms.type[i] in c_ele:
+                continue
+            if not self.Atoms.label[i] in labels:
+                continue
+            s_dist = {}
+            vdist = (B_xyz - atom) ** 2
+            vdist = np.sqrt(np.sum(vdist, axis=1))
+            cond1 = (vdist > min_d) * (vdist < max_d)
+            vlabel = B_label[cond1]
+            vele = B_Ele[cond1]
+            vdist = vdist[cond1]
+
+            Ord = np.argsort(vdist)
+            cond2 = [ele in elems for ele in vele[Ord]]
+            s_dist = {'dist': vdist[Ord][cond2],
+                      'label': list(vlabel[Ord][cond2]),
+                      'type': list(vele[Ord][cond2])}
+
+            distances[self.Atoms.label[i]] = s_dist
+
+        if simple:
+            # reduce the output for mixed site occupation
+            lab = [i for i,j in zip(self.Atoms.label, self.Atoms.type) if j in c_ele]
+            for i, site_i in enumerate(lab):
+                for site_j in lab[i + 1:]:
+                    uvw_i = self.Atoms[site_i].uvw()
+                    uvw_j = self.Atoms[site_j].uvw()
+                    if all(uvw_i == uvw_j):
+                        lab.remove(site_j)
+                        try:
+                            del distances[site_j]
+                        except KeyError:
+                            pass
+
+        return distances
+
     def __add__(self, other):
         return MultiCrystal([self, other])
 
     def info(self):
         """
         Returns information about the crystal structure
         :return: str
@@ -560,28 +650,27 @@
         return np.dot(HKL, self.UVstar())
 
     def indexQ(self, Q):
         """
         Convert coordinates [x,y,z], in an orthogonal basis, to
         coordinates [h,k,l], in the basis of the reciprocal lattice
                     H(h,k,l) = Q(x,y,z) / [A*,B*,C*]
-        
+
         E.G.
             HKL = indexQ([2.2046264, 1.2728417, 0.0000000]) # for a hexagonal system, a = 2.85
             > HKL = [1,0,0]
         """
         Q = np.reshape(np.asarray(Q, dtype=float), [-1, 3])
         return fc.indx(Q, self.UVstar())
 
     def calculateR(self, UVW):
         """
         Convert coordinates [u,v,w], in the basis of the unit cell, to
         coordinates [x,y,z], in an orthogonal basis, in units of A
                     R(x,y,z) = uA + vB + wC
-        
         E.G.
             R = Cell.calculateR([0.1,0,0]) # for a hexagonal system, a = 2.85
             > R = array([[0.285, 0, 0]])
         """
         UVW = np.reshape(np.asarray(UVW, dtype=float), [-1, 3])
         return np.dot(UVW, self.UV())
 
@@ -1026,14 +1115,16 @@
 
     def __call__(self, u=[0], v=[0], w=[0], type=None,
                  label=None, occupancy=None, uiso=None, mxmymz=None):
         """Re-initialises the class, generating new atomic positions"""
         self.__init__(u, v, w, type, label, occupancy, uiso, mxmymz=None)
 
     def __getitem__(self, idx):
+        if isinstance(idx, str):
+            idx = self.label.index(idx)
         return self.atom(idx)
 
     def fromcif(self, cifvals):
         """
         Import atom parameters from a cif dictionary
         Required cif keys:
             _atom_site_label
```

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/classes_fdmnes.py` & `dans_diffraction-3.2.1/Dans_Diffraction/classes_fdmnes.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/classes_multicrystal.py` & `dans_diffraction-3.2.1/Dans_Diffraction/classes_multicrystal.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/classes_orbitals.py` & `dans_diffraction-3.2.1/Dans_Diffraction/classes_orbitals.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/classes_orientation.py` & `dans_diffraction-3.2.1/Dans_Diffraction/classes_orientation.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/classes_plotting.py` & `dans_diffraction-3.2.1/Dans_Diffraction/classes_plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,51 @@
         ax.set_zlim(-lim/2, lim/2)
         # ax.axis('equal')
         ax.set_axis_off()
         
         plt.legend(fontsize=24, frameon=False)
         
         plt.title(self.xtl.name, fontsize=28, fontweight='bold')
-    
+
+    def plot_distance(self, min_d=0.65, max_d=3.20, labels=None,
+                      c_ele=None, elems=None, ranges=None, step=0.04):
+        """
+        Plot atoms interatomic distances form each label.
+        :param c_ele (list,string): only sites with noted elements
+                                    if None all site
+        :param elems (list,string): only distances with noted elements
+                                    if None all site
+        :param min_d: minimum distance
+        :param max_d: maximum distance
+        :return:
+        """
+        dist = self.xtl.search_distances(c_ele=c_ele, elems=elems,
+                                         labels=labels, min_d=min_d,
+                                         max_d=max_d)
+
+        if ranges is None:
+            all_d = np.hstack([i['dist'] for i in dist.values()])
+            ranges = (np.floor(min(all_d)), np.ceil(max(all_d)))
+        # Create plot
+        if len(dist) == 0:
+            print('no distance present')
+            return
+        fig, axs = plt.subplots(len(dist), constrained_layout=True)
+        if len(dist) == 1:
+            axs = [axs]
+        for i, site in enumerate(dist):
+            axs[i].set_title(site)
+            axs[i].hist(dist[site]['dist'], range=ranges,
+                        bins=int((ranges[1] - ranges[0]) / step))
+            axs[i].set(ylabel='n. Atoms')
+        axs[-1].set(xlabel='$\AA$')
+        if len(dist) > 1:
+            for ax in axs.flat:
+                ax.label_outer()
+
     def plot_layers(self, layers=None, layer_axis=2, layer_width=0.05, show_labels=False):
         """
         Separate the structure into layers along the chosen axis
         and plot the atoms in each layer in a separate figure.
         :param layers: list of layers to plot in fractional coordinates, or NOne for automatic determination
         :param layer_axis: axis (0,1,2) of direction normal to layers
         :param layer_width: distance from layer value to include in plot
```

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/classes_properties.py` & `dans_diffraction-3.2.1/Dans_Diffraction/classes_properties.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/classes_scattering.py` & `dans_diffraction-3.2.1/Dans_Diffraction/classes_scattering.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/classes_structures.py` & `dans_diffraction-3.2.1/Dans_Diffraction/classes_structures.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/data/Dans Element Properties.txt` & `dans_diffraction-3.2.1/Dans_Diffraction/data/Dans Element Properties.txt`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/data/Dans Element Properties_old.txt` & `dans_diffraction-3.2.1/Dans_Diffraction/data/Dans Element Properties_old.txt`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/data/Element_OxidationStates.txt` & `dans_diffraction-3.2.1/Dans_Diffraction/data/Element_OxidationStates.txt`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/data/PointGroups.json` & `dans_diffraction-3.2.1/Dans_Diffraction/data/PointGroups.json`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/data/SpaceGroups.json` & `dans_diffraction-3.2.1/Dans_Diffraction/data/SpaceGroups.json`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/data/SpaceGroupsMagnetic.json` & `dans_diffraction-3.2.1/Dans_Diffraction/data/SpaceGroupsMagnetic.json`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/data/XRayEdges.dat` & `dans_diffraction-3.2.1/Dans_Diffraction/data/XRayEdges.dat`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/data/XRayMassAtten_muenp.dat` & `dans_diffraction-3.2.1/Dans_Diffraction/data/XRayMassAtten_muenp.dat`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/data/XRayMassAtten_mup.dat` & `dans_diffraction-3.2.1/Dans_Diffraction/data/XRayMassAtten_mup.dat`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/data/atomic_scattering_factors.npy` & `dans_diffraction-3.2.1/Dans_Diffraction/data/atomic_scattering_factors.npy`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/data/f0_WaasKirf.dat` & `dans_diffraction-3.2.1/Dans_Diffraction/data/f0_WaasKirf.dat`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/data/peng.dat` & `dans_diffraction-3.2.1/Dans_Diffraction/data/peng.dat`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/functions_crystallography.py` & `dans_diffraction-3.2.1/Dans_Diffraction/functions_crystallography.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/functions_general.py` & `dans_diffraction-3.2.1/Dans_Diffraction/functions_general.py`

 * *Files 1% similar despite different names*

```diff
@@ -493,14 +493,33 @@
     line_diff = line_end - line_start
     unit_line = line_diff / np.sqrt(np.sum(line_diff ** 2))
 
     vec_arb = (line_start - point) - np.dot((line_start - point), unit_line) * unit_line
     return np.sqrt(np.sum(vec_arb ** 2))
 
 
+def distance2plane(line_start, line_end, point):
+    """
+    Calculate distance from a plane (defined by a perpendicular vector) to an arbitary point in space
+    :param vector_start: array, position lying on plane and vector start
+    :param line_end:  array, position of the end of the vector
+    :param point: array, arbitary position in space
+    :return: float
+    """
+    line_start = np.asarray(line_start)
+    line_end = np.asarray(line_end)
+    point = np.asarray(point)
+
+    line_diff = line_end - line_start
+    unit_line = line_diff / np.sqrt(np.sum(line_diff ** 2))
+
+    vec_arb = np.dot((point - line_start), unit_line)
+    return abs(vec_arb)
+
+
 def vector_intersection(point1, direction1, point2, direction2):
     """
     Calculate the point in 2D where two lines cross.
     If lines are parallel, return nan
     For derivation, see: http://paulbourke.net/geometry/pointlineplane/
     :param point1: [x,y] some coordinate on line 1
     :param direction1: [dx, dy] the direction of line 1
```

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/functions_plotting.py` & `dans_diffraction-3.2.1/Dans_Diffraction/functions_plotting.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/functions_scattering.py` & `dans_diffraction-3.2.1/Dans_Diffraction/functions_scattering.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/multiple_scattering.py` & `dans_diffraction-3.2.1/Dans_Diffraction/multiple_scattering.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/tensor_scattering.py` & `dans_diffraction-3.2.1/Dans_Diffraction/tensor_scattering.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/__init__.py` & `dans_diffraction-3.2.1/Dans_Diffraction/tkgui/__init__.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/basic_widgets.py` & `dans_diffraction-3.2.1/Dans_Diffraction/tkgui/basic_widgets.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/converter.py` & `dans_diffraction-3.2.1/Dans_Diffraction/tkgui/converter.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/crystal.py` & `dans_diffraction-3.2.1/Dans_Diffraction/tkgui/crystal.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/diffractometer.py` & `dans_diffraction-3.2.1/Dans_Diffraction/tkgui/diffractometer.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/fdmnes.py` & `dans_diffraction-3.2.1/Dans_Diffraction/tkgui/fdmnes.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/multi_crystal.py` & `dans_diffraction-3.2.1/Dans_Diffraction/tkgui/multi_crystal.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/multiple_scattering.py` & `dans_diffraction-3.2.1/Dans_Diffraction/tkgui/multiple_scattering.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/periodic_table.py` & `dans_diffraction-3.2.1/Dans_Diffraction/tkgui/periodic_table.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/properties.py` & `dans_diffraction-3.2.1/Dans_Diffraction/tkgui/properties.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/scattering.py` & `dans_diffraction-3.2.1/Dans_Diffraction/tkgui/scattering.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/spacegroups.py` & `dans_diffraction-3.2.1/Dans_Diffraction/tkgui/spacegroups.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction/tkgui/tensor_scattering.py` & `dans_diffraction-3.2.1/Dans_Diffraction/tkgui/tensor_scattering.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction.egg-info/PKG-INFO` & `dans_diffraction-3.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,14 @@
-Metadata-Version: 2.1
-Name: Dans-Diffraction
-Version: 3.2.0
-Summary: Generate diffracted intensities from crystals
-Home-page: https://github.com/DanPorter/Dans_Diffraction
-Author: Dan Porter
-Author-email: d.g.porter@outlook.com
-Keywords: crystal,cif,diffraction,crystallography,science,x-ray,neutron,resonant,magnetic,magnetism,multiple scattering,fdmnes,super structure,spacegroup,space group,diffractometer
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Development Status :: 3 - Alpha
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: matplotlib
-
 # Dans_Diffraction
 Reads crystallographic cif files, calculates crystal properties and simulates diffraction.
 
 **Version 3.2**
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8106031.svg)](https://doi.org/10.5281/zenodo.8106031)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/DanPorter/Dans_Diffraction/6be78ef800167276d61d3e73da3b74a8367dbbe7?urlpath=lab%2Ftree%2FDans_Diffraction.ipynb) 
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/DanPorter/Dans_Diffraction/master?labpath=Dans_Diffraction.ipynb) 
 [![](https://img.shields.io/github/forks/DanPorter/Dans_Diffraction?label=GitHub%20Repo&style=social)](https://github.com/DanPorter/Dans_Diffraction)
 
 
 By Dan Porter, Diamond Light Source
 2024
 
 #### TL;DR:
@@ -51,15 +33,15 @@
 
 # Start graphical user interface:
 xtl.start_gui()
 ```
 
 Full code documentation available [here](https://danporter.github.io/Dans_Diffraction/).
 
-Try it out on [mybinder!](https://mybinder.org/v2/gh/DanPorter/Dans_Diffraction/6be78ef800167276d61d3e73da3b74a8367dbbe7?urlpath=lab%2Ftree%2FDans_Diffraction.ipynb)
+Try it out on [mybinder!](https://mybinder.org/v2/gh/DanPorter/Dans_Diffraction/master?labpath=Dans_Diffraction.ipynb)
 
 For comments, queries or bugs - email [dan.porter@diamond.ac.uk](mailto:dan.porter@diamond.ac.uk)
 
 **Citation:** If you use this code (great!), please cite the published DOI: [10.5281/zenodo.8106031](https://doi.org/10.5281/zenodo.8106031)
 
 # Installation
 **Requirements:** 
@@ -75,20 +57,26 @@
 ```text
 $ python -m pip install git+https://github.com/DanPorter/Dans_Diffraction.git
 ```
 
 Or, Download the latest version from GitHub (with examples!):
 ```text
 $ git clone https://github.com/DanPorter/Dans_Diffraction.git
+$ cd Dans_Diffraction
+$ python -m pip install .
 ```
 
 
 
 # Operation
-Dans_Diffraction is best run within an interactive python environment:
+From version 3.2, installing Dans_Diffraction will include a run script for the gui:
+```text
+$ dansdiffraction
+```
+Alternatively, Dans_Diffraction is best run within an interactive python environment:
 ```text
 $ ipython -i -m Dans_Diffraction
 ```
 
 Dans_Diffraction can also be run in scripts as an import, example scripts are provided in the [Examples](https://github.com/DanPorter/Dans_Diffraction/blob/master/Examples) folder.
 ### Read CIF file
 ```python
@@ -273,33 +261,34 @@
 Once activated, FDMNES GUI elements become available from the main window, emulating functionality of the classes.
 
 ![FDMNES Run](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/GUI_08.png?raw=true)
 ![FDMNES Analyse](https://github.com/DanPorter/Dans_Diffraction/blob/master/Screenshots/GUI_09.png?raw=true)
 
 
 # Acknoledgements
-| Date       | Thanks to...                                                                            |
-|------------|-----------------------------------------------------------------------------------------|
-| 2018       | Thanks to Hepesu for help with Python3 support and ideas about breaking up calculations |
-| Dec 2019   | Thanks to Gareth Nisbet for allowing me to inlude his multiple scattering siumulation   |
-| April 2020 | Thanks to ChunHai Wang for helpful suggestions in readcif!                              |
-| May 2020   | Thanks to AndreEbel for helpful suggestions on citations                                |
-| Dec 2020   | Thanks to Chris Drozdowski for suggestions about reflection families                    |
-| Jan 2021   | Thanks to aslarsen for suggestions about outputting the structure factor                |
-| April 2021 | Thanks to Trygve RÃ¦der for suggestions about x-ray scattering factors                   |
-| Feb 2022   | Thanks to Mirko for pointing out the error in two-theta values in Scatter.powder        |
-| March 2022 | Thanks to yevgenyr for suggesting new peak profiles in Scatter.powder                   |
-| Jan 2023   | Thanks to Anuradha Vibhakar for pointing out the error in f0 + if'-if''                 |
-| Jan 2023   | Thanks to Andreas Rosnes for testing the installation in jupyterlab                     |
-| May 2023   | Thanks to Carmelo Prestipino for adding electron scattering factors                     |
-| June 2023  | Thanks to Sergio I. Rincon for pointing out the rounding error in Scatter.powder        |
-| July 2023  | Thanks to asteppke for suggested update to Arrow3D for matplotlib V>3.4                 |
-| July 2023  | Thanks to Yves Joly for helpful suggestions on FDMNES wrapper                           |
-| April 2024 | Thanks to Innbig for pointing out an issue with liquid crystal simulations              |
-| May 2024   | Thanks to paul-cares pointing out a silly spelling error in the title!                  |
+| Date        | Thanks to...                                                                            |
+|-------------|-----------------------------------------------------------------------------------------|
+| 2018        | Thanks to Hepesu for help with Python3 support and ideas about breaking up calculations |
+| Dec 2019    | Thanks to Gareth Nisbet for allowing me to inlude his multiple scattering siumulation   |
+| April 2020  | Thanks to ChunHai Wang for helpful suggestions in readcif!                              |
+| May 2020    | Thanks to AndreEbel for helpful suggestions on citations                                |
+| Dec 2020    | Thanks to Chris Drozdowski for suggestions about reflection families                    |
+| Jan 2021    | Thanks to aslarsen for suggestions about outputting the structure factor                |
+| April 2021  | Thanks to Trygve Ræder for suggestions about x-ray scattering factors                   |
+| Feb 2022    | Thanks to Mirko for pointing out the error in two-theta values in Scatter.powder        |
+| March 2022  | Thanks to yevgenyr for suggesting new peak profiles in Scatter.powder                   |
+| Jan 2023    | Thanks to Anuradha Vibhakar for pointing out the error in f0 + if'-if''                 |
+| Jan 2023    | Thanks to Andreas Rosnes for testing the installation in jupyterlab                     |
+| May 2023    | Thanks to Carmelo Prestipino for adding electron scattering factors                     |
+| June 2023   | Thanks to Sergio I. Rincon for pointing out the rounding error in Scatter.powder        |
+| July 2023   | Thanks to asteppke for suggested update to Arrow3D for matplotlib V>3.4                 |
+| July 2023   | Thanks to Yves Joly for helpful suggestions on FDMNES wrapper                           |
+| Jan 2024    | Thanks to Carmelo Prestipino for adding search_distance and plot_distance               | 
+| April 2024  | Thanks to Innbig for pointing out an issue with liquid crystal simulations              |
+| May 2024    | Thanks to paul-cares pointing out a silly spelling error in the title!                  |
 
 Copyright
 -----------------------------------------------------------------------------
    Copyright 2024 Diamond Light Source Ltd.
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
```

### Comparing `Dans_Diffraction-3.2.0/Dans_Diffraction.egg-info/SOURCES.txt` & `dans_diffraction-3.2.1/Dans_Diffraction.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+pyproject.toml
 setup.py
 Dans_Diffraction/__init__.py
 Dans_Diffraction/__main__.py
 Dans_Diffraction/classes_crystal.py
 Dans_Diffraction/classes_fdmnes.py
 Dans_Diffraction/classes_multicrystal.py
 Dans_Diffraction/classes_orbitals.py
@@ -17,14 +18,15 @@
 Dans_Diffraction/functions_plotting.py
 Dans_Diffraction/functions_scattering.py
 Dans_Diffraction/multiple_scattering.py
 Dans_Diffraction/tensor_scattering.py
 Dans_Diffraction.egg-info/PKG-INFO
 Dans_Diffraction.egg-info/SOURCES.txt
 Dans_Diffraction.egg-info/dependency_links.txt
+Dans_Diffraction.egg-info/entry_points.txt
 Dans_Diffraction.egg-info/requires.txt
 Dans_Diffraction.egg-info/top_level.txt
 Dans_Diffraction/Structures/Aluminium.cif
 Dans_Diffraction/Structures/BCC.cif
 Dans_Diffraction/Structures/Beryllium.cif
 Dans_Diffraction/Structures/Ca2RuO4.cif
 Dans_Diffraction/Structures/Ca3CoMnO6.mcif
```

### Comparing `Dans_Diffraction-3.2.0/LICENSE` & `dans_diffraction-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/setup.py` & `dans_diffraction-3.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.md') as f:
         return f.read()
 
 
 setup(
     name='Dans_Diffraction',
     packages=['Dans_Diffraction', 'Dans_Diffraction.tkgui'],
-    version='3.2.0',
+    version='3.2.1',
     description='Generate diffracted intensities from crystals',
     long_description_content_type='text/markdown',
     long_description=readme(),
     author='Dan Porter',
     author_email='d.g.porter@outlook.com',
     url='https://github.com/DanPorter/Dans_Diffraction',
     keywords=[
```

### Comparing `Dans_Diffraction-3.2.0/test/test_LS_magnetic_components.py` & `dans_diffraction-3.2.1/test/test_LS_magnetic_components.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_WaasKirf_xray_factors.py` & `dans_diffraction-3.2.1/test/test_WaasKirf_xray_factors.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_atom_properties.py` & `dans_diffraction-3.2.1/test/test_atom_properties.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_attenuation.py` & `dans_diffraction-3.2.1/test/test_attenuation.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_attenuation_length.py` & `dans_diffraction-3.2.1/test/test_attenuation_length.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_bmatrix.py` & `dans_diffraction-3.2.1/test/test_bmatrix.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_check_append_vs_unique.py` & `dans_diffraction-3.2.1/test/test_check_append_vs_unique.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_cif_files.py` & `dans_diffraction-3.2.1/test/test_cif_files.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_coherent_diffraction.py` & `dans_diffraction-3.2.1/test/test_coherent_diffraction.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_coherent_diffraction2.py` & `dans_diffraction-3.2.1/test/test_coherent_diffraction2.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_compare_intensity.py` & `dans_diffraction-3.2.1/test/test_compare_intensity.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_compare_intensity_calculation.py` & `dans_diffraction-3.2.1/test/test_compare_intensity_calculation.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_compound_name.py` & `dans_diffraction-3.2.1/test/test_compound_name.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_convolve2d.py` & `dans_diffraction-3.2.1/test/test_convolve2d.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_electron_density.py` & `dans_diffraction-3.2.1/test/test_electron_density.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_exchange_path.py` & `dans_diffraction-3.2.1/test/test_exchange_path.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_exchange_path2.py` & `dans_diffraction-3.2.1/test/test_exchange_path2.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_functions_scattering.py` & `dans_diffraction-3.2.1/test/test_functions_scattering.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_functions_scattering_dispersion.py` & `dans_diffraction-3.2.1/test/test_functions_scattering_dispersion.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_functions_scattering_new.py` & `dans_diffraction-3.2.1/test/test_functions_scattering_new.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_functions_scattering_pol.py` & `dans_diffraction-3.2.1/test/test_functions_scattering_pol.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_functions_scattering_xrm.py` & `dans_diffraction-3.2.1/test/test_functions_scattering_xrm.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_gaussian.py` & `dans_diffraction-3.2.1/test/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_gen_sym_mat.py` & `dans_diffraction-3.2.1/test/test_gen_sym_mat.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_i16_azimuth.py` & `dans_diffraction-3.2.1/test/test_i16_azimuth.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_intensity_grid.py` & `dans_diffraction-3.2.1/test/test_intensity_grid.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_isincell.py` & `dans_diffraction-3.2.1/test/test_isincell.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_laue_backscatter.py` & `dans_diffraction-3.2.1/test/test_laue_backscatter.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_nonresonant.py` & `dans_diffraction-3.2.1/test/test_nonresonant.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_nonresonant_plot.py` & `dans_diffraction-3.2.1/test/test_nonresonant_plot.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_nonresonant_sergio.py` & `dans_diffraction-3.2.1/test/test_nonresonant_sergio.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_parameter_plot.py` & `dans_diffraction-3.2.1/test/test_parameter_plot.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_plot_orbitals.py` & `dans_diffraction-3.2.1/test/test_plot_orbitals.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_plotintensity.py` & `dans_diffraction-3.2.1/test/test_plotintensity.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_plotintensity2.py` & `dans_diffraction-3.2.1/test/test_plotintensity2.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_readstfm.py` & `dans_diffraction-3.2.1/test/test_readstfm.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_refractive_index.py` & `dans_diffraction-3.2.1/test/test_refractive_index.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_scattering.py` & `dans_diffraction-3.2.1/test/test_scattering.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_supercell.py` & `dans_diffraction-3.2.1/test/test_supercell.py`

 * *Files identical despite different names*

### Comparing `Dans_Diffraction-3.2.0/test/test_symmetry_ops2magnetic.py` & `dans_diffraction-3.2.1/test/test_symmetry_ops2magnetic.py`

 * *Files identical despite different names*

