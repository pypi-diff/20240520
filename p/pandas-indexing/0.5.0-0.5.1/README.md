# Comparing `tmp/pandas-indexing-0.5.0.tar.gz` & `tmp/pandas_indexing-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-indexing-0.5.0.tar", last modified: Tue Apr  9 15:19:32 2024, max compression
+gzip compressed data, was "pandas_indexing-0.5.1.tar", last modified: Mon May 20 06:30:24 2024, max compression
```

## Comparing `pandas-indexing-0.5.0.tar` & `pandas_indexing-0.5.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:19:32.180150 pandas-indexing-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9212 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-09 15:19:32.180150 pandas-indexing-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:19:32.176149 pandas-indexing-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/docs/AUTHORS.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:19:32.176149 pandas-indexing-0.5.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:19:32.176149 pandas-indexing-0.5.0/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)   400307 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/docs/notebooks/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:19:32.180150 pandas-indexing-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:19:32.172150 pandas-indexing-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:19:32.180150 pandas-indexing-0.5.0/src/pandas_indexing/
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/src/pandas_indexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8792 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/src/pandas_indexing/accessors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/src/pandas_indexing/arithmetics.py
--rw-r--r--   0 runner    (1001) docker     (127)    33455 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/src/pandas_indexing/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:19:32.180150 pandas-indexing-0.5.0/src/pandas_indexing/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/src/pandas_indexing/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/src/pandas_indexing/datasets/remindhighre_power.csv
--rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/src/pandas_indexing/selectors.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/src/pandas_indexing/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/src/pandas_indexing/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-09 15:19:12.000000 pandas-indexing-0.5.0/src/pandas_indexing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:19:32.180150 pandas-indexing-0.5.0/src/pandas_indexing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-09 15:19:32.000000 pandas-indexing-0.5.0/src/pandas_indexing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-09 15:19:32.000000 pandas-indexing-0.5.0/src/pandas_indexing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:19:32.000000 pandas-indexing-0.5.0/src/pandas_indexing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-09 15:19:32.000000 pandas-indexing-0.5.0/src/pandas_indexing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-09 15:19:32.000000 pandas-indexing-0.5.0/src/pandas_indexing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:30:24.281048 pandas_indexing-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-20 06:30:24.281048 pandas_indexing-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:30:24.277048 pandas_indexing-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/docs/AUTHORS.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:30:24.277048 pandas_indexing-0.5.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:30:24.277048 pandas_indexing-0.5.1/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)   400307 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/docs/notebooks/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 06:30:24.281048 pandas_indexing-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:30:24.273048 pandas_indexing-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:30:24.277048 pandas_indexing-0.5.1/src/pandas_indexing/
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/src/pandas_indexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8792 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/src/pandas_indexing/accessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/src/pandas_indexing/arithmetics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33456 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/src/pandas_indexing/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:30:24.281048 pandas_indexing-0.5.1/src/pandas_indexing/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/src/pandas_indexing/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/src/pandas_indexing/datasets/remindhighre_power.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/src/pandas_indexing/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/src/pandas_indexing/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/src/pandas_indexing/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-20 06:30:10.000000 pandas_indexing-0.5.1/src/pandas_indexing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:30:24.281048 pandas_indexing-0.5.1/src/pandas_indexing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-20 06:30:24.000000 pandas_indexing-0.5.1/src/pandas_indexing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-20 06:30:24.000000 pandas_indexing-0.5.1/src/pandas_indexing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 06:30:24.000000 pandas_indexing-0.5.1/src/pandas_indexing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-20 06:30:24.000000 pandas_indexing-0.5.1/src/pandas_indexing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 06:30:24.000000 pandas_indexing-0.5.1/src/pandas_indexing.egg-info/top_level.txt
```

### Comparing `pandas-indexing-0.5.0/.readthedocs.yaml` & `pandas_indexing-0.5.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.5.0/CHANGELOG.rst` & `pandas_indexing-0.5.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 .. currentmodule:: pandas_indexing
 
 Changelog
 =========
 
+v0.5.1 (2024-05-20)
+------------------------------------------------------------
+* Fix :func:`~selectors.ismatch` to not interpret brackets as regex symbols
+* Fix :func:`~selectors.isin` to always return a series (instead of a numpy array)
+
 v0.5.0 (2024-04-09)
 ------------------------------------------------------------
 * **BREAKING**: Change :func:`~core.extractlevel` to drop split levels by default and
   accordingly rename the governing argument from ``drop=False`` to ``keep=False``
   :pull:`53`.
 * Add ``regex=True`` argument to :func:`~core.extractlevel` to use templates as
   manual extraction regex, f.ex.
```

### Comparing `pandas-indexing-0.5.0/CODE_OF_CONDUCT.md` & `pandas_indexing-0.5.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.5.0/CONTRIBUTING.rst` & `pandas_indexing-0.5.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.5.0/LICENSE` & `pandas_indexing-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.5.0/PKG-INFO` & `pandas_indexing-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-indexing
-Version: 0.5.0
+Version: 0.5.1
 Summary: Helpers to facilitate working with pandas indices in particular multiindices
 Author-email: Jonas Hörsch <coroa@posteo.de>
 License: MIT
 Project-URL: changelog, https://github.com/coroa/pandas-indexing/blob/main/CHANGELOG.rst
 Project-URL: documentation, https://pandas-indexing.readthedocs.io/en/latest/
 Project-URL: homepage, https://github.com/coroa/pandas-indexing
 Project-URL: repository, https://github.com/coroa/pandas-indexing.git
```

### Comparing `pandas-indexing-0.5.0/README.rst` & `pandas_indexing-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.5.0/docs/api.rst` & `pandas_indexing-0.5.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.5.0/docs/conf.py` & `pandas_indexing-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.5.0/docs/notebooks/introduction.ipynb` & `pandas_indexing-0.5.1/docs/notebooks/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.5.0/pyproject.toml` & `pandas_indexing-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.5.0/src/pandas_indexing/__init__.py` & `pandas_indexing-0.5.1/src/pandas_indexing/__init__.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.5.0/src/pandas_indexing/accessors.py` & `pandas_indexing-0.5.1/src/pandas_indexing/accessors.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.5.0/src/pandas_indexing/arithmetics.py` & `pandas_indexing-0.5.1/src/pandas_indexing/arithmetics.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.5.0/src/pandas_indexing/core.py` & `pandas_indexing-0.5.1/src/pandas_indexing/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
 @doc(
     index_or_data="""
     index_or_data : DataFrame, Series or Index
         Index, Series or DataFrame to project\
     """
 )
 def projectlevel(index_or_data: T, levels: Sequence[str], axis: Axis = 0) -> T:
-    """Project multiindex to given ``levels``.
+    """Project multiindex to given *levels*.
 
     Drops all levels except the ones explicitly mentioned from a given multiindex
     or an axis of a series or a dataframe.
 
     Parameters
     ----------\
     {index_or_data}
@@ -512,15 +512,15 @@
     how: Literal["left", "right", "inner", "outer"] = "left",
     level: Union[str, int, None] = None,
     sort: bool = False,
     axis: Axis = 0,
     fill_value: Any = no_default,
     fail_on_reorder: bool = False,
 ) -> S:
-    """Semijoin ``data`` by index ``other``.
+    """Semijoin *frame_or_series* by index *other*.
 
     Parameters
     ----------\
     {frame_or_series}
     other : Index
         Other index to join with
     how : {{'left', 'right', 'inner', 'outer'}}
@@ -539,20 +539,20 @@
     Returns
     -------
     DataFrame or Series
 
     Raises
     ------
     ValueError
-        If fail_on_reorder is True and the new index order does not correspond
+        If *fail_on_reorder* is True and the new index order does not correspond
         to the order of other
     ValueError
-        If axis is not 0, "index" or 1, "columns"
+        If *axis* is not 0, "index" or 1, "columns"
     TypeError
-        if frame_or_series does not derive from DataFrame or Series
+        if *frame_or_series* does not derive from DataFrame or Series
 
     See also
     --------
     pandas.Index.join
     """
 
     index = get_axis(frame_or_series, axis)
@@ -608,15 +608,15 @@
 def antijoin(
     index_or_data: S,
     other: Index,
     *,
     level: Union[str, int, None] = None,
     axis: Axis = 0,
 ) -> S:
-    """Antijoin ``index_or_data`` with index ``other``.
+    """Antijoin *index_or_data* with index *other*.
 
     ie remove all occurrences of other from data
 
     Parameters
     ----------\
     {index_or_data}
     other : Index
@@ -732,22 +732,26 @@
     keep: bool = False,
     dropna: bool = True,
     regex: bool = False,
     drop: Optional[bool] = None,
     axis: Axis = 0,
     **templates: str,
 ) -> T:
-    """Extract new index levels with ``templates`` matched against any index
+    """Extract new index levels with *templates* matched against any index
     level.
 
     The ``**templates`` argument defines pairs of level names and templates.
     Given level names are matched against the template, f.ex. ``"Emi|{{gas}}|{{sector}}"``.
     Patterns (``{{gas}}`` or ``{{sector}}``) appearing in the template are extracted
     from the successful matches and added as new levels.
 
+    .. versionchanged:: 0.5.0
+        *drop* replaced by *keep* and default changed to not keep.
+        *regex* added.
+
     Parameters
     ----------\
     {index_or_data}
     template : str, optional
         Extraction template for a single level
     keep : bool, default False
         Whether to keep the split dimension
@@ -826,18 +830,14 @@
     Elec  Bio     0
           Coal    1
     dtype: int64
 
     See also
     --------
     formatlevel
-
-    .. versionchanged:: 0.5.0
-        *drop* replaced by *keep* and default changed to not keep.
-        *regex* added.
     """
     if drop is not None:
         warnings.warn(
             "Argument `drop` is deprecated (use `keep` instead)", DeprecationWarning
         )
         keep = not drop
 
@@ -907,15 +907,15 @@
 )
 def formatlevel(
     index_or_data: T,
     drop: bool = False,
     axis: Axis = 0,
     **templates: str,
 ) -> T:
-    """Format index levels based on a ``template`` which can refer to other
+    """Format index levels based on a *template* which can refer to other
     levels.
 
     Parameters
     ----------\
     {index_or_data}
     drop : bool, default False
         Whether to drop the used index levels
@@ -927,15 +927,15 @@
     Returns
     -------
     Index, Series or DataFrame
 
     Raises
     ------
     ValueError
-        If ``templates`` refer to non-existant levels
+        If *templates* refer to non-existant levels
     """
     if isinstance(index_or_data, Index):
         return _formatlevel(index_or_data, drop, **templates)
 
     index = get_axis(index_or_data, axis)
     return index_or_data.set_axis(_formatlevel(index, drop, **templates), axis=axis)
 
@@ -1142,18 +1142,18 @@
 def add_zeros_like(
     data: T,
     reference: Union[MultiIndex, DataFrame, Series],
     *,
     derive: Optional[Dict[str, MultiIndex]] = None,
     **levels: Sequence[str],
 ) -> T:
-    """Add explicit `levels` to `data` as 0 values.
+    """Add explicit *levels* to *data* as 0 values.
 
-    Remaining levels in `data` not found in `levels` or `derive` are taken from
-    `reference` (or its index).
+    Remaining levels in *data* not found in *levels* or *derive* are taken from
+    *reference* (or its index).
 
     Parameters
     ----------\
     {data}
     reference : Index
         expected level labels (like model, scenario combinations)
     derive : dict
```

### Comparing `pandas-indexing-0.5.0/src/pandas_indexing/datasets/__init__.py` & `pandas_indexing-0.5.1/src/pandas_indexing/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.5.0/src/pandas_indexing/datasets/remindhighre_power.csv` & `pandas_indexing-0.5.1/src/pandas_indexing/datasets/remindhighre_power.csv`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.5.0/src/pandas_indexing/selectors.py` & `pandas_indexing-0.5.1/src/pandas_indexing/selectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,17 @@
             filters = {k: v for k, v in filters.items() if k in index.names}
 
         def apply_filter(value, level):
             if callable(value):
                 return value(index.get_level_values(level))
             return index.isin(np.atleast_1d(value), level=level)
 
-        return reduce(and_, (apply_filter(v, k) for k, v in filters.items()))
+        return Series(
+            reduce(and_, (apply_filter(v, k) for k, v in filters.items())), index
+        )
 
 
 def isin(
     df: Optional[Data] = None, ignore_missing_levels: bool = False, **filters: Any
 ) -> Union[Isin, Series]:
     """Constructs a MultiIndex selector.
```

### Comparing `pandas-indexing-0.5.0/src/pandas_indexing/units.py` & `pandas_indexing-0.5.1/src/pandas_indexing/units.py`

 * *Files identical despite different names*

### Comparing `pandas-indexing-0.5.0/src/pandas_indexing/utils.py` & `pandas_indexing-0.5.1/src/pandas_indexing/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,26 @@
 """Utils module.
 
 Simple utility functions not of greater interest
 """
 
+import re
 from typing import Union
 
 from pandas import DataFrame, Index, Series
 from pandas.util._decorators import doc  # noqa: F401
 
 from .types import Axis
 
 
 def shell_pattern_to_regex(s):
     """
     Escape characters with specific regexp use.
     """
-    return (
-        str(s)
-        .replace("|", r"\|")
-        .replace(".", r"\.")  # `.` has to be replaced before `*`
-        .replace("**", "__starstar__")  # temporarily __starstar__
-        .replace("*", r"[^|]*")
-        .replace("__starstar__", r".*")
-        .replace("+", r"\+")
-        .replace("(", r"\(")
-        .replace(")", r"\)")
-        .replace("$", r"\$")
-    )
+    return re.escape(s).replace(r"\*\*", ".*").replace(r"\*", r"[^|]*")
 
 
 def print_list(x, n):
     """Return a printable string of a list shortened to n characters.
 
     Copied from pyam.utils.print_list by Daniel Huppmann, licensed under
     Apache 2.0.
```

### Comparing `pandas-indexing-0.5.0/src/pandas_indexing.egg-info/PKG-INFO` & `pandas_indexing-0.5.1/src/pandas_indexing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-indexing
-Version: 0.5.0
+Version: 0.5.1
 Summary: Helpers to facilitate working with pandas indices in particular multiindices
 Author-email: Jonas Hörsch <coroa@posteo.de>
 License: MIT
 Project-URL: changelog, https://github.com/coroa/pandas-indexing/blob/main/CHANGELOG.rst
 Project-URL: documentation, https://pandas-indexing.readthedocs.io/en/latest/
 Project-URL: homepage, https://github.com/coroa/pandas-indexing
 Project-URL: repository, https://github.com/coroa/pandas-indexing.git
```

### Comparing `pandas-indexing-0.5.0/src/pandas_indexing.egg-info/SOURCES.txt` & `pandas_indexing-0.5.1/src/pandas_indexing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

