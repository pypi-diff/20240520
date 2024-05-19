# Comparing `tmp/pandorasat-0.5.8.tar.gz` & `tmp/pandorasat-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandorasat-0.5.8.tar", max compression
+gzip compressed data, was "pandorasat-0.5.9.tar", max compression
```

## Comparing `pandorasat-0.5.8.tar` & `pandorasat-0.5.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1073 2023-11-16 22:14:29.402553 pandorasat-0.5.8/LICENSE
--rw-r--r--   0        0        0     1096 2024-05-08 16:32:35.850355 pandorasat-0.5.8/pyproject.toml
--rw-r--r--   0        0        0      814 2024-05-03 17:37:40.383486 pandorasat-0.5.8/src/pandorasat/__init__.py
--rw-r--r--   0        0        0     2143 2023-11-16 22:14:29.405491 pandorasat-0.5.8/src/pandorasat/citations.py
--rw-r--r--   0        0        0     3018 2023-11-16 22:14:29.405618 pandorasat-0.5.8/src/pandorasat/data/Pandora.Pandora.Visible.xml
--rw-r--r--   0        0        0    14687 2023-11-16 22:14:29.405752 pandorasat-0.5.8/src/pandorasat/data/dichroic-transmission.csv
--rw-r--r--   0        0        0     2777 2023-11-16 22:14:29.405832 pandorasat-0.5.8/src/pandorasat/data/pandora.mplstyle
--rw-r--r--   0        0        0    25577 2023-11-16 22:14:29.406002 pandorasat-0.5.8/src/pandorasat/data/pixel_vs_wavelength.csv
--rw-r--r--   0        0        0     4412 2023-11-16 22:14:29.406102 pandorasat-0.5.8/src/pandorasat/data/pixel_vs_wavelength_vis.csv
--rw-r--r--   0        0        0    26996 2023-11-16 22:45:54.629516 pandorasat-0.5.8/src/pandorasat/data/test-star.p
--rw-r--r--   0        0        0   202494 2023-11-16 22:14:29.406866 pandorasat-0.5.8/src/pandorasat/data/vega.csv
--rw-r--r--   0        0        0   202600 2023-11-16 22:14:29.407639 pandorasat-0.5.8/src/pandorasat/data/vega.dat
--rw-r--r--   0        0        0      484 2023-11-16 22:39:51.932871 pandorasat-0.5.8/src/pandorasat/hardware.py
--rw-r--r--   0        0        0     5976 2024-05-03 17:37:51.198955 pandorasat-0.5.8/src/pandorasat/irdetector.py
--rw-r--r--   0        0        0      311 2023-11-16 22:14:29.407897 pandorasat-0.5.8/src/pandorasat/orbit.py
--rw-r--r--   0        0        0      832 2023-11-16 22:39:51.200812 pandorasat-0.5.8/src/pandorasat/pandorasat.py
--rw-r--r--   0        0        0     5947 2024-02-09 18:25:59.010581 pandorasat-0.5.8/src/pandorasat/phoenix.py
--rw-r--r--   0        0        0     5394 2024-02-08 20:03:23.913123 pandorasat-0.5.8/src/pandorasat/utils.py
--rw-r--r--   0        0        0     5911 2024-02-08 20:03:23.913317 pandorasat-0.5.8/src/pandorasat/visibledetector.py
--rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 pandorasat-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-11-16 22:14:29.402553 pandorasat-0.5.9/LICENSE
+-rw-r--r--   0        0        0     1215 2024-05-08 17:46:34.166903 pandorasat-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0      814 2024-05-03 17:37:40.383486 pandorasat-0.5.9/src/pandorasat/__init__.py
+-rw-r--r--   0        0        0     2143 2023-11-16 22:14:29.405491 pandorasat-0.5.9/src/pandorasat/citations.py
+-rw-r--r--   0        0        0     3018 2023-11-16 22:14:29.405618 pandorasat-0.5.9/src/pandorasat/data/Pandora.Pandora.Visible.xml
+-rw-r--r--   0        0        0    14687 2023-11-16 22:14:29.405752 pandorasat-0.5.9/src/pandorasat/data/dichroic-transmission.csv
+-rw-r--r--   0        0        0     2777 2023-11-16 22:14:29.405832 pandorasat-0.5.9/src/pandorasat/data/pandora.mplstyle
+-rw-r--r--   0        0        0    25577 2023-11-16 22:14:29.406002 pandorasat-0.5.9/src/pandorasat/data/pixel_vs_wavelength.csv
+-rw-r--r--   0        0        0     4412 2023-11-16 22:14:29.406102 pandorasat-0.5.9/src/pandorasat/data/pixel_vs_wavelength_vis.csv
+-rw-r--r--   0        0        0    26996 2023-11-16 22:45:54.629516 pandorasat-0.5.9/src/pandorasat/data/test-star.p
+-rw-r--r--   0        0        0   202494 2023-11-16 22:14:29.406866 pandorasat-0.5.9/src/pandorasat/data/vega.csv
+-rw-r--r--   0        0        0   202600 2023-11-16 22:14:29.407639 pandorasat-0.5.9/src/pandorasat/data/vega.dat
+-rw-r--r--   0        0        0      484 2023-11-16 22:39:51.932871 pandorasat-0.5.9/src/pandorasat/hardware.py
+-rw-r--r--   0        0        0     5976 2024-05-03 17:37:51.198955 pandorasat-0.5.9/src/pandorasat/irdetector.py
+-rw-r--r--   0        0        0      311 2023-11-16 22:14:29.407897 pandorasat-0.5.9/src/pandorasat/orbit.py
+-rw-r--r--   0        0        0      832 2023-11-16 22:39:51.200812 pandorasat-0.5.9/src/pandorasat/pandorasat.py
+-rw-r--r--   0        0        0     5947 2024-02-09 18:25:59.010581 pandorasat-0.5.9/src/pandorasat/phoenix.py
+-rw-r--r--   0        0        0     5394 2024-02-08 20:03:23.913123 pandorasat-0.5.9/src/pandorasat/utils.py
+-rw-r--r--   0        0        0     5911 2024-02-08 20:03:23.913317 pandorasat-0.5.9/src/pandorasat/visibledetector.py
+-rw-r--r--   0        0        0     1210 1970-01-01 00:00:00.000000 pandorasat-0.5.9/PKG-INFO
```

### Comparing `pandorasat-0.5.8/LICENSE` & `pandorasat-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.8/src/pandorasat/__init__.py` & `pandorasat-0.5.9/src/pandorasat/__init__.py`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.8/src/pandorasat/citations.py` & `pandorasat-0.5.9/src/pandorasat/citations.py`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.8/src/pandorasat/data/Pandora.Pandora.Visible.xml` & `pandorasat-0.5.9/src/pandorasat/data/Pandora.Pandora.Visible.xml`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.8/src/pandorasat/data/dichroic-transmission.csv` & `pandorasat-0.5.9/src/pandorasat/data/dichroic-transmission.csv`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.8/src/pandorasat/data/pandora.mplstyle` & `pandorasat-0.5.9/src/pandorasat/data/pandora.mplstyle`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.8/src/pandorasat/data/pixel_vs_wavelength.csv` & `pandorasat-0.5.9/src/pandorasat/data/pixel_vs_wavelength.csv`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.8/src/pandorasat/data/pixel_vs_wavelength_vis.csv` & `pandorasat-0.5.9/src/pandorasat/data/pixel_vs_wavelength_vis.csv`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.8/src/pandorasat/data/test-star.p` & `pandorasat-0.5.9/src/pandorasat/data/test-star.p`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.8/src/pandorasat/data/vega.csv` & `pandorasat-0.5.9/src/pandorasat/data/vega.csv`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.8/src/pandorasat/data/vega.dat` & `pandorasat-0.5.9/src/pandorasat/data/vega.dat`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.8/src/pandorasat/irdetector.py` & `pandorasat-0.5.9/src/pandorasat/irdetector.py`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.8/src/pandorasat/pandorasat.py` & `pandorasat-0.5.9/src/pandorasat/pandorasat.py`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.8/src/pandorasat/phoenix.py` & `pandorasat-0.5.9/src/pandorasat/phoenix.py`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.8/src/pandorasat/utils.py` & `pandorasat-0.5.9/src/pandorasat/utils.py`

 * *Files identical despite different names*

### Comparing `pandorasat-0.5.8/src/pandorasat/visibledetector.py` & `pandorasat-0.5.9/src/pandorasat/visibledetector.py`

 * *Files identical despite different names*

