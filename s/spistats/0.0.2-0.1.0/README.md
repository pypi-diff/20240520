# Comparing `tmp/spistats-0.0.2.tar.gz` & `tmp/spistats-0.1.0.tar.gz`

## Comparing `spistats-0.0.2.tar` & `spistats-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,78 @@
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 spistats-0.0.2/src/spistats/__init__.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 spistats-0.0.2/src/spistats/collision/__init__.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 spistats-0.0.2/src/spistats/desynchronization/__init__.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 spistats-0.0.2/src/spistats/desynchronization/dsync_count.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 spistats-0.0.2/src/spistats/desynchronization/law.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 spistats-0.0.2/src/spistats/desynchronization/law_multi.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 spistats-0.0.2/src/spistats/plot/__init__.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 spistats-0.0.2/src/spistats/plot/cdf.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 spistats-0.0.2/test/aa.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 spistats-0.0.2/test/main.py
--rw-r--r--   0        0        0    34668 2020-02-02 00:00:00.000000 spistats-0.0.2/LICENSE
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 spistats-0.0.2/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 spistats-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 spistats-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/Makefile
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/conf.py
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/make.bat
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/modules.rst
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/spistats.collision.rst
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/spistats.desynchronization.rst
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/spistats.plot.rst
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/spistats.rst
+-rw-r--r--   0        0        0   327680 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/doc_lora.tar
+-rw-r--r--   0        0        0   220064 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/doctrees/environment.pickle
+-rw-r--r--   0        0        0    14329 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/doctrees/index.doctree
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/doctrees/modules.doctree
+-rw-r--r--   0        0        0    26217 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/doctrees/spistats.collision.doctree
+-rw-r--r--   0        0        0    66248 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/doctrees/spistats.desynchronization.doctree
+-rw-r--r--   0        0        0     7902 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/doctrees/spistats.doctree
+-rw-r--r--   0        0        0     9694 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/doctrees/spistats.plot.doctree
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/.buildinfo
+-rw-r--r--   0        0        0    10776 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/genindex.html
+-rw-r--r--   0        0        0    14289 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/index.html
+-rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/modules.html
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/objects.inv
+-rw-r--r--   0        0        0     4921 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/py-modindex.html
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/search.html
+-rw-r--r--   0        0        0     8700 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/searchindex.js
+-rw-r--r--   0        0        0    11207 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/spistats.collision.html
+-rw-r--r--   0        0        0    25158 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/spistats.desynchronization.html
+-rw-r--r--   0        0        0    13424 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/spistats.html
+-rw-r--r--   0        0        0     6299 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/spistats.plot.html
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/_modules/index.html
+-rw-r--r--   0        0        0    12825 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/_modules/spistats/collision.html
+-rw-r--r--   0        0        0    20161 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/_modules/spistats/markov.html
+-rw-r--r--   0        0        0    16052 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/_modules/spistats/desynchronization/dsync_count.html
+-rw-r--r--   0        0        0    40983 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/_modules/spistats/desynchronization/law.html
+-rw-r--r--   0        0        0     9578 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/_modules/spistats/desynchronization/law_multi.html
+-rw-r--r--   0        0        0    13340 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/_modules/spistats/plot/cdf.html
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/_sources/modules.rst.txt
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/_sources/spistats.collision.rst.txt
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/_sources/spistats.desynchronization.rst.txt
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/_sources/spistats.plot.rst.txt
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/_sources/spistats.rst.txt
+-rw-r--r--   0        0        0    11143 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/_static/alabaster.css
+-rw-r--r--   0        0        0    15096 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/_static/basic.css
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/_static/custom.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/_static/doctools.js
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/_static/file.png
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/_static/plus.png
+-rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/_static/pygments.css
+-rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 spistats-0.1.0/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 spistats-0.1.0/src/spistats/__init__.py
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 spistats-0.1.0/src/spistats/markov.py
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 spistats-0.1.0/src/spistats/collision/__init__.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 spistats-0.1.0/src/spistats/desynchronization/__init__.py
+-rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 spistats-0.1.0/src/spistats/desynchronization/dsync_count.py
+-rw-r--r--   0        0        0     6078 2020-02-02 00:00:00.000000 spistats-0.1.0/src/spistats/desynchronization/law.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 spistats-0.1.0/src/spistats/desynchronization/law_multi.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 spistats-0.1.0/src/spistats/plot/__init__.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 spistats-0.1.0/src/spistats/plot/cdf.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 spistats-0.1.0/test/aa.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 spistats-0.1.0/test/bb.py
+-rw-r--r--   0        0        0   930998 2020-02-02 00:00:00.000000 spistats-0.1.0/test/data.py
+-rw-r--r--   0        0        0   931062 2020-02-02 00:00:00.000000 spistats-0.1.0/test/data2.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 spistats-0.1.0/test/main.aux
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 spistats-0.1.0/test/main.log
+-rw-r--r--   0        0        0    14735 2020-02-02 00:00:00.000000 spistats-0.1.0/test/main.pdf
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 spistats-0.1.0/test/main.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 spistats-0.1.0/test/main.tex
+-rw-r--r--   0        0        0   607110 2020-02-02 00:00:00.000000 spistats-0.1.0/test/vectors_of_plr.pickle
+-rw-r--r--   0        0        0   154810 2020-02-02 00:00:00.000000 spistats-0.1.0/test/vectors_of_total.pickle
+-rw-r--r--   0        0        0    34668 2020-02-02 00:00:00.000000 spistats-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 spistats-0.1.0/README.md
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 spistats-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 spistats-0.1.0/PKG-INFO
```

### Comparing `spistats-0.0.2/src/spistats/plot/cdf.py` & `spistats-0.1.0/src/spistats/plot/cdf.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,21 @@
+"""This module provides a function to plot the cdf of the law of the number of desynchronization before desynchronization."""
 import numpy as np
 import matplotlib.ticker as mtick
 import matplotlib.pyplot as plt
 
 def cdf(law, scale="linear"):
+    """Plot the cdf of the probability law of the number of desynchronization.
+
+    :param law: Probability law of the number of desynchronization.
+    :type law: spistats.desynchronization.NumberOfDsync()
+    :param scale: (Optional, default="linear") The scale of the graph. Can only be "linear" at the moment. Log scale is planned for a future version.
+    :type scale: string
+    """
+     
     start,end = law.cdf_position()
 
     num_samp = 100
     if scale=="linear":
         x = np.unique(np.linspace(start,end,num_samp).astype(int))
         curve = np.zeros(len(x)).astype(float)
         for xi,xx in enumerate(x):
```

### Comparing `spistats-0.0.2/test/main.py` & `spistats-0.1.0/test/main.py`

 * *Files identical despite different names*

### Comparing `spistats-0.0.2/LICENSE` & `spistats-0.1.0/LICENSE`

 * *Files identical despite different names*

