# Comparing `tmp/named-arrays-0.3.7.tar.gz` & `tmp/named_arrays-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "named-arrays-0.3.7.tar", last modified: Fri Mar 22 06:21:41 2024, max compression
+gzip compressed data, was "named_arrays-0.4.0.tar", last modified: Mon May 20 04:04:57 2024, max compression
```

## Comparing `named-arrays-0.3.7.tar` & `named_arrays-0.4.0.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:41.000195 named-arrays-0.3.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:40.976195 named-arrays-0.3.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:40.980195 named-arrays-0.3.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-03-22 06:21:36.000000 named-arrays-0.3.7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-22 06:21:36.000000 named-arrays-0.3.7/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-22 06:21:36.000000 named-arrays-0.3.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-22 06:21:36.000000 named-arrays-0.3.7/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-03-22 06:21:41.000195 named-arrays-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7331 2024-03-22 06:21:36.000000 named-arrays-0.3.7/README.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-03-22 06:21:36.000000 named-arrays-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:40.984195 named-arrays-0.3.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-22 06:21:36.000000 named-arrays-0.3.7/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:40.984195 named-arrays-0.3.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:36.000000 named-arrays-0.3.7/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:40.984195 named-arrays-0.3.7/docs/_static/favicon_io/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-22 06:21:36.000000 named-arrays-0.3.7/docs/_static/favicon_io/about.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-03-22 06:21:36.000000 named-arrays-0.3.7/docs/_static/favicon_io/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    23247 2024-03-22 06:21:36.000000 named-arrays-0.3.7/docs/_static/favicon_io/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-03-22 06:21:36.000000 named-arrays-0.3.7/docs/_static/favicon_io/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-22 06:21:36.000000 named-arrays-0.3.7/docs/_static/favicon_io/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-22 06:21:36.000000 named-arrays-0.3.7/docs/_static/favicon_io/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-03-22 06:21:36.000000 named-arrays-0.3.7/docs/_static/favicon_io/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-22 06:21:36.000000 named-arrays-0.3.7/docs/_static/favicon_io/site.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:40.984195 named-arrays-0.3.7/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-22 06:21:36.000000 named-arrays-0.3.7/docs/_templates/class_custom.rst
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-22 06:21:36.000000 named-arrays-0.3.7/docs/_templates/function_custom.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-03-22 06:21:36.000000 named-arrays-0.3.7/docs/_templates/module_custom.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-03-22 06:21:36.000000 named-arrays-0.3.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-22 06:21:36.000000 named-arrays-0.3.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-22 06:21:36.000000 named-arrays-0.3.7/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:40.984195 named-arrays-0.3.7/named_arrays/
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36280 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_core_array_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:40.988195 named-arrays-0.3.7/named_arrays/_functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13512 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_functions/function_array_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_functions/function_named_array_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23039 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_functions/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:40.988195 named-arrays-0.3.7/named_arrays/_functions/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_functions/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27923 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_functions/tests/test_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:40.988195 named-arrays-0.3.7/named_arrays/_matrices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_matrices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:40.992195 named-arrays-0.3.7/named_arrays/_matrices/cartesian/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_matrices/cartesian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_matrices/cartesian/matrices_cartesian.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_matrices/cartesian/matrices_cartesian_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_matrices/cartesian/matrices_cartesian_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_matrices/cartesian/matrices_cartesian_nd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:40.992195 named-arrays-0.3.7/named_arrays/_matrices/cartesian/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_matrices/cartesian/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_matrices/cartesian/tests/test_matrices_cartesian.py
--rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_matrices/cartesian/tests/test_matrices_cartesian_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    14049 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_matrices/matrices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_matrices/matrices_directional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_matrices/matrices_input_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_matrices/matrices_positional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_matrices/matrices_spectral.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_matrices/matrices_spectral_directional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_matrices/matrices_spectral_positional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_matrices/matrices_temporal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_matrices/matrices_temporal_spectral.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_matrices/matrices_temporal_spectral_directional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_matrices/matrices_temporal_spectral_positional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:40.992195 named-arrays-0.3.7/named_arrays/_matrices/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_matrices/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_matrices/tests/test_matrices.py
--rw-r--r--   0 runner    (1001) docker     (127)    18000 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_named_array_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:40.992195 named-arrays-0.3.7/named_arrays/_scalars/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_scalars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24010 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_scalars/scalar_array_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23920 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_scalars/scalar_named_array_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    36210 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_scalars/scalars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:40.992195 named-arrays-0.3.7/named_arrays/_scalars/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_scalars/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48768 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_scalars/tests/test_scalars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:40.992195 named-arrays-0.3.7/named_arrays/_scalars/uncertainties/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_scalars/uncertainties/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:40.992195 named-arrays-0.3.7/named_arrays/_scalars/uncertainties/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_scalars/uncertainties/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38913 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_scalars/uncertainties/tests/test_uncertainties.py
--rw-r--r--   0 runner    (1001) docker     (127)    29794 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_scalars/uncertainties/uncertainties.py
--rw-r--r--   0 runner    (1001) docker     (127)    25385 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_scalars/uncertainties/uncertainties_array_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14514 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_scalars/uncertainties/uncertainties_named_array_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:40.996195 named-arrays-0.3.7/named_arrays/_vectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:40.996195 named-arrays-0.3.7/named_arrays/_vectors/cartesian/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/cartesian/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:40.996195 named-arrays-0.3.7/named_arrays/_vectors/cartesian/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/cartesian/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/cartesian/tests/test_vectors_cartesian.py
--rw-r--r--   0 runner    (1001) docker     (127)    14705 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/cartesian/tests/test_vectors_cartesian_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    15853 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/cartesian/tests/test_vectors_cartesian_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8889 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/cartesian/tests/test_vectors_cartesian_nd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/cartesian/vectors_cartesian.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/cartesian/vectors_cartesian_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/cartesian/vectors_cartesian_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/cartesian/vectors_cartesian_nd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:41.000195 named-arrays-0.3.7/named_arrays/_vectors/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26127 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/tests/test_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/tests/test_vectors_directional.py
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/tests/test_vectors_input_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/tests/test_vectors_positional.py
--rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/tests/test_vectors_spectral.py
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/tests/test_vectors_spectral_directional.py
--rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/tests/test_vectors_spectral_positional.py
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/tests/test_vectors_temporal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/tests/test_vectors_temporal_spectral.py
--rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/tests/test_vectors_temporal_spectral_directional.py
--rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/tests/test_vectors_temporal_spectral_positional.py
--rw-r--r--   0 runner    (1001) docker     (127)    23972 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/vector_array_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13878 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/vector_named_array_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    29204 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/vectors_directional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/vectors_input_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/vectors_positional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/vectors_spectral.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/vectors_spectral_directional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/vectors_spectral_positional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/vectors_temporal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/vectors_temporal_spectral.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/vectors_temporal_spectral_directional.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/_vectors/vectors_temporal_spectral_positional.py
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)    24562 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/plt.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:41.000195 named-arrays-0.3.7/named_arrays/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52122 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/tests/test_transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)    14859 2024-03-22 06:21:36.000000 named-arrays-0.3.7/named_arrays/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 06:21:41.000195 named-arrays-0.3.7/named_arrays.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-03-22 06:21:40.000000 named-arrays-0.3.7/named_arrays.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-03-22 06:21:40.000000 named-arrays-0.3.7/named_arrays.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 06:21:40.000000 named-arrays-0.3.7/named_arrays.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-22 06:21:40.000000 named-arrays-0.3.7/named_arrays.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-22 06:21:40.000000 named-arrays-0.3.7/named_arrays.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-22 06:21:36.000000 named-arrays-0.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-22 06:21:36.000000 named-arrays-0.3.7/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 06:21:41.000195 named-arrays-0.3.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:57.816921 named_arrays-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:57.792921 named_arrays-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:57.796921 named_arrays-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-20 04:04:53.000000 named_arrays-0.4.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-20 04:04:53.000000 named_arrays-0.4.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 04:04:53.000000 named_arrays-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-20 04:04:53.000000 named_arrays-0.4.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-20 04:04:57.816921 named_arrays-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7331 2024-05-20 04:04:53.000000 named_arrays-0.4.0/README.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-05-20 04:04:53.000000 named_arrays-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:57.796921 named_arrays-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-20 04:04:53.000000 named_arrays-0.4.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:57.796921 named_arrays-0.4.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:53.000000 named_arrays-0.4.0/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:57.800921 named_arrays-0.4.0/docs/_static/favicon_io/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-20 04:04:53.000000 named_arrays-0.4.0/docs/_static/favicon_io/about.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-05-20 04:04:53.000000 named_arrays-0.4.0/docs/_static/favicon_io/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23247 2024-05-20 04:04:53.000000 named_arrays-0.4.0/docs/_static/favicon_io/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-05-20 04:04:53.000000 named_arrays-0.4.0/docs/_static/favicon_io/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-20 04:04:53.000000 named_arrays-0.4.0/docs/_static/favicon_io/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-20 04:04:53.000000 named_arrays-0.4.0/docs/_static/favicon_io/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-20 04:04:53.000000 named_arrays-0.4.0/docs/_static/favicon_io/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-20 04:04:53.000000 named_arrays-0.4.0/docs/_static/favicon_io/site.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:57.800921 named_arrays-0.4.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-20 04:04:53.000000 named_arrays-0.4.0/docs/_templates/class_custom.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-20 04:04:53.000000 named_arrays-0.4.0/docs/_templates/function_custom.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-20 04:04:53.000000 named_arrays-0.4.0/docs/_templates/module_custom.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-20 04:04:53.000000 named_arrays-0.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-20 04:04:53.000000 named_arrays-0.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-20 04:04:53.000000 named_arrays-0.4.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:57.800921 named_arrays-0.4.0/named_arrays/
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36948 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_core_array_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:57.804921 named_arrays-0.4.0/named_arrays/_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13512 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_functions/function_array_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_functions/function_named_array_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22857 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_functions/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:57.804921 named_arrays-0.4.0/named_arrays/_functions/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_functions/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28125 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_functions/tests/test_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:57.804921 named_arrays-0.4.0/named_arrays/_matrices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_matrices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:57.804921 named_arrays-0.4.0/named_arrays/_matrices/cartesian/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_matrices/cartesian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_matrices/cartesian/matrices_cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_matrices/cartesian/matrices_cartesian_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_matrices/cartesian/matrices_cartesian_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_matrices/cartesian/matrices_cartesian_nd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:57.808921 named_arrays-0.4.0/named_arrays/_matrices/cartesian/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_matrices/cartesian/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_matrices/cartesian/tests/test_matrices_cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_matrices/cartesian/tests/test_matrices_cartesian_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14055 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_matrices/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_matrices/matrices_directional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_matrices/matrices_input_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_matrices/matrices_positional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_matrices/matrices_spectral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_matrices/matrices_spectral_directional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_matrices/matrices_spectral_positional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_matrices/matrices_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_matrices/matrices_temporal_spectral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_matrices/matrices_temporal_spectral_directional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_matrices/matrices_temporal_spectral_positional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:57.808921 named_arrays-0.4.0/named_arrays/_matrices/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_matrices/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_matrices/tests/test_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23065 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_named_array_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:57.808921 named_arrays-0.4.0/named_arrays/_scalars/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_scalars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24010 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_scalars/scalar_array_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28529 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_scalars/scalar_named_array_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36138 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_scalars/scalars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:57.808921 named_arrays-0.4.0/named_arrays/_scalars/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_scalars/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51041 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_scalars/tests/test_scalars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:57.808921 named_arrays-0.4.0/named_arrays/_scalars/uncertainties/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_scalars/uncertainties/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:57.808921 named_arrays-0.4.0/named_arrays/_scalars/uncertainties/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_scalars/uncertainties/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39193 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_scalars/uncertainties/tests/test_uncertainties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29596 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_scalars/uncertainties/uncertainties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25385 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_scalars/uncertainties/uncertainties_array_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18553 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_scalars/uncertainties/uncertainties_named_array_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:57.812921 named_arrays-0.4.0/named_arrays/_vectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:57.812921 named_arrays-0.4.0/named_arrays/_vectors/cartesian/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/cartesian/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:57.812921 named_arrays-0.4.0/named_arrays/_vectors/cartesian/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/cartesian/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/cartesian/tests/test_vectors_cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15511 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/cartesian/tests/test_vectors_cartesian_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15853 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/cartesian/tests/test_vectors_cartesian_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8889 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/cartesian/tests/test_vectors_cartesian_nd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/cartesian/vectors_cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/cartesian/vectors_cartesian_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/cartesian/vectors_cartesian_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/cartesian/vectors_cartesian_nd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:57.816921 named_arrays-0.4.0/named_arrays/_vectors/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26796 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/tests/test_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/tests/test_vectors_directional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/tests/test_vectors_input_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/tests/test_vectors_positional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/tests/test_vectors_spectral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/tests/test_vectors_spectral_directional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/tests/test_vectors_spectral_positional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/tests/test_vectors_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/tests/test_vectors_temporal_spectral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/tests/test_vectors_temporal_spectral_directional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/tests/test_vectors_temporal_spectral_positional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23972 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/vector_array_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16107 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/vector_named_array_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28767 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/vectors_directional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/vectors_input_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/vectors_positional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/vectors_spectral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/vectors_spectral_directional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/vectors_spectral_positional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/vectors_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/vectors_temporal_spectral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/vectors_temporal_spectral_directional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/_vectors/vectors_temporal_spectral_positional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24563 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/plt.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:57.816921 named_arrays-0.4.0/named_arrays/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53204 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/tests/test_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14859 2024-05-20 04:04:53.000000 named_arrays-0.4.0/named_arrays/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:04:57.816921 named_arrays-0.4.0/named_arrays.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-20 04:04:57.000000 named_arrays-0.4.0/named_arrays.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-05-20 04:04:57.000000 named_arrays-0.4.0/named_arrays.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 04:04:57.000000 named_arrays-0.4.0/named_arrays.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-20 04:04:57.000000 named_arrays-0.4.0/named_arrays.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 04:04:57.000000 named_arrays-0.4.0/named_arrays.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-20 04:04:53.000000 named_arrays-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-20 04:04:53.000000 named_arrays-0.4.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 04:04:57.816921 named_arrays-0.4.0/setup.cfg
```

### Comparing `named-arrays-0.3.7/.github/workflows/publish.yml` & `named_arrays-0.4.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/.github/workflows/tests.yml` & `named_arrays-0.4.0/.github/workflows/tests.yml`

 * *Files 14% similar despite different names*

```diff
@@ -4,44 +4,43 @@
 on:
   push:
     branches:
       - main
   pull_request:
 
 jobs:
-  build:
+  test:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        array-type: ["tests", "_scalars", "_vectors", "_matrices", "_functions"]
+        python-version: ["3.12", ]
         os: [
           ubuntu-latest,
           windows-latest,
           macOS-latest,
         ]
-        python-version: ["3.12", ]
-    name: ${{ matrix.array-type }}, ${{ matrix.os }}, Python ${{ matrix.python-version }} lint and test
+        group: [1, 2, 3, 4, 5, 6]
+    name: Python ${{ matrix.python-version }}, ${{ matrix.os }}, Group ${{matrix.group}} test
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install package
         run: |
           python -m pip install --upgrade pip
           pip install setuptools wheel
           pip install -e .[test]
       - name: Test with pytest
         run: |
           pip install pytest pytest-cov
-          pytest -c pytest.ini --cov=. --cov-report=xml  named_arrays/${{ matrix.array-type }}
-      - name: Upload coverage to Codecov
-        uses: codecov/codecov-action@v3
+          pytest -c pytest.ini --cov=. --cov-report=xml  --splits 6 --group ${{matrix.group}}
+      - uses: codecov/codecov-action@v3
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
           file: coverage.xml
           flags: unittests
           env_vars: OS,PYTHON
           name: codecov-umbrella
           fail_ci_if_error: true
```

### Comparing `named-arrays-0.3.7/PKG-INFO` & `named_arrays-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: named-arrays
-Version: 0.3.7
+Version: 0.4.0
 Summary: Numpy arrays with labeled axes, similar to xarray but with support for uncertainties
 Author-email: "Roy T. Smart" <roytsmart@gmail.com>, "Jacob D. Parker" <jacobdparker@gmail.com>
 Project-URL: Homepage, https://github.com/sun-data/named-arrays
 Project-URL: Documentation, https://named-arrays.readthedocs.io/en/latest
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: typing_extensions
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: scipy
 Requires-Dist: astropy
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-split; extra == "test"
 Provides-Extra: doc
 Requires-Dist: pytest; extra == "doc"
 Requires-Dist: graphviz; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints; extra == "doc"
 Requires-Dist: pydata-sphinx-theme; extra == "doc"
 Requires-Dist: ipykernel; extra == "doc"
 Requires-Dist: jupyter-sphinx; extra == "doc"
```

### Comparing `named-arrays-0.3.7/README.ipynb` & `named_arrays-0.4.0/README.ipynb`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/README.md` & `named_arrays-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/docs/Makefile` & `named_arrays-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/docs/_static/favicon_io/android-chrome-192x192.png` & `named_arrays-0.4.0/docs/_static/favicon_io/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/docs/_static/favicon_io/android-chrome-512x512.png` & `named_arrays-0.4.0/docs/_static/favicon_io/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/docs/_static/favicon_io/apple-touch-icon.png` & `named_arrays-0.4.0/docs/_static/favicon_io/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/docs/_static/favicon_io/favicon-32x32.png` & `named_arrays-0.4.0/docs/_static/favicon_io/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/docs/_static/favicon_io/favicon.ico` & `named_arrays-0.4.0/docs/_static/favicon_io/favicon.ico`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/docs/_templates/class_custom.rst` & `named_arrays-0.4.0/docs/_templates/class_custom.rst`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/docs/_templates/module_custom.rst` & `named_arrays-0.4.0/docs/_templates/module_custom.rst`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/docs/conf.py` & `named_arrays-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/docs/make.bat` & `named_arrays-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/__init__.py` & `named_arrays-0.4.0/named_arrays/__init__.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_core.py` & `named_arrays-0.4.0/named_arrays/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     'AbstractSymmetricRangeMixin',
     'AbstractRandomSample',
     'AbstractParameterizedArray',
     'AbstractLinearParameterizedArrayMixin',
     'AbstractArrayRange',
     'AbstractSpace',
     'AbstractLinearSpace',
+    'strata',
     'AbstractStratifiedRandomSpace',
     'AbstractLogarithmicSpace',
     'AbstractGeometricSpace',
     'AbstractUniformRandomSample',
     'AbstractNormalRandomSample',
     'AbstractPoissonRandomSample',
 ]
@@ -356,22 +357,14 @@
         if this array has multiple components, broadcast them against each other.
 
         Equivalent to ``a.broadcast_to(a.shape)``
         """
         a = self.explicit
         return a.broadcast_to(a.shape)
 
-    @property
-    @abc.abstractmethod
-    def centers(self: Self) -> AbstractArray:
-        """
-        The central value for this array. Usually returns this array unless an instance of
-        :class:`named_arrays.AbstractStratifiedRandomSpace`
-        """
-
     @abc.abstractmethod
     def astype(
             self: Self,
             dtype: str | np.dtype | Type,
             order: str = 'K',
             casting='unsafe',
             subok: bool = True,
@@ -782,16 +775,16 @@
         item_base_0 = {**item_base, axis: x0}
         item_base_1 = {**item_base, axis: x1}
 
         if item:
             y0 = self._interp_linear_recursive(item=item, item_base=item_base_0, )
             y1 = self._interp_linear_recursive(item=item, item_base=item_base_1, )
         else:
-            y0 = self[item_base_0]
-            y1 = self[item_base_1]
+            y0 = self[item_base_0].astype(float)
+            y1 = self[item_base_1].astype(float)
 
         result = y0 + (x - x0) * (y1 - y0)
         return result
 
     def interp_linear(
             self: Self,
             item: dict[str, Self],
@@ -1047,18 +1040,14 @@
         return na.random.uniform(
             low=start,
             high=stop,
             shape_random=self.shape_random,
             seed=self.seed,
         )
 
-    @property
-    def centers(self: Self) -> Self:
-        return self
-
 
 @dataclasses.dataclass
 class AbstractNormalRandomSample(
     AbstractSymmetricRangeMixin,
     AbstractRandomSample,
     Generic[CenterT, WidthT],
 ):
@@ -1075,18 +1064,14 @@
         return na.random.normal(
             loc=center,
             scale=width,
             shape_random=self.shape_random,
             seed=self.seed,
         )
 
-    @property
-    def centers(self: Self) -> Self:
-        return self
-
 
 @dataclasses.dataclass
 class AbstractPoissonRandomSample(
     AbstractRandomSample,
     Generic[CenterT],
 ):
     center: CenterT = dataclasses.MISSING
@@ -1099,18 +1084,14 @@
 
         return na.random.poisson(
             lam=center,
             shape_random=self.shape_random,
             seed=self.seed,
         )
 
-    @property
-    def centers(self: Self) -> Self:
-        return self
-
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractParameterizedArray(
     AbstractImplicitArray,
 ):
 
     @property
@@ -1161,18 +1142,14 @@
             start=start,
             stop=stop,
             axis=self.axis,
             step=self.step,
         )
 
     @property
-    def centers(self: Self) -> Self:
-        return self
-
-    @property
     def num(self: Self) -> int:
         return np.ceil((self.stop - self.start) / self.step).astype(int)
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractSpace(
     AbstractParameterizedArray,
@@ -1193,67 +1170,123 @@
     Generic[StartT, StopT, AxisT, NumT],
 ):
     start: StartT = dataclasses.MISSING
     stop: StopT = dataclasses.MISSING
     axis: AxisT = dataclasses.MISSING
     num: NumT = 11
     endpoint: bool = True
+    centers: bool = False
 
     @property
     def explicit(self: Self) -> AbstractExplicitArray:
         return na.linspace(
             start=self._attr_normalized("start"),
             stop=self._attr_normalized("stop"),
             axis=self.axis,
             num=self.num,
-            endpoint=self.endpoint
+            endpoint=self.endpoint,
+            centers=self.centers,
         )
 
     @property
-    def centers(self: Self) -> Self:
-        return self
-
-    @property
     def step(self: Self) -> AbstractArray:
-        if self.endpoint:
-            return self.range / (self.num - 1)
+        if self.num == 1:
+            return self.range
         else:
-            return self.range / self.num
+            num = self.num
+            if self.endpoint:
+                num = num - 1
+            if self.centers:
+                num = num - 1
+            return self.range / num
+
+
+def strata(a: AbstractArray) -> AbstractArray:
+    """
+    If ``a`` is an instance of :class:`AbstractStratifiedRandomSpace`,
+    return ``a.strata``, otherwise return ``a``
+
+    Parameters
+    ----------
+    a
+        An array to isolate the strata of.
+
+    Examples
+    --------
+
+    Make a scatterplot of a 2D stratified random array and the centers of
+    the strata.
+
+    .. jupyter-execute::
+
+        import matplotlib.pyplot as plt
+        import named_arrays as na
+
+        # Define a 2D stratified random array.
+        a = na.Cartesian2dVectorStratifiedRandomSpace(
+            start=-1,
+            stop=1,
+            axis=na.Cartesian2dVectorArray("x", "y"),
+            num=11,
+        )
+
+        # Isolate the strata of the array
+        strata = na.strata(a)
+
+        # Plot the array and the strata
+        fig, ax = plt.subplots()
+        na.plt.scatter(
+            a.x,
+            a.y,
+            ax=ax,
+        )
+        na.plt.scatter(
+            strata.x,
+            strata.y,
+            ax=ax,
+        );
+    """
+    if isinstance(a, AbstractStratifiedRandomSpace):
+        return a.strata
+    else:
+        return a
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractStratifiedRandomSpace(
     AbstractRandomMixin,
     AbstractLinearSpace[StartT, StopT, AxisT, NumT],
 ):
+    centers: bool = True
     seed: None | int = None
 
     @property
     def explicit(self: Self) -> AbstractExplicitArray:
-        result = self.centers
+        result = self.strata
 
         step_size = self.step
 
         delta = na.random.uniform(
             low=-step_size / 2,
             high=step_size / 2,
             shape_random=result.shape,
             seed=self.seed,
         )
 
         return result + delta
 
     @property
-    def centers(self: Self) -> AbstractExplicitArray:
+    def strata(self: Self) -> AbstractExplicitArray:
         return na.linspace(
             start=self._attr_normalized("start"),
             stop=self._attr_normalized("stop"),
             num=self.num,
             endpoint=self.endpoint,
             axis=self.axis,
+            centers=self.centers,
         )
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractLogarithmicSpace(
     AbstractRangeMixin,
     AbstractSpace,
@@ -1274,18 +1307,14 @@
             axis=self.axis,
             num=self.num,
             endpoint=self.endpoint,
             base=self.base,
         )
 
     @property
-    def centers(self: Self) -> Self:
-        return self
-
-    @property
     def start(self: Self) -> ArrayLike:
         return self.base ** self.start_exponent
 
     @property
     def stop(self: Self) -> ArrayLike:
         return self.base ** self.stop_exponent
 
@@ -1307,11 +1336,7 @@
         return na.geomspace(
             start=self._attr_normalized("start"),
             stop=self._attr_normalized("stop"),
             axis=self.axis,
             num=self.num,
             endpoint=self.endpoint,
         )
-
-    @property
-    def centers(self: Self) -> Self:
-        return self
```

### Comparing `named-arrays-0.3.7/named_arrays/_core_array_functions.py` & `named_arrays-0.4.0/named_arrays/_core_array_functions.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_functions/function_array_functions.py` & `named_arrays-0.4.0/named_arrays/_functions/function_array_functions.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_functions/function_named_array_functions.py` & `named_arrays-0.4.0/named_arrays/_functions/function_named_array_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,25 +74,35 @@
         ),
     )
 
 
 @_implements(na.unit)
 def unit(
         a: na.AbstractFunctionArray,
+        unit_dimensionless: None | float | u.UnitBase = None,
         squeeze: bool = True,
 ) -> None | u.UnitBase | na.AbstractArray:
-    return na.unit(a.outputs, squeeze=squeeze)
+    return na.unit(
+        a=a.outputs,
+        unit_dimensionless=unit_dimensionless,
+        squeeze=squeeze,
+    )
 
 
 @_implements(na.unit_normalized)
 def unit_normalized(
         a: na.AbstractFunctionArray,
+        unit_dimensionless: float | u.UnitBase,
         squeeze: bool = True,
 ) -> u.UnitBase | na.AbstractArray:
-    return na.unit_normalized(a.outputs, squeeze=squeeze)
+    return na.unit_normalized(
+        a.outputs,
+        unit_dimensionless=unit_dimensionless,
+        squeeze=squeeze,
+    )
 
 
 @_implements(na.plt.pcolormesh)
 def pcolormesh(
     *XY: na.AbstractArray,
     C: na.AbstractFunctionArray,
     components: None | tuple[str, str] = None,
```

### Comparing `named-arrays-0.3.7/named_arrays/_functions/functions.py` & `named_arrays-0.4.0/named_arrays/_functions/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,21 +56,14 @@
     @property
     def value(self) -> FunctionArray:
         return self.type_explicit(
             inputs=self.inputs,
             outputs=self.outputs.value,
         )
 
-    @property
-    def centers(self) -> FunctionArray:
-        return self.type_explicit(
-            inputs=self.inputs.centers,
-            outputs=self.outputs.centers,
-        )
-
     def astype(
             self,
             dtype: str | np.dtype | type,
             order: str = 'K',
             casting='unsafe',
             subok: bool = True,
             copy: bool = True,
```

### Comparing `named-arrays-0.3.7/named_arrays/_functions/tests/test_functions.py` & `named_arrays-0.4.0/named_arrays/_functions/tests/test_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -695,14 +695,20 @@
 
         @pytest.mark.skip
         class TestOptimizeRoot(
             named_arrays.tests.test_core.AbstractTestAbstractArray.TestNamedArrayFunctions.TestOptimizeRoot,
         ):
             pass
 
+        @pytest.mark.skip
+        class TestOptimizeMinimum(
+            named_arrays.tests.test_core.AbstractTestAbstractArray.TestNamedArrayFunctions.TestOptimizeMinimum,
+        ):
+            pass
+
 
 @pytest.mark.parametrize("array", _function_arrays())
 class TestFunctionArray(
     AbstractTestAbstractFunctionArray,
     named_arrays.tests.test_core.AbstractTestAbstractExplicitArray,
 ):
```

### Comparing `named-arrays-0.3.7/named_arrays/_matrices/cartesian/matrices_cartesian.py` & `named_arrays-0.4.0/named_arrays/_matrices/cartesian/matrices_cartesian.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_matrices/cartesian/matrices_cartesian_2d.py` & `named_arrays-0.4.0/named_arrays/_matrices/cartesian/matrices_cartesian_2d.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,14 +106,15 @@
 ):
     pass
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractImplicitCartesian2dMatrixArray(
     na.AbstractImplicitCartesian2dVectorArray,
+    na.AbstractImplicitMatrixArray,
     AbstractCartesian2dMatrixArray,
 ):
     pass
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class Cartesian2dIdentityMatrixArray(
@@ -123,14 +124,20 @@
     @property
     def explicit(self):
         return na.Cartesian2dMatrixArray(
             x=na.Cartesian2dVectorArray(x=1, y=0),
             y=na.Cartesian2dVectorArray(x=0, y=1),
         )
 
+    def power(
+        self,
+        exponent: float | na.AbstractScalar,
+    ) -> AbstractCartesian2dMatrixArray:
+        return self
+
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractCartesian2dRotationMatrixArray(
     AbstractImplicitCartesian2dMatrixArray,
 ):
 
     @property
```

### Comparing `named-arrays-0.3.7/named_arrays/_matrices/cartesian/matrices_cartesian_3d.py` & `named_arrays-0.4.0/named_arrays/_matrices/cartesian/matrices_cartesian_3d.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_matrices/cartesian/matrices_cartesian_nd.py` & `named_arrays-0.4.0/named_arrays/_matrices/cartesian/matrices_cartesian_nd.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_matrices/cartesian/tests/test_matrices_cartesian.py` & `named_arrays-0.4.0/named_arrays/_matrices/cartesian/tests/test_matrices_cartesian.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_matrices/cartesian/tests/test_matrices_cartesian_2d.py` & `named_arrays-0.4.0/named_arrays/_matrices/cartesian/tests/test_matrices_cartesian_2d.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,40 +12,14 @@
 ]
 
 _num_x = named_arrays.tests.test_core.num_x
 _num_y = named_arrays.tests.test_core.num_y
 _num_distribution = named_arrays.tests.test_core.num_distribution
 
 
-class AbstractTestAbstractCartesian2dMatrixArray(
-    test_matrices_cartesian.AbstractTestAbstractCartesianMatrixArray,
-    named_arrays._vectors.cartesian.tests.test_vectors_cartesian_2d.AbstractTestAbstractCartesian2dVectorArray,
-):
-
-    @pytest.mark.parametrize("exponent", [1, 2, 5])
-    def test_power(
-        self,
-        array: na.AbstractCartesian2dMatrixArray,
-        exponent: int
-    ):
-        if na.unit(array.length) is not None:
-            return
-
-        if len(array.cartesian_nd.entries) != 4:
-            return
-
-        result = array.power(exponent)
-
-        result_expected = na.Cartesian2dIdentityMatrixArray()
-        for i in range(exponent):
-            result_expected = result_expected @ array
-
-        assert np.allclose(result, result_expected)
-
-
 def _cartesian_2d_matrices():
     arrays_xx = [
         4,
         na.ScalarUniformRandomSample(-4, 4, shape_random=dict(y=_num_y)),
     ]
     arrays_xy = [
         1,
@@ -160,27 +134,21 @@
                 y=na.Cartesian2dMatrixArray(
                     x=na.Cartesian2dVectorArray(x=1, y=2),
                     y=na.Cartesian2dVectorArray(x=1, y=2)),
             ),
         )
     )
 
-
     return scalars + matrices
 
 
-@pytest.mark.parametrize(
-    argnames='array',
-    argvalues=_cartesian_2d_matrices()
-)
-class TestCartesian2dMatrixArray(
-    AbstractTestAbstractCartesian2dMatrixArray,
+class AbstractTestAbstractCartesian2dMatrixArray(
     test_matrices_cartesian.AbstractTestAbstractCartesianMatrixArray,
+    named_arrays._vectors.cartesian.tests.test_vectors_cartesian_2d.AbstractTestAbstractCartesian2dVectorArray,
 ):
-
     @pytest.mark.parametrize(
         argnames='item',
         argvalues=[
             dict(y=0),
             dict(y=slice(0, 1)),
             dict(y=na.ScalarArrayRange(0, 2, axis='y')),
             dict(
@@ -223,15 +191,15 @@
                     y=na.ScalarLinearSpace(0, 1, axis='y', num=_num_y) > 0.4,
                 ),
                 y=na.Cartesian2dVectorArray(
                     x=na.ScalarLinearSpace(0, 1, axis='y', num=_num_y) > 0.5,
                     y=na.ScalarLinearSpace(0, 1, axis='y', num=_num_y) > 0.6,
                 ),
             ),
-        ]
+            ]
     )
     def test__getitem__(
             self,
             array: na.AbstractCartesian2dVectorArray,
             item: dict[str, int | slice | na.AbstractArray] | na.AbstractArray
     ):
         super().test__getitem__(array=array, item=item)
@@ -244,18 +212,62 @@
 
     @pytest.mark.parametrize('array_2', _cartesian_2d_matrices_2())
     class TestMatmul(
         test_matrices_cartesian.AbstractTestAbstractCartesianMatrixArray.TestMatmul
     ):
         pass
 
+    @pytest.mark.parametrize("exponent", [1, 2, 5])
+    def test_power(
+        self,
+        array: na.AbstractCartesian2dMatrixArray,
+        exponent: int
+    ):
+        if na.unit(array.length) is not None:
+            return
+
+        if len(array.cartesian_nd.entries) != 4:
+            return
+
+        result = array.power(exponent)
+
+        result_expected = na.Cartesian2dIdentityMatrixArray()
+        for i in range(exponent):
+            result_expected = result_expected @ array
+
+        assert np.allclose(result, result_expected)
+
+
+@pytest.mark.parametrize(
+    argnames='array',
+    argvalues=_cartesian_2d_matrices()
+)
+class TestCartesian2dMatrixArray(
+    AbstractTestAbstractCartesian2dMatrixArray,
+    test_matrices_cartesian.AbstractTestAbstractCartesianMatrixArray,
+):
+    pass
+
 
 @pytest.mark.parametrize("type_array", [na.Cartesian2dMatrixArray])
 class TestCartesian2dMatrixArrayCreation(
     test_matrices_cartesian.AbstractTestAbstractExplicitCartesianMatrixArrayCreation,
 ):
 
     @pytest.mark.parametrize("like", [None] + _cartesian_2d_matrices())
     class TestFromScalarArray(
         test_matrices_cartesian.AbstractTestAbstractExplicitCartesianMatrixArrayCreation.TestFromScalarArray,
     ):
         pass
+
+
+@pytest.mark.parametrize(
+    argnames="array",
+    argvalues=[
+        na.Cartesian2dIdentityMatrixArray(),
+    ],
+)
+class TestCartesian2dIdentityMatrixArray(
+    test_matrices_cartesian.AbstractTestAbstractImplicitCartesianMatrixArray,
+    AbstractTestAbstractCartesian2dMatrixArray,
+):
+    pass
```

### Comparing `named-arrays-0.3.7/named_arrays/_matrices/matrices.py` & `named_arrays-0.4.0/named_arrays/_matrices/matrices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from typing import Type
+from typing import Type, Self
 import abc
 import dataclasses
 import named_arrays as na
 import numpy as np
 
 __all__ = [
     'AbstractMatrixArray',
```

### Comparing `named-arrays-0.3.7/named_arrays/_matrices/matrices_directional.py` & `named_arrays-0.4.0/named_arrays/_matrices/matrices_directional.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_matrices/matrices_input_output.py` & `named_arrays-0.4.0/named_arrays/_matrices/matrices_input_output.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_matrices/matrices_positional.py` & `named_arrays-0.4.0/named_arrays/_matrices/matrices_positional.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_matrices/matrices_spectral.py` & `named_arrays-0.4.0/named_arrays/_matrices/matrices_spectral.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_matrices/matrices_spectral_directional.py` & `named_arrays-0.4.0/named_arrays/_matrices/matrices_spectral_directional.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_matrices/matrices_spectral_positional.py` & `named_arrays-0.4.0/named_arrays/_matrices/matrices_spectral_positional.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_matrices/matrices_temporal.py` & `named_arrays-0.4.0/named_arrays/_matrices/matrices_temporal.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_matrices/matrices_temporal_spectral.py` & `named_arrays-0.4.0/named_arrays/_matrices/matrices_temporal_spectral.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_matrices/matrices_temporal_spectral_directional.py` & `named_arrays-0.4.0/named_arrays/_matrices/matrices_temporal_spectral_directional.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_matrices/matrices_temporal_spectral_positional.py` & `named_arrays-0.4.0/named_arrays/_matrices/matrices_temporal_spectral_positional.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_matrices/tests/test_matrices.py` & `named_arrays-0.4.0/named_arrays/_matrices/tests/test_matrices.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     def test_rows(self, array: na.AbstractMatrixArray):
         assert np.all(array.rows == array.components)
 
     def test_is_consistent(self, array: na.AbstractMatrixArray):
 
         assert array.is_consistent
 
-        array_2 = array.copy()
+        array_2 = array.explicit.copy()
         array_2.x = 5
         assert not array_2.is_consistent
 
     def test_is_square(self, array: na.AbstractMatrixArray):
         assert array.is_square == (len(array.row_prototype.entries) == len(array.column_prototype.entries))
 
     def test_cartesian_nd(self, array: na.AbstractMatrixArray):
@@ -63,15 +63,15 @@
     def test_matrix(self, array: na.AbstractMatrixArray):
         assert np.all(array.matrix == array)
 
     def test_determinant(self, array: na.AbstractMatrixArray):
         if array.is_square:
             result = array.determinant
 
-            assert isinstance(result, (float, complex, u.Quantity, na.AbstractScalar))
+            assert isinstance(result, (int, float, complex, u.Quantity, na.AbstractScalar))
 
             assert np.all((2 ** 2) * result == (2 * array).determinant)
             assert np.all(result == array.matrix_transpose.determinant)
             assert np.allclose(result * result, (array @ array).determinant)
             assert np.allclose(result, 1 / array.inverse.determinant)
 
     def test_inverse(self, array: na.AbstractMatrixArray):
@@ -121,14 +121,20 @@
 
         @pytest.mark.skip
         class TestOptimizeRoot(
             named_arrays.tests.test_core.AbstractTestAbstractArray.TestNamedArrayFunctions.TestOptimizeRoot,
         ):
             pass
 
+        @pytest.mark.skip
+        class TestOptimizeMinimum(
+            named_arrays.tests.test_core.AbstractTestAbstractArray.TestNamedArrayFunctions.TestOptimizeMinimum,
+        ):
+            pass
+
 
 class AbstractTestAbstractExplicitMatrixArray(
     AbstractTestAbstractMatrixArray,
     named_arrays._vectors.tests.test_vectors.AbstractTestAbstractExplicitVectorArray,
 ):
     pass
```

### Comparing `named-arrays-0.3.7/named_arrays/_named_array_functions.py` & `named_arrays-0.4.0/named_arrays/_named_array_functions.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     'unit',
     'unit_normalized',
     'broadcast_to',
     'stack',
     'concatenate',
     'add_axes',
     "interp",
+    "histogram2d",
     'jacobian',
 ]
 
 ArrayT = TypeVar("ArrayT")
 LikeT = TypeVar("LikeT", bound="None | na.AbstractArray")
 AxisT = TypeVar("AxisT", bound="str | na.AbstractArray")
 NumT = TypeVar("NumT", bound="int | na.AbstractArray")
@@ -302,14 +303,15 @@
 def linspace(
         start: na.StartT,
         stop: na.StopT,
         axis: AxisT,
         num: NumT = 50,
         endpoint: bool = True,
         dtype: None | type | np.dtype = None,
+        centers: bool = False,
 ) -> na.StartT | na.StopT | AxisT | NumT:
     """
     Create an array of evenly-spaced numbers between :attr:`start` and :attr:`stop`
 
     Parameters
     ----------
     start
@@ -320,23 +322,60 @@
         The name of the new axis corresponding to the sequence
     num
         Number of values in the sequence
     endpoint
         Flag controlling whether :attr:`stop` should be included in the sequence.
     dtype
         :class:`numpy.dtype` of the result
+    centers
+        Flag controlling whether the returned values should be on cell centers.
+        The default is to return values on cell edges.
 
     See Also
     --------
     :func:`numpy.linspace` :  Corresponding numpy function.
 
     :class:`named_arrays.ScalarLinearSpace` : Corresponding implicit scalar array.
 
     :class:`named_arrays.UncertainScalarLinearSpace`: Corresponding implicit uncertain scalar array.
-    """
+
+    Examples
+    --------
+
+    Compare the points returned using ``centers=False`` to those returned
+    using ``centers=True``.
+
+    .. jupyter-execute::
+
+        import named_arrays as na
+        import matplotlib.pyplot as plt
+
+        # Define an array of cell edges
+        edges_x = na.linspace(0, 1, axis="x", num=11)
+        edges_y = na.linspace(0, 1, axis="y", num=11)
+
+        # Define an array of cell centers
+        centers_x = na.linspace(0, 1, axis="x", num=10, centers=True)
+        centers_y = na.linspace(0, 1, axis="y", num=10, centers=True)
+
+        # Plot the results as a scatterplot
+        fig, ax = plt.subplots()
+        na.plt.scatter(edges_x, edges_y, ax=ax, label="edges");
+        na.plt.scatter(centers_x, centers_y, ax=ax, label="centers");
+        ax.legend();
+    """
+
+    if centers:
+        if endpoint:
+            step = (stop - start) / (num - 1)
+        else:
+            step = (stop - start) / num
+        start = start + step / 2
+        stop = stop - step / 2
+
     return np.linspace(
         start=na.as_named_array(start),
         stop=stop,
         axis=axis,
         num=num,
         endpoint=endpoint,
         dtype=dtype,
@@ -443,85 +482,96 @@
     if not isinstance(a, na.AbstractArray):
         a = na.ScalarArray(a)
     return np.shape(a)
 
 
 def unit(
         a: Any,
+        unit_dimensionless: None | float | u.UnitBase = None,
         squeeze: bool = True,
 ) -> None | u.UnitBase | na.AbstractArray:
     """
     Isolate the physical units associated with the given object.
 
     If the array has no physical units, this function returns :obj:`None`.
 
     Parameters
     ----------
     a
         object to isolate the units of
+    unit_dimensionless
+        The unit to use for dimensionless objects.
     squeeze
         If the result is an instance of :class:`named_arrays.AbstractVectorArray`,
         and all the components are the same, simplify the result into a single
         :class:`astropy.units.Unit` instance.
 
     See Also
     --------
-    :func:`unit_normalized` : version of this function that returns :obj:`astropy.units.dimensionless_unscaled`
-        instead of :obj:`None` if there is no unit associated with the given object
+    :func:`unit_normalized` : version of this function that by default returns
+        :obj:`astropy.units.dimensionless_unscaled` instead of :obj:`None`
+        if there is no unit associated with the given object.
     """
     if isinstance(a, u.UnitBase):
         return a
     elif isinstance(a, u.Quantity):
         return a.unit
     elif isinstance(a, na.AbstractArray):
         return na._named_array_function(
             func=unit,
             a=a,
+            unit_dimensionless=unit_dimensionless,
             squeeze=squeeze,
         )
     else:
-        return None
+        return unit_dimensionless
 
 
 def unit_normalized(
         a: Any,
+        unit_dimensionless: float | u.UnitBase = u.dimensionless_unscaled,
         squeeze: bool = True,
 ) -> u.UnitBase | na.AbstractArray:
     """
-    Isolate the physical units associated with a given object, normalizing to dimensionless units
-    if the object does not have associated units.
+    Isolate the physical units associated with a given object,`
+    normalizing to the given dimensionless units if the object does not have
+    associated units.
 
 
     Parameters
     ----------
     a
         object to isolate the units of
+    unit_dimensionless
+        The unit to use for dimensionless objects.
     squeeze
         If the result is an instance of :class:`named_arrays.AbstractVectorArray`,
         and all the components are the same, simplify the result into a single
         :class:`astropy.units.Unit` instance.
 
     See Also
     --------
-    :func:`unit` : version of this function that returns :obj:`None` instead of
-        :obj:`astropy.units.dimensionless_unscaled` if there is no unit associated with the given object.
+    :func:`unit` : version of this function that by default returns :obj:`None`
+        instead of :obj:`astropy.units.dimensionless_unscaled` if there is no
+        unit associated with the given object.
 
     """
     if isinstance(a, u.UnitBase):
         return a
     elif isinstance(a, u.Quantity):
         return a.unit
     elif isinstance(a, na.AbstractArray):
         return na._named_array_function(
             func=unit_normalized,
             a=a,
+            unit_dimensionless=unit_dimensionless,
             squeeze=squeeze,
         )
     else:
-        return u.dimensionless_unscaled
+        return unit_dimensionless
 
 
 @overload
 def broadcast_to(array: float | complex | np.ndarray | u.Quantity, shape: dict[str, int]) -> na.ScalarArray:
     ...
 
 
@@ -627,29 +677,132 @@
         axis=axis,
         left=left,
         right=right,
         period=period,
     )
 
 
+def histogram2d(
+    x: na.AbstractScalarArray,
+    y: na.AbstractScalarArray,
+    bins: dict[str, int] | na.AbstractCartesian2dVectorArray,
+    axis: None | str | Sequence[str] = None,
+    min: None | na.AbstractScalarArray | na.AbstractCartesian2dVectorArray = None,
+    max: None | na.AbstractScalarArray | na.AbstractCartesian2dVectorArray = None,
+    density: bool = False,
+    weights: None | na.AbstractScalarArray = None,
+) -> na.FunctionArray[na.Cartesian2dVectorArray, na.ScalarArray]:
+    """
+    A thin wrapper around :func:`numpy.histogram2d` which adds an `axis` argument.
+
+    Parameters
+    ----------
+    x
+        An array containing the x coordinates of the points to be sampled.
+    y
+        An array containing the y coordinates of the points to be sampled.
+    bins
+        The bin specification of the histogram:
+         * If `bins` is a dictionary, the keys are interpreted as the axis names
+           and the values are the number of bins along each axis.
+         * If `bins` is a 2D Cartesian vector, each component of the vector
+           represents the bin edges in each dimension.
+    axis
+        The logical axes along which to histogram the data points.
+        If :obj:`None` (the default), the histogram will be computed along
+        all the axes of `x` and `y`.
+    min
+        The lower boundary of the histogram along each dimension.
+        If :obj:`None` (the default), the minimum of `x` and `y` is used.
+    max
+        The upper boundary of the histogram along each dimension.
+        If :obj:`None` (the default), the maximum of `x` and `y` is used.
+    density
+        If :obj:`False` (the default), returns the number of samples in each bin.
+        If :obj:`True`, returns the probability density in each bin.
+    weights
+        An optional array weighting each sample.
+
+    Examples
+    --------
+
+    Construct a 2D histogram with constant bin width.
+
+    .. jupyter-execute::
+
+        import numpy as np
+        import matplotlib.pyplot as plt
+        import named_arrays as na
+
+        # Define the bin edges
+        bins = dict(x=6, y=5)
+
+        # Define random points to collect into a histogram
+        x = na.random.normal(0, 2, shape_random=dict(h=101))
+        y = na.random.normal(0, 3, shape_random=dict(h=101))
+
+        # Compute the 2D histogram
+        hist = na.histogram2d(x, y, bins=bins)
+
+        # Plot the resulting histogram
+        fig, ax = plt.subplots()
+        na.plt.pcolormesh(C=hist);
+
+    Construct a 2D histogram with variable bin width.
+
+    .. jupyter-execute::
+
+        import matplotlib.pyplot as plt
+        import named_arrays as na
+
+        # Define the bin edges
+        bins = na.Cartesian2dVectorArray(
+            x=np.square(na.linspace(0, 2, axis="x", num=6)),
+            y=np.square(na.linspace(0, 2, axis="y", num=5)),
+        )
+
+        # Define random points to collect into a histogram
+        x = na.random.normal(0, 2, shape_random=dict(h=101))
+        y = na.random.normal(0, 3, shape_random=dict(h=101))
+
+        # Compute the 2D histogram
+        hist = na.histogram2d(x, y, bins=bins)
+
+        # Plot the resulting histogram
+        fig, ax = plt.subplots()
+        na.plt.pcolormesh(C=hist);
+    """
+    return _named_array_function(
+        func=histogram2d,
+        x=x,
+        y=y,
+        axis=axis,
+        bins=bins,
+        min=min,
+        max=max,
+        density=density,
+        weights=weights,
+    )
+
+
 def jacobian(
         function: Callable[[InputT], OutputT],
         x: InputT,
         dx: None | InputT = None,
 ) -> na.AbstractMatrixArray:
     """
     Compute the Jacobian of the given function using the first-order finite difference method.
 
     Parameters
     ----------
     function
         The function to compute the Jacobian of
     x
         The point to evaluate the function
-    step_size
+    dx
         The distance that ``x`` will be perturbed by to compute the slope
     """
 
     if dx is None:
         dx = 1e-10
         unit_x = na.unit(x)
         if unit_x is not None:
```

### Comparing `named-arrays-0.3.7/named_arrays/_scalars/scalar_array_functions.py` & `named_arrays-0.4.0/named_arrays/_scalars/scalar_array_functions.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_scalars/scalar_named_array_functions.py` & `named_arrays-0.4.0/named_arrays/_scalars/scalar_named_array_functions.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable, TypeVar
+from typing import Callable, Sequence
 import numpy as np
 import numpy.typing as npt
 import matplotlib.axes
 import matplotlib.artist
 import matplotlib.pyplot as plt
 import astropy.units as u
 import named_arrays as na
@@ -113,27 +113,33 @@
         axes=(axis,),
     )
 
 
 @_implements(na.unit)
 def unit(
         a: na.AbstractScalarArray,
+        unit_dimensionless: None | float | u.UnitBase = None,
         squeeze: bool = True,
 ) -> None | u.UnitBase:
-    return na.unit(a.ndarray)
+    return na.unit(
+        a=a.ndarray,
+        unit_dimensionless=unit_dimensionless,
+    )
 
 
 @_implements(na.unit_normalized)
 def unit_normalized(
         a: na.AbstractScalarArray,
+        unit_dimensionless: float | u.UnitBase = u.dimensionless_unscaled,
         squeeze: bool = True,
 ) -> u.UnitBase:
-    result = na.unit(a)
-    if result is None:
-        result = u.dimensionless_unscaled
+    result = na.unit(
+        a=a,
+        unit_dimensionless=unit_dimensionless,
+    )
     return result
 
 
 @_implements(na.interp)
 def interp(
         x: float | u.Quantity | na.AbstractScalarArray,
         xp:  na.AbstractScalarArray,
@@ -199,14 +205,138 @@
             ),
             axes=x.axes,
         )
 
     return result
 
 
+@_implements(na.histogram2d)
+def histogram2d(
+    x: na.AbstractScalarArray,
+    y: na.AbstractScalarArray,
+    bins: dict[str, int] | na.AbstractCartesian2dVectorArray,
+    axis: None | str | Sequence[str] = None,
+    min: None | na.AbstractScalarArray | na.AbstractCartesian2dVectorArray = None,
+    max: None | na.AbstractScalarArray | na.AbstractCartesian2dVectorArray = None,
+    density: bool = False,
+    weights: None | na.AbstractScalarArray = None,
+) -> na.FunctionArray[na.Cartesian2dVectorArray, na.ScalarArray]:
+    try:
+        x = scalars._normalize(x)
+        y = scalars._normalize(y)
+        weights = scalars._normalize(weights) if weights is not None else weights
+    except scalars.ScalarTypeError:  # pragma: nocover
+        return NotImplemented
+
+    shape = na.shape_broadcasted(x, y, weights)
+
+    x = na.broadcast_to(x, shape)
+    y = na.broadcast_to(y, shape)
+    weights = na.broadcast_to(weights, shape) if weights is not None else weights
+
+    if axis is None:
+        axis = tuple(shape)
+    elif isinstance(axis, str):
+        axis = (axis, )
+
+    shape_orthogonal = {a: shape[a] for a in shape if a not in axis}
+
+    if isinstance(bins, na.AbstractCartesian2dVectorArray):
+        shape_bins = bins.shape
+        if bins.x.ndim != 1:    # pragma: nocover
+            raise ValueError(
+                f"The x component of `bins` must have only one dimension, "
+                f"got {bins.x.shape}."
+            )
+        if bins.y.ndim != 1:    # pragma: nocover
+            raise ValueError(
+                f"The y component of `bins` must have only one dimension, "
+                f"got {bins.y.shape}."
+            )
+        bins = (
+            bins.x.ndarray,
+            bins.y.ndarray,
+        )
+    else:
+        shape_bins = {ax: bins[ax] + 1 for ax in bins}
+        bins = tuple(bins.values())
+
+    if set(shape_bins).issubset(shape_orthogonal):  # pragma: nocover
+        raise ValueError(
+            f"The histogram axes, {shape_bins}, should not be a subset of "
+            f"the orthogonal axes, {shape_orthogonal}."
+        )
+
+    axis_x, axis_y = shape_bins
+
+    a = na.Cartesian2dVectorArray(x, y)
+
+    if min is None:
+        min = a.min(axis)
+    elif not isinstance(min, na.AbstractCartesian2dVectorArray):
+        min = na.broadcast_to(min, shape_orthogonal)
+        min = na.Cartesian2dVectorArray.from_scalar(min)
+    else:
+        min = na.broadcast_to(min, shape_orthogonal)
+
+    if max is None:
+        max = a.max(axis)
+    elif not isinstance(max, na.AbstractCartesian2dVectorArray):
+        max = na.broadcast_to(max, shape_orthogonal)
+        max = na.Cartesian2dVectorArray.from_scalar(max)
+    else:
+        max = na.broadcast_to(max, shape_orthogonal)
+
+    shape_hist = {ax: shape_bins[ax] - 1 for ax in shape_bins}
+    shape_hist = na.broadcast_shapes(shape_orthogonal, shape_hist)
+
+    shape_x = na.broadcast_shapes(shape_orthogonal, {axis_x: shape_bins[axis_x]})
+    shape_y = na.broadcast_shapes(shape_orthogonal, {axis_y: shape_bins[axis_y]})
+
+    hist = na.ScalarArray.empty(shape_hist)
+    xedges = na.ScalarArray.empty(shape_x)
+    yedges = na.ScalarArray.empty(shape_y)
+
+    for i in na.ndindex(shape_orthogonal):
+        min_i = min[i]
+        max_i = max[i]
+        hist_i, xedges_i, yedges_i = np.histogram2d(
+            x=x[i].ndarray_aligned(axis).reshape(-1),
+            y=y[i].ndarray_aligned(axis).reshape(-1),
+            bins=bins,
+            range=[
+                [min_i.x.ndarray, max_i.x.ndarray],
+                [min_i.y.ndarray, max_i.y.ndarray],
+            ],
+            density=density,
+            weights=weights[i].ndarray_aligned(axis).reshape(-1) if weights is not None else weights,
+        )
+
+        hist[i] = na.ScalarArray(
+            ndarray=hist_i,
+            axes=tuple(shape_bins),
+        )
+        xedges[i] = na.ScalarArray(
+            ndarray=xedges_i,
+            axes=axis_x
+        )
+        yedges[i] = na.ScalarArray(
+            ndarray=yedges_i,
+            axes=axis_y,
+        )
+
+    return na.FunctionArray(
+        inputs=na.Cartesian2dVectorArray(
+            x=xedges,
+            y=yedges,
+        ),
+        outputs=hist,
+    )
+
+
 def random(
         func: Callable,
         *args: float | u.Quantity | na.AbstractScalarArray,
         shape_random: None | dict[str, int] = None,
         seed: None | int = None,
         **kwargs: float | u.Quantity | na.AbstractScalarArray,
 ) -> na.ScalarArray:
@@ -541,29 +671,37 @@
         ax = plt.gca()
     ax = na.as_named_array(ax)
 
     if axis_rgb is not None:    # pragma: nocover
         if axis_rgb not in C.shape:
             raise ValueError(f"`{axis_rgb=}` must be a member of `{C.shape=}`")
 
-    shape_C = na.shape_broadcasted(*XY, C, ax)
-    shape = {a: shape_C[a] for a in shape_C if a != axis_rgb}
     shape_orthogonal = ax.shape
 
-    XY = tuple(arg.broadcast_to(shape) for arg in XY)
+    shape_XY = na.shape_broadcasted(ax, *XY)
+    shape_C = na.shape_broadcasted(ax, C)
+
+    axes_XY = tuple(ax for ax in shape_C if ax not in shape_orthogonal)
+    axes_XY = tuple(ax for ax in axes_XY if ax != axis_rgb)
+
+    axes_C = axes_XY
+    if axis_rgb is not None:
+        axes_C = axes_C + (axis_rgb,)
+
+    XY = tuple(arg.broadcast_to(shape_XY) for arg in XY)
     C = C.broadcast_to(shape_C)
     vmin = vmin.broadcast_to(shape_orthogonal) if vmin is not None else vmin
     vmax = vmax.broadcast_to(shape_orthogonal) if vmax is not None else vmax
 
     result = na.ScalarArray.empty(shape_orthogonal, dtype=object)
 
     for index in na.ndindex(shape_orthogonal):
         result[index] = ax[index].ndarray.pcolormesh(
-            *[arg[index].ndarray for arg in XY],
-            C[index].ndarray,
+            *[arg[index].ndarray_aligned(axes_XY) for arg in XY],
+            C[index].ndarray_aligned(axes_C),
             cmap=cmap,
             norm=norm,
             vmin=vmin[index].ndarray if vmin is not None else vmin,
             vmax=vmax[index].ndarray if vmax is not None else vmax,
             **kwargs,
         )
```

### Comparing `named-arrays-0.3.7/named_arrays/_scalars/scalars.py` & `named_arrays-0.4.0/named_arrays/_scalars/scalars.py`

 * *Files 0% similar despite different names*

```diff
@@ -851,18 +851,14 @@
     def dtype(self: Self) -> np.dtype:
         return na.get_dtype(self.ndarray)
 
     @property
     def explicit(self: Self) -> Self:
         return self
 
-    @property
-    def centers(self: Self) -> Self:
-        return self
-
     def __setitem__(
             self: Self,
             item: dict[str, int | slice | AbstractScalarArray] | AbstractScalarArray,
             value: int | float | u.Quantity | AbstractScalarArray,
     ) -> None:
 
         shape_self = self.shape
```

### Comparing `named-arrays-0.3.7/named_arrays/_scalars/tests/test_scalars.py` & `named_arrays-0.4.0/named_arrays/_scalars/tests/test_scalars.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,25 +144,80 @@
             out = 0 * result
             result_out = np.matmul(array, array_2, out=out)
 
             assert np.all(result == result_expected)
             assert np.all(result == result_out)
             assert result_out is out
 
-    def test_interp_linear_identity(
-            self,
-            array: na.AbstractArray,
+    class TestNamedArrayFunctions(
+        tests.test_core.AbstractTestAbstractArray.TestNamedArrayFunctions,
     ):
-        if np.issubdtype(array.dtype, bool):
-            with pytest.raises(TypeError):
-                item = array.indices
-                array.interp_linear(item)
-            return
+        @pytest.mark.parametrize(
+            argnames="bins,min,max",
+            argvalues=[
+                (
+                    dict(hx=11, hy=12),
+                    -100,
+                    100,
+                ),
+                (
+                    na.Cartesian2dVectorArray(
+                        x=na.linspace(-100, 100, axis="hx", num=11),
+                        y=na.linspace(-100, 100, axis="hy", num=11),
+                    ),
+                    None,
+                    None,
+                )
+            ]
+        )
+        @pytest.mark.parametrize(
+            argnames="axis",
+            argvalues=[
+                None,
+                "y",
+            ]
+        )
+        @pytest.mark.parametrize(
+            argnames="weights",
+            argvalues=[
+                None,
+            ]
+        )
+        class TestHistogram2d:
+            def test_histogram2d(
+                self,
+                array: na.AbstractScalar,
+                bins: dict[str, int] | na.AbstractCartesian2dVectorArray,
+                axis: None | str | Sequence[str],
+                min: None | na.AbstractScalarArray | na.AbstractCartesian2dVectorArray,
+                max: None | na.AbstractScalarArray | na.AbstractCartesian2dVectorArray,
+                weights: None | na.AbstractScalarArray,
+            ):
+                if not array.shape:
+                    return
+
+                if isinstance(bins, na.AbstractCartesian2dVectorArray):
+                    bins = bins * array.unit_normalized
+                if min is not None:
+                    min = min * array.unit_normalized
+                if max is not None:
+                    max = max * array.unit_normalized
 
-        super().test_interp_linear_identity(array=array)
+                result = na.histogram2d(
+                    x=array,
+                    y=array,
+                    bins=bins,
+                    axis=axis,
+                    min=min,
+                    max=max,
+                    weights=weights,
+                )
+
+                assert np.all(result.outputs >= 0)
+                assert result.outputs.sum() > 0
 
 
 class AbstractTestAbstractScalarArray(
     AbstractTestAbstractScalar,
 ):
 
     def test_ndarray(self, array: na.AbstractScalarArray):
@@ -862,83 +917,83 @@
                 mode=mode,
             )
 
             assert result.axes == tuple(shape_broadcasted.keys())
             assert np.all(result.ndarray == result_expected)
 
     class TestNamedArrayFunctions(
-        tests.test_core.AbstractTestAbstractArray.TestNamedArrayFunctions
+        AbstractTestAbstractScalar.TestNamedArrayFunctions
     ):
         class TestInterp(
-            tests.test_core.AbstractTestAbstractArray.TestNamedArrayFunctions.TestInterp,
+            AbstractTestAbstractScalar.TestNamedArrayFunctions.TestInterp,
         ):
             def test_interp(
                     self,
                     array: na.AbstractScalarArray,
                     slope: float | na.AbstractArray,
             ):
                 if np.issubdtype(array.dtype, bool):
                     return
                 super().test_interp(array=array, slope=slope)
 
         @pytest.mark.parametrize(
             argnames="array_2",
-            argvalues=_scalar_arrays_2(),
-        )
-        @pytest.mark.parametrize(
-            argnames="where",
-            argvalues=[
-                np._NoValue,
-                True,
-                na.linspace(0, 1, axis="x", num=_num_x) > 0.5,
-            ]
+            argvalues=_scalar_arrays_2()[:8],
         )
         @pytest.mark.parametrize(
-            argnames="alpha",
+            argnames="where, alpha",
             argvalues=[
-                np._NoValue,
-                na.linspace(0, 1, axis="x", num=_num_x),
+                (
+                    np._NoValue,
+                    np._NoValue
+                ),
+                (
+                    True,
+                    na.linspace(0, 1, axis="x", num=_num_x, centers=True),
+                ),
+                (
+                    na.linspace(0, 1, axis="x", num=_num_x) > 0.5,
+                    0.5,
+                )
             ]
         )
         class TestPltPlotLikeFunctions(
-            tests.test_core.AbstractTestAbstractArray.TestNamedArrayFunctions.TestPltPlotLikeFunctions,
+            AbstractTestAbstractScalar.TestNamedArrayFunctions.TestPltPlotLikeFunctions,
         ):
             pass
 
         @pytest.mark.parametrize(
             argnames="array_2",
             argvalues=_scalar_arrays_2()[:8],
         )
         @pytest.mark.parametrize(
-            argnames="s",
+            argnames="s,c,where",
             argvalues=[
-                None,
-                5,
-            ]
-        )
-        @pytest.mark.parametrize(
-            argnames="c",
-            argvalues=[
-                None,
-                5,
-                na.ScalarArray(
-                    ndarray=np.array([.5, .5, .5, 1]),
-                    axes="rgba",
+                (
+                    None,
+                    None,
+                    None,
+                ),
+                (
+                    5,
+                    na.ScalarArray(
+                        ndarray=np.array([.5, .5, .5, 1]),
+                        axes="rgba",
+                    ),
+                    na.linspace(0, 1, axis="x", num=_num_x) > 0.5,
+                ),
+                (
+                    na.linspace(1, 2, axis="x", num=_num_x, endpoint=False, centers=True),
+                    5,
+                    True,
                 )
-            ]
-        )
-        @pytest.mark.parametrize(
-            argnames="where",
-            argvalues=[
-                True,
-                na.linspace(0, 1, axis="x", num=_num_x) > 0.5,
             ],
         )
         class TestPltScatter(
-            tests.test_core.AbstractTestAbstractArray.TestNamedArrayFunctions.TestPltScatter,
+            AbstractTestAbstractScalar.TestNamedArrayFunctions.TestPltScatter,
         ):
             pass
 
         @pytest.mark.parametrize("axis_x", ["x"])
         @pytest.mark.parametrize("axis_y", ["y"])
         class TestPltImshow:
 
@@ -1007,15 +1062,15 @@
                     2,
                     na.linspace(1, 2, num=6, axis="a"),
                     na.Cartesian2dVectorArray(2, 3),
                 ]
             ]
         )
         class TestJacobian(
-            tests.test_core.AbstractTestAbstractArray.TestNamedArrayFunctions.TestJacobian,
+            AbstractTestAbstractScalar.TestNamedArrayFunctions.TestJacobian,
         ):
             pass
 
         @pytest.mark.parametrize(
             argnames="func",
             argvalues=[
                 na.optimize.root_secant,
@@ -1030,15 +1085,21 @@
                     20,
                     na.linspace(19, 20, axis="c", num=6),
                 ]
                 for shift_vertical in [-1]
             ]
         )
         class TestOptimizeRoot(
-            tests.test_core.AbstractTestAbstractArray.TestNamedArrayFunctions.TestOptimizeRoot,
+            AbstractTestAbstractScalar.TestNamedArrayFunctions.TestOptimizeRoot,
+        ):
+            pass
+
+        @pytest.mark.skip
+        class TestOptimizeMinimum(
+            AbstractTestAbstractScalar.TestNamedArrayFunctions.TestOptimizeMinimum,
         ):
             pass
 
 
 @pytest.mark.parametrize('array', _scalar_arrays())
 class TestScalarArray(
     AbstractTestAbstractScalarArray,
@@ -1166,14 +1227,15 @@
             result = type_array.ones(shape, dtype=dtype)
             assert result.shape == shape
             assert np.all(result == 1)
             assert result.dtype == dtype
 
 
 class AbstractTestAbstractImplicitScalarArray(
+    AbstractTestAbstractScalarArray,
     tests.test_core.AbstractTestAbstractImplicitArray,
 ):
     pass
 
 
 class AbstractTestAbstractScalarRandomSample(
     AbstractTestAbstractImplicitScalarArray,
@@ -1302,26 +1364,37 @@
         na.ScalarArray(np.random.random(_num_x), axes=('x', )),
     ]
     stops = [
         10,
         na.ScalarArray(10 * np.random.random(_num_x) + 1, axes=('x', )),
     ]
     units = [None, u.mm]
+    nums = [_num_y]
     endpoints = [
         False,
         True,
     ]
+    centers = [
+        False,
+        True,
+    ]
     return [
         na.ScalarLinearSpace(
             start=start << unit if unit is not None else start,
             stop=stop << unit if unit is not None else stop,
             axis='y',
-            num=_num_y,
-            endpoint=endpoint
-        ) for start in starts for stop in stops for unit in units for endpoint in endpoints
+            num=num,
+            endpoint=endpoint,
+            centers=center,
+        )
+        for start in starts
+        for stop in stops
+        for unit in units
+        for num in nums
+        for endpoint, center in zip(endpoints, centers)
     ]
 
 
 @pytest.mark.parametrize('array', _scalar_linear_spaces())
 class TestScalarLinearSpace(
     AbstractTestAbstractScalarSpace,
     AbstractTestAbstractScalarArray,
```

### Comparing `named-arrays-0.3.7/named_arrays/_scalars/uncertainties/tests/test_uncertainties.py` & `named_arrays-0.4.0/named_arrays/_scalars/uncertainties/tests/test_uncertainties.py`

 * *Files 1% similar despite different names*

```diff
@@ -667,15 +667,15 @@
         @pytest.mark.parametrize('mode', ['full', 'same', 'valid'])
         def test_convolve(self, array: na.AbstractArray, v: na.AbstractArray, mode: str):
             super().test_convolve(array=array, v=v, mode=mode)
             with pytest.raises(ValueError, match="`numpy.convolve` is not supported .*"):
                 np.convolve(array, v=v, mode=mode)
 
     class TestNamedArrayFunctions(
-        named_arrays.tests.test_core.AbstractTestAbstractArray.TestNamedArrayFunctions
+        named_arrays._scalars.tests.test_scalars.AbstractTestAbstractScalar.TestNamedArrayFunctions
     ):
         @pytest.mark.parametrize(
             argnames="array_2",
             argvalues=_uncertain_scalar_arrays_2(),
         )
         @pytest.mark.parametrize(
             argnames="where",
@@ -689,15 +689,15 @@
             argnames="alpha",
             argvalues=[
                 np._NoValue,
                 na.linspace(0, 1, axis="x", num=_num_x),
             ]
         )
         class TestPltPlotLikeFunctions(
-            named_arrays.tests.test_core.AbstractTestAbstractArray.TestNamedArrayFunctions.TestPltPlotLikeFunctions,
+            named_arrays._scalars.tests.test_scalars.AbstractTestAbstractScalar.TestNamedArrayFunctions.TestPltPlotLikeFunctions,
         ):
             pass
 
         @pytest.mark.parametrize(
             argnames="array_2",
             argvalues=_uncertain_scalar_arrays_2(),
         )
@@ -717,15 +717,15 @@
             argnames="where",
             argvalues=[
                 True,
                 na.linspace(0, 1, axis="x", num=_num_x) > 0.5,
             ]
         )
         class TestPltScatter(
-            named_arrays.tests.test_core.AbstractTestAbstractArray.TestNamedArrayFunctions.TestPltScatter,
+            named_arrays._scalars.tests.test_scalars.AbstractTestAbstractScalar.TestNamedArrayFunctions.TestPltScatter,
         ):
             pass
 
         @pytest.mark.skip
         class TestPltPcolormesh(
             named_arrays._scalars.tests.test_scalars.AbstractTestAbstractScalar.TestNamedArrayFunctions.TestPltPcolormesh,
         ):
@@ -735,15 +735,15 @@
             argnames="function",
             argvalues=[
                 lambda x: a * x ** 3
                 for a in [2, na.UniformUncertainScalarArray(2, width=0.5, num_distribution=_num_distribution)]
             ]
         )
         class TestJacobian(
-            named_arrays.tests.test_core.AbstractTestAbstractArray.TestNamedArrayFunctions.TestJacobian,
+            named_arrays._scalars.tests.test_scalars.AbstractTestAbstractScalar.TestNamedArrayFunctions.TestJacobian,
         ):
             pass
 
         @pytest.mark.parametrize(
             argnames="func",
             argvalues=[
                 na.optimize.root_secant,
@@ -758,15 +758,21 @@
                     20,
                     na.UniformUncertainScalarArray(20, width=1, num_distribution=_num_distribution),
                 ]
                 for shift_vertical in [-1]
             ]
         )
         class TestOptimizeRoot(
-            named_arrays.tests.test_core.AbstractTestAbstractArray.TestNamedArrayFunctions.TestOptimizeRoot,
+            named_arrays._scalars.tests.test_scalars.AbstractTestAbstractScalar.TestNamedArrayFunctions.TestOptimizeRoot,
+        ):
+            pass
+
+        @pytest.mark.skip
+        class TestOptimizeMinimum(
+            named_arrays._scalars.tests.test_scalars.AbstractTestAbstractScalar.TestNamedArrayFunctions.TestOptimizeMinimum,
         ):
             pass
 
 
 @pytest.mark.parametrize('array', _uncertain_scalar_arrays())
 class TestUncertainScalarArray(
     AbstractTestAbstractUncertainScalarArray,
```

### Comparing `named-arrays-0.3.7/named_arrays/_scalars/uncertainties/uncertainties.py` & `named_arrays-0.4.0/named_arrays/_scalars/uncertainties/uncertainties.py`

 * *Files 2% similar despite different names*

```diff
@@ -565,18 +565,14 @@
     def size(self: Self) -> int:
         return int(np.array(tuple(self.shape.values())).prod())
 
     @property
     def explicit(self) -> Self:
         return self.copy_shallow()
 
-    @property
-    def centers(self) -> Self:
-        return self
-
     def __setitem__(
             self,
             item: dict[str, int | slice | na.AbstractScalar] | na.AbstractScalar,
             value: int | float | u.Quantity | na.AbstractScalar,
     ):
         shape_self = self.shape
 
@@ -701,18 +697,14 @@
     @property
     def explicit(self) -> UncertainScalarArray:
         return UncertainScalarArray(
             nominal=na.explicit(self.nominal),
             distribution=na.explicit(self.distribution),
         )
 
-    @property
-    def centers(self) -> Self:
-        return self
-
 
 @dataclasses.dataclass(eq=False, repr=False)
 class NormalUncertainScalarArray(
     AbstractImplicitUncertainScalarArray,
     na.AbstractRandomMixin,
     Generic[NominalArrayT, WidthT],
 ):
@@ -733,18 +725,14 @@
     @property
     def explicit(self) -> UncertainScalarArray:
         return UncertainScalarArray(
             nominal=na.explicit(self.nominal),
             distribution=na.explicit(self.distribution),
         )
 
-    @property
-    def centers(self) -> Self:
-        return self
-
 
 @dataclasses.dataclass(eq=False, repr=False)
 class AbstractUncertainScalarRandomSample(
     AbstractImplicitUncertainScalarArray,
     na.AbstractRandomSample,
 ):
     @property
```

### Comparing `named-arrays-0.3.7/named_arrays/_scalars/uncertainties/uncertainties_array_functions.py` & `named_arrays-0.4.0/named_arrays/_scalars/uncertainties/uncertainties_array_functions.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_scalars/uncertainties/uncertainties_named_array_functions.py` & `named_arrays-0.4.0/named_arrays/_scalars/uncertainties/uncertainties_named_array_functions.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable
+from typing import Callable, Sequence
 import numpy as np
 import numpy.typing as npt
 import matplotlib.axes
 import matplotlib.artist
 import matplotlib.pyplot as plt
 import astropy.units as u
 import named_arrays as na
@@ -80,25 +80,33 @@
         ),
     )
 
 
 @_implements(na.unit)
 def unit(
         a: na.AbstractUncertainScalarArray,
+        unit_dimensionless: None | float | u.UnitBase = None,
         squeeze: bool = True,
 ) -> None | u.UnitBase:
-    return na.unit(a.nominal)
+    return na.unit(
+        a=a.nominal,
+        unit_dimensionless=unit_dimensionless,
+    )
 
 
 @_implements(na.unit_normalized)
 def unit_normalized(
         a: na.AbstractUncertainScalarArray,
+        unit_dimensionless: float | u.UnitBase = u.dimensionless_unscaled,
         squeeze: bool = True,
 ) -> u.UnitBase:
-    return na.unit_normalized(a.nominal)
+    return na.unit_normalized(
+        a.nominal,
+        unit_dimensionless=unit_dimensionless,
+    )
 
 
 @_implements(na.interp)
 def interp(
         x: float | u.Quantity | na.AbstractScalar,
         xp:  na.AbstractScalar,
         fp: na.AbstractScalar,
@@ -135,14 +143,125 @@
             period=period.distribution,
         ),
     )
 
     return result
 
 
+@_implements(na.histogram2d)
+def histogram2d(
+    x: na.AbstractScalar,
+    y: na.AbstractScalar,
+    bins: dict[str, int] | na.AbstractCartesian2dVectorArray,
+    axis: None | str | Sequence[str] = None,
+    min: None | na.AbstractScalar | na.AbstractCartesian2dVectorArray = None,
+    max: None | na.AbstractScalar | na.AbstractCartesian2dVectorArray = None,
+    density: bool = False,
+    weights: None | na.AbstractScalar = None,
+) -> na.FunctionArray[na.Cartesian2dVectorArray, na.UncertainScalarArray]:
+    try:
+        x = uncertainties._normalize(x).broadcasted
+        y = uncertainties._normalize(y).broadcasted
+        weights = uncertainties._normalize(weights)
+
+        if isinstance(bins, na.AbstractCartesian2dVectorArray):
+            bins = na.Cartesian2dVectorArray(
+                x=uncertainties._normalize(bins.x),
+                y=uncertainties._normalize(bins.y),
+            )
+            bins_nominal = na.Cartesian2dVectorArray(
+                x=bins.x.nominal,
+                y=bins.y.nominal,
+            )
+            bins_distribution = na.Cartesian2dVectorArray(
+                x=bins.x.distribution,
+                y=bins.y.distribution,
+            )
+        else:
+            bins_nominal = bins_distribution = bins
+
+        if min is not None:
+            if not isinstance(min, na.AbstractCartesian2dVectorArray):
+                min = na.Cartesian2dVectorArray.from_scalar(min)
+            min = na.Cartesian2dVectorArray(
+                x=uncertainties._normalize(min.x),
+                y=uncertainties._normalize(min.y),
+            )
+            min_nominal = na.Cartesian2dVectorArray(
+                x=min.x.nominal,
+                y=min.y.nominal,
+            )
+            min_distribution = na.Cartesian2dVectorArray(
+                x=min.x.distribution,
+                y=min.y.distribution,
+            )
+        else:
+            min_nominal = min_distribution = min
+
+        if max is not None:
+            if not isinstance(max, na.AbstractCartesian2dVectorArray):
+                max = na.Cartesian2dVectorArray.from_scalar(max)
+            max = na.Cartesian2dVectorArray(
+                x=uncertainties._normalize(max.x),
+                y=uncertainties._normalize(max.y),
+            )
+            max_nominal = na.Cartesian2dVectorArray(
+                x=max.x.nominal,
+                y=max.y.nominal,
+            )
+            max_distribution = na.Cartesian2dVectorArray(
+                x=max.x.distribution,
+                y=max.y.distribution,
+            )
+        else:
+            max_nominal = max_distribution = max
+
+    except na.UncertainScalarTypeError:  # pragma: nocover
+        return NotImplemented
+
+    result_nominal = na.histogram2d(
+        x=x.nominal,
+        y=y.nominal,
+        bins=bins_nominal,
+        axis=axis,
+        min=min_nominal,
+        max=max_nominal,
+        density=density,
+        weights=weights.nominal,
+    )
+
+    result_distribution = na.histogram2d(
+        x=x.distribution,
+        y=y.distribution,
+        bins=bins_distribution,
+        axis=axis,
+        min=min_distribution,
+        max=max_distribution,
+        density=density,
+        weights=weights.distribution,
+    )
+
+    return na.FunctionArray(
+        inputs=na.Cartesian2dVectorArray(
+            x=na.UncertainScalarArray(
+                nominal=result_nominal.inputs.x,
+                distribution=result_distribution.inputs.x,
+            ),
+            y=na.UncertainScalarArray(
+                nominal=result_nominal.inputs.y,
+                distribution=result_distribution.inputs.y,
+            ),
+        ),
+        outputs=na.UncertainScalarArray(
+            nominal=result_nominal.outputs,
+            distribution=result_distribution.outputs,
+        ),
+    )
+
+
 def random(
         func: Callable,
         *args: float | u.Quantity | na.AbstractScalar,
         shape_random: None | dict[str, int] = None,
         seed: None | int = None,
         **kwargs: float | u.Quantity | na.AbstractScalar,
 ) -> na.UncertainScalarArray:
```

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/cartesian/tests/test_vectors_cartesian.py` & `named_arrays-0.4.0/named_arrays/_vectors/cartesian/tests/test_vectors_cartesian.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/cartesian/tests/test_vectors_cartesian_2d.py` & `named_arrays-0.4.0/named_arrays/_vectors/cartesian/tests/test_vectors_cartesian_2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,43 @@
         )
         class TestPercentileLikeFunctions(
             test_vectors_cartesian.AbstractTestAbstractCartesianVectorArray.TestArrayFunctions.
             TestPercentileLikeFunctions,
         ):
             pass
 
+    @pytest.mark.parametrize(
+        argnames="axes",
+        argvalues=[
+            ("x",),
+            ("x", "y"),
+        ],
+    )
+    def test_area(
+        self,
+        array: na.AbstractCartesian2dVectorArray,
+        axes: tuple[str, str],
+    ):
+        if not set(axes).issubset(array.shape):
+            with pytest.raises(ValueError):
+                array.area(axes)
+            return
+
+        if len(axes) != 2:
+            with pytest.raises(ValueError):
+                array.area(axes)
+            return
+
+        result = array.area(axes=axes)
+
+        sh = array.shape
+        shape_expected = {ax: sh[ax] - 1 if ax in axes else sh[ax] for ax in sh}
+        assert not result.shape or result.shape == shape_expected
+        assert np.allclose(result, array.explicit.area(axes=axes))
+
 
 @pytest.mark.parametrize('array', _cartesian2d_arrays())
 class TestCartesian2dVectorArray(
     AbstractTestAbstractCartesian2dVectorArray,
     test_vectors_cartesian.AbstractTestAbstractExplicitCartesianVectorArray,
 ):
```

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/cartesian/tests/test_vectors_cartesian_3d.py` & `named_arrays-0.4.0/named_arrays/_vectors/cartesian/tests/test_vectors_cartesian_3d.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/cartesian/tests/test_vectors_cartesian_nd.py` & `named_arrays-0.4.0/named_arrays/_vectors/cartesian/tests/test_vectors_cartesian_nd.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/cartesian/vectors_cartesian.py` & `named_arrays-0.4.0/named_arrays/_vectors/cartesian/vectors_cartesian.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/cartesian/vectors_cartesian_3d.py` & `named_arrays-0.4.0/named_arrays/_vectors/cartesian/vectors_cartesian_3d.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/cartesian/vectors_cartesian_nd.py` & `named_arrays-0.4.0/named_arrays/_vectors/cartesian/vectors_cartesian_nd.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/tests/test_vectors.py` & `named_arrays-0.4.0/named_arrays/_vectors/tests/test_vectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -584,14 +584,33 @@
             ],
         )
         class TestOptimizeRoot(
             named_arrays.tests.test_core.AbstractTestAbstractArray.TestNamedArrayFunctions.TestOptimizeRoot,
         ):
             pass
 
+        @pytest.mark.parametrize(
+            argnames="func",
+            argvalues=[
+                na.optimize.minimum_gradient_descent,
+            ],
+        )
+        @pytest.mark.parametrize(
+            argnames="function,expected",
+            argvalues=[
+                (lambda x: (np.square(na.value(x) - shift_horizontal) + shift_vertical).length, shift_horizontal)
+                for shift_horizontal in [20,]
+                for shift_vertical in [1,]
+            ]
+        )
+        class TestOptimizeMinimum(
+            named_arrays.tests.test_core.AbstractTestAbstractArray.TestNamedArrayFunctions.TestOptimizeMinimum,
+        ):
+            pass
+
 
 class AbstractTestAbstractExplicitVectorArray(
     AbstractTestAbstractVectorArray,
     named_arrays.tests.test_core.AbstractTestAbstractExplicitArray,
 ):
     pass
```

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/tests/test_vectors_directional.py` & `named_arrays-0.4.0/named_arrays/_vectors/tests/test_vectors_directional.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/tests/test_vectors_input_output.py` & `named_arrays-0.4.0/named_arrays/_vectors/tests/test_vectors_input_output.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/tests/test_vectors_positional.py` & `named_arrays-0.4.0/named_arrays/_vectors/tests/test_vectors_positional.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/tests/test_vectors_spectral.py` & `named_arrays-0.4.0/named_arrays/_vectors/tests/test_vectors_spectral.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/tests/test_vectors_spectral_directional.py` & `named_arrays-0.4.0/named_arrays/_vectors/tests/test_vectors_spectral_directional.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/tests/test_vectors_spectral_positional.py` & `named_arrays-0.4.0/named_arrays/_vectors/tests/test_vectors_spectral_positional.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/tests/test_vectors_temporal.py` & `named_arrays-0.4.0/named_arrays/_vectors/tests/test_vectors_temporal.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/tests/test_vectors_temporal_spectral.py` & `named_arrays-0.4.0/named_arrays/_vectors/tests/test_vectors_temporal_spectral.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/tests/test_vectors_temporal_spectral_directional.py` & `named_arrays-0.4.0/named_arrays/_vectors/tests/test_vectors_temporal_spectral_directional.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/tests/test_vectors_temporal_spectral_positional.py` & `named_arrays-0.4.0/named_arrays/_vectors/tests/test_vectors_temporal_spectral_positional.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/vector_array_functions.py` & `named_arrays-0.4.0/named_arrays/_vectors/vector_array_functions.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/vector_named_array_functions.py` & `named_arrays-0.4.0/named_arrays/_vectors/vector_named_array_functions.py`

 * *Files 15% similar despite different names*

```diff
@@ -121,35 +121,50 @@
 
     return prototype.type_explicit.from_components(components)
 
 
 @_implements(na.unit)
 def unit(
         a: na.AbstractVectorArray,
+        unit_dimensionless: None | float | u.UnitBase = None,
         squeeze: bool = True,
 ) -> None | u.UnitBase | na.AbstractVectorArray:
     components = a.components
-    components = {c: na.unit(components[c], squeeze=squeeze) for c in components}
+    components = {
+        c: na.unit(
+            a=components[c],
+            unit_dimensionless=unit_dimensionless,
+            squeeze=squeeze)
+        for c in components
+    }
     iter_components = iter(components)
     component_0 = components[next(iter_components)]
     if squeeze:
         if all(component_0 == components[c] for c in components):
             return component_0
 
     components = {c: 1 if components[c] is None else 1 * components[c] for c in components}
     return a.type_explicit.from_components(components,)
 
 
 @_implements(na.unit_normalized)
 def unit_normalized(
         a: na.AbstractVectorArray,
+        unit_dimensionless: float | u.UnitBase = u.dimensionless_unscaled,
         squeeze: bool = True,
 ) -> u.UnitBase | na.AbstractVectorArray:
     components = a.components
-    components = {c: na.unit_normalized(components[c], squeeze=squeeze) for c in components}
+    components = {
+        c: na.unit_normalized(
+            components[c],
+            unit_dimensionless=unit_dimensionless,
+            squeeze=squeeze
+        )
+        for c in components
+    }
     iter_components = iter(components)
     component_0 = components[next(iter_components)]
     if squeeze:
         if all(component_0 == components[c] for c in components):
             return component_0
 
     return a.type_explicit.from_components(components)
@@ -292,15 +307,25 @@
         return NotImplemented
 
     if len(XY) != 1:    # pragma: nocover
         raise ValueError("if any element of `XY` is a vector, `XY` must have a length of 1")
     XY = XY[0]
 
     components_XY = XY.components
-    components = [components_XY[c] for c in components]
+
+    if components is None:
+        if len(components_XY) == 2:
+            components = components_XY.values()
+        else:   # pragma: nocover
+            raise ValueError(
+                f"if `XY` is a vector and `components` is `None`, "
+                f"`XY` must have exactly 2 components, got {len(components_XY)}."
+            )
+    else:
+        components = [components_XY[c] for c in components]
 
     return na.plt.pcolormesh(
         *components,
         C=C,
         axis_rgb=axis_rgb,
         ax=ax,
         cmap=cmap,
@@ -429,7 +454,63 @@
         correction = jac.inverse @ f
 
         x = x - correction
 
         f = function(x)
 
     raise ValueError("Max iterations exceeded")
+
+
+@_implements(na.optimize.minimum_gradient_descent)
+def optimize_minimum_gradient_descent(
+    function: Callable[[na.AbstractVectorArray], na.AbstractScalar],
+    guess: na.AbstractVectorArray,
+    step_size: float | na.AbstractScalar,
+    gradient: None | Callable[[na.AbstractVectorArray], na.AbstractScalar],
+    min_gradient: na.ScalarLike,
+    max_iterations: int,
+    callback: (
+        None
+        | Callable[[int, na.AbstractVectorArray, na.ScalarLike, na.ScalarLike], None]
+    ),
+) -> na.ScalarArray:
+
+    x = guess
+    f = function(x)
+
+    if not isinstance(x, na.AbstractVectorArray):   # pragma: nocover
+        return NotImplemented
+
+    if not isinstance(na.as_named_array(f), na.AbstractScalar):  # pragma: nocover
+        return NotImplemented
+
+    if na.shape(min_gradient):  # pragma: nocover
+        raise ValueError(
+            f"argument `min_gradient` should have an empty shape, "
+            f"got {na.shape(min_gradient)}"
+        )
+
+    shape = na.shape_broadcasted(f, x)
+
+    converged = na.broadcast_to(0 * na.value(x), shape=shape).astype(bool)
+
+    x = na.broadcast_to(x, shape).astype(float)
+
+    for i in range(max_iterations):
+
+        if callback is not None:
+            callback(i, x, f, converged)
+
+        grad = gradient(x)
+
+        converged |= np.abs(grad) < min_gradient
+
+        if np.all(converged):
+            return x
+
+        correction = step_size * grad
+
+        x = x - correction
+
+        f = function(x)
+
+    raise ValueError("Max iterations exceeded")  # pragma: nocover
```

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/vectors.py` & `named_arrays-0.4.0/named_arrays/_vectors/vectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,25 +134,14 @@
     @property
     def value(self) -> na.AbstractExplicitVectorArray:
         components = self.components
         components = {c: na.value(components[c]) for c in components}
         return self.type_explicit.from_components(components)
 
     @property
-    def centers(self: Self) -> AbstractExplicitVectorArray:
-        components = self.components
-        components_result = dict()
-        for c in components:
-            if isinstance(components[c], na.AbstractArray):
-                components_result[c] = components[c].centers
-            else:
-                components_result[c] = components[c]
-        return self.type_explicit.from_components(components_result)
-
-    @property
     def prototype_vector(self) -> na.AbstractExplicitVectorArray:
         """
         Return vector of same type with all components zeroed.
         """
         return self.type_explicit.from_components(dict.fromkeys(self.components, 0))
 
     def astype(
```

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/vectors_directional.py` & `named_arrays-0.4.0/named_arrays/_vectors/vectors_directional.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/vectors_input_output.py` & `named_arrays-0.4.0/named_arrays/_vectors/vectors_input_output.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/vectors_positional.py` & `named_arrays-0.4.0/named_arrays/_vectors/vectors_positional.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/vectors_spectral.py` & `named_arrays-0.4.0/named_arrays/_vectors/vectors_spectral.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/vectors_spectral_directional.py` & `named_arrays-0.4.0/named_arrays/_vectors/vectors_spectral_directional.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/vectors_spectral_positional.py` & `named_arrays-0.4.0/named_arrays/_vectors/vectors_spectral_positional.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/vectors_temporal.py` & `named_arrays-0.4.0/named_arrays/_vectors/vectors_temporal.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/vectors_temporal_spectral.py` & `named_arrays-0.4.0/named_arrays/_vectors/vectors_temporal_spectral.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/vectors_temporal_spectral_directional.py` & `named_arrays-0.4.0/named_arrays/_vectors/vectors_temporal_spectral_directional.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/_vectors/vectors_temporal_spectral_positional.py` & `named_arrays-0.4.0/named_arrays/_vectors/vectors_temporal_spectral_positional.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/plt.py` & `named_arrays-0.4.0/named_arrays/plt.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         If :obj:`None`, the ``squeeze`` argument must be :obj:`True`.
     ncols
         Number of columns in the subplot grid
     sharex
         Controls whether all the :class:`matplotlib.axes.Axes` instances share the same horizontal axis properties.
         See the documentation of :func:`matplotlib.pyplot.subplots` for more information.
     sharey
-        Controls whether all the :class`matplotlib.axes.Axes` instances share the same vertical axis properties.
+        Controls whether all the :class:`matplotlib.axes.Axes` instances share the same vertical axis properties.
         See the documentation of :func:`matplotlib.pyplot.subplots` for more information.
     squeeze
         If :obj:`True`, :func:`numpy.squeeze` is called on the result, which removes singleton dimensions from the
         array.
         See the documentation of :func:`matplotlib.pyplot.subplots` for more information.
     kwargs
         Additional keyword arguments passed to :func:`matplotlib.pyplot.subplots`
```

### Comparing `named-arrays-0.3.7/named_arrays/random.py` & `named_arrays-0.4.0/named_arrays/random.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/tests/test_core.py` & `named_arrays-0.4.0/named_arrays/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,17 +198,14 @@
         assert not issubclass(array.type_abstract, na.AbstractImplicitArray)
 
     def test_broadcasted(self, array: na.AbstractArray):
         result = array.broadcasted
         assert result.shape == array.shape
         assert isinstance(result, array.type_explicit)
 
-    def test_centers(self, array: na.AbstractArray):
-        assert isinstance(array.centers, na.AbstractArray)
-
     @abc.abstractmethod
     def test_astype(self, array: na.AbstractArray, dtype: type):
         pass
 
     @abc.abstractmethod
     def test_to(self, array: na.AbstractArray, unit: None | u.UnitBase):
         pass
@@ -1095,14 +1092,18 @@
             if result is not None:
                 assert isinstance(result, (u.UnitBase, na.AbstractArray))
 
         def test_unit_normalized(self, array: na.AbstractArray):
             result = na.unit_normalized(array)
             assert isinstance(result, (u.UnitBase, na.AbstractArray))
 
+        def test_strata(self, array: na.AbstractArray):
+            result = na.strata(array)
+            assert result.type_abstract == array.type_abstract
+
         @pytest.mark.parametrize(
             argnames="slope",
             argvalues=[
                 2,
                 na.Cartesian2dVectorArray(x=2, y=3)
             ],
         )
@@ -1127,42 +1128,28 @@
                     fp=fp,
                     axis="interp",
                 )
 
                 assert np.allclose(result, slope * array)
 
         @pytest.mark.parametrize(
-            argnames="func",
+            argnames="func,axis,transformation",
             argvalues=[
-                na.plt.plot,
-                na.plt.fill,
+                (na.plt.plot, np._NoValue, np._NoValue),
+                (na.plt.fill, "y", na.transformations.Translation(0))
             ]
         )
         @pytest.mark.parametrize(
             argnames="ax",
             argvalues=[
                 np._NoValue,
                 plt.subplots()[1],
                 na.plt.subplots(axis_cols="x", ncols=num_x)[1],
             ]
         )
-        @pytest.mark.parametrize(
-            argnames="axis",
-            argvalues=[
-                np._NoValue,
-                "y",
-            ]
-        )
-        @pytest.mark.parametrize(
-            argnames="transformation",
-            argvalues=[
-                np._NoValue,
-                na.transformations.Translation(0),
-            ]
-        )
         class TestPltPlotLikeFunctions(abc.ABC):
 
             def test_plt_plot_like(
                     self,
                     func: Callable,
                     array: na.AbstractArray,
                     array_2: na.ArrayLike,
@@ -1230,31 +1217,32 @@
 
                 with astropy.visualization.quantity_support():
                     result = func(*args, **kwargs)
 
                 assert isinstance(result, na.AbstractArray)
                 assert result.dtype == matplotlib.artist.Artist
 
+                if where is None or where is np._NoValue:
+                    where_normalized = True
+                else:
+                    where_normalized = where
+                where_normalized = na.broadcast_to(where_normalized, shape_orthogonal)
+
                 for index in ax_normalized.ndindex():
-                    assert ax_normalized[index].ndarray.has_data()
+                    if np.any(where_normalized[index]):
+                        assert ax_normalized[index].ndarray.has_data()
+                    ax_normalized[index].ndarray.clear()
 
         @pytest.mark.parametrize(
-            argnames="ax",
+            argnames="ax, transformation",
             argvalues=[
-                None,
-                na.plt.subplots(axis_cols="x", ncols=num_x)[1],
+                (None, None),
+                (na.plt.subplots(axis_cols="x", ncols=num_x)[1], na.transformations.Translation(0))
             ],
         )
-        @pytest.mark.parametrize(
-            argnames="transformation",
-            argvalues=[
-                None,
-                na.transformations.Translation(0),
-            ]
-        )
         class TestPltScatter(abc.ABC):
             def test_plt_scatter(
                 self,
                 array: na.AbstractArray,
                 array_2: na.ArrayLike,
                 s: None | float | na.AbstractScalar,
                 c: None | str | na.AbstractScalar,
@@ -1273,14 +1261,24 @@
                         s=s,
                         c=c,
                         ax=ax,
                         where=where,
                         transformation=transformation,
                     )
 
+                if ax is None or ax is np._NoValue:
+                    ax_normalized = plt.gca()
+                else:
+                    ax_normalized = ax
+                ax_normalized = na.as_named_array(ax_normalized)
+
+                for index in ax_normalized.ndindex():
+                    assert ax_normalized[index].ndarray.has_data()
+                    ax_normalized[index].ndarray.clear()
+
         class TestPltPcolormesh:
 
             @pytest.mark.parametrize("axis_rgb", [None, "rgb"])
             def test_pcolormesh(
                 self,
                 array: na.AbstractScalarArray,
                 axis_rgb: None | str
@@ -1345,14 +1343,35 @@
                     guess=array,
                     callback=callback,
                 )
 
                 assert np.all(np.abs(function(result)) < 1e-8)
                 assert out is result
 
+        class TestOptimizeMinimum:
+            def test_optimize_minimum(
+                self,
+                func: Callable,
+                array: na.AbstractArray,
+                function: Callable[[na.AbstractArray], na.AbstractArray],
+                expected: na.AbstractArray,
+            ):
+                def callback(i, x, f, c):
+                    global out
+                    out = x
+
+                result = func(
+                    function=function,
+                    guess=array,
+                    callback=callback,
+                )
+
+                assert np.allclose(na.value(result), expected)
+                assert out is result
+
 
 class AbstractTestAbstractExplicitArray(
     AbstractTestAbstractArray,
 ):
 
     @abc.abstractmethod
     def test__setitem__(
```

### Comparing `named-arrays-0.3.7/named_arrays/tests/test_transformations.py` & `named_arrays-0.4.0/named_arrays/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays/transformations.py` & `named_arrays-0.4.0/named_arrays/transformations.py`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/named_arrays.egg-info/PKG-INFO` & `named_arrays-0.4.0/named_arrays.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: named-arrays
-Version: 0.3.7
+Version: 0.4.0
 Summary: Numpy arrays with labeled axes, similar to xarray but with support for uncertainties
 Author-email: "Roy T. Smart" <roytsmart@gmail.com>, "Jacob D. Parker" <jacobdparker@gmail.com>
 Project-URL: Homepage, https://github.com/sun-data/named-arrays
 Project-URL: Documentation, https://named-arrays.readthedocs.io/en/latest
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: typing_extensions
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: scipy
 Requires-Dist: astropy
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-split; extra == "test"
 Provides-Extra: doc
 Requires-Dist: pytest; extra == "doc"
 Requires-Dist: graphviz; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints; extra == "doc"
 Requires-Dist: pydata-sphinx-theme; extra == "doc"
 Requires-Dist: ipykernel; extra == "doc"
 Requires-Dist: jupyter-sphinx; extra == "doc"
```

### Comparing `named-arrays-0.3.7/named_arrays.egg-info/SOURCES.txt` & `named_arrays-0.4.0/named_arrays.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `named-arrays-0.3.7/pyproject.toml` & `named_arrays-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     'astropy',
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = [
     "pytest",
+    "pytest-split",
 ]
 doc = [
     "pytest",
     "graphviz",
     "sphinx-autodoc-typehints",
     "pydata-sphinx-theme",
     "ipykernel",
```

