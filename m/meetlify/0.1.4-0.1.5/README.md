# Comparing `tmp/meetlify-0.1.4.tar.gz` & `tmp/meetlify-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meetlify-0.1.4.tar", last modified: Tue May 14 00:41:15 2024, max compression
+gzip compressed data, was "meetlify-0.1.5.tar", last modified: Mon May 20 21:32:15 2024, max compression
```

## Comparing `meetlify-0.1.4.tar` & `meetlify-0.1.5.tar`

### file list

```diff
@@ -1,114 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.655336 meetlify-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-14 00:41:04.000000 meetlify-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-14 00:41:04.000000 meetlify-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-05-14 00:41:15.655336 meetlify-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-14 00:41:04.000000 meetlify-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-14 00:41:04.000000 meetlify-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-14 00:41:15.655336 meetlify-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-05-14 00:41:04.000000 meetlify-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.623336 meetlify-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.627336 meetlify-0.1.4/src/meetlify/
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9240 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/meetup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.631336 meetlify-0.1.4/src/meetlify/share/
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/share/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/share/configs.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.623336 meetlify-0.1.4/src/meetlify/share/content/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.631336 meetlify-0.1.4/src/meetlify/share/content/images/
--rw-r--r--   0 runner    (1001) docker     (127)   128599 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/share/content/images/fatureimage.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.631336 meetlify-0.1.4/src/meetlify/share/content/meetups/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/share/content/meetups/0001.md
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/share/content/meetups/0002.md
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/share/content/meetups/0003.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.631336 meetlify-0.1.4/src/meetlify/share/content/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/share/content/pages/contact.md
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/share/content/pages/home.md
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/share/content/pages/privacy.md
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/share/content/pages/terms.md
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/share/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.623336 meetlify-0.1.4/src/meetlify/themes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.623336 meetlify-0.1.4/src/meetlify/themes/lindau/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.623336 meetlify-0.1.4/src/meetlify/themes/lindau/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.631336 meetlify-0.1.4/src/meetlify/themes/lindau/static/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   362926 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/assets/about.png
--rw-r--r--   0 runner    (1001) docker     (127)    50969 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/assets/author.png
--rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/assets/banner.png
--rw-r--r--   0 runner    (1001) docker     (127)    22993 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/assets/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/assets/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.647336 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    70329 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.css
--rw-r--r--   0 runner    (1001) docker     (127)   203221 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    51795 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   115986 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    70403 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   203225 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    51870 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   116063 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    65696 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css
--rw-r--r--   0 runner    (1001) docker     (127)   129371 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    51369 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   129386 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    63943 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   107823 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css
--rw-r--r--   0 runner    (1001) docker     (127)   267535 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    85352 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   180381 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   107691 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   267476 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    85281 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   180217 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   281046 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   679755 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   232803 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   589892 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   280259 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css
--rw-r--r--   0 runner    (1001) docker     (127)   679615 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   232911 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   589087 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    12184 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/cookiealert.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.647336 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   113656 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)    85044 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   238335 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/css/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.651336 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)   207819 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)   444579 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    80721 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   332090 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   135829 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.esm.js
--rw-r--r--   0 runner    (1001) docker     (127)   305438 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.esm.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    73935 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   222455 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   145401 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (127)   306606 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    60635 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   220561 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/cookiealert.js
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/static/js/scripts.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.655336 meetlify-0.1.4/src/meetlify/themes/lindau/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/templates/meetup.html
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/templates/meetups.html
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/themes/lindau/templates/page.html
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-14 00:41:04.000000 meetlify-0.1.4/src/meetlify/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.655336 meetlify-0.1.4/src/meetlify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-05-14 00:41:15.000000 meetlify-0.1.4/src/meetlify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-05-14 00:41:15.000000 meetlify-0.1.4/src/meetlify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 00:41:15.000000 meetlify-0.1.4/src/meetlify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 00:41:15.000000 meetlify-0.1.4/src/meetlify.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 00:41:15.000000 meetlify-0.1.4/src/meetlify.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-14 00:41:15.000000 meetlify-0.1.4/src/meetlify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 00:41:15.000000 meetlify-0.1.4/src/meetlify.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:41:15.655336 meetlify-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-14 00:41:04.000000 meetlify-0.1.4/tests/test_meetups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.911187 meetlify-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-20 21:32:07.000000 meetlify-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-20 21:32:07.000000 meetlify-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-20 21:32:15.911187 meetlify-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-20 21:32:07.000000 meetlify-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-20 21:32:07.000000 meetlify-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-20 21:32:15.911187 meetlify-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-05-20 21:32:07.000000 meetlify-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.875187 meetlify-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.879187 meetlify-0.1.5/src/meetlify/
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/meetup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.883187 meetlify-0.1.5/src/meetlify/share/
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/share/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/share/configs.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.875187 meetlify-0.1.5/src/meetlify/share/content/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.883187 meetlify-0.1.5/src/meetlify/share/content/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   128599 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/share/content/images/fatureimage.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.883187 meetlify-0.1.5/src/meetlify/share/content/meetups/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/share/content/meetups/0001.md
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/share/content/meetups/0002.md
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/share/content/meetups/0003.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.883187 meetlify-0.1.5/src/meetlify/share/content/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/share/content/pages/contact.md
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/share/content/pages/home.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/share/content/pages/privacy.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/share/content/pages/terms.md
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/share/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/sitemap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.875187 meetlify-0.1.5/src/meetlify/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.879187 meetlify-0.1.5/src/meetlify/themes/lindau/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.879187 meetlify-0.1.5/src/meetlify/themes/lindau/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.887187 meetlify-0.1.5/src/meetlify/themes/lindau/static/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   362926 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/assets/about.png
+-rw-r--r--   0 runner    (1001) docker     (127)    50969 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/assets/author.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/assets/banner.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22993 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/assets/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/assets/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.899187 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    70329 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.css
+-rw-r--r--   0 runner    (1001) docker     (127)   203221 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    51795 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   115986 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    70403 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   203225 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    51870 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   116063 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    65696 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css
+-rw-r--r--   0 runner    (1001) docker     (127)   129371 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    10126 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    51369 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   129386 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    63943 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   107823 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css
+-rw-r--r--   0 runner    (1001) docker     (127)   267535 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    85352 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   180381 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   107691 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   267476 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    85281 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   180217 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   281046 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)   679755 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   232803 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   589892 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   280259 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css
+-rw-r--r--   0 runner    (1001) docker     (127)   679615 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   232911 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   589087 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/cookiealert.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.899187 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   113656 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    85044 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   238502 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/css/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.907187 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   207819 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)   444579 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    80721 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   332090 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   135829 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.esm.js
+-rw-r--r--   0 runner    (1001) docker     (127)   305438 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.esm.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    73935 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   222455 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   145401 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)   306606 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    60635 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   220561 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/cookiealert.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/static/js/scripts.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.907187 meetlify-0.1.5/src/meetlify/themes/lindau/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/templates/meetup.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/templates/meetups.html
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/templates/sitemap-index.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/themes/lindau/templates/sitemap.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-20 21:32:07.000000 meetlify-0.1.5/src/meetlify/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.907187 meetlify-0.1.5/src/meetlify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-20 21:32:15.000000 meetlify-0.1.5/src/meetlify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-20 21:32:15.000000 meetlify-0.1.5/src/meetlify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:32:15.000000 meetlify-0.1.5/src/meetlify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-20 21:32:15.000000 meetlify-0.1.5/src/meetlify.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:32:15.000000 meetlify-0.1.5/src/meetlify.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-20 21:32:15.000000 meetlify-0.1.5/src/meetlify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 21:32:15.000000 meetlify-0.1.5/src/meetlify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:32:15.907187 meetlify-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-20 21:32:07.000000 meetlify-0.1.5/tests/test_meetups.py
```

### Comparing `meetlify-0.1.4/LICENSE` & `meetlify-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/PKG-INFO` & `meetlify-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: meetlify
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python Package to Generate Meetup Websites
 Home-page: https://github.com/pybodensee/meetlify
-Download-URL: https://github.com/pybodensee/meetlify/releases/v0.1.4.tar.gz
+Download-URL: https://github.com/pybodensee/meetlify/releases/v0.1.5.tar.gz
 Author: Faisal Shahzad
 Author-email: pybodensee@gmail.com
 License: MIT
 Keywords: meetups,static-site-generators,seo,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Environment :: X11 Applications
@@ -55,24 +55,24 @@
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: pymdown-extensions; extra == "dev"
 Provides-Extra: all
 Requires-Dist: pytest; extra == "all"
-Requires-Dist: python-language-server[all]; extra == "all"
-Requires-Dist: pymdown-extensions; extra == "all"
-Requires-Dist: setuptools; extra == "all"
+Requires-Dist: wheel; extra == "all"
 Requires-Dist: black; extra == "all"
-Requires-Dist: mkdocs-gen-files; extra == "all"
 Requires-Dist: mkdocstrings[python]; extra == "all"
-Requires-Dist: wheel; extra == "all"
-Requires-Dist: twine; extra == "all"
-Requires-Dist: mkdocs; extra == "all"
 Requires-Dist: pytest-cov; extra == "all"
+Requires-Dist: pymdown-extensions; extra == "all"
+Requires-Dist: mkdocs; extra == "all"
+Requires-Dist: python-language-server[all]; extra == "all"
+Requires-Dist: mkdocs-gen-files; extra == "all"
+Requires-Dist: setuptools; extra == "all"
+Requires-Dist: twine; extra == "all"
 
 # meetlify
 
 Python based Static Site Genrators for Meetups/Meetup Webites.
 
 [![license](https://img.shields.io/pypi/l/meetlify.svg?style=flat-square "Project License: MIT")](https://github.com/pybodensee/meetlify/blob/master/LICENSE)
 [![status](https://img.shields.io/pypi/status/meetlify.svg?style=flat-square "Project Development Status")](https://github.com/pybodensee/meetlify/milestone/1)
@@ -98,15 +98,15 @@
 2. Now execute ``meetlify setup`` which will setup the all folders as per your configurations. 
 
 3. Now execute ``meetlify make`` which will generate full website in output folder.
 
 
 ### Using Application Programming Interface (API)
 
-You can embed ```meetilify`` into your existing workflow easily. Here is a sample snippet.
+You can embed ``meetilify`` into your existing workflow easily. Here is a sample snippet.
 
 ```python
 from pathlib import Path
 from meetlify.api import Meetlify
 from meetlify.utils import initialize
 
 destination_path = Path("/home/user/Desktop/sample_webiste/")
```

### Comparing `meetlify-0.1.4/README.md` & `meetlify-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 2. Now execute ``meetlify setup`` which will setup the all folders as per your configurations. 
 
 3. Now execute ``meetlify make`` which will generate full website in output folder.
 
 
 ### Using Application Programming Interface (API)
 
-You can embed ```meetilify`` into your existing workflow easily. Here is a sample snippet.
+You can embed ``meetilify`` into your existing workflow easily. Here is a sample snippet.
 
 ```python
 from pathlib import Path
 from meetlify.api import Meetlify
 from meetlify.utils import initialize
 
 destination_path = Path("/home/user/Desktop/sample_webiste/")
```

### Comparing `meetlify-0.1.4/setup.py` & `meetlify-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/__init__.py` & `meetlify-0.1.5/src/meetlify/__init__.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/api.py` & `meetlify-0.1.5/src/meetlify/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,32 +34,34 @@
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # STANDARD LIBARY IMPORTS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 import codecs
 import shutil
 from pathlib import Path
+from datetime import datetime
 
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # 3rd PARTY LIBRARY IMPORTS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 import markdown
 from jinja2 import Environment, FileSystemLoader
 
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # INTERNAL IMPORTS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
-
 from .configs import Configs
 from .page import Page
 from .meetup import Meetup
+from .sitemap import Sitemap
+from .constants import STATUS
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # IMPLEMENATIONS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 
 class Meetlify:
@@ -74,14 +76,16 @@
 
         self.renderer = Environment(
             loader=FileSystemLoader(
                 Path(self.dest, "themes", self.configs.theme, "templates")
             )
         )
         self.meetups = []
+        self.pages = []
+        self.sitemaps = []
 
     def setup(self) -> None:
         """Setup Current Folder for Meetlify Website."""
 
         Path(self.dest, self.configs.folders.output).mkdir(parents=True, exist_ok=True)
 
         # TODO: Support to update themes folder - switch between multiple folders
@@ -115,17 +119,52 @@
         """Parse all Meetup events available as Markdown"""
 
         self.meetups = [
             Meetup.from_markdown(mt)
             for mt in Path(self.dest, self.configs.folders.content, "meetups").iterdir()
             if mt.is_file() and mt.suffix == ".md"
         ]
-        self.meetups = [mt for mt in self.meetups if mt.status in ["open", "close"]]
+        self.meetups = [
+            mt
+            for mt in self.meetups
+            if mt.status in [STATUS.PROGRESS.value, STATUS.DONE.value]
+        ]
         self.meetups = sorted(self.meetups, key=lambda x: x.id, reverse=True)
 
+        self.sitemaps.append(
+            Sitemap.from_dict(
+                {
+                    "name": "meetups",
+                    "slug": "/meetups/",
+                    "modifieddate": datetime.now(),
+                    "items": self.meetups,
+                }
+            )
+        )
+
+    def parse_pages(self):
+        """Parse Pages avaialable as Markdown"""
+
+        self.pages = [
+            Page.from_markdown(mt)
+            for mt in Path(self.dest, self.configs.folders.content, "pages").iterdir()
+            if mt.is_file() and mt.name in ["privacy.md", "terms.md", "contact.md"]
+        ]
+
+        self.sitemaps.append(
+            Sitemap.from_dict(
+                {
+                    "name": "pages",
+                    "slug": "/",
+                    "modifieddate": datetime.now(),
+                    "items": self.pages,
+                }
+            )
+        )
+
     def render_home(self):
         """Render home page"""
         with codecs.open(
             Path(
                 self.dest,
                 self.configs.folders.content,
                 self.configs.folders.pages,
@@ -149,59 +188,88 @@
                     meta=self.configs,
                     home_content="".join(home_content),
                     meetups=self.meetups[0:3],
                 )
             )
             print("... wrote output/home")
 
-    def render_pages(self):
-        """Render permanent pages"""
-
-        for _page in ["privacy", "terms", "contact"]:
-            _page_content = Page.from_markdown(
-                Path(
-                    self.dest,
-                    self.configs.folders.content,
-                    "pages",
-                    f"{_page}.md",
+        with open(
+            Path(self.dest, self.configs.folders.output, "404.html"),
+            mode="w",
+            encoding="utf-8",
+        ) as file:
+            file.write(
+                self.renderer.get_template("404.html").render(
+                    meta=self.configs, meetups=self.meetups[0:3]
                 )
             )
+            print("... wrote output/404")
+
+    def render_pages(self):
+        """Render permanent pages"""
 
-            Path(self.dest, self.configs.folders.output, _page).mkdir(
+        for _page in self.pages:
+            Path(self.dest, self.configs.folders.output, _page.slug).mkdir(
                 parents=True, exist_ok=True
             )
 
             with open(
-                Path(self.dest, self.configs.folders.output, _page, "index.html"),
+                Path(self.dest, self.configs.folders.output, _page.slug, "index.html"),
                 mode="w",
                 encoding="utf-8",
             ) as file:
                 file.write(
                     self.renderer.get_template("page.html").render(
-                        meta=self.configs, front=_page_content
+                        meta=self.configs, front=_page
                     )
                 )
-                print(f"... wrote output/{_page}")
+                print(f"... wrote output/{_page.slug}")
 
-    def render_meetups(self):
-        """Render meetup pages and Meetup index page"""
+    def render_sitemaps(self):
+        """Render Sitemaps"""
+
+        for sitemap in self.sitemaps:
+            with open(
+                Path(
+                    self.dest,
+                    self.configs.folders.output,
+                    f"sitemap-{sitemap.name}.xml",
+                ),
+                mode="w",
+                encoding="utf-8",
+            ) as file:
+                file.write(
+                    self.renderer.get_template("sitemap.xml").render(
+                        meta=self.configs,
+                        category=sitemap.slug,
+                        items=sitemap.items,
+                    )
+                )
+                print(f"... wrote output/{sitemap.name}/sitemap")
 
-        # TODO: Check if there are less than 3 meetups and runs without error? make 3 config variable
         with open(
-            Path(self.dest, self.configs.folders.output, "404.html"),
+            Path(
+                self.dest,
+                self.configs.folders.output,
+                "sitemap-index.xml",
+            ),
             mode="w",
             encoding="utf-8",
         ) as file:
             file.write(
-                self.renderer.get_template("404.html").render(
-                    meta=self.configs, meetups=self.meetups[0:3]
+                self.renderer.get_template("sitemap-index.xml").render(
+                    meta=self.configs, sitemaps=self.sitemaps
                 )
             )
-            print("... wrote output/404")
+            print("... wrote output/sitemap-index")
 
+    def render_meetups(self):
+        """Render meetup pages and Meetup index page"""
+
+        # TODO: Check if there are less than 3 meetups and runs without error? make 3 config variable
         for _meetup in self.meetups:
             Path(self.dest, self.configs.folders.output, "meetups", _meetup.slug).mkdir(
                 parents=True, exist_ok=True
             )
 
             with open(
                 Path(
@@ -275,11 +343,13 @@
             )
             print("... copied output/robots.txt filed")
 
     def make(self):
         """Make Static Site and Save to Output folder"""
 
         self.parse_meetups()
+        self.parse_pages()
         self.render_home()
         self.render_meetups()
         self.render_pages()
+        self.render_sitemaps()
         self.copy_assests()
```

### Comparing `meetlify-0.1.4/src/meetlify/cli.py` & `meetlify-0.1.5/src/meetlify/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -83,26 +83,34 @@
 
 
 @main.command("make", help="Make Current Project")
 @click.option("--meetups/--no-meetups", default=False)
 @click.option("--home/--no-home", default=False)
 @click.option("--pages/--no-pages", default=False)
 @click.option("--assets/--no-assets", default=False)
-def make(meetups, home, pages, assets):
+@click.option("--sitemap/--no-sitemap", default=False)
+def make(meetups, home, pages, assets, sitemap):
     click.echo("Make Current Project")
     _mlfy = Meetlify(dest_=Path(os.getcwd()))
-    _mlfy.parse_meetups()
 
     if meetups:
+        _mlfy.parse_meetups()
         _mlfy.render_meetups()
 
     if home:
+        _mlfy.parse_meetups()
         _mlfy.render_home()
 
     if pages:
+        _mlfy.parse_pages()
         _mlfy.render_pages()
 
     if assets:
         _mlfy.copy_assests()
 
-    if not any([meetups, home, pages, assets]):
+    if sitemap:
+        _mlfy.parse_meetups()
+        _mlfy.parse_pages()
+        _mlfy.render_sitemaps()
+
+    if not any([meetups, home, pages, assets, sitemap]):
         _mlfy.make()
```

### Comparing `meetlify-0.1.4/src/meetlify/configs.py` & `meetlify-0.1.5/src/meetlify/configs.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/constants.py` & `meetlify-0.1.5/src/meetlify/share/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,31 @@
 # -*- coding: utf-8 -*-
 
 """
 Meetlify: Static Site Generator for Meetup Websites
 A Python Package for Generating Static Website for Meetups.
 https://github.com/pybodensee/meetlify
 
-    src\meetlify\constants.py
-    
+    src\meetlify\share\__init__.py
+
     Copyright (C) 2024-2024 Faisal Shahzad <info@serpwings.com>
 
 <LICENSE_BLOCK>
-Permission is hereby granted, free of charge, to any person obtaining a copy of 
-this software and associated documentation files (the "Software"), to deal in 
-the Software without restriction, including without limitation the rights to 
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies 
-of the Software, and to permit persons to whom the Software is furnished to do 
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
+of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all 
+The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, 
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE 
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, 
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE 
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 </LICENSE_BLOCK>
 """
-
-
-# +++++++++++++++++++++++++++++++++++++++++++++++++++++
-# DATABASE/CONSTANTS LIST
-# +++++++++++++++++++++++++++++++++++++++++++++++++++++
-
-VERSION_MAJOR = 0
-VERSION_MINOR = 1
-VERSION_REVISION = 4
-
-FULL_VERSION = f"{VERSION_MAJOR}.{VERSION_MINOR}.{VERSION_REVISION}"
```

### Comparing `meetlify-0.1.4/src/meetlify/meetup.py` & `meetlify-0.1.5/src/meetlify/meetup.py`

 * *Files 24% similar despite different names*

```diff
@@ -33,15 +33,16 @@
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # STANDARD LIBARY IMPORTS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 import codecs
 from dataclasses import dataclass
-
+from pathlib import Path
+from datetime import datetime, timezone 
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # 3rd PARTY LIBRARY IMPORTS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 import markdown
 from slugify import slugify
@@ -54,15 +55,16 @@
 
 @dataclass
 class Meetup:
     """Meetup Data Class"""
 
     id: str
     title: float
-    date: int
+    date: str
+    modifieddate: str
     author: str
     slug: str
     status: str
     featureimage: str
     address: str
     description: str
     content: str
@@ -84,18 +86,22 @@
 
             slug_ = (
                 "".join(_md.Meta["slug"])
                 if _md.Meta.get("slug")
                 else slugify("".join(_md.Meta["title"]))
             )
 
+
             return cls(
                 content=content_,
                 id="".join(_md.Meta["id"]),
                 date="".join(_md.Meta["date"]),
+                modifieddate=datetime.fromtimestamp(
+                    Path(meetup_).stat().st_mtime, tz=timezone.utc
+                ),
                 author="".join(_md.Meta["author"]),
                 title="".join(_md.Meta["title"]),
                 description="".join(_md.Meta["description"]),
                 slug=slug_,
                 featureimage="".join(_md.Meta["featureimage"]),
                 address="".join(_md.Meta["address"]),
                 status="".join(_md.Meta["status"]),
```

### Comparing `meetlify-0.1.4/src/meetlify/page.py` & `meetlify-0.1.5/src/meetlify/page.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # STANDARD LIBARY IMPORTS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 import codecs
 from dataclasses import dataclass
-
+from datetime import datetime, timezone
+from pathlib import Path
 
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 # 3rd PARTY LIBRARY IMPORTS
 # +++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 import markdown
 
@@ -51,15 +52,16 @@
 
 
 @dataclass
 class Page:
     """Page Data Class"""
 
     title: float
-    date: int
+    date: str
+    modifieddate: str
     author: str
     slug: str
     status: str
     description: str
     content: str
 
     @classmethod
@@ -71,16 +73,20 @@
 
         Returns:
             Page: Return Constructed Page Object
         """
         _md = markdown.Markdown(extensions=["meta", "attr_list"])
         with codecs.open(page_, "r", encoding="utf-8") as f:
             data = f.read()
+
             return cls(
                 content=_md.convert(data),
                 date="".join(_md.Meta["date"]),
+                modifieddate=datetime.fromtimestamp(
+                    Path(page_).stat().st_mtime, tz=timezone.utc
+                ),
                 author="".join(_md.Meta["author"]),
                 title="".join(_md.Meta["title"]),
                 description="".join(_md.Meta["description"]),
                 slug="".join(_md.Meta["slug"]),
                 status="".join(_md.Meta["status"]),
             )
```

### Comparing `meetlify-0.1.4/src/meetlify/share/__init__.py` & `meetlify-0.1.5/tests/test_meetups.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 # -*- coding: utf-8 -*-
 
 """
 Meetlify: Static Site Generator for Meetup Websites
 A Python Package for Generating Static Website for Meetups.
 https://github.com/pybodensee/meetlify
 
-    src\meetlify\share\__init__.py
-
+    tests\test_meetups.py
+    
     Copyright (C) 2024-2024 Faisal Shahzad <info@serpwings.com>
 
 <LICENSE_BLOCK>
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
-of the Software, and to permit persons to whom the Software is furnished to do
+Permission is hereby granted, free of charge, to any person obtaining a copy of 
+this software and associated documentation files (the "Software"), to deal in 
+the Software without restriction, including without limitation the rights to 
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies 
+of the Software, and to permit persons to whom the Software is furnished to do 
 so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
+The above copyright notice and this permission notice shall be included in all 
 copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, 
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE 
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, 
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE 
 SOFTWARE.
 </LICENSE_BLOCK>
 """
+
+
+def test_init():
+    pass
```

### Comparing `meetlify-0.1.4/src/meetlify/share/configs.json` & `meetlify-0.1.5/src/meetlify/share/configs.json`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/share/content/images/fatureimage.png` & `meetlify-0.1.5/src/meetlify/share/content/images/fatureimage.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/share/content/meetups/0001.md` & `meetlify-0.1.5/src/meetlify/share/content/meetups/0001.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/share/content/meetups/0002.md` & `meetlify-0.1.5/src/meetlify/share/content/meetups/0002.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/share/content/meetups/0003.md` & `meetlify-0.1.5/src/meetlify/share/content/meetups/0003.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/share/content/pages/contact.md` & `meetlify-0.1.5/src/meetlify/share/content/pages/contact.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/share/content/pages/home.md` & `meetlify-0.1.5/src/meetlify/share/content/pages/home.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/share/content/pages/privacy.md` & `meetlify-0.1.5/src/meetlify/share/content/pages/privacy.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/share/content/pages/terms.md` & `meetlify-0.1.5/src/meetlify/share/content/pages/terms.md`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/assets/about.png` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/assets/about.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/assets/author.png` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/assets/author.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/assets/banner.png` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/assets/banner.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/assets/favicon.png` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/assets/logo.png` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/assets/logo.png`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.css` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.css.map` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css.map` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css.map` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css.map` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-icons.css` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css.map` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css.map` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css.map` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css.map` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css.map` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css.map` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css.map` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css.map` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.css` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.css.map` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.min.css` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.min.css.map` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css.map` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css.map` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff2` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/css/styles.css` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/css/styles.css`

 * *Files 0% similar despite different names*

```diff
@@ -12634,14 +12634,23 @@
 
 .sidebar {
   position: -webkit-sticky;
   position: sticky;
   top: 0;
 }
 
+.footer {
+  --bs-text-opacity: 1;
+  font-weight: 400 !important;
+  margin-bottom: 1.15rem !important;
+  font-size: 1.15rem;
+  margin-top: 0;
+  margin-bottom: 1rem;
+}
+
 p,
 ul {
   --bs-text-opacity: 1;
   color: #6c757d !important;
   font-weight: 400 !important;
   margin-bottom: 1.15rem !important;
   font-size: 1.15rem;
```

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js.map` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js.map` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.esm.js` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.esm.js.map` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js.map` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.js` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.js.map` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.min.js` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/js/bootstrap.min.js.map` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/static/js/scripts.js` & `meetlify-0.1.5/src/meetlify/themes/lindau/static/js/scripts.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: ASCII text*

 * *Files 0% similar despite different names*

```diff
@@ -57,9 +57,8 @@
 00000380: 3b0a 7d3b 0a0a 7472 7920 7b0a 2020 2020  ;.};..try {.    
 00000390: 646f 6375 6d65 6e74 0a20 2020 2020 2020  document.       
 000003a0: 202e 7175 6572 7953 656c 6563 746f 7228   .querySelector(
 000003b0: 2266 6f72 6d22 290a 2020 2020 2020 2020  "form").        
 000003c0: 2e61 6464 4576 656e 744c 6973 7465 6e65  .addEventListene
 000003d0: 7228 2273 7562 6d69 7422 2c20 6861 6e64  r("submit", hand
 000003e0: 6c65 5375 626d 6974 293b 0a7d 2063 6174  leSubmit);.} cat
-000003f0: 6368 2028 6572 726f 7229 207b 0a7d 0a0a  ch (error) {.}..
-00000400: 0a                                       .
+000003f0: 6368 2028 6572 726f 7229 207b 0a7d       ch (error) {.}
```

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/templates/404.html` & `meetlify-0.1.5/src/meetlify/themes/lindau/templates/404.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 {% extends "base.html" %}
 
 {% block main_header %}
 <meta name="description" content="{{meta.description}}" />
 <meta name="author" content="{{meta.author}}" />
+<link href="{{meta.URL}}" rel="canonical" />
 <title>{{meta.title}}</title>
+<meta content="{{meta.title}}" property="og:title" />
+<meta content="{{meta.description}}" property="og:description" />
+<meta content="{{meta.url}}" property="og:url" />
 {% endblock main_header %}
 
 {% block main_content %}
 <!-- Header-->
 <header class="bg-dark py-5" id="home">
     <div class="container px-5">
         <div class="row gx-5 align-items-center justify-content-center">
```

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/templates/index.html` & `meetlify-0.1.5/src/meetlify/themes/lindau/templates/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 {% extends "base.html" %}
 
 {% block main_header %}
 <meta name="description" content="{{meta.description}}" />
 <meta name="author" content="{{meta.author}}" />
 <link href="{{meta.URL}}" rel="canonical" />
 <title>{{meta.title}}</title>
+<meta content="{{meta.title}}" property="og:title" />
+<meta content="{{meta.description}}" property="og:description" />
+<meta content="{{meta.url}}" property="og:url" />
 {% endblock main_header %}
 
 {% block main_content %}
 <!-- Header-->
 <header class="bg-dark py-5" id="home">
     <div class="container px-5">
         <div class="row gx-5 align-items-center justify-content-center">
```

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/templates/meetup.html` & `meetlify-0.1.5/src/meetlify/themes/lindau/templates/meetup.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 {% extends "base.html" %}
 
 {% block main_header %}
 <meta name="description" content="{{front.description}}" />
 <meta name="author" content="{{front.author}}" />
 <link href="{{meta.URL}}/meetups/{{front.slug}}/" rel="canonical" />
 <title>{{front.title}}</title>
+<meta content="{{front.title}}" property="og:title" />
+<meta content="{{front.description}}" property="og:description" />
+<meta content="{{meta.URL}}/meetups/{{front.slug}}/" property="og:url" />
 {% endblock main_header %}
 
+
 {% block main_content %}
 <!-- Page Content-->
 <section class="py-5">
     <div class="container px-5 my-5">
         <div class="row gx-5">
             <div class="col-lg-8">
                 <!-- Post content-->
```

### Comparing `meetlify-0.1.4/src/meetlify/themes/lindau/templates/meetups.html` & `meetlify-0.1.5/src/meetlify/themes/lindau/templates/meetups.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 {% extends "base.html" %}
 
 {% block main_header %}
 <meta name="description" content="Here is the list of upcoming Meetups organized by {{meta.name}}" />
 <meta name="author" content="{{meta.author}}" />
 <link href="{{meta.URL}}/meetups/" rel="canonical" />
 <title>Python Meetups in Bodensee Regions</title>
+<meta content="upcoming Meetups organized by {{meta.name}}" property="og:title" />
+<meta content="Here is the list of upcoming Meetups organized by {{meta.name}}" property="og:description" />
+<meta content="{{meta.URL}}/meetups/" property="og:url" />
 {% endblock main_header %}
 
+
 {% block main_content %}
 <!-- Page Content-->
 <section class="py-5 bg-light">
     <div class="container px-5">
         <h1 class="fw-bolder mb-4">Next Meetup</h1>
         <div class="card border-0 shadow rounded-3 overflow-hidden">
             <div class="card-body p-0">
```

### Comparing `meetlify-0.1.4/src/meetlify/utils.py` & `meetlify-0.1.5/src/meetlify/utils.py`

 * *Files identical despite different names*

### Comparing `meetlify-0.1.4/src/meetlify.egg-info/PKG-INFO` & `meetlify-0.1.5/src/meetlify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: meetlify
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python Package to Generate Meetup Websites
 Home-page: https://github.com/pybodensee/meetlify
-Download-URL: https://github.com/pybodensee/meetlify/releases/v0.1.4.tar.gz
+Download-URL: https://github.com/pybodensee/meetlify/releases/v0.1.5.tar.gz
 Author: Faisal Shahzad
 Author-email: pybodensee@gmail.com
 License: MIT
 Keywords: meetups,static-site-generators,seo,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Environment :: X11 Applications
@@ -55,24 +55,24 @@
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: pymdown-extensions; extra == "dev"
 Provides-Extra: all
 Requires-Dist: pytest; extra == "all"
-Requires-Dist: python-language-server[all]; extra == "all"
-Requires-Dist: pymdown-extensions; extra == "all"
-Requires-Dist: setuptools; extra == "all"
+Requires-Dist: wheel; extra == "all"
 Requires-Dist: black; extra == "all"
-Requires-Dist: mkdocs-gen-files; extra == "all"
 Requires-Dist: mkdocstrings[python]; extra == "all"
-Requires-Dist: wheel; extra == "all"
-Requires-Dist: twine; extra == "all"
-Requires-Dist: mkdocs; extra == "all"
 Requires-Dist: pytest-cov; extra == "all"
+Requires-Dist: pymdown-extensions; extra == "all"
+Requires-Dist: mkdocs; extra == "all"
+Requires-Dist: python-language-server[all]; extra == "all"
+Requires-Dist: mkdocs-gen-files; extra == "all"
+Requires-Dist: setuptools; extra == "all"
+Requires-Dist: twine; extra == "all"
 
 # meetlify
 
 Python based Static Site Genrators for Meetups/Meetup Webites.
 
 [![license](https://img.shields.io/pypi/l/meetlify.svg?style=flat-square "Project License: MIT")](https://github.com/pybodensee/meetlify/blob/master/LICENSE)
 [![status](https://img.shields.io/pypi/status/meetlify.svg?style=flat-square "Project Development Status")](https://github.com/pybodensee/meetlify/milestone/1)
@@ -98,15 +98,15 @@
 2. Now execute ``meetlify setup`` which will setup the all folders as per your configurations. 
 
 3. Now execute ``meetlify make`` which will generate full website in output folder.
 
 
 ### Using Application Programming Interface (API)
 
-You can embed ```meetilify`` into your existing workflow easily. Here is a sample snippet.
+You can embed ``meetilify`` into your existing workflow easily. Here is a sample snippet.
 
 ```python
 from pathlib import Path
 from meetlify.api import Meetlify
 from meetlify.utils import initialize
 
 destination_path = Path("/home/user/Desktop/sample_webiste/")
```

### Comparing `meetlify-0.1.4/src/meetlify.egg-info/SOURCES.txt` & `meetlify-0.1.5/src/meetlify.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/meetlify/__init__.py
 src/meetlify/api.py
 src/meetlify/cli.py
 src/meetlify/configs.py
 src/meetlify/constants.py
 src/meetlify/meetup.py
 src/meetlify/page.py
+src/meetlify/sitemap.py
 src/meetlify/utils.py
 src/meetlify.egg-info/PKG-INFO
 src/meetlify.egg-info/SOURCES.txt
 src/meetlify.egg-info/dependency_links.txt
 src/meetlify.egg-info/entry_points.txt
 src/meetlify.egg-info/not-zip-safe
 src/meetlify.egg-info/requires.txt
@@ -88,8 +89,10 @@
 src/meetlify/themes/lindau/static/js/scripts.js
 src/meetlify/themes/lindau/templates/404.html
 src/meetlify/themes/lindau/templates/base.html
 src/meetlify/themes/lindau/templates/index.html
 src/meetlify/themes/lindau/templates/meetup.html
 src/meetlify/themes/lindau/templates/meetups.html
 src/meetlify/themes/lindau/templates/page.html
+src/meetlify/themes/lindau/templates/sitemap-index.xml
+src/meetlify/themes/lindau/templates/sitemap.xml
 tests/test_meetups.py
```

