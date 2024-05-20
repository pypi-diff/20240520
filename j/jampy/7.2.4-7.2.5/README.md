# Comparing `tmp/jampy-7.2.4.tar.gz` & `tmp/jampy-7.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jampy-7.2.4.tar", last modified: Wed Jan 10 11:09:03 2024, max compression
+gzip compressed data, was "jampy-7.2.5.tar", last modified: Mon May 20 10:28:46 2024, max compression
```

## Comparing `jampy-7.2.4.tar` & `jampy-7.2.5.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-01-10 11:09:03.388464 jampy-7.2.4/
--rw-rw-rw-   0        0        0    53355 2024-01-10 11:09:03.388464 jampy-7.2.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-01-10 11:09:03.325365 jampy-7.2.4/jampy/
--rw-rw-rw-   0        0        0    15455 2024-01-10 11:08:33.000000 jampy-7.2.4/jampy/CHANGELOG.rst
--rw-rw-rw-   0        0        0      398 2024-01-10 10:22:16.000000 jampy-7.2.4/jampy/LICENSE.txt
--rw-rw-rw-   0        0        0     3564 2022-10-02 22:25:04.000000 jampy-7.2.4/jampy/README.rst
--rw-rw-rw-   0        0        0       23 2024-01-10 11:08:57.000000 jampy-7.2.4/jampy/__init__.py
--rw-rw-rw-   0        0        0     3589 2023-11-10 13:44:59.000000 jampy-7.2.4/jampy/cosmology_distance.py
-drwxrwxrwx   0        0        0        0 2024-01-10 11:09:03.388464 jampy-7.2.4/jampy/examples/
--rw-rw-rw-   0        0        0       36 2018-04-16 16:12:03.000000 jampy-7.2.4/jampy/examples/__init__.py
--rw-rw-rw-   0        0        0     1019 2022-02-07 11:29:21.000000 jampy-7.2.4/jampy/examples/cappellari2020_table1.txt
--rw-rw-rw-   0        0        0     3092 2023-11-21 10:16:53.000000 jampy-7.2.4/jampy/examples/jam_axi_intr_example.py
--rw-rw-rw-   0        0        0     4524 2023-09-26 12:17:37.000000 jampy-7.2.4/jampy/examples/jam_axi_proj_example.py
--rw-rw-rw-   0        0        0     6951 2023-11-21 10:13:37.000000 jampy-7.2.4/jampy/examples/jam_black_hole_bayes_example.py
--rw-rw-rw-   0        0        0    10335 2023-11-21 10:14:24.000000 jampy-7.2.4/jampy/examples/jam_dark_halo_bayes_example.py
--rw-rw-rw-   0        0        0    10260 2023-10-26 10:27:06.000000 jampy-7.2.4/jampy/examples/jam_hernquist_model_example.py
--rw-rw-rw-   0        0        0     8544 2018-05-01 13:45:20.000000 jampy-7.2.4/jampy/examples/jam_mock_kinematics_black_hole.txt
--rw-rw-rw-   0        0        0     8592 2021-12-21 19:35:32.000000 jampy-7.2.4/jampy/examples/jam_mock_kinematics_dark_halo.txt
--rw-rw-rw-   0        0        0     2592 2023-10-03 08:02:30.000000 jampy-7.2.4/jampy/examples/jam_sph_proj_example.py
--rw-rw-rw-   0        0        0     2251 2023-11-30 14:21:13.000000 jampy-7.2.4/jampy/examples/mge_vcirc_example.py
--rw-rw-rw-   0        0        0    36000 2023-12-06 21:30:23.000000 jampy-7.2.4/jampy/jam_axi_intr.py
--rw-rw-rw-   0        0        0    48843 2024-01-10 10:52:03.000000 jampy-7.2.4/jampy/jam_axi_proj.py
--rw-rw-rw-   0        0        0    11772 2024-01-10 11:05:56.000000 jampy-7.2.4/jampy/jam_axi_sersic.py
--rw-rw-rw-   0        0        0     8141 2023-05-31 18:20:50.000000 jampy-7.2.4/jampy/jam_sph_intr.py
--rw-rw-rw-   0        0        0    29191 2023-10-28 17:33:46.000000 jampy-7.2.4/jampy/jam_sph_proj.py
--rw-rw-rw-   0        0        0     6549 2023-09-26 18:06:21.000000 jampy-7.2.4/jampy/mge_half_light_isophote.py
--rw-rw-rw-   0        0        0     3568 2019-10-24 18:03:59.000000 jampy-7.2.4/jampy/mge_radial_density.py
--rw-rw-rw-   0        0        0     3166 2023-07-30 10:13:08.000000 jampy-7.2.4/jampy/mge_radial_mass.py
--rw-rw-rw-   0        0        0     7036 2023-11-30 14:22:33.000000 jampy-7.2.4/jampy/mge_vcirc.py
--rw-rw-rw-   0        0        0    19470 2023-06-13 12:02:24.000000 jampy-7.2.4/jampy/quad1d.py
--rw-rw-rw-   0        0        0    13058 2023-07-22 09:58:07.000000 jampy-7.2.4/jampy/quad2d.py
-drwxrwxrwx   0        0        0        0 2024-01-10 11:09:03.372810 jampy-7.2.4/jampy.egg-info/
--rw-rw-rw-   0        0        0    53355 2024-01-10 11:09:02.000000 jampy-7.2.4/jampy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      985 2024-01-10 11:09:02.000000 jampy-7.2.4/jampy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-10 11:09:02.000000 jampy-7.2.4/jampy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-01-10 11:09:02.000000 jampy-7.2.4/jampy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-01-10 11:09:02.000000 jampy-7.2.4/jampy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-01-10 11:09:02.000000 jampy-7.2.4/jampy.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-01-10 11:09:03.388464 jampy-7.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1750 2021-06-24 13:30:54.000000 jampy-7.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:28:46.166280 jampy-7.2.5/
+-rw-rw-rw-   0        0        0    53631 2024-05-20 10:28:46.166280 jampy-7.2.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 10:28:45.891385 jampy-7.2.5/jampy/
+-rw-rw-rw-   0        0        0    15724 2024-05-20 10:28:08.000000 jampy-7.2.5/jampy/CHANGELOG.rst
+-rw-rw-rw-   0        0        0      398 2024-01-10 10:22:16.000000 jampy-7.2.5/jampy/LICENSE.txt
+-rw-rw-rw-   0        0        0     3564 2022-10-02 22:25:04.000000 jampy-7.2.5/jampy/README.rst
+-rw-rw-rw-   0        0        0       23 2024-05-20 10:28:26.000000 jampy-7.2.5/jampy/__init__.py
+-rw-rw-rw-   0        0        0     3589 2023-11-10 13:44:59.000000 jampy-7.2.5/jampy/cosmology_distance.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:28:46.166280 jampy-7.2.5/jampy/examples/
+-rw-rw-rw-   0        0        0       36 2018-04-16 16:12:03.000000 jampy-7.2.5/jampy/examples/__init__.py
+-rw-rw-rw-   0        0        0     1019 2022-02-07 11:29:21.000000 jampy-7.2.5/jampy/examples/cappellari2020_table1.txt
+-rw-rw-rw-   0        0        0     3092 2023-11-21 10:16:53.000000 jampy-7.2.5/jampy/examples/jam_axi_intr_example.py
+-rw-rw-rw-   0        0        0     4523 2024-05-02 21:39:16.000000 jampy-7.2.5/jampy/examples/jam_axi_proj_example.py
+-rw-rw-rw-   0        0        0     6951 2023-11-21 10:13:37.000000 jampy-7.2.5/jampy/examples/jam_black_hole_bayes_example.py
+-rw-rw-rw-   0        0        0    10335 2024-01-30 09:15:51.000000 jampy-7.2.5/jampy/examples/jam_dark_halo_bayes_example.py
+-rw-rw-rw-   0        0        0    10260 2023-10-26 10:27:06.000000 jampy-7.2.5/jampy/examples/jam_hernquist_model_example.py
+-rw-rw-rw-   0        0        0     8544 2018-05-01 13:45:20.000000 jampy-7.2.5/jampy/examples/jam_mock_kinematics_black_hole.txt
+-rw-rw-rw-   0        0        0     8592 2021-12-21 19:35:32.000000 jampy-7.2.5/jampy/examples/jam_mock_kinematics_dark_halo.txt
+-rw-rw-rw-   0        0        0     2592 2023-10-03 08:02:30.000000 jampy-7.2.5/jampy/examples/jam_sph_proj_example.py
+-rw-rw-rw-   0        0        0     2251 2024-04-24 12:40:59.000000 jampy-7.2.5/jampy/examples/mge_vcirc_example.py
+-rw-rw-rw-   0        0        0    36002 2024-05-03 13:51:05.000000 jampy-7.2.5/jampy/jam_axi_intr.py
+-rw-rw-rw-   0        0        0    49265 2024-05-03 13:50:52.000000 jampy-7.2.5/jampy/jam_axi_proj.py
+-rw-rw-rw-   0        0        0    11883 2024-01-11 18:06:12.000000 jampy-7.2.5/jampy/jam_axi_sersic.py
+-rw-rw-rw-   0        0        0     8204 2024-02-08 15:57:21.000000 jampy-7.2.5/jampy/jam_sph_intr.py
+-rw-rw-rw-   0        0        0    29329 2024-02-08 16:52:45.000000 jampy-7.2.5/jampy/jam_sph_proj.py
+-rw-rw-rw-   0        0        0     2957 2024-04-04 17:44:48.000000 jampy-7.2.5/jampy/mge_cylindrical_mass.py
+-rw-rw-rw-   0        0        0     6612 2024-04-04 16:08:33.000000 jampy-7.2.5/jampy/mge_half_light_isophote.py
+-rw-rw-rw-   0        0        0     3635 2024-04-04 16:08:46.000000 jampy-7.2.5/jampy/mge_radial_density.py
+-rw-rw-rw-   0        0        0     3233 2024-04-04 16:09:03.000000 jampy-7.2.5/jampy/mge_radial_mass.py
+-rw-rw-rw-   0        0        0     7097 2024-04-04 16:09:33.000000 jampy-7.2.5/jampy/mge_vcirc.py
+-rw-rw-rw-   0        0        0    19563 2024-02-21 19:29:58.000000 jampy-7.2.5/jampy/quad1d.py
+-rw-rw-rw-   0        0        0    13131 2024-04-05 11:10:48.000000 jampy-7.2.5/jampy/quad2d.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:28:46.166280 jampy-7.2.5/jampy.egg-info/
+-rw-rw-rw-   0        0        0    53631 2024-05-20 10:28:45.000000 jampy-7.2.5/jampy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1015 2024-05-20 10:28:45.000000 jampy-7.2.5/jampy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 10:28:45.000000 jampy-7.2.5/jampy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-20 10:28:45.000000 jampy-7.2.5/jampy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-20 10:28:45.000000 jampy-7.2.5/jampy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-05-20 10:28:45.000000 jampy-7.2.5/jampy.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-05-20 10:28:46.166280 jampy-7.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1750 2021-06-24 13:30:54.000000 jampy-7.2.5/setup.py
```

### Comparing `jampy-7.2.4/PKG-INFO` & `jampy-7.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jampy
-Version: 7.2.4
+Version: 7.2.5
 Summary: JamPy: Jeans Anisotropic Models for Galactic Dynamics
 Home-page: https://purl.org/cappellari/software
 Author: Michele Cappellari
 Author-email: michele.cappellari@physics.ox.ac.uk
 License: Other/Proprietary License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -810,14 +810,21 @@
 redistribute the code.
 
 ###########################################################################
 
 Changelog
 ---------
 
+V7.2.5: MC, Oxford 20 May 2024
+++++++++++++++++++++++++++++++
+
+- ``quad1d`` and ``quad2d``: Require positive values for either ``epsrel`` or
+  ``epsabs`` keywords. Thanks to Carlos Melo (cufrgs.br) for the feedback.
+- ``jam_axi_proj``: Dropped support for Python 3.9.
+
 V7.2.4: MC, Oxford, 10 January 2024
 +++++++++++++++++++++++++++++++++++
 
 - ``jam_axi_proj``: Support prolate models with ``qobs_lum > 1`` or 
   ``qobs_pot > 1``.
 - ``jam_axi_proj``: Output unconvolved surface brightness ``jam.flux`` when no
   PSF/aperture convolution is applied to the kinematics, due to zero
```

### Comparing `jampy-7.2.4/jampy/CHANGELOG.rst` & `jampy-7.2.5/jampy/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 
 Changelog
 ---------
 
+V7.2.5: MC, Oxford 20 May 2024
+++++++++++++++++++++++++++++++
+
+- ``quad1d`` and ``quad2d``: Require positive values for either ``epsrel`` or
+  ``epsabs`` keywords. Thanks to Carlos Melo (cufrgs.br) for the feedback.
+- ``jam_axi_proj``: Dropped support for Python 3.9.
+
 V7.2.4: MC, Oxford, 10 January 2024
 +++++++++++++++++++++++++++++++++++
 
 - ``jam_axi_proj``: Support prolate models with ``qobs_lum > 1`` or 
   ``qobs_pot > 1``.
 - ``jam_axi_proj``: Output unconvolved surface brightness ``jam.flux`` when no
   PSF/aperture convolution is applied to the kinematics, due to zero
```

### Comparing `jampy-7.2.4/jampy/README.rst` & `jampy-7.2.5/jampy/README.rst`

 * *Files identical despite different names*

### Comparing `jampy-7.2.4/jampy/cosmology_distance.py` & `jampy-7.2.5/jampy/cosmology_distance.py`

 * *Files identical despite different names*

### Comparing `jampy-7.2.4/jampy/examples/cappellari2020_table1.txt` & `jampy-7.2.5/jampy/examples/cappellari2020_table1.txt`

 * *Files identical despite different names*

### Comparing `jampy-7.2.4/jampy/examples/jam_axi_intr_example.py` & `jampy-7.2.5/jampy/examples/jam_axi_intr_example.py`

 * *Files identical despite different names*

### Comparing `jampy-7.2.4/jampy/examples/jam_axi_proj_example.py` & `jampy-7.2.5/jampy/examples/jam_axi_proj_example.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     # See jam_dark_halo_bayes_example.py and e.g. Cappellari (2013) for an example
     # https://ui.adsabs.harvard.edu/abs/2013MNRAS.432.1709C
 
     surf_lum = surf_pot = surf
     sigma_lum = sigma_pot = sigma
     qobs_lum = qobs_pot = qobs
 
-    sigmapsf =  [0.6, 1.2]
+    sigmapsf = [0.6, 1.2]
     normpsf = [0.7, 0.3]
     pixsize = 0.8
     goodbins = r > 10  # Arbitrarily exclude the center to illustrate how to use goodbins
 
     # I use a loop below, just to highlight the fact that all parameters
     # remain the same for the two JAM calls, except for 'moment' and 'data'
     plt.figure(1)
```

### Comparing `jampy-7.2.4/jampy/examples/jam_black_hole_bayes_example.py` & `jampy-7.2.5/jampy/examples/jam_black_hole_bayes_example.py`

 * *Files identical despite different names*

### Comparing `jampy-7.2.4/jampy/examples/jam_dark_halo_bayes_example.py` & `jampy-7.2.5/jampy/examples/jam_dark_halo_bayes_example.py`

 * *Files identical despite different names*

### Comparing `jampy-7.2.4/jampy/examples/jam_hernquist_model_example.py` & `jampy-7.2.5/jampy/examples/jam_hernquist_model_example.py`

 * *Files identical despite different names*

### Comparing `jampy-7.2.4/jampy/examples/jam_mock_kinematics_black_hole.txt` & `jampy-7.2.5/jampy/examples/jam_mock_kinematics_black_hole.txt`

 * *Files identical despite different names*

### Comparing `jampy-7.2.4/jampy/examples/jam_mock_kinematics_dark_halo.txt` & `jampy-7.2.5/jampy/examples/jam_mock_kinematics_dark_halo.txt`

 * *Files identical despite different names*

### Comparing `jampy-7.2.4/jampy/examples/jam_sph_proj_example.py` & `jampy-7.2.5/jampy/examples/jam_sph_proj_example.py`

 * *Files identical despite different names*

### Comparing `jampy-7.2.4/jampy/examples/mge_vcirc_example.py` & `jampy-7.2.5/jampy/examples/mge_vcirc_example.py`

 * *Files identical despite different names*

### Comparing `jampy-7.2.4/jampy/jam_axi_intr.py` & `jampy-7.2.5/jampy/jam_axi_intr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-    Copyright (C) 2019-2023, Michele Cappellari
+    Copyright (C) 2019-2024, Michele Cappellari
 
     E-mail: michele.cappellari_at_physics.ox.ac.uk
 
     Updated versions of the software are available from my web page
     https://purl.org/cappellari/software
 
     This software is provided as is without any warranty whatsoever.
@@ -162,15 +162,15 @@
         beta = (beta0 + betainf*(abs(z)/zab)**alpha)/(1 + (abs(z)/zab)**alpha)
         zag, gamma0, gammainf, alpha = gamma
         gamma = (gamma0 + gammainf*(abs(z)/zag)**alpha)/(1 + (abs(z)/zag)**alpha)
     else:
         if not np.ptp(beta): beta = beta[0]
         if not np.ptp(gamma): gamma = gamma[0]
 
-    if mbh > 0:
+    if mbh > 0:  
         mom += intrinsic_moments_cyl_bh(
             R, z, dens_lum, sigma_lum, qintr_lum, mbh, beta, gamma, all_mom)
 
     if all_mom:
         sig2z, v2phi, sig2R, sig2phi = mom
     else:
         sig2z, v2phi = mom
```

### Comparing `jampy-7.2.4/jampy/jam_axi_proj.py` & `jampy-7.2.5/jampy/jam_axi_proj.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-    Copyright (C) 2019-2023, Michele Cappellari
+    Copyright (C) 2019-2024, Michele Cappellari
 
     E-mail: michele.cappellari_at_physics.ox.ac.uk
 
     Updated versions of the software are available from my web page
     http://purl.org/cappellari/software
 
     This software is provided as is without any warranty whatsoever.
@@ -81,26 +81,27 @@
     # The triple loop in (j, k, u) is replaced by broadcast Numpy array operations.
     e2u2_pot = e2_pot*u2
     a = 0.5*(u2/s2_pot + 1/s2_lum)               # equation (29) in C08
     b = 0.5*(e2u2_pot*u2/(s2_pot*(1 - e2u2_pot)) + e2_lum/s2q2_lum) # equation (30) in C08
     c = e2_pot - s2q2_lum/s2_pot                  # equation (22) in C08
     d = 1 - kani*q2_lum - ((1 - kani)*c + e2_pot*kani)*u2  # equation (23) in C08
     e = a + b*ci2
-    if tensor == 'xx':
-        f = kani*s2q2_lum + d*((y1*ci*(a+b)/e)**2 + si2/(2*e)) # equation (4) in C12
-    elif tensor == 'yy':
-        f = s2q2_lum*(si2 + kani*ci2) + d*x2*ci2  # equation (5) in C12
-    elif tensor == 'zz':
-        f = s2q2_lum*(ci2 + kani*si2) + d*x2*si2  # z' LOS equation (28) in C08
-    elif tensor == 'xy':
-        f = -d*np.abs(x1*y1)*ci2*(a+b)/e          # equation (6) in C12
-    elif tensor == 'xz':
-        f = -d*np.abs(x1*y1)*si*ci*(a+b)/e         # -equation (7) in C12
-    elif tensor == 'yz':
-        f = -si*ci*(s2q2_lum*(1 - kani) - d*x2)   # -equation (8) in C12
+    match tensor:
+        case 'xx':
+            f = kani*s2q2_lum + d*((y1*ci*(a+b)/e)**2 + si2/(2*e)) # equation (4) in C12
+        case 'yy':
+            f = s2q2_lum*(si2 + kani*ci2) + d*x2*ci2  # equation (5) in C12
+        case 'zz':
+            f = s2q2_lum*(ci2 + kani*si2) + d*x2*si2  # z' LOS equation (28) in C08
+        case 'xy':
+            f = -d*np.abs(x1*y1)*ci2*(a+b)/e          # equation (6) in C12
+        case 'xz':
+            f = -d*np.abs(x1*y1)*si*ci*(a+b)/e        # -equation (7) in C12
+        case 'yz':
+            f = -si*ci*(s2q2_lum*(1 - kani) - d*x2)   # -equation (8) in C12
 
     # arr has the dimensions (q_lum.size, q_pot.size, u.size)
 
     arr = q_pot*dens_pot*dens_lum*u2*f*np.exp(-a*(x2 + y2*(a + b)/e))/(
             (1 - c*u2)*np.sqrt((1 - e2u2_pot)*e))
 
     G = 0.004301  # (km/s)^2 pc/Msun [6.674e-11 SI units (CODATA2018)]
@@ -306,23 +307,24 @@
         vel = vel2 = None
     else:
         # Numeric line-of-sight integral
         vel, vel2 = vmom_proj(x_pol, y_pol, inc, mbh, beta, gamma, logistic,
                               dens_lum, sigma_lum, qintr_lum,
                               dens_pot, sigma_pot, qintr_pot,
                               nrad, nang, nlos, epsrel, align, step)
-        model = {'xx': vel2[0, 0],
-                 'yy': vel2[1, 1],
-                 'zz': vel2[2, 2],
-                 'xy': vel2[0, 1],
-                 'xz': vel2[0, 2],
-                 'yz': vel2[1, 2],
-                 'x': vel[0],
-                 'y': vel[1],
-                 'z': vel[2]}[moment]   # match-case before Python 3.10
+        match moment:
+            case 'xx': model = vel2[0, 0]
+            case 'yy': model = vel2[1, 1]
+            case 'zz': model = vel2[2, 2]
+            case 'xy': model = vel2[0, 1]
+            case 'xz': model = vel2[0, 2]
+            case 'yz': model = vel2[1, 2]
+            case 'x': model = vel[0]
+            case 'y': model = vel[1]
+            case 'z': model = vel[2]
 
     if interp and psf_convolution:  # PSF convolution
 
         nx = int(np.ceil(rmax/step))
         ny = int(np.ceil(rmax*qmed/step))
         x1 = np.linspace(0.5 - nx, nx - 0.5, 2*nx)*step
         y1 = np.linspace(0.5 - ny, ny - 0.5, 2*ny)*step
@@ -332,20 +334,21 @@
         # Interpolate moment over cartesian grid.
         # Interpolating "nu_v2/surf" instead of "nu_v2" or "np.log(nu_v2)" reduces interpolation error.
         r1 = 0.5*np.log(x_car**2 + (y_car/qmed)**2)  # Log elliptical radius of cartesian grid
         e1 = np.arctan2(np.abs(y_car/qmed), np.abs(x_car))    # Eccentric anomaly of cartesian grid
         model_car = mge_car*bilinear_interpolate(np.log(rad), ang, model.reshape(nang, nrad), r1, e1)
 
         # Calculation was done in positive quadrant: use symmetries
-        if moment in ['xy', 'xz']:
-            model_car *= np.sign(x_car*y_car)
-        elif moment in ['y', 'z']:
-            model_car *= np.sign(x_car)
-        elif moment == 'x':
-            model_car *= np.sign(y_car)
+        match moment:
+            case 'xy' | 'xz':
+                model_car *= np.sign(x_car*y_car)
+            case 'y' | 'z':
+                model_car *= np.sign(x_car)
+            case 'x':
+                model_car *= np.sign(y_car)
 
         nk = int(np.ceil(mx/step))
         kgrid = np.linspace(-nk, nk, 2*nk + 1)*step
         xgrid, ygrid = np.meshgrid(kgrid, kgrid)  # Kernel is square
         if pixAng != 0:
             xgrid, ygrid = rotate_points(xgrid, ygrid, pixAng)
 
@@ -374,20 +377,21 @@
             mu = model
         else:                      # Interpolate values
             r1 = 0.5*np.log(x**2 + (y/qmed)**2) # Log elliptical radius of input (x,y)
             e1 = np.arctan2(np.abs(y/qmed), np.abs(x))    # Eccentric anomaly of input (x,y)
             mu = bilinear_interpolate(np.log(rad), ang, model.reshape(nang, nrad), r1, e1)
 
             # Calculation was done in positive quadrant: use symmetries
-            if moment in ('xy', 'xz'):
-                mu *= np.sign(x*y)
-            elif moment in ('y', 'z'):
-                mu *= np.sign(x)
-            elif moment == 'x':
-                mu *= np.sign(y)
+            match moment:
+                case 'xy' | 'xz':
+                    mu *= np.sign(x*y)
+                case 'y' | 'z':
+                    mu *= np.sign(x)
+                case 'x':
+                    mu *= np.sign(y)
 
     return mu, psf_convolution, interp, vel, vel2
 
 ##############################################################################
 
 class jam_axi_proj:
     """
@@ -902,26 +906,30 @@
             mbh, beta, gamma, logistic, moment, align, sigmaPsf_pc, normpsf,
             pixSize_pc, pixang, step_pc, nrad, nang, nlos, epsrel,
             interp, analytic_los)
 
         if moment in str2[:3]:
             model = np.sqrt(model.clip(0))  # sqrt and clip to allow for rounding errors
 
+        # If PSF convolution is applied, it returns the MGE model that has been
+        # convolved with the PSF (but ignoring pixel integration). Otherwise,
+        # it returns the original MGE model without PSF convolution.
         # Analytic convolution of the MGE model with an MGE circular PSF
-        # using Equations (4,5) of Cappellari (2002, MNRAS, 333, 400).
+        # uses Equations (4,5) of Cappellari (2002, MNRAS, 333, 400).
+        # https://ui.adsabs.harvard.edu/abs/2002MNRAS.333..400C
         # Broadcast triple loop over (n_MGE, n_PSF, n_bins)
         if psfConvolution:
             sigmaX2 = sigma_lum**2 + sigmapsf[:, None]**2
             sigmaY2 = (sigma_lum*qobs_lum)**2 + sigmapsf[:, None]**2
+            surf_lum_pc = surf_lum_pc*qobs_lum*sigma_lum**2*normpsf[:, None]/np.sqrt(sigmaX2*sigmaY2)
         else:
             sigmaX2 = sigma_lum**2
-            sigmaY2 = (sigma_lum*qobs_lum)**2
-        surf_conv = surf_lum_pc*qobs_lum*sigma_lum**2*normpsf[:, None]/np.sqrt(sigmaX2*sigmaY2)
-        flux = surf_conv[..., None]*np.exp(-0.5*(xbin**2/sigmaX2[..., None] + ybin**2/sigmaY2[..., None]))
-        flux = flux.sum((0, 1))  # PSF-convolved Lsun/pc^2
+            sigmaY2 = (sigma_lum*qobs_lum)**2            
+        flux = surf_lum_pc[..., None]*np.exp(-0.5*(xbin**2/sigmaX2[..., None] + ybin**2/sigmaY2[..., None]))
+        flux = flux.reshape(-1, xbin.size).sum(0)  # PSF-convolved Lsun/pc^2
 
         if flux_obs is None:
             flux_obs = flux
 
         if data is None:
 
             chi2 = np.nan
```

### Comparing `jampy-7.2.4/jampy/jam_axi_sersic.py` & `jampy-7.2.5/jampy/jam_axi_sersic.py`

 * *Files 3% similar despite different names*

```diff
@@ -216,17 +216,14 @@
                            sigmapsf=sigma_psf, quiet=quiet, pixsize=pixsize)
 
         sigma_ap2 = (jam.flux*jam.model**2).sum()/jam.flux.sum()
         scale = sigma_ap**2/sigma_ap2
         lg_mjam = np.log10(mass*scale)
         d_lg_mjam = 2*sigma_ap_err/(sigma_ap*np.log(10))   # error propagation
 
-        if not quiet:
-            print(f'lg(M_JAM/M_Sun) = ({lg_mjam:.2f} +/- {d_lg_mjam:.2f})')
-
         if plot:
             plt.clf()        
             plot_velfield(xbin, ybin, jam.model, flux=jam.flux, nodots=1)
             plt.title("JAM $V_{\\rm rms}$")
             plt.pause(1)
 
         # Compute the effective velocity second moment sigma_e within the
@@ -250,14 +247,21 @@
 
         self.lg_mjam = lg_mjam
         self.d_lg_mjam = d_lg_mjam
         self.mge_pot = surf*scale, sigma, qobs_mge  # mass MGE
         self.sigma_e = np.sqrt(sigma_e2)
         self.sigma_ap = sigma_ap
 
+        if not quiet:
+            print(f"Aperture {dx:.1f}x{dy:.1f} arcsec at angle = {angle:.0f} deg")
+            print(f"Input sigma_ap within the aperture: ({sigma_ap:.0f} +/- {sigma_ap_err:.0f}) km/s")
+            print(f"Corrected sigma_e within Re: {self.sigma_e:.3g} km/s")
+            print(f'lg(M_JAM/M_Sun) = {lg_mjam:.2f} +/- {d_lg_mjam:.2f}')
+
+
 ###############################################################################
 
 def jam_axi_sersic_mass_example():
     """Usage example for jam_axi_sersic_mass"""
 
     # Input parameters
     dxy_ap = [1.0, 0.5]     # sides of rectangular aperture in arcsec
@@ -272,16 +276,15 @@
     sigma_ap_err = 15       # km/s. 1sigma uncertainty on sigma_ap
 
     # Computation
     dist_ang = angular_diameter_distance(redshift)  # D_A angular diameter distance
 
     jam = jam_axi_sersic_mass(re_maj_ser, n_ser, qobs, qintr, sigma_ap, sigma_ap_err, 
                               dxy_ap, sigma_psf, dist_ang, angle=30, beta=beta)
-    print(f"Sersic Mass (M_Sun): {10**jam.lg_mjam:.3g}")
-    print(f"Observed sigma_ap within the aperture (km/s): {sigma_ap:.3g}")
-    print(f"Seeing/aperture-corrected sigma_e within Re (km/s): {jam.sigma_e:.3g}")
+    
+    print(f"\nSersic Mass (M_Sun): {10**jam.lg_mjam:.3g}")
 
 ###############################################################################
 
 if __name__ == '__main__':
 
     jam_axi_sersic_mass_example()
```

### Comparing `jampy-7.2.4/jampy/jam_sph_intr.py` & `jampy-7.2.5/jampy/jam_sph_intr.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 Updated versions of the software are available from my web page
 http://purl.org/cappellari/software
 
 If you have found this software useful for your research,
 I would appreciate an acknowledgement to the use of the
 "JAM modelling method of Cappellari (2008)"
 
+        https://ui.adsabs.harvard.edu/abs/2008MNRAS.390...71C
+
 This software is provided as is without any warranty whatsoever.
 Permission to use, for non-commercial purposes is granted.
 Permission to modify for personal or internal use is granted,
 provided this copyright and disclaimer are included unchanged
 at the beginning of the file. All other rights are reserved.
 In particular, redistribution of the code is not allowed.
```

### Comparing `jampy-7.2.4/jampy/jam_sph_proj.py` & `jampy-7.2.5/jampy/jam_sph_proj.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 Updated versions of the software are available from my web page
 http://purl.org/cappellari/software
 
 If you have found this software useful for your research,
 I would appreciate an acknowledgement to the use of the
 "JAM modelling method of Cappellari (2008, 2020)"
 
+    https://ui.adsabs.harvard.edu/abs/2008MNRAS.390...71C
+    https://ui.adsabs.harvard.edu/abs/2020MNRAS.494.4819C
+
 This software is provided as is without any warranty whatsoever.
 Permission to use, for non-commercial purposes is granted.
 Permission to modify for personal or internal use is granted,
 provided this copyright and disclaimer are included unchanged
 at the beginning of the file. All other rights are reserved.
 In particular, redistribution of the code is not allowed.
 
@@ -254,15 +257,15 @@
         rr = np.geomspace(step/np.sqrt(2), rmax, nrad)   # Linear grid in np.log(rr)
         logRad = np.log(rr)
 
         # The model Vrms computation is only performed on the radial grid
         # which is then used to interpolate the values at any other location
         #
         wm2Pol = np.empty_like(rr)
-        for j, rj in enumerate(rr):     # Integration of equation (50)
+        for j, rj in enumerate(rr):     # Integration of equation (50) of Cappellari (2008)
             args = [sig_lum, sig_pot, dens_lum, mass, Mbh, rj, beta, tensor]
             if logistic:
                 wm2Pol[j] = quad2d(integrand2d, lim, lim, epsrel=epsrel, args=args).integ
             else:
                 wm2Pol[j] = quad1d(integrand1d, lim, epsrel=epsrel, args=args+[ra]).integ
 
         nx = int(np.ceil(rmax/step))
```

### Comparing `jampy-7.2.4/jampy/mge_half_light_isophote.py` & `jampy-7.2.5/jampy/mge_half_light_isophote.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 
 Updated versions of the software are available from my web page
 http://purl.org/cappellari/software
 
 If you have found this software useful for your research,
 I would appreciate an acknowledgement to the use of the
 "JAM modelling package of Cappellari (2008)"
+
+    https://ui.adsabs.harvard.edu/abs/2008MNRAS.390...71C
+
 or an explicit reference to the equation given below.
 
 This software is provided as is without any warranty whatsoever.
 Permission to use, for non-commercial purposes is granted.
 Permission to modify for personal or internal use is granted,
 provided this copyright and disclaimer are included unchanged
 at the beginning of the file. All other rights are reserved.
```

### Comparing `jampy-7.2.4/jampy/mge_radial_density.py` & `jampy-7.2.5/jampy/mge_radial_density.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 
 Updated versions of the software are available from my web page
 http://purl.org/cappellari/software
 
 If you have found this software useful for your research,
 I would appreciate an acknowledgement to the use of the
 "JAM modelling package of Cappellari (2008)"
+
+    https://ui.adsabs.harvard.edu/abs/2008MNRAS.390...71C
+    
 or a reference to Note 11 of Cappellari et al. (2015).
 
 This software is provided as is without any warranty whatsoever.
 Permission to use, for non-commercial purposes is granted.
 Permission to modify for personal or internal use is granted,
 provided this copyright and disclaimer are included unchanged
 at the beginning of the file. All other rights are reserved.
```

### Comparing `jampy-7.2.4/jampy/mge_radial_mass.py` & `jampy-7.2.5/jampy/mge_radial_mass.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 
 Updated versions of the software are available from my web page
 http://purl.org/cappellari/software
 
 If you have found this software useful for your research,
 I would appreciate an acknowledgement to the use of the
 "JAM modelling package of Cappellari (2008)"
+
+    https://ui.adsabs.harvard.edu/abs/2008MNRAS.390...71C
+    
 or an explicit reference to the equations given below.
 
 This software is provided as is without any warranty whatsoever.
 Permission to use, for non-commercial purposes is granted.
 Permission to modify for personal or internal use is granted,
 provided this copyright and disclaimer are included unchanged
 at the beginning of the file. All other rights are reserved.
```

### Comparing `jampy-7.2.4/jampy/mge_vcirc.py` & `jampy-7.2.5/jampy/mge_vcirc.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 E-mail: michele.cappellari_at_physics.ox.ac.uk
 
 Updated versions of the software are available from my web page
 http://purl.org/cappellari/software
 
 If you have found this software useful for your research,
 I would appreciate an acknowledgement to the use of the
-"mge_vcirc routine in the Python modelling package JamPy of Cappellari (2020)"
+"mge_vcirc routine in the Python modelling package JamPy of Cappellari (2008)"
+
+    https://ui.adsabs.harvard.edu/abs/2008MNRAS.390...71C
 
 This software is provided as is without any warranty whatsoever.
 Permission to use, for non-commercial purposes is granted.
 Permission to modify for personal or internal use is granted,
 provided this copyright and disclaimer are included unchanged
 at the beginning of the file. All other rights are reserved.
 In particular, redistribution of the code is not allowed.
```

### Comparing `jampy-7.2.4/jampy/quad1d.py` & `jampy-7.2.5/jampy/quad1d.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,20 +295,20 @@
     When ``INTERVAL = [A,B]``, computes the integral of a continuous function
     ``f(x)`` from A to B for A < B.  A can be ``-np.inf`` and/or B can be
     ``np.inf``.
 
     FUN accepts a row vector X and returns a vector Y with ``Y[m] = f(X[m])``
     for ``m = 1,...,len(X)``.
 
-    FUN can also be a vector function. In this case the function must return a
-    matrix, where every row ``matrix[j, m] = f(X[m])``. In this case the
-    procedure returns the integral of all components, computed using the same
-    set of evaluation points. The convergence criterion ensures that all
-    components satisfy the required tolerance.
-
+    FUN can also be a vector function ``fun = [f_1, f_2,... f_n]``.
+    In this case the FUN must return a ``matrix[j, :] = f_j(X)``.
+    In this case the procedure returns the integral of all components,
+    computed using the same set of evaluation points. The convergence
+    criterion ensures that all components satisfy the required tolerance.
+    
     quad1d returns an approximation Ifx to the integral and optionally an
     approximate bound, ERRBND, on the error ``|integral - Ifx|``. It attempts
     to compute Ifx such that ``|Ifx - integral| <= max(ABSTOL,RELTOL*|Ifx|)``.
     If quad1d is unsuccessful, Ifx and ERRBND are still meaningful, so a
     warning is issued that includes ERRBND.
 
     If the interval is infinite, say ``[a, np.inf)``, then for the integral to
@@ -321,15 +321,15 @@
     ``f(x)`` that behave like ``log|x - c|`` or ``|x - c|^p`` for ``p >= -1/2``
     with ``c = a`` and/or ``c = b``. If ``f(x)`` is singular at points inside
     ``(A,B)``, write the integral as a sum of integrals over subintervals with
     the singular points as end points, compute them with quad1d, and add the
     results.
 
     quad1d starts with samples of ``f(x)`` at 150 points in ``(A,B)``. It must
-    be able to recognize the behavior of ``f(x)`` from these samples, so if
+    be able to recognize the behaviour of ``f(x)`` from these samples, so if
     ``f(x)`` oscillates very rapidly or has sharp peaks, it may be necessary to
     subdivide the interval. To do this, make INTERVAL an array with entries
     (breakpoints) that increase from ``A = INTERVAL[0]`` to ``B = INTERVAL[-1]``.
     If ``f(x)`` is only piecewise smooth, the points of discontinuity should
     be breakpoints.
 
     Based on the algorithm "Vectorized Adaptive Quadrature in Matlab"
@@ -340,14 +340,15 @@
     def __init__(self, fun, interval, epsrel=1e-5, epsabs=0, plot=False,
                  verbose=False, singular=False, args=()):
 
         interval = np.asarray(interval)
         nint = interval.size
         assert nint >= 2, "INTERVAL must be a real vector of at least two entries."
         assert np.all(np.diff(interval) > 0), "Entries of INTERVAL must strictly increase."
+        assert epsrel > 0 or epsabs > 0, "Either `epsrel` or `epsabs` must be positive"
 
         a = interval[0]
         b = interval[-1]
 
         # Generally the error test is a mixed one, but pure absolute error
         # and pure relative error are allowed.  If a pure relative error
         # test is specified, the tolerance must be at least 100*EPS.
```

### Comparing `jampy-7.2.4/jampy/quad2d.py` & `jampy-7.2.5/jampy/quad2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,14 @@
         bound ``res.errbnd`` on the error that satisfies  ``res.errbnd <= 1e-5``.
 
         ``fun`` can also be a vector function ``fun = [f_1, f_2,... f_n]``.
         In this case the ``fun`` must return a ``matrix[j, :] = f_j(X, Y)``.
         In this case the procedure returns the integral of all components,
         computed using the same set of evaluation points. The convergence
         criterion ensures that all components satisfy the required tolerance.
-
     epsabs:
         Absolute error tolerance
     epsrel:
         Relative error tolerance
 
         quad2d attempts to satisfy ERRBND <= max(epsabs, epsrel*|Q|).
         This is absolute error control when |Q| is sufficiently small and
@@ -98,14 +97,16 @@
     args:
         Parameters to pass to the user function ``fun``
 
     """
     def __init__(self, fun, xlim, ylim, epsrel=1e-5, epsabs=0,
                  plot=False, verbose=False, singular=False, args=()):
 
+        assert epsrel > 0 or epsabs > 0, "Either `epsrel` or `epsabs` must be positive"
+
         a, b = xlim
         c, d = ylim
         if callable(c):
             self.phiBvar = c
         elif np.isscalar(c):
             self.phiBvar = lambda x: np.full_like(x, c)
         else:
@@ -289,38 +290,38 @@
     def Save2LIST(self, Qsub, esub, thetaL, thetaR, phiB, phiT):
         """
         Save to the list information about subrectangles for which the
         integral is not sufficiently accurate. NLIST is the number of
         subrectangles to be processed.
 
         """
-        dtheta = thetaR - thetaL
-        dphi = phiT - phiB
-        localtol = self.TOL*(dtheta/2)*(dphi/2)/self.AREA
+        dtheta = (thetaR - thetaL)/2
+        dphi = (phiT - phiB)/2
+        localtol = self.TOL*dtheta*dphi/self.AREA
         localtol = np.maximum(localtol, self.EPS*abs(Qsub.sum(1)))
 
         adjerr = self.ADJUST[:, None]*esub
 
         if np.all(adjerr[:, 0] > localtol):
-            self.LIST.append([Qsub[:, 0], esub[:, 0], thetaL, thetaL + dtheta/2, phiB, phiB + dphi/2, adjerr[:, 0]])
+            self.LIST.append([Qsub[:, 0], esub[:, 0], thetaL, thetaL + dtheta, phiB, phiB + dphi, adjerr[:, 0]])
         else:
             self.ERR_OK += adjerr[:, 0]
 
         if np.all(adjerr[:, 1] > localtol):
-            self.LIST.append([Qsub[:, 1], esub[:, 1], thetaL + dtheta/2, thetaR, phiB, phiB + dphi/2, adjerr[:, 1]])
+            self.LIST.append([Qsub[:, 1], esub[:, 1], thetaL + dtheta, thetaR, phiB, phiB + dphi, adjerr[:, 1]])
         else:
             self.ERR_OK += adjerr[:, 1]
 
         if np.all(adjerr[:, 2] > localtol):
-            self.LIST.append([Qsub[:, 2], esub[:, 2], thetaL, thetaL + dtheta/2, phiB + dphi/2, phiT, adjerr[:, 2]])
+            self.LIST.append([Qsub[:, 2], esub[:, 2], thetaL, thetaL + dtheta, phiB + dphi, phiT, adjerr[:, 2]])
         else:
             self.ERR_OK += adjerr[:, 2]
 
         if np.all(adjerr[:, 3] > localtol):
-            self.LIST.append([Qsub[:, 3], esub[:, 3], thetaL + dtheta/2, thetaR, phiB + dphi/2, phiT, adjerr[:, 3]])
+            self.LIST.append([Qsub[:, 3], esub[:, 3], thetaL + dtheta, thetaR, phiB + dphi, phiT, adjerr[:, 3]])
         else:
             self.ERR_OK += adjerr[:, 3]
 
         adjerr = [a[6] for a in self.LIST]
         self.errbnd = self.ERR_OK + np.sum(adjerr, 0)
 
 ################################################################################
```

### Comparing `jampy-7.2.4/jampy.egg-info/PKG-INFO` & `jampy-7.2.5/jampy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jampy
-Version: 7.2.4
+Version: 7.2.5
 Summary: JamPy: Jeans Anisotropic Models for Galactic Dynamics
 Home-page: https://purl.org/cappellari/software
 Author: Michele Cappellari
 Author-email: michele.cappellari@physics.ox.ac.uk
 License: Other/Proprietary License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -810,14 +810,21 @@
 redistribute the code.
 
 ###########################################################################
 
 Changelog
 ---------
 
+V7.2.5: MC, Oxford 20 May 2024
+++++++++++++++++++++++++++++++
+
+- ``quad1d`` and ``quad2d``: Require positive values for either ``epsrel`` or
+  ``epsabs`` keywords. Thanks to Carlos Melo (cufrgs.br) for the feedback.
+- ``jam_axi_proj``: Dropped support for Python 3.9.
+
 V7.2.4: MC, Oxford, 10 January 2024
 +++++++++++++++++++++++++++++++++++
 
 - ``jam_axi_proj``: Support prolate models with ``qobs_lum > 1`` or 
   ``qobs_pot > 1``.
 - ``jam_axi_proj``: Output unconvolved surface brightness ``jam.flux`` when no
   PSF/aperture convolution is applied to the kinematics, due to zero
```

### Comparing `jampy-7.2.4/jampy.egg-info/SOURCES.txt` & `jampy-7.2.5/jampy.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 jampy/__init__.py
 jampy/cosmology_distance.py
 jampy/jam_axi_intr.py
 jampy/jam_axi_proj.py
 jampy/jam_axi_sersic.py
 jampy/jam_sph_intr.py
 jampy/jam_sph_proj.py
+jampy/mge_cylindrical_mass.py
 jampy/mge_half_light_isophote.py
 jampy/mge_radial_density.py
 jampy/mge_radial_mass.py
 jampy/mge_vcirc.py
 jampy/quad1d.py
 jampy/quad2d.py
 jampy.egg-info/PKG-INFO
```

### Comparing `jampy-7.2.4/setup.py` & `jampy-7.2.5/setup.py`

 * *Files identical despite different names*

