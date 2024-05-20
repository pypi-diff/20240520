# Comparing `tmp/shadowfinder-0.2.0.tar.gz` & `tmp/shadowfinder-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shadowfinder-0.2.0.tar", max compression
+gzip compressed data, was "shadowfinder-0.2.1.tar", max compression
```

## Comparing `shadowfinder-0.2.0.tar` & `shadowfinder-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1077 2024-05-17 15:55:35.988639 shadowfinder-0.2.0/LICENSE
--rw-r--r--   0        0        0      483 2024-05-17 15:55:35.988639 shadowfinder-0.2.0/README.md
--rw-r--r--   0        0        0     1051 2024-05-17 15:55:35.988639 shadowfinder-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-17 15:55:35.988639 shadowfinder-0.2.0/shadowfinder/__init__.py
--rw-r--r--   0        0        0     1509 2024-05-17 15:55:35.988639 shadowfinder-0.2.0/shadowfinder/cli.py
--rw-r--r--   0        0        0      164 2024-05-17 15:55:35.988639 shadowfinder-0.2.0/shadowfinder/main.py
--rw-r--r--   0        0        0     6500 2024-05-17 15:55:35.988639 shadowfinder-0.2.0/shadowfinder/shadowfinder.py
--rw-r--r--   0        0        0     1717 1970-01-01 00:00:00.000000 shadowfinder-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-20 15:11:24.407491 shadowfinder-0.2.1/LICENSE
+-rw-r--r--   0        0        0      483 2024-05-20 15:11:24.407491 shadowfinder-0.2.1/README.md
+-rw-r--r--   0        0        0     1052 2024-05-20 15:11:24.407491 shadowfinder-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-20 15:11:24.407491 shadowfinder-0.2.1/shadowfinder/__init__.py
+-rw-r--r--   0        0        0     1509 2024-05-20 15:11:24.407491 shadowfinder-0.2.1/shadowfinder/cli.py
+-rw-r--r--   0        0        0      164 2024-05-20 15:11:24.407491 shadowfinder-0.2.1/shadowfinder/main.py
+-rw-r--r--   0        0        0     6548 2024-05-20 15:11:24.407491 shadowfinder-0.2.1/shadowfinder/shadowfinder.py
+-rw-r--r--   0        0        0     1717 1970-01-01 00:00:00.000000 shadowfinder-0.2.1/PKG-INFO
```

### Comparing `shadowfinder-0.2.0/LICENSE` & `shadowfinder-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shadowfinder-0.2.0/pyproject.toml` & `shadowfinder-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ShadowFinder"
-version = "0.2.0"
+version = "0.2.1"
 description = "Find possible locations of shadows."
 authors = ["Bellingcat"]
 license = "MIT License"
 readme = "README.md"
 repository = "https://github.com/bellingcat/ShadowFinder"
 classifiers = [
   "Intended Audience :: Developers",
@@ -35,8 +35,8 @@
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.2.0"
 
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `shadowfinder-0.2.0/shadowfinder/cli.py` & `shadowfinder-0.2.1/shadowfinder/cli.py`

 * *Files identical despite different names*

### Comparing `shadowfinder-0.2.0/shadowfinder/shadowfinder.py` & `shadowfinder-0.2.1/shadowfinder/shadowfinder.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             self.time_format = time_format
 
     def quick_find(self):
         self.generate_timezone_grid()
         self.find_shadows()
         fig = self.plot_shadows()
         fig.savefig(
-            f"shadow_finder_{self.date_time.strftime('%Y%m%d-%H%M%S-%Z')}_{self.object_height}_{self.shadow_length}.png"
+            f"shadow_finder_{self.date_time.strftime('%Y%m%d-%H%M%S')}-{self.time_format.title()}_{self.object_height}_{self.shadow_length}.png"
         )
 
     def generate_timezone_grid(self):
         lats = np.arange(self.min_lat, self.max_lat, self.angular_resolution)
         lons = np.arange(self.min_lon, self.max_lon, self.angular_resolution)
 
         self.lons, self.lats = np.meshgrid(lons, lats)
@@ -177,11 +177,11 @@
         norm = colors.BoundaryNorm(np.arange(0, 0.2, 0.02), cmap.N)
 
         # Plot the data
         m.pcolormesh(x, y, np.abs(self.shadow_lengths), cmap=cmap, norm=norm, alpha=0.7)
 
         # plt.colorbar(label='Relative Shadow Length Difference')
         plt.title(
-            f"Possible Locations at {self.date_time.strftime('%Y-%m-%d %H:%M:%S %Z')}\n(object height: {self.object_height}, shadow length: {self.shadow_length})"
+            f"Possible Locations at {self.date_time.strftime('%Y-%m-%d %H:%M:%S')} {self.time_format.title()}\n(object height: {self.object_height}, shadow length: {self.shadow_length})"
         )
         self.fig = fig
         return fig
```

### Comparing `shadowfinder-0.2.0/PKG-INFO` & `shadowfinder-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShadowFinder
-Version: 0.2.0
+Version: 0.2.1
 Summary: Find possible locations of shadows.
 Home-page: https://github.com/bellingcat/ShadowFinder
 License: MIT
 Keywords: shadow,finder,locator,map
 Author: Bellingcat
 Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 3 - Alpha
```

