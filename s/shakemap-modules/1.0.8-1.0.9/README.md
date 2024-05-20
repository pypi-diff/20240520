# Comparing `tmp/shakemap-modules-1.0.8.tar.gz` & `tmp/shakemap-modules-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shakemap-modules-1.0.8.tar", last modified: Mon Feb 12 18:00:59 2024, max compression
+gzip compressed data, was "shakemap-modules-1.0.9.tar", last modified: Tue Mar  5 18:35:56 2024, max compression
```

## Comparing `shakemap-modules-1.0.8.tar` & `shakemap-modules-1.0.9.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-12 18:00:59.828133 shakemap-modules-1.0.8/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1627 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/LICENSE.md
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       59 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/MANIFEST.in
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     9514 2024-02-12 18:00:59.824133 shakemap-modules-1.0.8/PKG-INFO
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      651 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/README.md
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5434 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/pyproject.toml
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2024-02-12 18:00:59.828133 shakemap-modules-1.0.8/setup.cfg
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      175 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/setup.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-12 18:00:59.752132 shakemap-modules-1.0.8/src/
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-12 18:00:59.752132 shakemap-modules-1.0.8/src/shakemap_modules/
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-12 18:00:59.760132 shakemap-modules-1.0.8/src/shakemap_modules/base/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7807 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/base/base.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11389 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/base/cli.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11339 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/base/transfer_base.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-12 18:00:59.772132 shakemap-modules-1.0.8/src/shakemap_modules/coremods/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    24606 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/assemble.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3212 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/associate.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    12736 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/augment.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11159 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/contour.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9319 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/coverage.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8493 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/dyfi.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      903 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/exception.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10877 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/gridxml.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4441 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/history.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3540 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/info.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    31270 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/kml.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11333 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/makecsv.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    20974 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/mapping.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   121587 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/model.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    13799 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/plotregr.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5559 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/raster.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3316 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/rupture.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1400 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/save.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11322 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/shape.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2803 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/sleep.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9237 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/sm_select.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3353 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/stations.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4548 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/transfer_email.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4904 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/transfer_pdl.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3088 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/transfer_scp.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    15833 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/uncertaintymaps.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6780 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/xtestimage.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3644 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/xtestplot.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5365 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/xtestplot_multi.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4048 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/coremods/xtestplot_spectra.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-12 18:00:59.780132 shakemap-modules-1.0.8/src/shakemap_modules/data/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   353304 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/fdsn_networks.json
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-12 18:00:59.784133 shakemap-modules-1.0.8/src/shakemap_modules/data/gis/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      145 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/gis/WGS1984.prj
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9216 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/gis/mi.lyr
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7269 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/gis/mi.shp.xml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10240 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/gis/pga.lyr
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7249 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/gis/pga.shp.xml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10240 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/gis/pgv.lyr
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7259 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/gis/pgv.shp.xml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10240 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/gis/psa0p3.lyr
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7311 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/gis/psa0p3.shp.xml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10240 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/gis/psa1p0.lyr
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7569 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/gis/psa1p0.shp.xml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9728 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/gis/psa3p0.lyr
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7569 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/gis/psa3p0.shp.xml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    16629 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/gmpe_sets.conf
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-12 18:00:59.792133 shakemap-modules-1.0.8/src/shakemap_modules/data/layers/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1927 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/layers/australia.wkt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      351 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/layers/california.wkt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1410 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/layers/chile.wkt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1036 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/layers/china.wkt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      354 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/layers/europe_share.wkt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1135 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/layers/greece.wkt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      719 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/layers/hawaii.wkt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      122 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/layers/induced.wkt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1854 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/layers/italy.wkt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      893 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/layers/japan.wkt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1054 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/layers/new_zealand.wkt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      801 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/layers/taiwan.wkt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1824 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/layers/turkey.wkt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2963 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/logging.conf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      657 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/loggingspec.conf
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-12 18:00:59.796133 shakemap-modules-1.0.8/src/shakemap_modules/data/mapping/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1225 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/mapping/circle.png
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7733 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/mapping/intensity_legend.png
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3348 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/mapping/map_strings.cn
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3377 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/mapping/map_strings.en
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3376 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/mapping/map_strings.en-AU
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1943 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/mapping/map_strings.en-CA
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3412 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/mapping/map_strings.es
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2020 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/mapping/map_strings.fr-CA
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3459 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/mapping/map_strings.it
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3351 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/mapping/map_strings.tw
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      678 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/mapping/triangle.png
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3294 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/migrate.conf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      119 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/migratespec.conf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    19430 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/model.conf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2920 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/modelspec.conf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8150 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/modules.conf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       90 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/modulesspec.conf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10555 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/products.conf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      898 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/productsspec.conf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11481 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/queue.conf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      638 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/queuespec.conf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11369 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/select.conf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2569 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/selectspec.conf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1369 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/shake.conf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      144 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/shakespec.conf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      132 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/simulationspec.conf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8774 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/transfer.conf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      373 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/transfer_reviewed_origin.conf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      795 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/data/transferspec.conf
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-12 18:00:59.796133 shakemap-modules-1.0.8/src/shakemap_modules/mapping/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    61981 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/mapping/mapmaker.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    14748 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/mapping/mercatormap.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    12826 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/mapping/scalebar.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-12 18:00:59.800133 shakemap-modules-1.0.8/src/shakemap_modules/utils/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    34798 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/utils/amps.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      861 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/utils/comcat.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    23536 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/utils/config.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     4925 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/utils/dataframe.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6791 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/utils/generic_amp.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7311 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/utils/layers.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10758 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/utils/logging.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2178 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/utils/macros.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3780 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/utils/points_to_station.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    18035 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/utils/probs.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    24092 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/utils/smclone.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5899 2024-02-12 16:29:35.000000 shakemap-modules-1.0.8/src/shakemap_modules/utils/utils.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-12 18:00:59.800133 shakemap-modules-1.0.8/src/shakemap_modules.egg-info/
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     9514 2024-02-12 18:00:59.000000 shakemap-modules-1.0.8/src/shakemap_modules.egg-info/PKG-INFO
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     4876 2024-02-12 18:00:59.000000 shakemap-modules-1.0.8/src/shakemap_modules.egg-info/SOURCES.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2024-02-12 18:00:59.000000 shakemap-modules-1.0.8/src/shakemap_modules.egg-info/dependency_links.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     1270 2024-02-12 18:00:59.000000 shakemap-modules-1.0.8/src/shakemap_modules.egg-info/entry_points.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     2367 2024-02-12 18:00:59.000000 shakemap-modules-1.0.8/src/shakemap_modules.egg-info/requires.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       17 2024-02-12 18:00:59.000000 shakemap-modules-1.0.8/src/shakemap_modules.egg-info/top_level.txt
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-03-05 18:35:56.667655 shakemap-modules-1.0.9/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1627 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/LICENSE.md
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       59 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/MANIFEST.in
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     9514 2024-03-05 18:35:56.667655 shakemap-modules-1.0.9/PKG-INFO
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      651 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/README.md
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5434 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/pyproject.toml
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2024-03-05 18:35:56.667655 shakemap-modules-1.0.9/setup.cfg
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      175 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/setup.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-03-05 18:35:56.627654 shakemap-modules-1.0.9/src/
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-03-05 18:35:56.627654 shakemap-modules-1.0.9/src/shakemap_modules/
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-03-05 18:35:56.631654 shakemap-modules-1.0.9/src/shakemap_modules/base/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7807 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/base/base.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11389 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/base/cli.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11339 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/base/transfer_base.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-03-05 18:35:56.639654 shakemap-modules-1.0.9/src/shakemap_modules/coremods/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    24606 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/assemble.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3212 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/associate.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    12736 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/augment.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11159 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/contour.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9319 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/coverage.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8493 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/dyfi.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      903 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/exception.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10877 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/gridxml.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4441 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/history.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3540 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/info.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    31270 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/kml.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11333 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/makecsv.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    20974 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/mapping.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   121587 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/model.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    13799 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/plotregr.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5559 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/raster.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3316 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/rupture.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1400 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/save.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11322 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/shape.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2803 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/sleep.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9237 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/sm_select.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3353 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/stations.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4548 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/transfer_email.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4904 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/transfer_pdl.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3088 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/transfer_scp.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    15833 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/uncertaintymaps.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6780 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/xtestimage.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3644 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/xtestplot.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5365 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/xtestplot_multi.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4048 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/coremods/xtestplot_spectra.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-03-05 18:35:56.643654 shakemap-modules-1.0.9/src/shakemap_modules/data/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   353304 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/fdsn_networks.json
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-03-05 18:35:56.647654 shakemap-modules-1.0.9/src/shakemap_modules/data/gis/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      145 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/gis/WGS1984.prj
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9216 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/gis/mi.lyr
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7269 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/gis/mi.shp.xml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10240 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/gis/pga.lyr
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7249 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/gis/pga.shp.xml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10240 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/gis/pgv.lyr
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7259 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/gis/pgv.shp.xml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10240 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/gis/psa0p3.lyr
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7311 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/gis/psa0p3.shp.xml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10240 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/gis/psa1p0.lyr
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7569 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/gis/psa1p0.shp.xml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9728 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/gis/psa3p0.lyr
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7569 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/gis/psa3p0.shp.xml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    16629 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/gmpe_sets.conf
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-03-05 18:35:56.647654 shakemap-modules-1.0.9/src/shakemap_modules/data/layers/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1927 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/layers/australia.wkt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      351 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/layers/california.wkt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1410 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/layers/chile.wkt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1036 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/layers/china.wkt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      354 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/layers/europe_share.wkt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1135 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/layers/greece.wkt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      719 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/layers/hawaii.wkt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      122 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/layers/induced.wkt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1854 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/layers/italy.wkt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      893 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/layers/japan.wkt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1054 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/layers/new_zealand.wkt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      801 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/layers/taiwan.wkt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1824 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/layers/turkey.wkt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2963 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/logging.conf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      657 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/loggingspec.conf
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-03-05 18:35:56.651654 shakemap-modules-1.0.9/src/shakemap_modules/data/mapping/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1225 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/mapping/circle.png
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7733 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/mapping/intensity_legend.png
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3348 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/mapping/map_strings.cn
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3377 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/mapping/map_strings.en
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3376 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/mapping/map_strings.en-AU
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1943 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/mapping/map_strings.en-CA
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3412 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/mapping/map_strings.es
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2020 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/mapping/map_strings.fr-CA
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3459 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/mapping/map_strings.it
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3351 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/mapping/map_strings.tw
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      678 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/mapping/triangle.png
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3294 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/migrate.conf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      119 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/migratespec.conf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    19430 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/model.conf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2920 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/modelspec.conf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8141 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/modules.conf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       90 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/modulesspec.conf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10555 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/products.conf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      898 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/productsspec.conf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11481 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/queue.conf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      638 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/queuespec.conf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11369 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/select.conf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2569 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/selectspec.conf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1369 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/shake.conf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      144 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/shakespec.conf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      132 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/simulationspec.conf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8774 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/transfer.conf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      373 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/transfer_reviewed_origin.conf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      795 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/data/transferspec.conf
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-03-05 18:35:56.651654 shakemap-modules-1.0.9/src/shakemap_modules/mapping/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    61981 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/mapping/mapmaker.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    14748 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/mapping/mercatormap.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    12826 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/mapping/scalebar.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-03-05 18:35:56.651654 shakemap-modules-1.0.9/src/shakemap_modules/utils/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    34798 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/utils/amps.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      861 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/utils/comcat.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    23536 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/utils/config.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     4925 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/utils/dataframe.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6791 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/utils/generic_amp.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7311 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/utils/layers.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10758 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/utils/logging.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2178 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/utils/macros.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3780 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/utils/points_to_station.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    18035 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/utils/probs.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    24092 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/utils/smclone.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5899 2024-03-05 17:36:00.000000 shakemap-modules-1.0.9/src/shakemap_modules/utils/utils.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-03-05 18:35:56.655655 shakemap-modules-1.0.9/src/shakemap_modules.egg-info/
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     9514 2024-03-05 18:35:56.000000 shakemap-modules-1.0.9/src/shakemap_modules.egg-info/PKG-INFO
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     4876 2024-03-05 18:35:56.000000 shakemap-modules-1.0.9/src/shakemap_modules.egg-info/SOURCES.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2024-03-05 18:35:56.000000 shakemap-modules-1.0.9/src/shakemap_modules.egg-info/dependency_links.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     1270 2024-03-05 18:35:56.000000 shakemap-modules-1.0.9/src/shakemap_modules.egg-info/entry_points.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     2367 2024-03-05 18:35:56.000000 shakemap-modules-1.0.9/src/shakemap_modules.egg-info/requires.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       17 2024-03-05 18:35:56.000000 shakemap-modules-1.0.9/src/shakemap_modules.egg-info/top_level.txt
```

### Comparing `shakemap-modules-1.0.8/LICENSE.md` & `shakemap-modules-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/PKG-INFO` & `shakemap-modules-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shakemap-modules
-Version: 1.0.8
+Version: 1.0.9
 Summary: USGS Earthquake Impact ShakeMap Modules
 Author-email: Bruce Worden <cbworden@contractor.usgs.gov>, Eric Thompson <emthompsone@usgs.gov>, Mike Hearne <mhearne@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
```

### Comparing `shakemap-modules-1.0.8/README.md` & `shakemap-modules-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/pyproject.toml` & `shakemap-modules-1.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/base/base.py` & `shakemap-modules-1.0.9/src/shakemap_modules/base/base.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/base/cli.py` & `shakemap-modules-1.0.9/src/shakemap_modules/base/cli.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/base/transfer_base.py` & `shakemap-modules-1.0.9/src/shakemap_modules/base/transfer_base.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/assemble.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/assemble.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/associate.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/associate.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/augment.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/augment.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/contour.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/contour.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/coverage.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/coverage.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/dyfi.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/dyfi.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/exception.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/exception.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/gridxml.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/gridxml.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/history.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/history.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/info.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/info.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/kml.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/kml.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/makecsv.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/makecsv.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/mapping.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/mapping.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/model.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/model.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/plotregr.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/plotregr.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/raster.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/raster.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/rupture.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/rupture.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/save.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/save.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/shape.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/shape.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/sleep.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/sleep.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/sm_select.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/sm_select.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/stations.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/stations.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/transfer_email.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/transfer_email.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/transfer_pdl.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/transfer_pdl.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/transfer_scp.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/transfer_scp.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/uncertaintymaps.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/uncertaintymaps.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/xtestimage.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/xtestimage.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/xtestplot.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/xtestplot.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/xtestplot_multi.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/xtestplot_multi.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/coremods/xtestplot_spectra.py` & `shakemap-modules-1.0.9/src/shakemap_modules/coremods/xtestplot_spectra.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/fdsn_networks.json` & `shakemap-modules-1.0.9/src/shakemap_modules/data/fdsn_networks.json`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/gis/mi.lyr` & `shakemap-modules-1.0.9/src/shakemap_modules/data/gis/mi.lyr`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/gis/mi.shp.xml` & `shakemap-modules-1.0.9/src/shakemap_modules/data/gis/mi.shp.xml`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/gis/pga.lyr` & `shakemap-modules-1.0.9/src/shakemap_modules/data/gis/pga.lyr`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/gis/pga.shp.xml` & `shakemap-modules-1.0.9/src/shakemap_modules/data/gis/pga.shp.xml`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/gis/pgv.lyr` & `shakemap-modules-1.0.9/src/shakemap_modules/data/gis/pgv.lyr`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/gis/pgv.shp.xml` & `shakemap-modules-1.0.9/src/shakemap_modules/data/gis/pgv.shp.xml`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/gis/psa0p3.lyr` & `shakemap-modules-1.0.9/src/shakemap_modules/data/gis/psa0p3.lyr`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/gis/psa0p3.shp.xml` & `shakemap-modules-1.0.9/src/shakemap_modules/data/gis/psa0p3.shp.xml`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/gis/psa1p0.lyr` & `shakemap-modules-1.0.9/src/shakemap_modules/data/gis/psa1p0.lyr`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/gis/psa1p0.shp.xml` & `shakemap-modules-1.0.9/src/shakemap_modules/data/gis/psa1p0.shp.xml`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/gis/psa3p0.lyr` & `shakemap-modules-1.0.9/src/shakemap_modules/data/gis/psa3p0.lyr`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/gis/psa3p0.shp.xml` & `shakemap-modules-1.0.9/src/shakemap_modules/data/gis/psa3p0.shp.xml`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/gmpe_sets.conf` & `shakemap-modules-1.0.9/src/shakemap_modules/data/gmpe_sets.conf`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/layers/australia.wkt` & `shakemap-modules-1.0.9/src/shakemap_modules/data/layers/australia.wkt`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/layers/chile.wkt` & `shakemap-modules-1.0.9/src/shakemap_modules/data/layers/chile.wkt`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/layers/china.wkt` & `shakemap-modules-1.0.9/src/shakemap_modules/data/layers/china.wkt`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/layers/greece.wkt` & `shakemap-modules-1.0.9/src/shakemap_modules/data/layers/greece.wkt`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/layers/hawaii.wkt` & `shakemap-modules-1.0.9/src/shakemap_modules/data/layers/hawaii.wkt`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/layers/italy.wkt` & `shakemap-modules-1.0.9/src/shakemap_modules/data/layers/italy.wkt`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/layers/japan.wkt` & `shakemap-modules-1.0.9/src/shakemap_modules/data/layers/japan.wkt`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/layers/new_zealand.wkt` & `shakemap-modules-1.0.9/src/shakemap_modules/data/layers/new_zealand.wkt`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/layers/taiwan.wkt` & `shakemap-modules-1.0.9/src/shakemap_modules/data/layers/taiwan.wkt`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/layers/turkey.wkt` & `shakemap-modules-1.0.9/src/shakemap_modules/data/layers/turkey.wkt`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/logging.conf` & `shakemap-modules-1.0.9/src/shakemap_modules/data/logging.conf`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/loggingspec.conf` & `shakemap-modules-1.0.9/src/shakemap_modules/data/loggingspec.conf`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/mapping/circle.png` & `shakemap-modules-1.0.9/src/shakemap_modules/data/mapping/circle.png`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/mapping/intensity_legend.png` & `shakemap-modules-1.0.9/src/shakemap_modules/data/mapping/intensity_legend.png`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/mapping/map_strings.cn` & `shakemap-modules-1.0.9/src/shakemap_modules/data/mapping/map_strings.cn`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/mapping/map_strings.en` & `shakemap-modules-1.0.9/src/shakemap_modules/data/mapping/map_strings.en`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/mapping/map_strings.en-AU` & `shakemap-modules-1.0.9/src/shakemap_modules/data/mapping/map_strings.en-AU`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/mapping/map_strings.en-CA` & `shakemap-modules-1.0.9/src/shakemap_modules/data/mapping/map_strings.en-CA`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/mapping/map_strings.es` & `shakemap-modules-1.0.9/src/shakemap_modules/data/mapping/map_strings.es`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/mapping/map_strings.fr-CA` & `shakemap-modules-1.0.9/src/shakemap_modules/data/mapping/map_strings.fr-CA`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/mapping/map_strings.it` & `shakemap-modules-1.0.9/src/shakemap_modules/data/mapping/map_strings.it`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/mapping/map_strings.tw` & `shakemap-modules-1.0.9/src/shakemap_modules/data/mapping/map_strings.tw`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/mapping/triangle.png` & `shakemap-modules-1.0.9/src/shakemap_modules/data/mapping/triangle.png`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/migrate.conf` & `shakemap-modules-1.0.9/src/shakemap_modules/data/migrate.conf`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/model.conf` & `shakemap-modules-1.0.9/src/shakemap_modules/data/model.conf`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/modelspec.conf` & `shakemap-modules-1.0.9/src/shakemap_modules/data/modelspec.conf`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/modules.conf` & `shakemap-modules-1.0.9/src/shakemap_modules/data/modules.conf`

 * *Files 1% similar despite different names*

```diff
@@ -115,17 +115,17 @@
 # ##########################################################################
 # Similar to gmpe_modules and ipe_modules, above, but for ground motion/
 # intensity conversion equations (GMICE). The modules must conform to the
 # API of the ShakeLib GMICE modules. See esi_shakelib.gmice.wgrw12 for an
 # example
 # ##########################################################################
 [gmice_modules]
-    WGRW12 = WGRW12, esi_utils_gmice.gmice.wgrw12
-    Wald99 = Wald99, esi_utils_gmice.gmice.wald99
-    AK07 = AK07, esi_utils_gmice.gmice.ak07
+    WGRW12 = WGRW12, esi_shakelib.gmice.wgrw12
+    Wald99 = Wald99, esi_shakelib.gmice.wald99
+    AK07 = AK07, esi_shakelib.gmice.ak07
 
 # ##########################################################################
 # ccf_modules -- Cross-correlation modules. Similar to gmice_modules,
 # above, these modules specify the cross correlation function used in 
 # the interpolation process. The modules must conform to the ShakeLib 
 # API for cross-correlation modules. See 
 # esi_shakelib.correlation.loth_baker_2013 for an example.
```

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/products.conf` & `shakemap-modules-1.0.9/src/shakemap_modules/data/products.conf`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/productsspec.conf` & `shakemap-modules-1.0.9/src/shakemap_modules/data/productsspec.conf`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/queue.conf` & `shakemap-modules-1.0.9/src/shakemap_modules/data/queue.conf`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/queuespec.conf` & `shakemap-modules-1.0.9/src/shakemap_modules/data/queuespec.conf`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/select.conf` & `shakemap-modules-1.0.9/src/shakemap_modules/data/select.conf`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/selectspec.conf` & `shakemap-modules-1.0.9/src/shakemap_modules/data/selectspec.conf`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/shake.conf` & `shakemap-modules-1.0.9/src/shakemap_modules/data/shake.conf`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/transfer.conf` & `shakemap-modules-1.0.9/src/shakemap_modules/data/transfer.conf`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/data/transferspec.conf` & `shakemap-modules-1.0.9/src/shakemap_modules/data/transferspec.conf`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/mapping/mapmaker.py` & `shakemap-modules-1.0.9/src/shakemap_modules/mapping/mapmaker.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/mapping/mercatormap.py` & `shakemap-modules-1.0.9/src/shakemap_modules/mapping/mercatormap.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/mapping/scalebar.py` & `shakemap-modules-1.0.9/src/shakemap_modules/mapping/scalebar.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/utils/amps.py` & `shakemap-modules-1.0.9/src/shakemap_modules/utils/amps.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/utils/comcat.py` & `shakemap-modules-1.0.9/src/shakemap_modules/utils/comcat.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/utils/config.py` & `shakemap-modules-1.0.9/src/shakemap_modules/utils/config.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/utils/dataframe.py` & `shakemap-modules-1.0.9/src/shakemap_modules/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/utils/generic_amp.py` & `shakemap-modules-1.0.9/src/shakemap_modules/utils/generic_amp.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/utils/layers.py` & `shakemap-modules-1.0.9/src/shakemap_modules/utils/layers.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/utils/logging.py` & `shakemap-modules-1.0.9/src/shakemap_modules/utils/logging.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/utils/macros.py` & `shakemap-modules-1.0.9/src/shakemap_modules/utils/macros.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/utils/points_to_station.py` & `shakemap-modules-1.0.9/src/shakemap_modules/utils/points_to_station.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/utils/probs.py` & `shakemap-modules-1.0.9/src/shakemap_modules/utils/probs.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/utils/smclone.py` & `shakemap-modules-1.0.9/src/shakemap_modules/utils/smclone.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules/utils/utils.py` & `shakemap-modules-1.0.9/src/shakemap_modules/utils/utils.py`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules.egg-info/PKG-INFO` & `shakemap-modules-1.0.9/src/shakemap_modules.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shakemap-modules
-Version: 1.0.8
+Version: 1.0.9
 Summary: USGS Earthquake Impact ShakeMap Modules
 Author-email: Bruce Worden <cbworden@contractor.usgs.gov>, Eric Thompson <emthompsone@usgs.gov>, Mike Hearne <mhearne@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
```

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules.egg-info/SOURCES.txt` & `shakemap-modules-1.0.9/src/shakemap_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules.egg-info/entry_points.txt` & `shakemap-modules-1.0.9/src/shakemap_modules.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `shakemap-modules-1.0.8/src/shakemap_modules.egg-info/requires.txt` & `shakemap-modules-1.0.9/src/shakemap_modules.egg-info/requires.txt`

 * *Files identical despite different names*

