# Comparing `tmp/red_web_dashboard-1.6.0.tar.gz` & `tmp/red_web_dashboard-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "red_web_dashboard-1.6.0.tar", last modified: Sun May 12 17:17:10 2024, max compression
+gzip compressed data, was "red_web_dashboard-1.6.2.tar", last modified: Mon May 20 14:49:49 2024, max compression
```

## Comparing `red_web_dashboard-1.6.0.tar` & `red_web_dashboard-1.6.2.tar`

### file list

```diff
@@ -1,298 +1,298 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.252249 red_web_dashboard-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34625 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-05-12 17:17:10.252249 red_web_dashboard-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.252249 red_web_dashboard-1.6.0/Red_Web_Dashboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-05-12 17:17:10.000000 red_web_dashboard-1.6.0/Red_Web_Dashboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15998 2024-05-12 17:17:10.000000 red_web_dashboard-1.6.0/Red_Web_Dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 17:17:10.000000 red_web_dashboard-1.6.0/Red_Web_Dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-12 17:17:10.000000 red_web_dashboard-1.6.0/Red_Web_Dashboard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-12 17:17:10.000000 red_web_dashboard-1.6.0/Red_Web_Dashboard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-12 17:17:10.000000 red_web_dashboard-1.6.0/Red_Web_Dashboard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.196249 red_web_dashboard-1.6.0/reddash/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.196249 red_web_dashboard-1.6.0/reddash/app/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.200249 red_web_dashboard-1.6.0/reddash/app/base/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43241 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/base/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.200249 red_web_dashboard-1.6.0/reddash/app/login/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/login/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.192249 red_web_dashboard-1.6.0/reddash/app/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.204249 red_web_dashboard-1.6.0/reddash/app/static/assets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/biometric-icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.208249 red_web_dashboard-1.6.0/reddash/app/static/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)   480562 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/css/argon-dashboard.css
--rw-r--r--   0 runner    (1001) docker     (127)  1218638 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/css/argon-dashboard.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   381006 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/css/argon-dashboard.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/css/nucleo-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/css/nucleo-svg.css
--rw-r--r--   0 runner    (1001) docker     (127)    10929 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/css/simplemde.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.208249 red_web_dashboard-1.6.0/reddash/app/static/assets/css/themes/
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/css/themes/background_theme_dark.css
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/css/themes/background_theme_white.css
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/css/themes/sidenav_theme_dark.css
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/css/themes/sidenav_theme_white.css
--rw-r--r--   0 runner    (1001) docker     (127)   635325 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/error-403.gif
--rw-r--r--   0 runner    (1001) docker     (127)   884014 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/error-404.gif
--rw-r--r--   0 runner    (1001) docker     (127)   824431 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/error-500.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.212249 red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo-icons.eot
--rw-r--r--   0 runner    (1001) docker     (127)   126098 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo-icons.svg
--rw-r--r--   0 runner    (1001) docker     (127)    18292 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    10220 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    26524 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo.eot
--rw-r--r--   0 runner    (1001) docker     (127)    26364 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo.woff2
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/gulpfile.js
--rw-r--r--   0 runner    (1001) docker     (127)    34128 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/icon-documentation.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.212249 red_web_dashboard-1.6.0/reddash/app/static/assets/js/
--rw-r--r--   0 runner    (1001) docker     (127)    24834 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/js/argon-dashboard.js
--rw-r--r--   0 runner    (1001) docker     (127)    15415 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/js/argon-dashboard.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.212249 red_web_dashboard-1.6.0/reddash/app/static/assets/js/core/
--rw-r--r--   0 runner    (1001) docker     (127)    48944 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/js/core/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   288580 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/js/core/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    19188 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/js/core/popper.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.216249 red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/Chart.extension.js
--rw-r--r--   0 runner    (1001) docker     (127)    47524 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/Simple-Full-featured-jQuery-Pagination-System-Pagination-js.zip
--rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/bootstrap-notify.js
--rw-r--r--   0 runner    (1001) docker     (127)   176853 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/chartjs.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    19411 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/perfect-scrollbar.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    48421 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/smooth-scrollbar.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/utils.js
--rw-r--r--   0 runner    (1001) docker     (127)   140628 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/oauth.png
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/pdf.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/random.svg
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.216249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.220249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_alert.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_avatars.scss
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_breadcrumbs.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_cards.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_dark-version.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_dropdown.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_dropup.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_fixed-plugin.scss
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_footer.scss
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_gradients.scss
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_header.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_info-areas.scss
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_misc.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_nav.scss
--rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_navbar-vertical.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_navbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_popovers.scss
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_progress.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_rtl.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_social-buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_tables.scss
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_tilt.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_timeline.scss
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_tooltips.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_typography.scss
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_utilities-extend.scss
--rw-r--r--   0 runner    (1001) docker     (127)    16957 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)    68466 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_variables.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.228249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_accordion.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_alert.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_breadcrumb.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_button-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_card.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_carousel.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_close.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_containers.scss
--rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_dropdown.scss
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_functions.scss
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_grid.scss
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_helpers.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_images.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_list-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_maps.scss
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_mixins.scss
--rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_modal.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_nav.scss
--rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_navbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_offcanvas.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_placeholders.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_popover.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_progress.scss
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_reboot.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_root.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_spinners.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tables.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_toasts.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tooltip.scss
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_transitions.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_type.scss
--rw-r--r--   0 runner    (1001) docker     (127)    14817 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)    68547 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-grid.scss
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-reboot.scss
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.232249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_floating-labels.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-check.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-control.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-range.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-select.scss
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-text.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_input-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_labels.scss
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_validation.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.232249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_clearfix.scss
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_color-bg.scss
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_colored-links.scss
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_position.scss
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_ratio.scss
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_stacks.scss
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_stretched-link.scss
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_text-truncation.scss
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_visually-hidden.scss
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_vr.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.236249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_alert.scss
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_backdrop.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_border-radius.scss
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_box-shadow.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_breakpoints.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_caret.scss
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_clearfix.scss
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_color-scheme.scss
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_container.scss
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_deprecate.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_gradients.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_grid.scss
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_image.scss
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_list-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_lists.scss
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_reset-text.scss
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_resize.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_table-variants.scss
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_text-truncate.scss
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_transition.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_visually-hidden.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.236249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/_api.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.236249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)    10029 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/_rfs.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.236249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/cards/card-background.scss
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/cards/card-carousel.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.240249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/custom/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/custom/_styles.scss
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/custom/_variables.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.240249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/forms/
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-check.scss
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-select.scss
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-switch.scss
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/forms/_forms.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/forms/_input-group.scss
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/forms/_inputs.scss
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/forms/_labels.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.240249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_colored-shadows.scss
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_hover.scss
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_social-buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/mixins/mixins.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.192249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.240249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/
--rw-r--r--   0 runner    (1001) docker     (127)    20327 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_flatpickr.scss
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_nouislider.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_perfect-scrollbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_prism.scss
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/plugins.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/theme.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.248249 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_animations.scss
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_avatars.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_breadcrumb.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards-extend.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards.scss
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_choices.scss
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dark-version.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dropdowns.scss
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_fixed-plugin.scss
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_form-switch.scss
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_full-calendar.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_header.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_info-areas.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc-extend.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc.scss
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar-vertical.scss
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar.scss
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_rtl.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_social-buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_table.scss
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_timeline.scss
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities-extend.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities.scss
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_virtual-reality.scss
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard.scss
--rw-r--r--   0 runner    (1001) docker     (127)     7853 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/tasks_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.248249 red_web_dashboard-1.6.0/reddash/app/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.248249 red_web_dashboard-1.6.0/reddash/app/templates/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/errors/403.html
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/errors/404.html
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/errors/500.html
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/errors/blacklisted.html
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/errors/custom.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.248249 red_web_dashboard-1.6.0/reddash/app/templates/includes/
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/includes/fixed-plugin.html
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/includes/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/includes/navigation.html
--rw-r--r--   0 runner    (1001) docker     (127)    11413 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/includes/scripts.html
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/includes/sidenav.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.248249 red_web_dashboard-1.6.0/reddash/app/templates/layouts/
--rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/layouts/base-fullscreen.html
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/layouts/base.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.248249 red_web_dashboard-1.6.0/reddash/app/templates/pages/
--rw-r--r--   0 runner    (1001) docker     (127)    29579 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/pages/admin.html
--rw-r--r--   0 runner    (1001) docker     (127)    17016 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/pages/commands.html
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/pages/credits.html
--rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/pages/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (127)    30814 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/pages/dashboard_guild.html
--rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/pages/guild_profile.html
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/pages/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.252249 red_web_dashboard-1.6.0/reddash/app/templates/pages/login/
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/pages/login/login.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.252249 red_web_dashboard-1.6.0/reddash/app/templates/pages/third_parties/
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/pages/third_parties/oauth.html
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/pages/third_parties/third_parties.html
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/pages/third_parties/third_parties_list.html
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/templates/pages/third_parties/third_party.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 17:17:10.252249 red_web_dashboard-1.6.0/reddash/app/third_parties/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/third_parties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14084 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/third_parties/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    27042 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/reddash/app/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-12 17:17:10.252249 red_web_dashboard-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-12 17:17:06.000000 red_web_dashboard-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.712114 red_web_dashboard-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    34625 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-05-20 14:49:49.712114 red_web_dashboard-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.712114 red_web_dashboard-1.6.2/Red_Web_Dashboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-05-20 14:49:49.000000 red_web_dashboard-1.6.2/Red_Web_Dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15998 2024-05-20 14:49:49.000000 red_web_dashboard-1.6.2/Red_Web_Dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:49:49.000000 red_web_dashboard-1.6.2/Red_Web_Dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-20 14:49:49.000000 red_web_dashboard-1.6.2/Red_Web_Dashboard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-20 14:49:49.000000 red_web_dashboard-1.6.2/Red_Web_Dashboard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 14:49:49.000000 red_web_dashboard-1.6.2/Red_Web_Dashboard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.664114 red_web_dashboard-1.6.2/reddash/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.664114 red_web_dashboard-1.6.2/reddash/app/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6267 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.668114 red_web_dashboard-1.6.2/reddash/app/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43241 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/base/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.668114 red_web_dashboard-1.6.2/reddash/app/login/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/login/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.660114 red_web_dashboard-1.6.2/reddash/app/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.672114 red_web_dashboard-1.6.2/reddash/app/static/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/biometric-icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.676114 red_web_dashboard-1.6.2/reddash/app/static/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   480562 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/css/argon-dashboard.css
+-rw-r--r--   0 runner    (1001) docker     (127)  1218638 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/css/argon-dashboard.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   381006 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/css/argon-dashboard.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/css/nucleo-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/css/nucleo-svg.css
+-rw-r--r--   0 runner    (1001) docker     (127)    10929 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/css/simplemde.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.676114 red_web_dashboard-1.6.2/reddash/app/static/assets/css/themes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/css/themes/background_theme_dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/css/themes/background_theme_white.css
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/css/themes/sidenav_theme_dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/css/themes/sidenav_theme_white.css
+-rw-r--r--   0 runner    (1001) docker     (127)   635325 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/error-403.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   884014 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/error-404.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   824431 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/error-500.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.676114 red_web_dashboard-1.6.2/reddash/app/static/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/fonts/nucleo-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   126098 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/fonts/nucleo-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    18292 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/fonts/nucleo-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    10220 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/fonts/nucleo-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/fonts/nucleo-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    26524 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/fonts/nucleo.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    26364 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/fonts/nucleo.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/fonts/nucleo.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/fonts/nucleo.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/gulpfile.js
+-rw-r--r--   0 runner    (1001) docker     (127)    34128 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/icon-documentation.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.676114 red_web_dashboard-1.6.2/reddash/app/static/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    24834 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/js/argon-dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15415 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/js/argon-dashboard.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.680114 red_web_dashboard-1.6.2/reddash/app/static/assets/js/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    48944 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/js/core/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   288580 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/js/core/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19188 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/js/core/popper.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.680114 red_web_dashboard-1.6.2/reddash/app/static/assets/js/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/js/plugins/Chart.extension.js
+-rw-r--r--   0 runner    (1001) docker     (127)    47524 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/js/plugins/Simple-Full-featured-jQuery-Pagination-System-Pagination-js.zip
+-rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/js/plugins/bootstrap-notify.js
+-rw-r--r--   0 runner    (1001) docker     (127)   176853 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/js/plugins/chartjs.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19411 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/js/plugins/perfect-scrollbar.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    48421 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/js/plugins/smooth-scrollbar.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/js/plugins/utils.js
+-rw-r--r--   0 runner    (1001) docker     (127)   140628 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/oauth.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/random.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.680114 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.688114 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_alert.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_avatars.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_badge.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_breadcrumbs.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_cards.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_dark-version.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_dropdown.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_dropup.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_fixed-plugin.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_footer.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_gradients.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_header.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_info-areas.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_misc.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_nav.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_navbar-vertical.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_navbar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_popovers.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_progress.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_rtl.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_social-buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_tables.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_tilt.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_timeline.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_tooltips.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_typography.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_utilities-extend.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    16957 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    68466 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.692114 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_accordion.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_alert.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_badge.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_breadcrumb.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_button-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_card.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_carousel.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_close.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_containers.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_dropdown.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_functions.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_grid.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_helpers.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_images.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_list-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_maps.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_mixins.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_modal.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_nav.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_navbar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_offcanvas.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_placeholders.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_popover.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_progress.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_reboot.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_root.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_spinners.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tables.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_toasts.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tooltip.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_transitions.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_type.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    14817 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    68547 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_variables.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-grid.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-reboot.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.696114 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_floating-labels.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-check.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-control.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-range.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-select.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-text.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_input-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_labels.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_validation.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.696114 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_clearfix.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_color-bg.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_colored-links.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_position.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_ratio.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_stacks.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_stretched-link.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_text-truncation.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_visually-hidden.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_vr.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.700114 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_alert.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_backdrop.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_border-radius.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_box-shadow.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_breakpoints.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_caret.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_clearfix.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_color-scheme.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_container.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_deprecate.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_gradients.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_grid.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_image.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_list-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_lists.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_reset-text.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_resize.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_table-variants.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_text-truncate.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_transition.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_visually-hidden.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.700114 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/_api.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.700114 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)    10029 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/_rfs.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.700114 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/cards/card-background.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/cards/card-carousel.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.700114 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/custom/_styles.scss
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/custom/_variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.704114 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/forms/_form-check.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/forms/_form-select.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/forms/_form-switch.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/forms/_forms.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/forms/_input-group.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/forms/_inputs.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/forms/_labels.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.704114 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/mixins/_badge.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/mixins/_colored-shadows.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/mixins/_hover.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/mixins/_social-buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/mixins/mixins.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.660114 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.704114 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/plugins/free/
+-rw-r--r--   0 runner    (1001) docker     (127)    20327 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_flatpickr.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_nouislider.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_perfect-scrollbar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_prism.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/plugins/free/plugins.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/theme.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.708114 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_animations.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_avatars.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_badge.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_breadcrumb.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_cards-extend.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_cards.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_choices.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_dark-version.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_dropdowns.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_fixed-plugin.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_form-switch.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_full-calendar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_header.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_info-areas.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_misc-extend.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_misc.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar-vertical.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_rtl.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_social-buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_table.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_timeline.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities-extend.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_virtual-reality.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     7853 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/tasks_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.708114 red_web_dashboard-1.6.2/reddash/app/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/templates/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.708114 red_web_dashboard-1.6.2/reddash/app/templates/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/templates/errors/403.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/templates/errors/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/templates/errors/500.html
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/templates/errors/blacklisted.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/templates/errors/custom.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.708114 red_web_dashboard-1.6.2/reddash/app/templates/includes/
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/templates/includes/fixed-plugin.html
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/templates/includes/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/templates/includes/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11526 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/templates/includes/scripts.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/templates/includes/sidenav.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.712114 red_web_dashboard-1.6.2/reddash/app/templates/layouts/
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/templates/layouts/base-fullscreen.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/templates/layouts/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.712114 red_web_dashboard-1.6.2/reddash/app/templates/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)    29579 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/templates/pages/admin.html
+-rw-r--r--   0 runner    (1001) docker     (127)    17056 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/templates/pages/commands.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/templates/pages/credits.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/templates/pages/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (127)    30814 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/templates/pages/dashboard_guild.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/templates/pages/guild_profile.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/templates/pages/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.712114 red_web_dashboard-1.6.2/reddash/app/templates/pages/login/
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/templates/pages/login/login.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.712114 red_web_dashboard-1.6.2/reddash/app/templates/pages/third_parties/
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/templates/pages/third_parties/oauth.html
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/templates/pages/third_parties/third_parties.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/templates/pages/third_parties/third_parties_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/templates/pages/third_parties/third_party.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:49:49.712114 red_web_dashboard-1.6.2/reddash/app/third_parties/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/third_parties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/third_parties/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27785 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/reddash/app/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-20 14:49:49.716114 red_web_dashboard-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-20 14:49:45.000000 red_web_dashboard-1.6.2/setup.py
```

### Comparing `red_web_dashboard-1.6.0/LICENSE` & `red_web_dashboard-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/PKG-INFO` & `red_web_dashboard-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Red-Web-Dashboard
-Version: 1.6.0
+Version: 1.6.2
 Summary: An easy-to-use interactive web Dashboard to control your Red bot!
 Home-page: https://github.com/AAA3A-AAA3A/Red-Dashboard
 Author: Neuro Assassin & AAA3A
 License: AGPL-3.0
 Project-URL: Third Party Discord Server, https://discord.gg/red-cog-support-240154543684321280
 Project-URL: Documentation, https://red-web-dashboard.readthedocs.io/en/latest/
 Project-URL: Donate on Buy Me a Coffee, https://www.buymeacoffee.com/aaa3a
```

### Comparing `red_web_dashboard-1.6.0/README.md` & `red_web_dashboard-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/Red_Web_Dashboard.egg-info/PKG-INFO` & `red_web_dashboard-1.6.2/Red_Web_Dashboard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Red-Web-Dashboard
-Version: 1.6.0
+Version: 1.6.2
 Summary: An easy-to-use interactive web Dashboard to control your Red bot!
 Home-page: https://github.com/AAA3A-AAA3A/Red-Dashboard
 Author: Neuro Assassin & AAA3A
 License: AGPL-3.0
 Project-URL: Third Party Discord Server, https://discord.gg/red-cog-support-240154543684321280
 Project-URL: Documentation, https://red-web-dashboard.readthedocs.io/en/latest/
 Project-URL: Donate on Buy Me a Coffee, https://www.buymeacoffee.com/aaa3a
```

### Comparing `red_web_dashboard-1.6.0/Red_Web_Dashboard.egg-info/SOURCES.txt` & `red_web_dashboard-1.6.2/Red_Web_Dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/pyproject.toml` & `red_web_dashboard-1.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/__main__.py` & `red_web_dashboard-1.6.2/reddash/__main__.py`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/app.py` & `red_web_dashboard-1.6.2/reddash/app/app.py`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/base/routes.py` & `red_web_dashboard-1.6.2/reddash/app/base/routes.py`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/login/routes.py` & `red_web_dashboard-1.6.2/reddash/app/login/routes.py`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/biometric-icon.svg` & `red_web_dashboard-1.6.2/reddash/app/static/assets/biometric-icon.svg`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/css/argon-dashboard.css` & `red_web_dashboard-1.6.2/reddash/app/static/assets/css/argon-dashboard.css`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/css/argon-dashboard.css.map` & `red_web_dashboard-1.6.2/reddash/app/static/assets/css/argon-dashboard.css.map`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/css/argon-dashboard.min.css` & `red_web_dashboard-1.6.2/reddash/app/static/assets/css/argon-dashboard.min.css`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/css/nucleo-icons.css` & `red_web_dashboard-1.6.2/reddash/app/static/assets/css/nucleo-icons.css`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/css/nucleo-svg.css` & `red_web_dashboard-1.6.2/reddash/app/static/assets/css/nucleo-svg.css`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/css/simplemde.min.css` & `red_web_dashboard-1.6.2/reddash/app/static/assets/css/simplemde.min.css`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/css/themes/background_theme_dark.css` & `red_web_dashboard-1.6.2/reddash/app/static/assets/css/themes/background_theme_dark.css`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,45 @@
-body:not(.sidenav):not(.sidenav > *):not(.sidenav *),
-div.card:not(.sidenav):not(.sidenav > *):not(.sidenav *),
-div.card-header:not(.sidenav):not(.sidenav > *):not(.sidenav *) {
+body:not(.sidenav),
+div.card:not(.sidenav),
+div.card-header:not(.sidenav),
+div.card-body:not(.sidenav),
+.nav:not(.sidenav,.nav-item) {
     background-color: #333 !important;
+    color: white !important;
+}
+
+div.card:not(.sidenav), div.card:not(.sidenav) > *,
+.nav:not(.sidenav), .nav:not(.sidenav) > * {
+    border-radius: var(--bs-card-border-radius) !important;
 }
 
-body:not(.sidenav):not(.sidenav > *):not(.sidenav *),
-div.card:not(.sidenav):not(.sidenav > *):not(.sidenav *),
-div.card:not(.sidenav):not(.sidenav > *):not(.sidenav *) > *,
-div.card-header:not(.sidenav):not(.sidenav > *):not(.sidenav *),
-div.card-header:not(.sidenav):not(.sidenav > *):not(.sidenav *) > *,
-div.card-body:not(.sidenav):not(.sidenav > *):not(.sidenav *) {
+.nav.nav-pills .nav-link {
     color: white !important;
 }
+.moving-tab .nav-link {
+    color: black !important;
+}
+.moving-tab .nav-link.active {
+    color: black !important;
+    box-shadow: 0px 1px 5px 1px black !important;
+    background: black !important;
+}
+
+body:not(.sidenav) a:not(.btn,.nav-link,.nav-item,.paginationjs-page),
+div.card:not(.sidenav) a:not(.btn,.nav-link,.nav-item,.paginationjs-page),
+div.card-header:not(.sidenav) a:not(.btn,.nav-link,.nav-item,.paginationjs-page) {
+    color: var(--bs-indigo);
+}
 
-.choices__item--choice {
+.choices__item--choice,
+.choices[data-type=select-one] .choices__item {
     color: black !important;
 }
 
-div.card:not(.sidenav):not(.sidenav > *):not(.sidenav *) {
-    border-radius: var(--bs-card-border-radius) !important;
+.editor-toolbar button:not(.active,:hover),
+h1, h2, h3, h4, h5, h6, h1 *, h2 *, h3 *, h4 *, h5 *, h6 * {
+    color: white !important;
 }
 
-body:not(.sidenav):not(.sidenav > *) a:not(.btn,.nav-link,.nav-item,h6):not(.sidenav a:not(.btn,.nav-link,.nav-item,h6)),
-div.card:not(.sidenav):not(.sidenav > *) a:not(.btn,h6,.nav-link,.nav-item):not(.sidenav a:not(.btn,.nav-link,.nav-item,h6)),
-div.card-header:not(.sidenav):not(.sidenav > *) a:not(.btn,h6,.nav-link,.nav-item):not(.sidenav a:not(.btn,.nav-link,.nav-item,h6)) {
-    color: var(--bs-indigo);
+hr {
+    border-color: white !important;
 }
```

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/error-403.gif` & `red_web_dashboard-1.6.2/reddash/app/static/assets/error-403.gif`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/error-404.gif` & `red_web_dashboard-1.6.2/reddash/app/static/assets/error-404.gif`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/error-500.gif` & `red_web_dashboard-1.6.2/reddash/app/static/assets/error-500.gif`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo-icons.eot` & `red_web_dashboard-1.6.2/reddash/app/static/assets/fonts/nucleo-icons.eot`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo-icons.svg` & `red_web_dashboard-1.6.2/reddash/app/static/assets/fonts/nucleo-icons.svg`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo-icons.ttf` & `red_web_dashboard-1.6.2/reddash/app/static/assets/fonts/nucleo-icons.ttf`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo-icons.woff` & `red_web_dashboard-1.6.2/reddash/app/static/assets/fonts/nucleo-icons.woff`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo-icons.woff2` & `red_web_dashboard-1.6.2/reddash/app/static/assets/fonts/nucleo-icons.woff2`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo.eot` & `red_web_dashboard-1.6.2/reddash/app/static/assets/fonts/nucleo.eot`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo.ttf` & `red_web_dashboard-1.6.2/reddash/app/static/assets/fonts/nucleo.ttf`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo.woff` & `red_web_dashboard-1.6.2/reddash/app/static/assets/fonts/nucleo.woff`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/fonts/nucleo.woff2` & `red_web_dashboard-1.6.2/reddash/app/static/assets/fonts/nucleo.woff2`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/gulpfile.js` & `red_web_dashboard-1.6.2/reddash/app/static/assets/gulpfile.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/icon-documentation.svg` & `red_web_dashboard-1.6.2/reddash/app/static/assets/icon-documentation.svg`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/js/argon-dashboard.js` & `red_web_dashboard-1.6.2/reddash/app/static/assets/js/argon-dashboard.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/js/argon-dashboard.js.map` & `red_web_dashboard-1.6.2/reddash/app/static/assets/js/argon-dashboard.js.map`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/js/core/bootstrap.min.js` & `red_web_dashboard-1.6.2/reddash/app/static/assets/js/core/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/js/core/jquery.min.js` & `red_web_dashboard-1.6.2/reddash/app/static/assets/js/core/jquery.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/js/core/popper.min.js` & `red_web_dashboard-1.6.2/reddash/app/static/assets/js/core/popper.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/Chart.extension.js` & `red_web_dashboard-1.6.2/reddash/app/static/assets/js/plugins/Chart.extension.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/Simple-Full-featured-jQuery-Pagination-System-Pagination-js.zip` & `red_web_dashboard-1.6.2/reddash/app/static/assets/js/plugins/Simple-Full-featured-jQuery-Pagination-System-Pagination-js.zip`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/bootstrap-notify.js` & `red_web_dashboard-1.6.2/reddash/app/static/assets/js/plugins/bootstrap-notify.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/chartjs.min.js` & `red_web_dashboard-1.6.2/reddash/app/static/assets/js/plugins/chartjs.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/perfect-scrollbar.min.js` & `red_web_dashboard-1.6.2/reddash/app/static/assets/js/plugins/perfect-scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/smooth-scrollbar.min.js` & `red_web_dashboard-1.6.2/reddash/app/static/assets/js/plugins/smooth-scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/js/plugins/utils.js` & `red_web_dashboard-1.6.2/reddash/app/static/assets/js/plugins/utils.js`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/oauth.png` & `red_web_dashboard-1.6.2/reddash/app/static/assets/oauth.png`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/pdf.svg` & `red_web_dashboard-1.6.2/reddash/app/static/assets/pdf.svg`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/random.svg` & `red_web_dashboard-1.6.2/reddash/app/static/assets/random.svg`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_avatars.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_avatars.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_breadcrumbs.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_breadcrumbs.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_buttons.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_cards.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_cards.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_dark-version.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_dark-version.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_dropdown.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_dropup.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_dropup.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_fixed-plugin.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_fixed-plugin.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_forms.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_forms.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_gradients.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_gradients.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_header.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_header.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_info-areas.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_info-areas.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_misc.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_misc.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_nav.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_nav.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_navbar-vertical.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_navbar-vertical.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_navbar.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_navbar.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_pagination.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_pagination.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_rtl.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_rtl.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_social-buttons.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_social-buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_tables.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_tables.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_timeline.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_timeline.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_typography.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_typography.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_utilities.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_utilities.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/_variables.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/_variables.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_accordion.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_accordion.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_alert.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_alert.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_badge.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_badge.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_breadcrumb.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_button-group.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_button-group.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_buttons.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_card.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_card.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_carousel.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_carousel.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_close.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_close.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_containers.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_containers.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_dropdown.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_functions.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_functions.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_grid.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_grid.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_images.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_images.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_list-group.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_list-group.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_maps.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_maps.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_mixins.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_mixins.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_modal.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_modal.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_nav.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_nav.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_navbar.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_navbar.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_offcanvas.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_offcanvas.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_pagination.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_pagination.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_placeholders.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_placeholders.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_popover.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_popover.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_progress.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_progress.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_reboot.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_reboot.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_root.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_root.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_spinners.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_spinners.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tables.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tables.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_toasts.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_toasts.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tooltip.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_type.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_type.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_utilities.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_utilities.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_variables.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/_variables.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-grid.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_floating-labels.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_floating-labels.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-check.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-control.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-control.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-range.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-range.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-select.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_form-select.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_input-group.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_labels.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/forms/_labels.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_position.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/helpers/_position.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_border-radius.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_breakpoints.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_buttons.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_caret.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_deprecate.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_forms.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_gradients.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_grid.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_table-variants.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_table-variants.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_transition.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_transition.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_utilities.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_utilities.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_visually-hidden.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/mixins/_visually-hidden.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/_api.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/utilities/_api.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/_rfs.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/bootstrap/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/cards/card-background.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/cards/card-background.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-check.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/forms/_form-switch.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/forms/_form-switch.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/forms/_input-group.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/mixins/_social-buttons.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/mixins/_social-buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_flatpickr.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_flatpickr.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_nouislider.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_nouislider.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_perfect-scrollbar.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_perfect-scrollbar.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_prism.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/plugins/free/_prism.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/theme.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/theme.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_animations.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_animations.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_avatars.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_avatars.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_badge.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_badge.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards-extend.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_cards-extend.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_cards.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_cards.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dark-version.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_dark-version.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_dropdowns.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_dropdowns.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_header.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_header.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_info-areas.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_info-areas.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc-extend.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_misc-extend.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_misc.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_misc.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar-vertical.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar-vertical.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_navbar.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_pagination.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_pagination.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_social-buttons.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_social-buttons.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_table.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_table.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_timeline.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_timeline.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities-extend.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities-extend.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard/variables/_utilities.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/static/assets/scss/argon-dashboard.scss` & `red_web_dashboard-1.6.2/reddash/app/static/assets/scss/argon-dashboard.scss`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/tasks_manager.py` & `red_web_dashboard-1.6.2/reddash/app/tasks_manager.py`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/templates/errors/403.html` & `red_web_dashboard-1.6.2/reddash/app/templates/errors/403.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/templates/errors/404.html` & `red_web_dashboard-1.6.2/reddash/app/templates/errors/404.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/templates/errors/500.html` & `red_web_dashboard-1.6.2/reddash/app/templates/errors/500.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/templates/errors/blacklisted.html` & `red_web_dashboard-1.6.2/reddash/app/templates/errors/blacklisted.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/templates/errors/custom.html` & `red_web_dashboard-1.6.2/reddash/app/templates/errors/custom.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/templates/includes/fixed-plugin.html` & `red_web_dashboard-1.6.2/reddash/app/templates/includes/fixed-plugin.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/templates/includes/footer.html` & `red_web_dashboard-1.6.2/reddash/app/templates/includes/footer.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/templates/includes/navigation.html` & `red_web_dashboard-1.6.2/reddash/app/templates/includes/navigation.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/templates/includes/scripts.html` & `red_web_dashboard-1.6.2/reddash/app/templates/includes/scripts.html`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,16 @@
         {% if messages %}
             {% for category, message in messages %}
                 toastr.{{ category }}("{{ message|replace('\n', ' ') }}");
             {% endfor %}
         {% endif %}
     {% endwith %}
 </script>
-<script src="//cdnjs.cloudflare.com/ajax/libs/highlight.js/11.7.0/highlight.min.js"></script>
+<script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/highlight.min.js"></script>
+<script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/languages/python.min.js"></script>
 <script>
     document.addEventListener("DOMContentLoaded", (event) => {
         document.querySelectorAll("pre code").forEach((block) => {
             hljs.highlightBlock(block);
         });
     });
 </script>
```

### Comparing `red_web_dashboard-1.6.0/reddash/app/templates/includes/sidenav.html` & `red_web_dashboard-1.6.2/reddash/app/templates/includes/sidenav.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/templates/layouts/base-fullscreen.html` & `red_web_dashboard-1.6.2/reddash/app/templates/layouts/base-fullscreen.html`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
      <style>
        body #toast-container > div {
          opacity: 1;
          margin-top: 6px;
          width: 500px !important;
        }
      </style>
-     <link href="//cdnjs.cloudflare.com/ajax/libs/highlight.js/11.7.0/styles/default.min.css" rel="stylesheet" />
+     <link href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/styles/default.min.css" rel="stylesheet" />
      <link href="https://cdn.jsdelivr.net/npm/easymde/dist/easymde.min.css" rel="stylesheet" />
      <style>
        .EasyMDEContainer {
          .editor-toolbar i.separator {
            position: relative; /* Fix separator icons display. */
            height: auto;
          }
```

### Comparing `red_web_dashboard-1.6.0/reddash/app/templates/layouts/base.html` & `red_web_dashboard-1.6.2/reddash/app/templates/layouts/base.html`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     <style>
       body #toast-container > div {
         opacity: 1;
         margin-top: 6px;
         width: 500px !important;
       }
     </style>
-    <link href="//cdnjs.cloudflare.com/ajax/libs/highlight.js/11.7.0/styles/default.min.css" rel="stylesheet" />
+    <link href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/styles/default.min.css" rel="stylesheet" />
     <link href="https://cdn.jsdelivr.net/npm/easymde/dist/easymde.min.css" rel="stylesheet" />
     <style>
       .EasyMDEContainer {
         .editor-toolbar i.separator {
           position: relative; /* Fix separator icons display. */
           height: auto;
         }
```

### Comparing `red_web_dashboard-1.6.0/reddash/app/templates/pages/admin.html` & `red_web_dashboard-1.6.2/reddash/app/templates/pages/admin.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/templates/pages/commands.html` & `red_web_dashboard-1.6.2/reddash/app/templates/pages/commands.html`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,16 @@
                                                 <div class="col-sm-12">
                                                     <h3 class="card-title">{{ cog }}</h3>
                                                     <p>{{ cogs[cog]["description"]|markdown }}</p>
                                                 </div>
                                               </div>
                                               <div class="row">
                                                 <div class="col-ms-8">
-                                                    <p class="mb-0">{{ (_("Author(s): {author}")).format(author=cogs[cog]["author"])}}</p>
-                                                    <p>{{ _("Repo:") }} <a {% if cogs[cog]["repo"] != "Unknown" %}href="{{ cogs[cog]["repo"] }}"{% endif %}>{{ cogs[cog]["repo"] }}</a></p>
+                                                    <p class="mb-0"><b>{{ _("Author(s):") }}</b> {{ cogs[cog]["author"] }}</p>
+                                                    <p><b>{{ _("Repo:") }}</b> <a {% if cogs[cog]["repo"] != "Unknown" %}href="{{ cogs[cog]["repo"] }}"{% endif %}>{{ cogs[cog]["repo"] }}</a></p>
                                                 </div>
                                                 <div class="col-sm-4 text-left">
                                                     <div class="dropdown show">
                                                         <a class="btn bg-gradient-{{ variables["meta"]["color"] }} dropdown-toggle" href="#" role="button" id="prefixdrop_dropdown" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                                             {{ _("Prefix") }}
                                                         </a>
                                                         <ul class="dropdown-menu prefixdiv" aria-labelledby="prefixdrop_dropdown">
@@ -90,15 +90,15 @@
                                                           {% if command.signature or command.aliases %}
                                                             <tr>
                                                               <td colspan="2" style="border: none; padding: 0px;">
                                                                 <div class="collapse" id="collapse_{{ command.name }}">
                                                                   <div class="d-flex card card-body text-wrap">
                                                                     {% if command.signature %}
                                                                       <strong>{{ _("Usage:") }}</strong>
-                                                                      <div class="d-flex"><code>{{ prefixes[0] }}{{ command.name }} {{ command.signature }}</code> <a href="javascript:copyTextToClipboard('{{ prefixes[0] }}{{ command.name }} {{ command.signature }}');" title="{{ _("Copy to clipboard") }}"><i class="far fa-copy me-2"></i></a></div>
+                                                                      <div class="d-flex"><code>{{ prefixes[0] }}{{ command.name }} {{ command.signature }}</code> <a href="javascript:copyTextToClipboard('{{ prefixes[0] }}{{ command.name }} {{ command.signature }}');" title="{{ _("Copy to clipboard") }}" style="margin-left: 10px;"><i class="far fa-copy me-2"></i></a></div>
                                                                     {% endif %}
                                                                     <br />
                                                                     {% if command.aliases %}
                                                                       <strong>{{ _("Aliases:") }}</strong>
                                                                       <code>{{ command.aliases|join(", ") }}</code>
                                                                     {% endif %}
                                                                   </div>
@@ -162,15 +162,15 @@
                                             {% if command.signature or command.aliases %}
                                               <tr>
                                                 <td colspan="2" style="border: none; padding: 0px;">
                                                   <div class="collapse" id="collapse_{{ command.name }}">
                                                     <div class="d-flex card card-body text-wrap">
                                                       {% if command.signature %}
                                                         <strong>{{ _("Usage:") }}</strong>
-                                                        <div class="d-flex"><code>{{ prefixes[0] }}{{ command.name }} {{ command.signature }}</code> <a href="javascript:copyTextToClipboard('{{ prefixes[0] }}{{ command.name }} {{ command.signature }}');" title="{{ _("Copy to clipboard") }}"><i class="far fa-copy me-2"></i></a></div>
+                                                        <div class="d-flex"><code>{{ prefixes[0] }}{{ command.name }} {{ command.signature }}</code> <a href="javascript:copyTextToClipboard('{{ prefixes[0] }}{{ command.name }} {{ command.signature }}');" title="{{ _("Copy to clipboard") }}" style="margin-left: 10px;"><i class="far fa-copy me-2"></i></a></div>
                                                       {% endif %}
                                                       <br />
                                                       {% if command.aliases %}
                                                         <strong>{{ _("Aliases:") }}</strong>
                                                         <code>{{ command.aliases|join(", ") }}</code>
                                                       {% endif %}
                                                     </div>
@@ -211,52 +211,54 @@
     </div>
   </main>
 {% endblock %}
 
 {% block javascripts %}
   <script>
     window.onload = function() {
-        resize_event = new Event("resize");
-        window.dispatchEvent(resize_event);
+      resize_event = new Event("resize");
+      window.dispatchEvent(resize_event);
     }
   </script>
   <script>
     function changePage(tab_name) {
-        var tab_nav_link = document.querySelector("#" + tab_name + "-tab");
-        if (tab_nav_link) {
-            tab_nav_link.parentElement.parentElement.onmouseover(tab_nav_link);
-            tab_nav_link.click();
-        }
+      var tab_nav_link = document.querySelector("#" + tab_name + "-tab");
+      if (tab_nav_link) {
+        tab_nav_link.parentElement.parentElement.onmouseover(tab_nav_link);
+        tab_nav_link.click();
+      }
     }
     {% if tab_name %}
-        document.addEventListener("DOMContentLoaded", function() {
-            changePage("{{ tab_name }}");
-        });
+      document.addEventListener("DOMContentLoaded", function() {
+        setTimeout(function() {
+          changePage("{{ tab_name }}");
+        }, 500);
+      });
     {% endif %}
   </script>
   <script>
     $('#commands-tabs a[data-toggle="pill"]').on("shown.bs.tab", function(e) {
-        var target_id = e.target.id.slice(0, -4);
-        var new_url = "/commands/" + target_id;
-        if (!(window.location.pathname.startsWith(new_url))) {
-            // window.location.pathname = new_url;
-            window.history.pushState({}, "", new_url);
-        }
+      var target_id = e.target.id.slice(0, -4);
+      var new_url = "/commands/" + target_id;
+      if (!(window.location.pathname.startsWith(new_url))) {
+        // window.location.pathname = new_url;
+        window.history.pushState({}, "", new_url);
+      }
     });
   </script>
   <script>
     $(".prefix-option").click(function () {
-        let prefix = $(this).text();
-        $(".prefix").text(prefix);
-        // Change others to inactive, and the correct ones to active.
-        $(".prefix-option").removeClass("active");
-        let index = $(this).index();
-        $(".prefixdiv").each(function (someotherindexidontneed) {
-            $(this).children().eq(index).addClass("active");
-        })
+      let prefix = $(this).text();
+      $(".prefix").text(prefix);
+      // Change others to inactive, and the correct ones to active.
+      $(".prefix-option").removeClass("active");
+      let index = $(this).index();
+      $(".prefixdiv").each(function (someotherindexidontneed) {
+        $(this).children().eq(index).addClass("active");
+      })
     })
   </script>
   <script>
     function submitSearch(event) {
       event.preventDefault();
       let input = document.getElementById("command-search");
       let query = input.value.trim();
```

### Comparing `red_web_dashboard-1.6.0/reddash/app/templates/pages/credits.html` & `red_web_dashboard-1.6.2/reddash/app/templates/pages/credits.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/templates/pages/dashboard_guild.html` & `red_web_dashboard-1.6.2/reddash/app/templates/pages/dashboard_guild.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/templates/pages/guild_profile.html` & `red_web_dashboard-1.6.2/reddash/app/templates/pages/guild_profile.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/templates/pages/index.html` & `red_web_dashboard-1.6.2/reddash/app/templates/pages/index.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/templates/pages/login/login.html` & `red_web_dashboard-1.6.2/reddash/app/templates/pages/login/login.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/templates/pages/third_parties/oauth.html` & `red_web_dashboard-1.6.2/reddash/app/templates/pages/third_parties/oauth.html`

 * *Files identical despite different names*

### Comparing `red_web_dashboard-1.6.0/reddash/app/templates/pages/third_parties/third_parties_list.html` & `red_web_dashboard-1.6.2/reddash/app/templates/pages/third_parties/third_parties_list.html`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,16 @@
                                         <div class="col-sm-12">
                                             <h3 class="card-title">{{ third_party }}</h3>
                                             <p>{{ third_parties_infos[third_party]["description"]|markdown }}</p>
                                         </div>
                                       </div>
                                       <div class="row">
                                           <div class="col-ms-8">
-                                              <p class="mb-0">{{ (_("Author(s): {author}")).format(author=third_parties_infos[third_party]["author"])}}</p>
-                                              <p>{{ _("Repo:") }} <a {% if third_parties_infos[third_party]["repo"] != "Unknown" %}href="{{ third_parties_infos[third_party]["repo"] }}"{% endif %}>{{ third_parties_infos[third_party]["repo"] }}</a></p>
+                                              <p class="mb-0"><b>{{ _("Author(s):") }}</b> {{ third_parties_infos[third_party]["author"] }}</p>
+                                              <p><b>{{ _("Repo:") }}</b> <a {% if third_parties_infos[third_party]["repo"] != "Unknown" %}href="{{ third_parties_infos[third_party]["repo"] }}"{% endif %}>{{ third_parties_infos[third_party]["repo"] }}</a></p>
                                           </div>
                                       </div>
                                       <table class="table tablesorter">
                                           <thead class="text-primary">
                                               <tr>
                                                   <th>{{ _("Page") }}</th>
                                                   <th>{{ _("Description") }}</th>
@@ -86,38 +86,40 @@
       </div>
     {% endif %}
   </div>
 
 {% block javascripts %}
   <script>
     window.onload = function() {
-        resize_event = new Event("resize");
-        window.dispatchEvent(resize_event);
+      resize_event = new Event("resize");
+      window.dispatchEvent(resize_event);
     }
   </script>
   <script>
     function changePage(tab_name) {
-        var tab_nav_link = document.querySelector("#" + tab_name + "-tab");
-        if (tab_nav_link) {
-            tab_nav_link.parentElement.parentElement.onmouseover(tab_nav_link);
-            tab_nav_link.click();
-        }
+      var tab_nav_link = document.querySelector("#" + tab_name + "-tab");
+      if (tab_nav_link) {
+        tab_nav_link.parentElement.parentElement.onmouseover(tab_nav_link);
+        tab_nav_link.click();
+      }
     }
     {% if tab_name %}
-        document.addEventListener("DOMContentLoaded", function() {
-            changePage("{{ tab_name }}");
-        });
+      document.addEventListener("DOMContentLoaded", function() {
+        setTimeout(function() {
+          changePage("{{ tab_name }}");
+        }, 500);
+      });
     {% endif %}
   </script>
   <script>
     document.querySelectorAll('#third-parties-tabs a[data-toggle="pill"]').forEach(function(element) {
       element.addEventListener("shown.bs.tab", function(e) {
-          var target_id = e.target.id.slice(0, -4);
-          var new_url = "/third-parties/" + target_id;
-          if (!(window.location.pathname.startsWith(new_url))) {
-              // window.location.pathname = new_url;
-              window.history.pushState({}, "", new_url);
-          }
+        var target_id = e.target.id.slice(0, -4);
+        var new_url = "/third-parties/" + target_id;
+        if (!(window.location.pathname.startsWith(new_url))) {
+          // window.location.pathname = new_url;
+          window.history.pushState({}, "", new_url);
+        }
       });
     });
   </script>
 {% endblock %}
```

### Comparing `red_web_dashboard-1.6.0/reddash/app/templates/pages/third_parties/third_party.html` & `red_web_dashboard-1.6.2/reddash/app/templates/pages/third_parties/third_party.html`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                                                 {% endif %}
                                             {% else %}
                                                 <h2 class="card-title"><a href="{{ url_for("third_parties_blueprint.third_parties", third_party=name) }}">🔙 {{ name }}</a>{% if page %} / {{ page|replace("_", " ")|replace("-", " ")|title }}{% endif %}</h2>
                                             {% endif %}
                                         </div>
                                     </div>
                                 </div>
-                                <div class="container mt-4">
+                                <div id="third-party-content" class="container mt-4">
                                     {{ source_content|safe }}
                                 </div>
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
```

### Comparing `red_web_dashboard-1.6.0/reddash/app/utils.py` & `red_web_dashboard-1.6.2/reddash/app/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 from flask_sitemapper import Sitemapper
 from flask_talisman import Talisman
 from flask_wtf.csrf import CSRFProtect
 from flask_wtf.file import FileAllowed, FileField, MultipleFileField
 from wtforms import Field, SelectFieldBase, FormField
 from fuzzywuzzy import process
 from markdown import Markdown
+from pygments import highlight
+from pygments.formatters import HtmlFormatter
+from pygments.lexers import Python3TracebackLexer, get_lexer_by_name
 import bleach
 from markupsafe import Markup
 
 settings.configure()
 from django_user_agents.utils import get_user_agent
 
 AVAILABLE_COLORS: typing.List[str] = [
@@ -198,15 +201,16 @@
             ("192.168.0.0", "192.168.255.255"),
         ]
         if any(start <= request.remote_addr <= end for start, end in private_ip_ranges):
             return
         return old_force_https()
 
     app.talisman._force_https = _force_https
-    app.talisman.init_app(app, force_https=False, content_security_policy=None)
+    allow_unsecure_http_requests = app.data["core"]["allow_unsecure_http_requests"]
+    app.talisman.init_app(app, force_https=not allow_unsecure_http_requests, session_cookie_secure=not allow_unsecure_http_requests, content_security_policy=None)
 
     app.config["WTF_CSRF_ENABLED"]: bool = True
     app.config["WTF_CSRF_SECRET_KEY"]: str = base64.urlsafe_b64decode(
         Fernet.generate_key().decode()
     )
     app.csrf_protect: CSRFProtect = CSRFProtect()
     app.csrf_protect.init_app(app)
@@ -274,14 +278,24 @@
     app.markdown: Markdown = Markdown()
 
     @app.template_filter("markdown")
     def markdown_filter(text: str) -> Markup:
         text = bleach.clean(text, tags=[], strip=False)
         return Markup(app.markdown.convert(text.replace("\n", "<br />")))
 
+    @app.template_filter("highlight")
+    def highlight_filter(code, language="python"):
+        code = bleach.clean(code, tags=[], strip=False).replace("&lt;", "<").replace("&gt;", ">")
+        if language == "traceback":
+            lexer = Python3TracebackLexer()
+        else:
+            lexer = get_lexer_by_name(language, stripall=True)
+        formatter = HtmlFormatter()
+        return highlight(code, lexer, formatter)
+
     app.site_mapper: Sitemapper = Sitemapper(https=not app.testing)
 
 
 def register_blueprints(app: Flask) -> None:
     for module_name in ("base", "login", "third_parties"):
         module = import_module(f"reddash.app.{module_name}.routes")
         app.register_blueprint(module.blueprint)
```

### Comparing `red_web_dashboard-1.6.0/setup.cfg` & `red_web_dashboard-1.6.2/setup.cfg`

 * *Files identical despite different names*
