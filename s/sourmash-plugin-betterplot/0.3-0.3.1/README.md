# Comparing `tmp/sourmash_plugin_betterplot-0.3.tar.gz` & `tmp/sourmash_plugin_betterplot-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourmash_plugin_betterplot-0.3.tar", last modified: Sun May 19 15:10:36 2024, max compression
+gzip compressed data, was "sourmash_plugin_betterplot-0.3.1.tar", last modified: Sun May 19 17:16:53 2024, max compression
```

## Comparing `sourmash_plugin_betterplot-0.3.tar` & `sourmash_plugin_betterplot-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-19 15:10:36.845518 sourmash_plugin_betterplot-0.3/
--rw-r--r--   0 t          (502) staff       (20)     1540 2024-05-17 15:38:24.000000 sourmash_plugin_betterplot-0.3/LICENSE
--rw-r--r--   0 t          (502) staff       (20)     6202 2024-05-19 15:10:36.845306 sourmash_plugin_betterplot-0.3/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)     5841 2024-05-19 15:10:31.000000 sourmash_plugin_betterplot-0.3/README.md
--rw-r--r--   0 t          (502) staff       (20)      654 2024-05-19 15:10:31.000000 sourmash_plugin_betterplot-0.3/pyproject.toml
--rw-r--r--   0 t          (502) staff       (20)       38 2024-05-19 15:10:36.845556 sourmash_plugin_betterplot-0.3/setup.cfg
-drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-19 15:10:36.843729 sourmash_plugin_betterplot-0.3/src/
-drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-19 15:10:36.845090 sourmash_plugin_betterplot-0.3/src/sourmash_plugin_betterplot.egg-info/
--rw-r--r--   0 t          (502) staff       (20)     6202 2024-05-19 15:10:36.000000 sourmash_plugin_betterplot-0.3/src/sourmash_plugin_betterplot.egg-info/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)      422 2024-05-19 15:10:36.000000 sourmash_plugin_betterplot-0.3/src/sourmash_plugin_betterplot.egg-info/SOURCES.txt
--rw-r--r--   0 t          (502) staff       (20)        1 2024-05-19 15:10:36.000000 sourmash_plugin_betterplot-0.3/src/sourmash_plugin_betterplot.egg-info/dependency_links.txt
--rw-r--r--   0 t          (502) staff       (20)      270 2024-05-19 15:10:36.000000 sourmash_plugin_betterplot-0.3/src/sourmash_plugin_betterplot.egg-info/entry_points.txt
--rw-r--r--   0 t          (502) staff       (20)       55 2024-05-19 15:10:36.000000 sourmash_plugin_betterplot-0.3/src/sourmash_plugin_betterplot.egg-info/requires.txt
--rw-r--r--   0 t          (502) staff       (20)       27 2024-05-19 15:10:36.000000 sourmash_plugin_betterplot-0.3/src/sourmash_plugin_betterplot.egg-info/top_level.txt
--rw-r--r--   0 t          (502) staff       (20)    17963 2024-05-19 15:10:31.000000 sourmash_plugin_betterplot-0.3/src/sourmash_plugin_betterplot.py
-drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-19 15:10:36.844707 sourmash_plugin_betterplot-0.3/tests/
--rw-r--r--   0 t          (502) staff       (20)      446 2024-05-17 15:38:24.000000 sourmash_plugin_betterplot-0.3/tests/test_sourmash_plugin.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-19 17:16:53.996033 sourmash_plugin_betterplot-0.3.1/
+-rw-r--r--   0 t          (502) staff       (20)     1540 2024-05-17 15:38:24.000000 sourmash_plugin_betterplot-0.3.1/LICENSE
+-rw-r--r--   0 t          (502) staff       (20)     6844 2024-05-19 17:16:53.995745 sourmash_plugin_betterplot-0.3.1/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)     6458 2024-05-19 17:16:22.000000 sourmash_plugin_betterplot-0.3.1/README.md
+-rw-r--r--   0 t          (502) staff       (20)      726 2024-05-19 17:16:22.000000 sourmash_plugin_betterplot-0.3.1/pyproject.toml
+-rw-r--r--   0 t          (502) staff       (20)       38 2024-05-19 17:16:53.996071 sourmash_plugin_betterplot-0.3.1/setup.cfg
+drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-19 17:16:53.993608 sourmash_plugin_betterplot-0.3.1/src/
+drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-19 17:16:53.995398 sourmash_plugin_betterplot-0.3.1/src/sourmash_plugin_betterplot.egg-info/
+-rw-r--r--   0 t          (502) staff       (20)     6844 2024-05-19 17:16:53.000000 sourmash_plugin_betterplot-0.3.1/src/sourmash_plugin_betterplot.egg-info/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)      422 2024-05-19 17:16:53.000000 sourmash_plugin_betterplot-0.3.1/src/sourmash_plugin_betterplot.egg-info/SOURCES.txt
+-rw-r--r--   0 t          (502) staff       (20)        1 2024-05-19 17:16:53.000000 sourmash_plugin_betterplot-0.3.1/src/sourmash_plugin_betterplot.egg-info/dependency_links.txt
+-rw-r--r--   0 t          (502) staff       (20)      327 2024-05-19 17:16:53.000000 sourmash_plugin_betterplot-0.3.1/src/sourmash_plugin_betterplot.egg-info/entry_points.txt
+-rw-r--r--   0 t          (502) staff       (20)       63 2024-05-19 17:16:53.000000 sourmash_plugin_betterplot-0.3.1/src/sourmash_plugin_betterplot.egg-info/requires.txt
+-rw-r--r--   0 t          (502) staff       (20)       27 2024-05-19 17:16:53.000000 sourmash_plugin_betterplot-0.3.1/src/sourmash_plugin_betterplot.egg-info/top_level.txt
+-rw-r--r--   0 t          (502) staff       (20)    21676 2024-05-19 17:16:22.000000 sourmash_plugin_betterplot-0.3.1/src/sourmash_plugin_betterplot.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-19 17:16:53.995076 sourmash_plugin_betterplot-0.3.1/tests/
+-rw-r--r--   0 t          (502) staff       (20)      446 2024-05-17 15:38:24.000000 sourmash_plugin_betterplot-0.3.1/tests/test_sourmash_plugin.py
```

### Comparing `sourmash_plugin_betterplot-0.3/LICENSE` & `sourmash_plugin_betterplot-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_betterplot-0.3/PKG-INFO` & `sourmash_plugin_betterplot-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: sourmash_plugin_betterplot
-Version: 0.3
+Version: 0.3.1
 Summary: sourmash plugin for improved plotting/viz and cluster examination.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sourmash<5,>=4.8.8
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
+Requires-Dist: seaborn
 
 # sourmash_plugin_betterplot
 
 [sourmash](https://sourmash.readthedocs.io/) is a tool for biological
 sequence analysis and comparisons.
 
 `betterplot` is a sourmash plugin that provides improved plotting/viz
@@ -56,15 +57,15 @@
 See the examples below.
 
 ## Examples
 
 The command lines below are executable in the `examples/` subdirectory
 of the repository after installing the plugin.
 
-### Basic 3 sketches example: plot2
+### `plot2` - basic 3 sketches example
 
 Compare 3 sketches, and cluster.
 
 This command:
 ```
 sourmash compare sketches/{2,47,63}.sig.zip -o 3sketches.cmp
     --labels-to 3sketches.cmp.labels_to.csv
@@ -73,15 +74,15 @@
     -o examples/plot2.3sketches.cmp.png
 ```
 
 produces this plot:
 
 ![basic 3-sketches example](examples/plot2.3sketches.cmp.png)
 
-### 3 sketches example with a cut line: plot2 --cut-point 1.2
+### `plot2` - 3 sketches example with a cut line: plot2 --cut-point 1.2
 
 Compare 3 sketches, cluster, and show a cut point.
 
 This command:
 ```
 sourmash compare sketches/{2,47,63}.sig.zip -o 3sketches.cmp
     --labels-to 3sketches.cmp.labels_to.csv
@@ -91,15 +92,15 @@
     --cut-point=1.2
 ```
 
 produces this plot:
 
 ![3-sketches example w/cut line](examples/plot2.cut.3sketches.cmp.png)
 
-### Dendrogram of 10 sketches with a cut line + cluster extraction
+### `plot2` - dendrogram of 10 sketches with a cut line + cluster extraction
 
 Compare 10 sketches, cluster, and use a cut point to extract
 multiple clusters. Use `--dendrogram-only` to plot just the dendrogram.
 
 This command:
 ```
 sourmash compare sketches/{2,47,48,49,51,52,53,59,60}.sig.zip \
@@ -113,33 +114,33 @@
 
 produces this plot:
 
 ![10-sketches example w/cut line](examples/plot2.cut.dendro.10sketches.cmp.png)
 
 as well as a set of 6 clusters to `10sketches.cmp.*.csv`.
 
-### Multidimensional Scaling (MDS) plot of 10-sketch comparison
+### `mds`- multidimensional Scaling (MDS) plot of 10-sketch comparison
 
 Use MDS to display a comparison.
 
-This command:
+These commands:
 ```
 sourmash compare sketches/{2,47,48,49,51,52,53,59,60}.sig.zip \
     -o 10sketches.cmp \
     --labels-to 10sketches.cmp.labels_to.csv
 
 sourmash scripts mds 10sketches.cmp 10sketches.cmp.labels_to.csv \
     -o mds.10sketches.cmp.png \
     -C 10sketches-categories.csv
 ```
 
 produces this plot:
 ![10-sketches plotted using MDS](examples/mds.10sketches.cmp.png)
 
-### Multidimensional Scaling (MDS) plot of 10-sketch comparisons from `pairwise` output
+### `mds2` - multidimensional Scaling (MDS) plot of 10-sketch comparisons from `pairwise` output
 
 Use MDS to display a sparse comparison created using the
 [branchwater plugin's](https://github.com/sourmash-bio/sourmash_plugin_branchwater)
 `pairwise` command. The output of `pairwise` is distinct from the
 `sourmash compare` output: `pairwise` produces a sparse CSV file that
 contains just the matches above threshold, while `sourmash compare`
 produces a dense numpy matrix.
@@ -154,15 +155,15 @@
     -o mds.10sketches.cmp.png \
     -C 10sketches-categories.csv
 ```
 
 produces this plot:
 ![10-sketches plotted using MDS2](examples/mds2.10sketches.cmp.png)
 
-### Convert `pairwise` output to `sourmash compare` output and plot
+### `pairwise_to_compare` - convert `pairwise` output to `sourmash compare` output and plot
 
 These commands:
 ```
 # build pairwise
 sourmash sig cat sketches/{2,47,48,49,51,52,53,59,60}.sig.zip \
     -o 10sketches.sig.zip
 sourmash scripts pairwise 10sketches.sig.zip -o 10sketches.pairwise.csv
@@ -178,14 +179,34 @@
     -o plot2.pairwise.10sketches.cmp.png
 ```
 
 produce this plot:
 
 ![10-sketches plotted from pairwise](examples/plot2.pairwise.10sketches.cmp.png)
 
+### `plot3` - seaborn clustermap with color categories
+
+The
+[`seaborn` clustermap](https://seaborn.pydata.org/generated/seaborn.clustermap.html)
+offers some nice visualization options.
+
+These commands:
+```
+sourmash compare sketches/{2,47,48,49,51,52,53,59,60}.sig.zip \
+    -o 10sketches.cmp \
+    --labels-to 10sketches.cmp.labels_to.csv
+
+sourmash scripts plot3 10sketches.cmp 10sketches.cmp.labels_to.csv \
+    -o plot3.10sketches.cmp.png -C 10sketches-categories.csv
+```
+
+produce this plot:
+
+![plot3 10 sketches](examples/plot3.10sketches.cmp.png)
+
 
 ## Support
 
 We suggest filing issues in [the main sourmash issue tracker](https://github.com/dib-lab/sourmash/issues) as that receives more attention!
 
 ## Dev docs
```

### Comparing `sourmash_plugin_betterplot-0.3/README.md` & `sourmash_plugin_betterplot-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 See the examples below.
 
 ## Examples
 
 The command lines below are executable in the `examples/` subdirectory
 of the repository after installing the plugin.
 
-### Basic 3 sketches example: plot2
+### `plot2` - basic 3 sketches example
 
 Compare 3 sketches, and cluster.
 
 This command:
 ```
 sourmash compare sketches/{2,47,63}.sig.zip -o 3sketches.cmp
     --labels-to 3sketches.cmp.labels_to.csv
@@ -60,15 +60,15 @@
     -o examples/plot2.3sketches.cmp.png
 ```
 
 produces this plot:
 
 ![basic 3-sketches example](examples/plot2.3sketches.cmp.png)
 
-### 3 sketches example with a cut line: plot2 --cut-point 1.2
+### `plot2` - 3 sketches example with a cut line: plot2 --cut-point 1.2
 
 Compare 3 sketches, cluster, and show a cut point.
 
 This command:
 ```
 sourmash compare sketches/{2,47,63}.sig.zip -o 3sketches.cmp
     --labels-to 3sketches.cmp.labels_to.csv
@@ -78,15 +78,15 @@
     --cut-point=1.2
 ```
 
 produces this plot:
 
 ![3-sketches example w/cut line](examples/plot2.cut.3sketches.cmp.png)
 
-### Dendrogram of 10 sketches with a cut line + cluster extraction
+### `plot2` - dendrogram of 10 sketches with a cut line + cluster extraction
 
 Compare 10 sketches, cluster, and use a cut point to extract
 multiple clusters. Use `--dendrogram-only` to plot just the dendrogram.
 
 This command:
 ```
 sourmash compare sketches/{2,47,48,49,51,52,53,59,60}.sig.zip \
@@ -100,33 +100,33 @@
 
 produces this plot:
 
 ![10-sketches example w/cut line](examples/plot2.cut.dendro.10sketches.cmp.png)
 
 as well as a set of 6 clusters to `10sketches.cmp.*.csv`.
 
-### Multidimensional Scaling (MDS) plot of 10-sketch comparison
+### `mds`- multidimensional Scaling (MDS) plot of 10-sketch comparison
 
 Use MDS to display a comparison.
 
-This command:
+These commands:
 ```
 sourmash compare sketches/{2,47,48,49,51,52,53,59,60}.sig.zip \
     -o 10sketches.cmp \
     --labels-to 10sketches.cmp.labels_to.csv
 
 sourmash scripts mds 10sketches.cmp 10sketches.cmp.labels_to.csv \
     -o mds.10sketches.cmp.png \
     -C 10sketches-categories.csv
 ```
 
 produces this plot:
 ![10-sketches plotted using MDS](examples/mds.10sketches.cmp.png)
 
-### Multidimensional Scaling (MDS) plot of 10-sketch comparisons from `pairwise` output
+### `mds2` - multidimensional Scaling (MDS) plot of 10-sketch comparisons from `pairwise` output
 
 Use MDS to display a sparse comparison created using the
 [branchwater plugin's](https://github.com/sourmash-bio/sourmash_plugin_branchwater)
 `pairwise` command. The output of `pairwise` is distinct from the
 `sourmash compare` output: `pairwise` produces a sparse CSV file that
 contains just the matches above threshold, while `sourmash compare`
 produces a dense numpy matrix.
@@ -141,15 +141,15 @@
     -o mds.10sketches.cmp.png \
     -C 10sketches-categories.csv
 ```
 
 produces this plot:
 ![10-sketches plotted using MDS2](examples/mds2.10sketches.cmp.png)
 
-### Convert `pairwise` output to `sourmash compare` output and plot
+### `pairwise_to_compare` - convert `pairwise` output to `sourmash compare` output and plot
 
 These commands:
 ```
 # build pairwise
 sourmash sig cat sketches/{2,47,48,49,51,52,53,59,60}.sig.zip \
     -o 10sketches.sig.zip
 sourmash scripts pairwise 10sketches.sig.zip -o 10sketches.pairwise.csv
@@ -165,14 +165,34 @@
     -o plot2.pairwise.10sketches.cmp.png
 ```
 
 produce this plot:
 
 ![10-sketches plotted from pairwise](examples/plot2.pairwise.10sketches.cmp.png)
 
+### `plot3` - seaborn clustermap with color categories
+
+The
+[`seaborn` clustermap](https://seaborn.pydata.org/generated/seaborn.clustermap.html)
+offers some nice visualization options.
+
+These commands:
+```
+sourmash compare sketches/{2,47,48,49,51,52,53,59,60}.sig.zip \
+    -o 10sketches.cmp \
+    --labels-to 10sketches.cmp.labels_to.csv
+
+sourmash scripts plot3 10sketches.cmp 10sketches.cmp.labels_to.csv \
+    -o plot3.10sketches.cmp.png -C 10sketches-categories.csv
+```
+
+produce this plot:
+
+![plot3 10 sketches](examples/plot3.10sketches.cmp.png)
+
 
 ## Support
 
 We suggest filing issues in [the main sourmash issue tracker](https://github.com/dib-lab/sourmash/issues) as that receives more attention!
 
 ## Dev docs
```

### Comparing `sourmash_plugin_betterplot-0.3/pyproject.toml` & `sourmash_plugin_betterplot-0.3.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [project]
 name = "sourmash_plugin_betterplot"
 description = "sourmash plugin for improved plotting/viz and cluster examination."
 readme = "README.md"
 requires-python = ">=3.10"
-version = "0.3"
+version = "0.3.1"
 
 dependencies = ["sourmash>=4.8.8,<5",
-                "matplotlib", "numpy", "scipy", "scikit-learn"]
+                "matplotlib", "numpy", "scipy", "scikit-learn", "seaborn"]
 
 [metadata]
 license = { text = "BSD 3-Clause License" }
 
 [project.entry-points."sourmash.cli_script"]
 plot2_command = "sourmash_plugin_betterplot:Command_Plot2"
+plot3_command = "sourmash_plugin_betterplot:Command_Plot3"
 mds_command = "sourmash_plugin_betterplot:Command_MDS"
 mds2_command = "sourmash_plugin_betterplot:Command_MDS2"
 pairwise_to_compare_command = "sourmash_plugin_betterplot:Command_PairwiseToCompare"
```

### Comparing `sourmash_plugin_betterplot-0.3/src/sourmash_plugin_betterplot.egg-info/PKG-INFO` & `sourmash_plugin_betterplot-0.3.1/src/sourmash_plugin_betterplot.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: sourmash_plugin_betterplot
-Version: 0.3
+Version: 0.3.1
 Summary: sourmash plugin for improved plotting/viz and cluster examination.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sourmash<5,>=4.8.8
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
+Requires-Dist: seaborn
 
 # sourmash_plugin_betterplot
 
 [sourmash](https://sourmash.readthedocs.io/) is a tool for biological
 sequence analysis and comparisons.
 
 `betterplot` is a sourmash plugin that provides improved plotting/viz
@@ -56,15 +57,15 @@
 See the examples below.
 
 ## Examples
 
 The command lines below are executable in the `examples/` subdirectory
 of the repository after installing the plugin.
 
-### Basic 3 sketches example: plot2
+### `plot2` - basic 3 sketches example
 
 Compare 3 sketches, and cluster.
 
 This command:
 ```
 sourmash compare sketches/{2,47,63}.sig.zip -o 3sketches.cmp
     --labels-to 3sketches.cmp.labels_to.csv
@@ -73,15 +74,15 @@
     -o examples/plot2.3sketches.cmp.png
 ```
 
 produces this plot:
 
 ![basic 3-sketches example](examples/plot2.3sketches.cmp.png)
 
-### 3 sketches example with a cut line: plot2 --cut-point 1.2
+### `plot2` - 3 sketches example with a cut line: plot2 --cut-point 1.2
 
 Compare 3 sketches, cluster, and show a cut point.
 
 This command:
 ```
 sourmash compare sketches/{2,47,63}.sig.zip -o 3sketches.cmp
     --labels-to 3sketches.cmp.labels_to.csv
@@ -91,15 +92,15 @@
     --cut-point=1.2
 ```
 
 produces this plot:
 
 ![3-sketches example w/cut line](examples/plot2.cut.3sketches.cmp.png)
 
-### Dendrogram of 10 sketches with a cut line + cluster extraction
+### `plot2` - dendrogram of 10 sketches with a cut line + cluster extraction
 
 Compare 10 sketches, cluster, and use a cut point to extract
 multiple clusters. Use `--dendrogram-only` to plot just the dendrogram.
 
 This command:
 ```
 sourmash compare sketches/{2,47,48,49,51,52,53,59,60}.sig.zip \
@@ -113,33 +114,33 @@
 
 produces this plot:
 
 ![10-sketches example w/cut line](examples/plot2.cut.dendro.10sketches.cmp.png)
 
 as well as a set of 6 clusters to `10sketches.cmp.*.csv`.
 
-### Multidimensional Scaling (MDS) plot of 10-sketch comparison
+### `mds`- multidimensional Scaling (MDS) plot of 10-sketch comparison
 
 Use MDS to display a comparison.
 
-This command:
+These commands:
 ```
 sourmash compare sketches/{2,47,48,49,51,52,53,59,60}.sig.zip \
     -o 10sketches.cmp \
     --labels-to 10sketches.cmp.labels_to.csv
 
 sourmash scripts mds 10sketches.cmp 10sketches.cmp.labels_to.csv \
     -o mds.10sketches.cmp.png \
     -C 10sketches-categories.csv
 ```
 
 produces this plot:
 ![10-sketches plotted using MDS](examples/mds.10sketches.cmp.png)
 
-### Multidimensional Scaling (MDS) plot of 10-sketch comparisons from `pairwise` output
+### `mds2` - multidimensional Scaling (MDS) plot of 10-sketch comparisons from `pairwise` output
 
 Use MDS to display a sparse comparison created using the
 [branchwater plugin's](https://github.com/sourmash-bio/sourmash_plugin_branchwater)
 `pairwise` command. The output of `pairwise` is distinct from the
 `sourmash compare` output: `pairwise` produces a sparse CSV file that
 contains just the matches above threshold, while `sourmash compare`
 produces a dense numpy matrix.
@@ -154,15 +155,15 @@
     -o mds.10sketches.cmp.png \
     -C 10sketches-categories.csv
 ```
 
 produces this plot:
 ![10-sketches plotted using MDS2](examples/mds2.10sketches.cmp.png)
 
-### Convert `pairwise` output to `sourmash compare` output and plot
+### `pairwise_to_compare` - convert `pairwise` output to `sourmash compare` output and plot
 
 These commands:
 ```
 # build pairwise
 sourmash sig cat sketches/{2,47,48,49,51,52,53,59,60}.sig.zip \
     -o 10sketches.sig.zip
 sourmash scripts pairwise 10sketches.sig.zip -o 10sketches.pairwise.csv
@@ -178,14 +179,34 @@
     -o plot2.pairwise.10sketches.cmp.png
 ```
 
 produce this plot:
 
 ![10-sketches plotted from pairwise](examples/plot2.pairwise.10sketches.cmp.png)
 
+### `plot3` - seaborn clustermap with color categories
+
+The
+[`seaborn` clustermap](https://seaborn.pydata.org/generated/seaborn.clustermap.html)
+offers some nice visualization options.
+
+These commands:
+```
+sourmash compare sketches/{2,47,48,49,51,52,53,59,60}.sig.zip \
+    -o 10sketches.cmp \
+    --labels-to 10sketches.cmp.labels_to.csv
+
+sourmash scripts plot3 10sketches.cmp 10sketches.cmp.labels_to.csv \
+    -o plot3.10sketches.cmp.png -C 10sketches-categories.csv
+```
+
+produce this plot:
+
+![plot3 10 sketches](examples/plot3.10sketches.cmp.png)
+
 
 ## Support
 
 We suggest filing issues in [the main sourmash issue tracker](https://github.com/dib-lab/sourmash/issues) as that receives more attention!
 
 ## Dev docs
```

### Comparing `sourmash_plugin_betterplot-0.3/src/sourmash_plugin_betterplot.py` & `sourmash_plugin_betterplot-0.3.1/src/sourmash_plugin_betterplot.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 import argparse
 import sourmash
 from sourmash import sourmash_args
 import os
 import csv
 from collections import defaultdict
 
-
 import numpy
 import pylab
 import matplotlib.pyplot as plt
 import scipy.cluster.hierarchy as sch
 from sklearn.manifold import MDS
 from scipy.sparse import lil_matrix, csr_matrix
 from matplotlib.lines import Line2D
+import seaborn as sns
 
 from sourmash.logging import debug_literal, error, notify, print_results
 from sourmash.plugins import CommandLinePlugin
 
 
 ###
 
@@ -327,15 +327,15 @@
         force=args.force,
         cut_point=args.cut_point,
         figsize_x=args.figsize_x,
         figsize_y=args.figsize_y,
         dendrogram_only=args.dendrogram_only,
     )
     fig.savefig(args.output_figure, bbox_inches="tight")
-    notify(f"wrote numpy distance matrix to: {args.output_figure}")
+    notify(f"wrote plot to: {args.output_figure}")
 
     # re-order labels along rows, top to bottom
     # reordered_labels = [labelinfo[i] for i in idx1]
 
     # output reordered labels with their clusters?
     if args.cut_point is not None and args.cluster_out:
         cut_point = float(args.cut_point)
@@ -563,7 +563,111 @@
 
     if colors and category_map:
         # create a custom legend of just the categories
         legend_elements = []
         for k, v in category_map.items():
             legend_elements.append(Line2D([0], [0], color=v, label=k, marker="o", lw=0))
         plt.legend(handles=legend_elements)
+
+
+class Command_Plot3(CommandLinePlugin):
+    command = "plot3"  # 'scripts <command>'
+    description = "plot a distance matrix produced by 'sourmash compare'"  # output with -h
+    usage = "sourmash scripts plot <matrix> <labels_csv> -o <output.png>"  # output with no args/bad args as well as -h
+    epilog = epilog  # output with -h
+    formatter_class = argparse.RawTextHelpFormatter  # do not reformat multiline
+
+    def __init__(self, subparser):
+        super().__init__(subparser)
+        subparser.add_argument("distances", help='output from "sourmash compare"')
+        subparser.add_argument(
+            "labels_from", help='output from "sourmash compare --labels-to"'
+        )
+        subparser.add_argument(
+            "--vmin",
+            default=0.0,
+            type=float,
+            help="lower limit of heatmap scale; default=%(default)f",
+        )
+        subparser.add_argument(
+            "--vmax",
+            default=1.0,
+            type=float,
+            help="upper limit of heatmap scale; default=%(default)f",
+        )
+        subparser.add_argument("--figsize-x", type=int, default=11)
+        subparser.add_argument("--figsize-y", type=int, default=8)
+        subparser.add_argument(
+            "--subsample",
+            type=int,
+            metavar="N",
+            help="randomly downsample to this many samples, max",
+        )
+        subparser.add_argument(
+            "--subsample-seed",
+            type=int,
+            default=1,
+            metavar="S",
+            help="random seed for --subsample; default=1",
+        )
+        subparser.add_argument(
+            "-o", "--output-figure", help="output figure to this file", required=True
+        )
+        subparser.add_argument(
+            "-C", "--categories-csv", help="CSV mapping label columns to categories"
+        )
+
+    def main(self, args):
+        super().main(args)
+        D_filename = args.distances
+
+        notify(f"loading comparison matrix from {D_filename}...")
+        with open(D_filename, "rb") as f:
+            D = numpy.load(f)
+        notify(f"...got {D.shape[0]} x {D.shape[1]} matrix.", *D.shape)
+
+        labelfilename = args.labels_from
+        notify(f"loading labels from CSV file '{labelfilename}'")
+        labelinfo = load_labelinfo_csv(labelfilename)
+
+        if len(labelinfo) != D.shape[0]:
+            error("{} labels != matrix size, exiting", len(labeltext))
+            sys.exit(-1)
+
+        # load categories?
+        category_map = None
+        colors = None
+        if args.categories_csv:
+            category_map, colors = load_categories_csv(args.categories_csv, labelinfo)
+        # subsample?
+        if args.subsample:
+            numpy.random.seed(args.subsample_seed)
+
+            sample_idx = list(range(len(labelinfo)))
+            numpy.random.shuffle(sample_idx)
+            sample_idx = sample_idx[: args.subsample]
+
+            np_idx = numpy.array(sample_idx)
+            D = D[numpy.ix_(np_idx, np_idx)]
+            labelinfo = [labelinfo[idx] for idx in sample_idx]
+
+        # turn into dissimilarity matrix
+        #dissim = 1 - D
+        #numpy.fill_diagonal(dissim, 1)
+        dissim = D
+
+        #plot!
+        fig = sns.clustermap(
+            dissim,
+            figsize=(args.figsize_x, args.figsize_y),
+            vmin=args.vmin,
+            vmax=args.vmax,
+            col_colors=colors,
+            yticklabels=[ x["label"].split(' ')[0] for x in labelinfo ],
+            xticklabels=[],
+            cmap="flare",
+        )
+        # turn off column dendrogram
+        fig.ax_row_dendrogram.set_visible(False)
+
+        fig.savefig(args.output_figure, bbox_inches="tight")
+        notify(f"wrote plot to: {args.output_figure}")
```

