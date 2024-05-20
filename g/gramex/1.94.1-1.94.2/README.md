# Comparing `tmp/gramex-1.94.1.tar.gz` & `tmp/gramex-1.94.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gramex-1.94.1.tar", last modified: Sat Mar  2 06:01:17 2024, max compression
+gzip compressed data, was "gramex-1.94.2.tar", last modified: Mon May 20 10:34:05 2024, max compression
```

## Comparing `gramex-1.94.1.tar` & `gramex-1.94.2.tar`

### file list

```diff
@@ -1,397 +1,324 @@
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.861294 gramex-1.94.1/
--rw-rw-rw-   0        0        0     1968 2023-07-31 04:30:40.000000 gramex-1.94.1/.gitignore
--rw-rw-rw-   0        0        0     1274 2023-07-31 04:30:40.000000 gramex-1.94.1/LICENSE
--rw-rw-rw-   0        0        0      641 2023-07-31 04:30:40.000000 gramex-1.94.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5875 2024-03-02 06:01:17.861294 gramex-1.94.1/PKG-INFO
--rw-rw-rw-   0        0        0     1212 2023-07-31 04:30:40.000000 gramex-1.94.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.211133 gramex-1.94.1/gramex/
--rw-rw-rw-   0        0        0    15372 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/__init__.py
--rw-rw-rw-   0        0        0      242 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/__main__.py
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.259077 gramex-1.94.1/gramex/apps/
--rw-rw-rw-   0        0        0        0 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.261259 gramex-1.94.1/gramex/apps/admin/
--rw-rw-rw-   0        0        0        9 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/admin/.gitignore
--rw-rw-rw-   0        0        0      129 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/admin/gramex.yaml
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.284435 gramex-1.94.1/gramex/apps/admin2/
--rw-rw-rw-   0        0        0      228 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/admin2/admin.css
--rw-rw-rw-   0        0        0     3152 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/apps/admin2/gramex.yaml
--rw-rw-rw-   0        0        0    12443 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/apps/admin2/gramexadmin.py
--rw-rw-rw-   0        0        0     8420 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/admin2/index.html
--rw-rw-rw-   0        0        0     5216 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/admin2/schedule.js
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.342045 gramex-1.94.1/gramex/apps/capture/
--rw-rw-rw-   0        0        0      293 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/apps/capture/.snyk
--rw-rw-rw-   0        0        0     4061 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/capture/README.md
--rw-rw-rw-   0        0        0     9487 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/apps/capture/capture.js
--rw-rw-rw-   0        0        0    12290 2023-09-21 00:20:48.000000 gramex-1.94.1/gramex/apps/capture/chromecapture.js
--rw-rw-rw-   0        0        0     4197 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/capture/index.html
--rw-rw-rw-   0        0        0    80190 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/apps/capture/package-lock.json
--rw-rw-rw-   0        0        0      863 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/capture/package.json
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.348690 gramex-1.94.1/gramex/apps/filemanager/
--rw-rw-rw-   0        0        0     2845 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/filemanager/README.html
--rw-rw-rw-   0        0        0      700 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/filemanager/drivehandler-snippet.html
--rw-rw-rw-   0        0        0      612 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/filemanager/filemanager-snippet.html
--rw-rw-rw-   0        0        0     2578 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/filemanager/filemanager.html
--rw-rw-rw-   0        0        0     3070 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/filemanager/filemanager.js
--rw-rw-rw-   0        0        0      926 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/filemanager/filemanager.py
--rw-rw-rw-   0        0        0      621 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/filemanager/gramex.yaml
--rw-rw-rw-   0        0        0      914 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/filemanager/index.html
--rw-rw-rw-   0        0        0      872 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/filemanager/navbar.html
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.050123 gramex-1.94.1/gramex/apps/init/
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.367333 gramex-1.94.1/gramex/apps/init/default/
--rw-rw-rw-   0        0        0      578 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/init/default/.eslintrc.yml
--rw-rw-rw-   0        0        0       71 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/init/default/.flake8
--rw-rw-rw-   0        0        0      756 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/init/default/.gitlab-ci.yml
--rw-rw-rw-   0        0        0      383 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/apps/init/default/.secrets.yaml
--rw-rw-rw-   0        0        0     1635 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/init/default/.template.gitignore
--rw-rw-rw-   0        0        0      248 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/init/default/README.template.md
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.368337 gramex-1.94.1/gramex/apps/init/default/assets/
--rw-rw-rw-   0        0        0      519 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/init/default/assets/README.template.md
--rw-rw-rw-   0        0        0     1756 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/init/default/gramex.template.yaml
--rw-rw-rw-   0        0        0      694 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/init/default/index.template.html
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.368337 gramex-1.94.1/gramex/apps/init/default/js/
--rw-rw-rw-   0        0        0      602 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/init/default/js/README.template.md
--rw-rw-rw-   0        0        0     2608 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/init/default/login.template.html
--rw-rw-rw-   0        0        0      352 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/init/default/package.template.json
--rw-rw-rw-   0        0        0       80 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/init/default/style.scss
--rw-rw-rw-   0        0        0     3499 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/init/default/template-navbar.template.html
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.370349 gramex-1.94.1/gramex/apps/init/ide/
--rw-rw-rw-   0        0        0      378 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/init/ide/.gitlab-ci.template.yml
--rw-rw-rw-   0        0        0      244 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/init/ide/gramex.template.yaml
--rw-rw-rw-   0        0        0      738 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/init/ide/index.template.html
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.371353 gramex-1.94.1/gramex/apps/init/minimal/
--rw-rw-rw-   0        0        0      247 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/init/minimal/gramex.template.yaml
--rw-rw-rw-   0        0        0      757 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/init/minimal/index.template.html
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.373353 gramex-1.94.1/gramex/apps/languagetool/
--rw-rw-rw-   0        0        0      709 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/languagetool/README.md
--rw-rw-rw-   0        0        0        0 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/languagetool/__init__.py
--rw-rw-rw-   0        0        0      788 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/languagetool/gramex.yaml
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.392980 gramex-1.94.1/gramex/apps/logviewer/
--rw-rw-rw-   0        0        0        0 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/logviewer/__init__.py
--rw-rw-rw-   0        0        0     3466 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/logviewer/config.yaml
--rw-rw-rw-   0        0        0     6278 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/apps/logviewer/gramex.yaml
--rw-rw-rw-   0        0        0     4958 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/logviewer/index.html
--rw-rw-rw-   0        0        0    13287 2024-01-29 15:13:34.000000 gramex-1.94.1/gramex/apps/logviewer/logviewer.py
--rw-rw-rw-   0        0        0      210 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/logviewer/lv-card-deck.html
--rw-rw-rw-   0        0        0      386 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/logviewer/lv-card.html
--rw-rw-rw-   0        0        0      526 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/logviewer/lv-datepicker.html
--rw-rw-rw-   0        0        0      331 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/logviewer/lv-dropdown.html
--rw-rw-rw-   0        0        0      465 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/logviewer/lv-filters.html
--rw-rw-rw-   0        0        0      113 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/logviewer/lv-header.html
--rw-rw-rw-   0        0        0      335 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/logviewer/lv-kpi.html
--rw-rw-rw-   0        0        0      514 2024-03-02 05:49:23.000000 gramex-1.94.1/gramex/apps/logviewer/package-lock.json
--rw-rw-rw-   0        0        0      179 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/logviewer/package.json
--rw-rw-rw-   0        0        0     6928 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/logviewer/render.js
--rw-rw-rw-   0        0        0     5390 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/logviewer/script.js
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.394976 gramex-1.94.1/gramex/apps/mail/
--rw-rw-rw-   0        0        0      430 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/mail/gramex.yaml
--rw-rw-rw-   0        0        0     3032 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/mail/index.html
--rw-rw-rw-   0        0        0      251 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/mail/mailapp.py
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.428172 gramex-1.94.1/gramex/apps/mlhandler/
--rw-rw-rw-   0        0        0    15151 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/apps/mlhandler/template.html
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.438784 gramex-1.94.1/gramex/apps/pynode/
--rw-rw-rw-   0        0        0       47 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/pynode/README.md
--rw-rw-rw-   0        0        0     4127 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/pynode/index.js
--rw-rw-rw-   0        0        0     1902 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/apps/pynode/package-lock.json
--rw-rw-rw-   0        0        0      187 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/pynode/package.json
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.440288 gramex-1.94.1/gramex/apps/smartalerts/
--rw-rw-rw-   0        0        0       89 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/smartalerts/gramex.yaml
--rw-rw-rw-   0        0        0      429 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/smartalerts/index.html
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.482011 gramex-1.94.1/gramex/apps/ui/
--rw-rw-rw-   0        0        0      856 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/apps/ui/.snyk
--rw-rw-rw-   0        0        0    13166 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/apps/ui/__init__.py
--rw-rw-rw-   0        0        0      648 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/bootstrap-theme.scss
--rw-rw-rw-   0        0        0     1056 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/config.yaml
--rw-rw-rw-   0        0        0     2082 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/gramex.yaml
--rw-rw-rw-   0        0        0    25271 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/gramexui.scss
--rw-rw-rw-   0        0        0    96908 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/apps/ui/package-lock.json
--rw-rw-rw-   0        0        0      265 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/apps/ui/package.json
--rw-rw-rw-   0        0        0     2490 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/setup.js
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.487011 gramex-1.94.1/gramex/apps/ui/theme/
--rw-rw-rw-   0        0        0    19355 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootstrap5.scss
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.513474 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/
--rw-rw-rw-   0        0        0     6324 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/cerulean.png
--rw-rw-rw-   0        0        0      175 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/cerulean.scss
--rw-rw-rw-   0        0        0     4833 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/cosmo.png
--rw-rw-rw-   0        0        0      166 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/cosmo.scss
--rw-rw-rw-   0        0        0     6569 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/cyborg.png
--rw-rw-rw-   0        0        0      169 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/cyborg.scss
--rw-rw-rw-   0        0        0     5932 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/darkly.png
--rw-rw-rw-   0        0        0      169 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/darkly.scss
--rw-rw-rw-   0        0        0     5114 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/flatly.png
--rw-rw-rw-   0        0        0      169 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/flatly.scss
--rw-rw-rw-   0        0        0     5335 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/journal.png
--rw-rw-rw-   0        0        0      172 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/journal.scss
--rw-rw-rw-   0        0        0     6141 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/litera.png
--rw-rw-rw-   0        0        0      169 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/litera.scss
--rw-rw-rw-   0        0        0     4958 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/lumen.png
--rw-rw-rw-   0        0        0      166 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/lumen.scss
--rw-rw-rw-   0        0        0     4818 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/lux.png
--rw-rw-rw-   0        0        0      160 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/lux.scss
--rw-rw-rw-   0        0        0     5791 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/materia.png
--rw-rw-rw-   0        0        0      172 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/materia.scss
--rw-rw-rw-   0        0        0     5662 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/minty.png
--rw-rw-rw-   0        0        0      166 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/minty.scss
--rw-rw-rw-   0        0        0     4777 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/pulse.png
--rw-rw-rw-   0        0        0      166 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/pulse.scss
--rw-rw-rw-   0        0        0     5246 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/sandstone.png
--rw-rw-rw-   0        0        0      178 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/sandstone.scss
--rw-rw-rw-   0        0        0     6213 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/simplex.png
--rw-rw-rw-   0        0        0      172 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/simplex.scss
--rw-rw-rw-   0        0        0     7371 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/sketchy.png
--rw-rw-rw-   0        0        0      172 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/sketchy.scss
--rw-rw-rw-   0        0        0     6288 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/slate.png
--rw-rw-rw-   0        0        0      166 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/slate.scss
--rw-rw-rw-   0        0        0     6158 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/solar.png
--rw-rw-rw-   0        0        0      166 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/solar.scss
--rw-rw-rw-   0        0        0     6501 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/spacelab.png
--rw-rw-rw-   0        0        0      175 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/spacelab.scss
--rw-rw-rw-   0        0        0     6357 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/superhero.png
--rw-rw-rw-   0        0        0      178 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/superhero.scss
--rw-rw-rw-   0        0        0     5432 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/united.png
--rw-rw-rw-   0        0        0      169 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/united.scss
--rw-rw-rw-   0        0        0     4842 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/yeti.png
--rw-rw-rw-   0        0        0      163 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/bootswatch/yeti.scss
--rw-rw-rw-   0        0        0     4573 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/default.png
--rw-rw-rw-   0        0        0       20 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/default.scss
--rw-rw-rw-   0        0        0      831 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/index.html
--rw-rw-rw-   0        0        0    71063 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/sample.html
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.531329 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/
--rw-rw-rw-   0        0        0     6383 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/blue_voltage.png
--rw-rw-rw-   0        0        0      630 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/blue_voltage.scss
--rw-rw-rw-   0        0        0     6282 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/boldstrap.png
--rw-rw-rw-   0        0        0      478 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/boldstrap.scss
--rw-rw-rw-   0        0        0     6215 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/bootstrap_purple.png
--rw-rw-rw-   0        0        0      268 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/bootstrap_purple.scss
--rw-rw-rw-   0        0        0     6153 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/darkster.png
--rw-rw-rw-   0        0        0     2559 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/darkster.scss
--rw-rw-rw-   0        0        0     5497 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/fresca.png
--rw-rw-rw-   0        0        0      362 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/fresca.scss
--rw-rw-rw-   0        0        0     5525 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/greyson.png
--rw-rw-rw-   0        0        0      571 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/greyson.scss
--rw-rw-rw-   0        0        0     5153 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/hello_kiddie.png
--rw-rw-rw-   0        0        0      621 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/hello_kiddie.scss
--rw-rw-rw-   0        0        0     5523 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/herbie.png
--rw-rw-rw-   0        0        0      480 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/herbie.scss
--rw-rw-rw-   0        0        0     6585 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/hootstrap.png
--rw-rw-rw-   0        0        0      487 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/hootstrap.scss
--rw-rw-rw-   0        0        0     5491 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/lovey.png
--rw-rw-rw-   0        0        0      461 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/lovey.scss
--rw-rw-rw-   0        0        0     6009 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/monotony.png
--rw-rw-rw-   0        0        0      486 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/monotony.scss
--rw-rw-rw-   0        0        0     5546 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/poypull.png
--rw-rw-rw-   0        0        0      541 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/poypull.scss
--rw-rw-rw-   0        0        0     5430 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/signal.png
--rw-rw-rw-   0        0        0      576 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/signal.scss
--rw-rw-rw-   0        0        0     5338 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/tequila.png
--rw-rw-rw-   0        0        0      371 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes-guide/tequila.scss
--rw-rw-rw-   0        0        0      801 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/ui/theme/themes.json
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.553969 gramex-1.94.1/gramex/apps/uifactory/
--rw-rw-rw-   0        0        0      739 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/.eslintrc.js
--rw-rw-rw-   0        0        0       46 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/.gitattributes
--rw-rw-rw-   0        0        0       57 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/.gitignore
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.554969 gramex-1.94.1/gramex/apps/uifactory/assets/
--rw-rw-rw-   0        0        0      432 2023-07-31 04:30:41.000000 gramex-1.94.1/gramex/apps/uifactory/assets/README.md
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.602988 gramex-1.94.1/gramex/apps/uifactory/assets/data/
--rw-rw-rw-   0        0        0     1674 2023-07-31 04:30:41.000000 gramex-1.94.1/gramex/apps/uifactory/assets/data/input.json
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.606978 gramex-1.94.1/gramex/apps/uifactory/assets/img/
--rw-rw-rw-   0        0        0      706 2023-07-31 04:30:41.000000 gramex-1.94.1/gramex/apps/uifactory/assets/img/arrows-move.svg
--rw-rw-rw-   0        0        0      496 2023-07-31 04:30:41.000000 gramex-1.94.1/gramex/apps/uifactory/assets/img/clipboard.svg
--rw-rw-rw-   0        0        0      978 2023-07-31 04:30:41.000000 gramex-1.94.1/gramex/apps/uifactory/assets/img/gramener-favicon-blue.png
--rw-rw-rw-   0        0        0      573 2023-07-31 04:30:41.000000 gramex-1.94.1/gramex/apps/uifactory/assets/img/trash.svg
--rw-rw-rw-   0        0        0     6667 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/create.html
--rw-rw-rw-   0        0        0     2673 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/edit.html
--rw-rw-rw-   0        0        0      694 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/field-actions.html
--rw-rw-rw-   0        0        0     4361 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/form_builder.py
--rw-rw-rw-   0        0        0     4749 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/gramex.yaml
--rw-rw-rw-   0        0        0     6274 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/index.html
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.612164 gramex-1.94.1/gramex/apps/uifactory/js/
--rw-rw-rw-   0        0        0      601 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/js/README.md
--rw-rw-rw-   0        0        0      436 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/js/embed.js
--rw-rw-rw-   0        0        0    16411 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/js/fields.js
--rw-rw-rw-   0        0        0     1943 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/js/fork-form.js
--rw-rw-rw-   0        0        0     3080 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/js/index.js
--rw-rw-rw-   0        0        0     9232 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/js/script.js
--rw-rw-rw-   0        0        0      829 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/js/utils.js
--rw-rw-rw-   0        0        0     2779 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/js/viewform.js
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.616155 gramex-1.94.1/gramex/apps/uifactory/modals/
--rw-rw-rw-   0        0        0     1117 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/modals/add-field.html
--rw-rw-rw-   0        0        0     4107 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/modals/embed.html
--rw-rw-rw-   0        0        0      898 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/modals/remove.html
--rw-rw-rw-   0        0        0      952 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/modals/rename.html
--rw-rw-rw-   0        0        0     1323 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/modals/themes.html
--rw-rw-rw-   0        0        0     3257 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/apps/uifactory/package-lock.json
--rw-rw-rw-   0        0        0      206 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/package.json
--rw-rw-rw-   0        0        0     1548 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/popover-form.html
--rw-rw-rw-   0        0        0     1952 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/sample.html
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.617164 gramex-1.94.1/gramex/apps/uifactory/snippets/
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.617164 gramex-1.94.1/gramex/apps/uifactory/snippets/button/
--rw-rw-rw-   0        0        0     2795 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/snippets/button/bs4-button.js
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.618155 gramex-1.94.1/gramex/apps/uifactory/snippets/checkbox/
--rw-rw-rw-   0        0        0     1225 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/snippets/checkbox/bs4-checkbox.js
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.619164 gramex-1.94.1/gramex/apps/uifactory/snippets/email/
--rw-rw-rw-   0        0        0      604 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/snippets/email/bs4-email.js
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.619164 gramex-1.94.1/gramex/apps/uifactory/snippets/hidden/
--rw-rw-rw-   0        0        0      327 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/snippets/hidden/bs4-hidden.js
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.620165 gramex-1.94.1/gramex/apps/uifactory/snippets/html/
--rw-rw-rw-   0        0        0      292 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/snippets/html/bs4-html.js
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.620687 gramex-1.94.1/gramex/apps/uifactory/snippets/multiselect/
--rw-rw-rw-   0        0        0     4735 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/snippets/multiselect/bs4-multiselect.js
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.621695 gramex-1.94.1/gramex/apps/uifactory/snippets/number/
--rw-rw-rw-   0        0        0      736 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/snippets/number/bs4-number.js
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.621695 gramex-1.94.1/gramex/apps/uifactory/snippets/password/
--rw-rw-rw-   0        0        0      375 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/snippets/password/bs4-password.js
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.622695 gramex-1.94.1/gramex/apps/uifactory/snippets/radio/
--rw-rw-rw-   0        0        0     1034 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/snippets/radio/bs4-radio.js
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.622695 gramex-1.94.1/gramex/apps/uifactory/snippets/range/
--rw-rw-rw-   0        0        0      610 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/snippets/range/bs4-range.js
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.623694 gramex-1.94.1/gramex/apps/uifactory/snippets/select/
--rw-rw-rw-   0        0        0     1617 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/snippets/select/bs4-select.js
--rw-rw-rw-   0        0        0      947 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/snippets/setup.js
--rw-rw-rw-   0        0        0        3 2024-02-20 10:41:31.000000 gramex-1.94.1/gramex/apps/uifactory/snippets/snippets.json
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.624695 gramex-1.94.1/gramex/apps/uifactory/snippets/text/
--rw-rw-rw-   0        0        0      974 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/snippets/text/bs4-text.js
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.624695 gramex-1.94.1/gramex/apps/uifactory/snippets/textarea/
--rw-rw-rw-   0        0        0     1094 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/snippets/textarea/bs4-textarea.js
--rw-rw-rw-   0        0        0     1815 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/style.scss
--rw-rw-rw-   0        0        0     2013 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/template-navbar-view-form.html
--rw-rw-rw-   0        0        0     1020 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/template-navbar.html
--rw-rw-rw-   0        0        0      415 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/toast.html
--rw-rw-rw-   0        0        0     6516 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/uifactory/viewform.html
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.627695 gramex-1.94.1/gramex/apps/update/
--rw-rw-rw-   0        0        0      565 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/update/README.md
--rw-rw-rw-   0        0        0     2397 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/update/gramex.yaml
--rw-rw-rw-   0        0        0     4593 2024-01-29 15:13:34.000000 gramex-1.94.1/gramex/apps/update/gramexupdate.py
--rw-rw-rw-   0        0        0     3310 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps/update/index.html
--rw-rw-rw-   0        0        0      277 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/apps.yaml
--rw-rw-rw-   0        0        0    58499 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/cache.py
--rw-rw-rw-   0        0        0    35197 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/config.py
--rw-rw-rw-   0        0        0    93533 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/data.py
--rw-rw-rw-   0        0        0     6409 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/debug.py
--rw-rw-rw-   0        0        0     1825 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/deploy.yaml
--rw-rw-rw-   0        0        0     1467 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/download.vega.js
--rw-rw-rw-   0        0        0    12057 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/favicon.ico
--rw-rw-rw-   0        0        0    15621 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/gramex.yaml
--rw-rw-rw-   0        0        0     6262 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/gramexfeatures.csv
--rw-rw-rw-   0        0        0    14340 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/gramexsize.csv
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.687235 gramex-1.94.1/gramex/handlers/
--rw-rw-rw-   0        0        0     1368 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/handlers/400.html
--rw-rw-rw-   0        0        0     2079 2023-09-12 09:13:58.000000 gramex-1.94.1/gramex/handlers/401.html
--rw-rw-rw-   0        0        0     2526 2023-09-12 09:13:58.000000 gramex-1.94.1/gramex/handlers/403.html
--rw-rw-rw-   0        0        0     1399 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/handlers/404.html
--rw-rw-rw-   0        0        0     2163 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/handlers/500.html
--rw-rw-rw-   0        0        0     3085 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/handlers/__init__.py
--rw-rw-rw-   0        0        0      532 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/handlers/auth.recaptcha.template.html
--rw-rw-rw-   0        0        0     3862 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/handlers/auth.template.html
--rw-rw-rw-   0        0        0    17347 2024-01-29 15:13:34.000000 gramex-1.94.1/gramex/handlers/authhandler.py
--rw-rw-rw-   0        0        0    67084 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/handlers/basehandler.py
--rw-rw-rw-   0        0        0    16094 2024-01-29 15:13:34.000000 gramex-1.94.1/gramex/handlers/capturehandler.py
--rw-rw-rw-   0        0        0     6755 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/handlers/chatgpthandler.py
--rw-rw-rw-   0        0        0     1477 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/handlers/comichandler.py
--rw-rw-rw-   0        0        0    10534 2024-01-29 15:13:34.000000 gramex-1.94.1/gramex/handlers/drivehandler.py
--rw-rw-rw-   0        0        0    14917 2024-01-29 15:13:34.000000 gramex-1.94.1/gramex/handlers/filehandler.py
--rw-rw-rw-   0        0        0     1271 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/handlers/filehandler.template.html
--rw-rw-rw-   0        0        0      198 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/handlers/filterhandler.py
--rw-rw-rw-   0        0        0    13125 2024-01-29 15:13:34.000000 gramex-1.94.1/gramex/handlers/formhandler.py
--rw-rw-rw-   0        0        0     3774 2024-01-29 15:13:34.000000 gramex-1.94.1/gramex/handlers/functionhandler.py
--rw-rw-rw-   0        0        0     6706 2024-01-29 15:13:34.000000 gramex-1.94.1/gramex/handlers/jsonhandler.py
--rw-rw-rw-   0        0        0     6838 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/handlers/messagehandler.py
--rw-rw-rw-   0        0        0    16154 2024-01-29 15:13:34.000000 gramex-1.94.1/gramex/handlers/mlhandler.py
--rw-rw-rw-   0        0        0     7492 2024-01-29 15:13:34.000000 gramex-1.94.1/gramex/handlers/modelhandler.py
--rw-rw-rw-   0        0        0     1413 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/handlers/openapiconfig.yaml
--rw-rw-rw-   0        0        0     7326 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/handlers/openapihandler.py
--rw-rw-rw-   0        0        0      818 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/handlers/pptxhandler.py
--rw-rw-rw-   0        0        0     5145 2024-01-29 15:13:34.000000 gramex-1.94.1/gramex/handlers/processhandler.py
--rw-rw-rw-   0        0        0     7882 2024-01-29 15:13:34.000000 gramex-1.94.1/gramex/handlers/proxyhandler.py
--rw-rw-rw-   0        0        0     1362 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/handlers/queryhandler.template.html
--rw-rw-rw-   0        0        0    11338 2024-01-29 15:13:34.000000 gramex-1.94.1/gramex/handlers/socialhandler.py
--rw-rw-rw-   0        0        0     9434 2024-01-29 15:13:34.000000 gramex-1.94.1/gramex/handlers/uploadhandler.py
--rw-rw-rw-   0        0        0     2121 2024-01-29 15:13:34.000000 gramex-1.94.1/gramex/handlers/websockethandler.py
--rw-rw-rw-   0        0        0     1458 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/http.py
--rw-rw-rw-   0        0        0    35700 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/install.py
--rw-rw-rw-   0        0        0     2086 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/license.py
--rw-rw-rw-   0        0        0     2005 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/migrate.py
--rw-rw-rw-   0        0        0    18682 2024-01-29 15:13:34.000000 gramex-1.94.1/gramex/ml.py
--rw-rw-rw-   0        0        0    13687 2024-01-29 15:13:34.000000 gramex-1.94.1/gramex/ml_api.py
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.743355 gramex-1.94.1/gramex/pptgen/
--rw-rw-rw-   0        0        0    10024 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/pptgen/__init__.py
--rw-rw-rw-   0        0        0    18868 2024-01-29 15:13:34.000000 gramex-1.94.1/gramex/pptgen/color.py
--rw-rw-rw-   0        0        0     7779 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/pptgen/colors.json
--rw-rw-rw-   0        0        0    45631 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/pptgen/commands.py
--rw-rw-rw-   0        0        0     6351 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/pptgen/fonts.json
--rw-rw-rw-   0        0        0     1305 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/pptgen/fontwidth.py
--rw-rw-rw-   0        0        0    26251 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/pptgen/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.761008 gramex-1.94.1/gramex/pptgen2/
--rw-rw-rw-   0        0        0    23438 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/pptgen2/__init__.py
--rw-rw-rw-   0        0        0    34452 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/pptgen2/commands.py
--rw-rw-rw-   0        0        0    12068 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/pptgen2/config.yaml
--rw-rw-rw-   0        0        0     4279 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/pynode.py
--rw-rw-rw-   0        0        0     2979 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/scale.py
--rw-rw-rw-   0        0        0     1057 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/secrets.py
--rw-rw-rw-   0        0        0     2508 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/servicenow.yaml
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.800677 gramex-1.94.1/gramex/services/
--rw-rw-rw-   0        0        0    39784 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/services/__init__.py
--rw-rw-rw-   0        0        0    11451 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/services/emailer.py
--rw-rw-rw-   0        0        0     3724 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/services/rediscache.py
--rw-rw-rw-   0        0        0     7164 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/services/scheduler.py
--rw-rw-rw-   0        0        0     3720 2023-10-23 22:11:53.000000 gramex-1.94.1/gramex/services/sms.py
--rw-rw-rw-   0        0        0     6385 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/services/ttlcache.py
--rw-rw-rw-   0        0        0     4522 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/services/urlcache.py
--rw-rw-rw-   0        0        0     5822 2024-01-29 15:13:34.000000 gramex-1.94.1/gramex/services/watcher.py
--rw-rw-rw-   0        0        0     3831 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/sm_api.py
--rw-rw-rw-   0        0        0     8568 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/topcause.py
--rw-rw-rw-   0        0        0     8710 2024-01-29 15:13:34.000000 gramex-1.94.1/gramex/transformers.py
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.831912 gramex-1.94.1/gramex/transforms/
--rw-rw-rw-   0        0        0      787 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/transforms/__init__.py
--rw-rw-rw-   0        0        0     1659 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/transforms/auth.py
--rw-rw-rw-   0        0        0     3022 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/transforms/template.py
--rw-rw-rw-   0        0        0    32992 2024-03-02 06:00:42.000000 gramex-1.94.1/gramex/transforms/transforms.py
--rw-rw-rw-   0        0        0    10095 2023-07-31 04:30:40.000000 gramex-1.94.1/gramex/transforms/twitterstream.py
--rw-rw-rw-   0        0        0     6808 2024-01-29 15:13:34.000000 gramex-1.94.1/gramex/winservice.py
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.858758 gramex-1.94.1/gramex.egg-info/
--rw-rw-rw-   0        0        0     5875 2024-03-02 06:01:15.000000 gramex-1.94.1/gramex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11950 2024-03-02 06:01:17.000000 gramex-1.94.1/gramex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-02 06:01:15.000000 gramex-1.94.1/gramex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2024-03-02 06:01:15.000000 gramex-1.94.1/gramex.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      953 2024-03-02 06:01:15.000000 gramex-1.94.1/gramex.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-02 06:01:15.000000 gramex-1.94.1/gramex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6171 2024-03-02 06:00:42.000000 gramex-1.94.1/pyproject.toml
--rw-rw-rw-   0        0        0      503 2024-03-02 06:01:17.873294 gramex-1.94.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-02 06:01:17.857762 gramex-1.94.1/tests/
--rw-rw-rw-   0        0        0     5233 2023-07-31 04:30:40.000000 gramex-1.94.1/tests/test_admin.py
--rw-rw-rw-   0        0        0     9054 2023-07-31 04:30:40.000000 gramex-1.94.1/tests/test_alerts.py
--rw-rw-rw-   0        0        0     3981 2023-07-31 04:30:40.000000 gramex-1.94.1/tests/test_args.py
--rw-rw-rw-   0        0        0    39128 2023-07-31 04:30:40.000000 gramex-1.94.1/tests/test_auth.py
--rw-rw-rw-   0        0        0    14612 2023-07-31 04:30:40.000000 gramex-1.94.1/tests/test_cache.py
--rw-rw-rw-   0        0        0    15151 2023-09-21 00:20:48.000000 gramex-1.94.1/tests/test_capturehandler.py
--rw-rw-rw-   0        0        0     1288 2023-07-31 04:30:40.000000 gramex-1.94.1/tests/test_comichandler.py
--rw-rw-rw-   0        0        0    12571 2023-07-31 04:30:40.000000 gramex-1.94.1/tests/test_drivehandler.py
--rw-rw-rw-   0        0        0    17308 2023-07-31 04:30:40.000000 gramex-1.94.1/tests/test_filehandler.py
--rw-rw-rw-   0        0        0     6797 2023-07-31 04:30:40.000000 gramex-1.94.1/tests/test_filterhandler.py
--rw-rw-rw-   0        0        0    35746 2023-07-31 04:30:40.000000 gramex-1.94.1/tests/test_formhandler.py
--rw-rw-rw-   0        0        0     8787 2023-09-12 09:13:58.000000 gramex-1.94.1/tests/test_functionhandler.py
--rw-rw-rw-   0        0        0     3201 2023-07-31 04:30:40.000000 gramex-1.94.1/tests/test_gramexlog.py
--rw-rw-rw-   0        0        0    19008 2023-07-31 04:30:40.000000 gramex-1.94.1/tests/test_handlers.py
--rw-rw-rw-   0        0        0     1475 2023-07-31 04:30:40.000000 gramex-1.94.1/tests/test_init.py
--rw-rw-rw-   0        0        0     8931 2023-07-31 04:30:40.000000 gramex-1.94.1/tests/test_install.py
--rw-rw-rw-   0        0        0     6361 2023-07-31 04:30:40.000000 gramex-1.94.1/tests/test_jsonhandler.py
--rw-rw-rw-   0        0        0     3896 2023-07-31 04:30:40.000000 gramex-1.94.1/tests/test_ldapauth.py
--rw-rw-rw-   0        0        0     7519 2023-07-31 04:30:40.000000 gramex-1.94.1/tests/test_logviewer.py
--rw-rw-rw-   0        0        0    32878 2023-07-31 04:30:40.000000 gramex-1.94.1/tests/test_mlhandler.py
--rw-rw-rw-   0        0        0     4745 2023-07-31 04:30:40.000000 gramex-1.94.1/tests/test_modelhandler.py
--rw-rw-rw-   0        0        0     7082 2023-07-31 04:30:40.000000 gramex-1.94.1/tests/test_openapihandler.py
--rw-rw-rw-   0        0        0     1411 2023-07-31 04:30:40.000000 gramex-1.94.1/tests/test_pptxhandler.py
--rw-rw-rw-   0        0        0     3530 2023-07-31 04:30:40.000000 gramex-1.94.1/tests/test_processhandler.py
--rw-rw-rw-   0        0        0     3834 2023-07-31 04:30:40.000000 gramex-1.94.1/tests/test_proxyhandler.py
--rw-rw-rw-   0        0        0     1527 2023-07-31 04:30:40.000000 gramex-1.94.1/tests/test_pynode.py
--rw-rw-rw-   0        0        0     1220 2023-07-31 04:30:40.000000 gramex-1.94.1/tests/test_schedule.py
--rw-rw-rw-   0        0        0      757 2023-07-31 04:30:40.000000 gramex-1.94.1/tests/test_secrets.py
--rw-rw-rw-   0        0        0      330 2023-07-31 04:30:41.000000 gramex-1.94.1/tests/test_sms.py
--rw-rw-rw-   0        0        0      180 2023-07-31 04:30:41.000000 gramex-1.94.1/tests/test_subapp.py
--rw-rw-rw-   0        0        0     5382 2023-07-31 04:30:41.000000 gramex-1.94.1/tests/test_subprocess.py
--rw-rw-rw-   0        0        0     2277 2023-07-31 04:30:41.000000 gramex-1.94.1/tests/test_translater.py
--rw-rw-rw-   0        0        0     2895 2023-07-31 04:30:41.000000 gramex-1.94.1/tests/test_twitterresthandler.py
--rw-rw-rw-   0        0        0     2352 2023-07-31 04:30:41.000000 gramex-1.94.1/tests/test_ui.py
--rw-rw-rw-   0        0        0     2359 2023-07-31 04:30:41.000000 gramex-1.94.1/tests/test_update.py
--rw-rw-rw-   0        0        0     6563 2023-07-31 04:30:41.000000 gramex-1.94.1/tests/test_uploadhandler.py
--rw-rw-rw-   0        0        0     1966 2023-07-31 04:30:41.000000 gramex-1.94.1/tests/test_watcher.py
--rw-rw-rw-   0        0        0     2647 2023-07-31 04:30:41.000000 gramex-1.94.1/tests/test_websockethandler.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.496286 gramex-1.94.2/
+-rw-rw-rw-   0        0        0     1968 2023-07-31 04:30:40.000000 gramex-1.94.2/.gitignore
+-rw-rw-rw-   0        0        0     1274 2023-07-31 04:30:40.000000 gramex-1.94.2/LICENSE
+-rw-rw-rw-   0        0        0      641 2023-07-31 04:30:40.000000 gramex-1.94.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5875 2024-05-20 10:34:05.496286 gramex-1.94.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1212 2023-07-31 04:30:40.000000 gramex-1.94.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.257625 gramex-1.94.2/gramex/
+-rw-rw-rw-   0        0        0    15372 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/__init__.py
+-rw-rw-rw-   0        0        0      242 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.295720 gramex-1.94.2/gramex/apps/
+-rw-rw-rw-   0        0        0        0 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.296724 gramex-1.94.2/gramex/apps/admin/
+-rw-rw-rw-   0        0        0        9 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/admin/.gitignore
+-rw-rw-rw-   0        0        0      129 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/admin/gramex.yaml
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.300731 gramex-1.94.2/gramex/apps/admin2/
+-rw-rw-rw-   0        0        0      228 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/admin2/admin.css
+-rw-rw-rw-   0        0        0     3152 2024-03-02 06:00:42.000000 gramex-1.94.2/gramex/apps/admin2/gramex.yaml
+-rw-rw-rw-   0        0        0    12441 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/apps/admin2/gramexadmin.py
+-rw-rw-rw-   0        0        0     8420 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/admin2/index.html
+-rw-rw-rw-   0        0        0     5216 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/admin2/schedule.js
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.304724 gramex-1.94.2/gramex/apps/capture/
+-rw-rw-rw-   0        0        0      293 2024-03-02 06:00:42.000000 gramex-1.94.2/gramex/apps/capture/.snyk
+-rw-rw-rw-   0        0        0     4061 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/capture/README.md
+-rw-rw-rw-   0        0        0     9487 2024-05-20 10:29:24.000000 gramex-1.94.2/gramex/apps/capture/capture.js
+-rw-rw-rw-   0        0        0    12290 2023-09-21 00:20:48.000000 gramex-1.94.2/gramex/apps/capture/chromecapture.js
+-rw-rw-rw-   0        0        0     4197 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/capture/index.html
+-rw-rw-rw-   0        0        0    80816 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/apps/capture/package-lock.json
+-rw-rw-rw-   0        0        0      863 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/capture/package.json
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.311281 gramex-1.94.2/gramex/apps/filemanager/
+-rw-rw-rw-   0        0        0     2845 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/filemanager/README.html
+-rw-rw-rw-   0        0        0      700 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/filemanager/drivehandler-snippet.html
+-rw-rw-rw-   0        0        0      612 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/filemanager/filemanager-snippet.html
+-rw-rw-rw-   0        0        0     2578 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/filemanager/filemanager.html
+-rw-rw-rw-   0        0        0     3070 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/filemanager/filemanager.js
+-rw-rw-rw-   0        0        0      926 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/filemanager/filemanager.py
+-rw-rw-rw-   0        0        0      621 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/filemanager/gramex.yaml
+-rw-rw-rw-   0        0        0      914 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/filemanager/index.html
+-rw-rw-rw-   0        0        0      872 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/filemanager/navbar.html
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.227946 gramex-1.94.2/gramex/apps/init/
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.319804 gramex-1.94.2/gramex/apps/init/default/
+-rw-rw-rw-   0        0        0      578 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/init/default/.eslintrc.yml
+-rw-rw-rw-   0        0        0      756 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/init/default/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0      383 2024-03-02 06:00:42.000000 gramex-1.94.2/gramex/apps/init/default/.secrets.yaml
+-rw-rw-rw-   0        0        0     1635 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/init/default/.template.gitignore
+-rw-rw-rw-   0        0        0      248 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/init/default/README.template.md
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.319804 gramex-1.94.2/gramex/apps/init/default/assets/
+-rw-rw-rw-   0        0        0      519 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/init/default/assets/README.template.md
+-rw-rw-rw-   0        0        0     1756 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/init/default/gramex.template.yaml
+-rw-rw-rw-   0        0        0      694 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/init/default/index.template.html
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.320803 gramex-1.94.2/gramex/apps/init/default/js/
+-rw-rw-rw-   0        0        0      602 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/init/default/js/README.template.md
+-rw-rw-rw-   0        0        0     2608 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/init/default/login.template.html
+-rw-rw-rw-   0        0        0      352 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/init/default/package.template.json
+-rw-rw-rw-   0        0        0       80 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/init/default/style.scss
+-rw-rw-rw-   0        0        0     3499 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/init/default/template-navbar.template.html
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.323811 gramex-1.94.2/gramex/apps/init/ide/
+-rw-rw-rw-   0        0        0      378 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/init/ide/.gitlab-ci.template.yml
+-rw-rw-rw-   0        0        0      244 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/init/ide/gramex.template.yaml
+-rw-rw-rw-   0        0        0      738 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/init/ide/index.template.html
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.325284 gramex-1.94.2/gramex/apps/init/minimal/
+-rw-rw-rw-   0        0        0      247 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/init/minimal/gramex.template.yaml
+-rw-rw-rw-   0        0        0      757 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/init/minimal/index.template.html
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.326818 gramex-1.94.2/gramex/apps/languagetool/
+-rw-rw-rw-   0        0        0      709 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/languagetool/README.md
+-rw-rw-rw-   0        0        0        0 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/languagetool/__init__.py
+-rw-rw-rw-   0        0        0      788 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/languagetool/gramex.yaml
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.341751 gramex-1.94.2/gramex/apps/logviewer/
+-rw-rw-rw-   0        0        0        0 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/logviewer/__init__.py
+-rw-rw-rw-   0        0        0     3466 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/logviewer/config.yaml
+-rw-rw-rw-   0        0        0     6278 2024-03-02 06:00:42.000000 gramex-1.94.2/gramex/apps/logviewer/gramex.yaml
+-rw-rw-rw-   0        0        0     4958 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/logviewer/index.html
+-rw-rw-rw-   0        0        0    13285 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/apps/logviewer/logviewer.py
+-rw-rw-rw-   0        0        0      210 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/logviewer/lv-card-deck.html
+-rw-rw-rw-   0        0        0      386 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/logviewer/lv-card.html
+-rw-rw-rw-   0        0        0      526 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/logviewer/lv-datepicker.html
+-rw-rw-rw-   0        0        0      331 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/logviewer/lv-dropdown.html
+-rw-rw-rw-   0        0        0      465 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/logviewer/lv-filters.html
+-rw-rw-rw-   0        0        0      113 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/logviewer/lv-header.html
+-rw-rw-rw-   0        0        0      335 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/logviewer/lv-kpi.html
+-rw-rw-rw-   0        0        0      514 2024-05-20 10:24:26.000000 gramex-1.94.2/gramex/apps/logviewer/package-lock.json
+-rw-rw-rw-   0        0        0      179 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/logviewer/package.json
+-rw-rw-rw-   0        0        0     6928 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/logviewer/render.js
+-rw-rw-rw-   0        0        0     5390 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/logviewer/script.js
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.343748 gramex-1.94.2/gramex/apps/mail/
+-rw-rw-rw-   0        0        0      430 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/mail/gramex.yaml
+-rw-rw-rw-   0        0        0     3032 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/mail/index.html
+-rw-rw-rw-   0        0        0      251 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/mail/mailapp.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.343748 gramex-1.94.2/gramex/apps/mlhandler/
+-rw-rw-rw-   0        0        0    15151 2024-03-02 06:00:42.000000 gramex-1.94.2/gramex/apps/mlhandler/template.html
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.346779 gramex-1.94.2/gramex/apps/pynode/
+-rw-rw-rw-   0        0        0       47 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/pynode/README.md
+-rw-rw-rw-   0        0        0     4127 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/pynode/index.js
+-rw-rw-rw-   0        0        0     1902 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/apps/pynode/package-lock.json
+-rw-rw-rw-   0        0        0      187 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/pynode/package.json
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.349774 gramex-1.94.2/gramex/apps/smartalerts/
+-rw-rw-rw-   0        0        0       89 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/smartalerts/gramex.yaml
+-rw-rw-rw-   0        0        0      429 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/smartalerts/index.html
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.357286 gramex-1.94.2/gramex/apps/ui/
+-rw-rw-rw-   0        0        0     1047 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/apps/ui/.snyk
+-rw-rw-rw-   0        0        0    13158 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/apps/ui/__init__.py
+-rw-rw-rw-   0        0        0      648 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/bootstrap-theme.scss
+-rw-rw-rw-   0        0        0     1056 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/config.yaml
+-rw-rw-rw-   0        0        0     2082 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/gramex.yaml
+-rw-rw-rw-   0        0        0    25271 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/gramexui.scss
+-rw-rw-rw-   0        0        0    96298 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/apps/ui/package-lock.json
+-rw-rw-rw-   0        0        0      265 2024-03-02 06:00:42.000000 gramex-1.94.2/gramex/apps/ui/package.json
+-rw-rw-rw-   0        0        0     2490 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/setup.js
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.362288 gramex-1.94.2/gramex/apps/ui/theme/
+-rw-rw-rw-   0        0        0    19355 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootstrap5.scss
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.396458 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/
+-rw-rw-rw-   0        0        0     6324 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/cerulean.png
+-rw-rw-rw-   0        0        0      175 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/cerulean.scss
+-rw-rw-rw-   0        0        0     4833 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/cosmo.png
+-rw-rw-rw-   0        0        0      166 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/cosmo.scss
+-rw-rw-rw-   0        0        0     6569 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/cyborg.png
+-rw-rw-rw-   0        0        0      169 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/cyborg.scss
+-rw-rw-rw-   0        0        0     5932 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/darkly.png
+-rw-rw-rw-   0        0        0      169 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/darkly.scss
+-rw-rw-rw-   0        0        0     5114 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/flatly.png
+-rw-rw-rw-   0        0        0      169 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/flatly.scss
+-rw-rw-rw-   0        0        0     5335 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/journal.png
+-rw-rw-rw-   0        0        0      172 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/journal.scss
+-rw-rw-rw-   0        0        0     6141 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/litera.png
+-rw-rw-rw-   0        0        0      169 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/litera.scss
+-rw-rw-rw-   0        0        0     4958 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/lumen.png
+-rw-rw-rw-   0        0        0      166 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/lumen.scss
+-rw-rw-rw-   0        0        0     4818 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/lux.png
+-rw-rw-rw-   0        0        0      160 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/lux.scss
+-rw-rw-rw-   0        0        0     5791 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/materia.png
+-rw-rw-rw-   0        0        0      172 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/materia.scss
+-rw-rw-rw-   0        0        0     5662 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/minty.png
+-rw-rw-rw-   0        0        0      166 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/minty.scss
+-rw-rw-rw-   0        0        0     4777 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/pulse.png
+-rw-rw-rw-   0        0        0      166 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/pulse.scss
+-rw-rw-rw-   0        0        0     5246 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/sandstone.png
+-rw-rw-rw-   0        0        0      178 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/sandstone.scss
+-rw-rw-rw-   0        0        0     6213 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/simplex.png
+-rw-rw-rw-   0        0        0      172 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/simplex.scss
+-rw-rw-rw-   0        0        0     7371 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/sketchy.png
+-rw-rw-rw-   0        0        0      172 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/sketchy.scss
+-rw-rw-rw-   0        0        0     6288 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/slate.png
+-rw-rw-rw-   0        0        0      166 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/slate.scss
+-rw-rw-rw-   0        0        0     6158 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/solar.png
+-rw-rw-rw-   0        0        0      166 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/solar.scss
+-rw-rw-rw-   0        0        0     6501 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/spacelab.png
+-rw-rw-rw-   0        0        0      175 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/spacelab.scss
+-rw-rw-rw-   0        0        0     6357 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/superhero.png
+-rw-rw-rw-   0        0        0      178 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/superhero.scss
+-rw-rw-rw-   0        0        0     5432 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/united.png
+-rw-rw-rw-   0        0        0      169 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/united.scss
+-rw-rw-rw-   0        0        0     4842 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/yeti.png
+-rw-rw-rw-   0        0        0      163 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/bootswatch/yeti.scss
+-rw-rw-rw-   0        0        0     4573 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/default.png
+-rw-rw-rw-   0        0        0       20 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/default.scss
+-rw-rw-rw-   0        0        0      831 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/index.html
+-rw-rw-rw-   0        0        0    71063 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/sample.html
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.416646 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/
+-rw-rw-rw-   0        0        0     6383 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/blue_voltage.png
+-rw-rw-rw-   0        0        0      630 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/blue_voltage.scss
+-rw-rw-rw-   0        0        0     6282 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/boldstrap.png
+-rw-rw-rw-   0        0        0      478 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/boldstrap.scss
+-rw-rw-rw-   0        0        0     6215 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/bootstrap_purple.png
+-rw-rw-rw-   0        0        0      268 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/bootstrap_purple.scss
+-rw-rw-rw-   0        0        0     6153 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/darkster.png
+-rw-rw-rw-   0        0        0     2559 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/darkster.scss
+-rw-rw-rw-   0        0        0     5497 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/fresca.png
+-rw-rw-rw-   0        0        0      362 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/fresca.scss
+-rw-rw-rw-   0        0        0     5525 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/greyson.png
+-rw-rw-rw-   0        0        0      571 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/greyson.scss
+-rw-rw-rw-   0        0        0     5153 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/hello_kiddie.png
+-rw-rw-rw-   0        0        0      621 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/hello_kiddie.scss
+-rw-rw-rw-   0        0        0     5523 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/herbie.png
+-rw-rw-rw-   0        0        0      480 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/herbie.scss
+-rw-rw-rw-   0        0        0     6585 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/hootstrap.png
+-rw-rw-rw-   0        0        0      487 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/hootstrap.scss
+-rw-rw-rw-   0        0        0     5491 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/lovey.png
+-rw-rw-rw-   0        0        0      461 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/lovey.scss
+-rw-rw-rw-   0        0        0     6009 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/monotony.png
+-rw-rw-rw-   0        0        0      486 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/monotony.scss
+-rw-rw-rw-   0        0        0     5546 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/poypull.png
+-rw-rw-rw-   0        0        0      541 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/poypull.scss
+-rw-rw-rw-   0        0        0     5430 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/signal.png
+-rw-rw-rw-   0        0        0      576 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/signal.scss
+-rw-rw-rw-   0        0        0     5338 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/tequila.png
+-rw-rw-rw-   0        0        0      371 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes-guide/tequila.scss
+-rw-rw-rw-   0        0        0      801 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/ui/theme/themes.json
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.419325 gramex-1.94.2/gramex/apps/update/
+-rw-rw-rw-   0        0        0      565 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/update/README.md
+-rw-rw-rw-   0        0        0     2397 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/update/gramex.yaml
+-rw-rw-rw-   0        0        0     4593 2024-01-29 15:13:34.000000 gramex-1.94.2/gramex/apps/update/gramexupdate.py
+-rw-rw-rw-   0        0        0     3310 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps/update/index.html
+-rw-rw-rw-   0        0        0      277 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/apps.yaml
+-rw-rw-rw-   0        0        0    58547 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/cache.py
+-rw-rw-rw-   0        0        0    35193 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/config.py
+-rw-rw-rw-   0        0        0    93700 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/data.py
+-rw-rw-rw-   0        0        0     6409 2024-03-02 06:00:42.000000 gramex-1.94.2/gramex/debug.py
+-rw-rw-rw-   0        0        0     1825 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/deploy.yaml
+-rw-rw-rw-   0        0        0     1467 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/download.vega.js
+-rw-rw-rw-   0        0        0    12057 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/favicon.ico
+-rw-rw-rw-   0        0        0    15621 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/gramex.yaml
+-rw-rw-rw-   0        0        0     6262 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/gramexfeatures.csv
+-rw-rw-rw-   0        0        0    14265 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/gramexsize.csv
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.444389 gramex-1.94.2/gramex/handlers/
+-rw-rw-rw-   0        0        0     1368 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/handlers/400.html
+-rw-rw-rw-   0        0        0     2079 2023-09-12 09:13:58.000000 gramex-1.94.2/gramex/handlers/401.html
+-rw-rw-rw-   0        0        0     2526 2023-09-12 09:13:58.000000 gramex-1.94.2/gramex/handlers/403.html
+-rw-rw-rw-   0        0        0     1399 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/handlers/404.html
+-rw-rw-rw-   0        0        0     2163 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/handlers/500.html
+-rw-rw-rw-   0        0        0     3085 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/handlers/__init__.py
+-rw-rw-rw-   0        0        0      532 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/handlers/auth.recaptcha.template.html
+-rw-rw-rw-   0        0        0     3862 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/handlers/auth.template.html
+-rw-rw-rw-   0        0        0    17347 2024-01-29 15:13:34.000000 gramex-1.94.2/gramex/handlers/authhandler.py
+-rw-rw-rw-   0        0        0    67083 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/handlers/basehandler.py
+-rw-rw-rw-   0        0        0    16092 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/handlers/capturehandler.py
+-rw-rw-rw-   0        0        0     6755 2024-03-02 06:00:42.000000 gramex-1.94.2/gramex/handlers/chatgpthandler.py
+-rw-rw-rw-   0        0        0     1477 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/handlers/comichandler.py
+-rw-rw-rw-   0        0        0    10533 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/handlers/drivehandler.py
+-rw-rw-rw-   0        0        0    14917 2024-01-29 15:13:34.000000 gramex-1.94.2/gramex/handlers/filehandler.py
+-rw-rw-rw-   0        0        0     1271 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/handlers/filehandler.template.html
+-rw-rw-rw-   0        0        0      198 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/handlers/filterhandler.py
+-rw-rw-rw-   0        0        0    13125 2024-01-29 15:13:34.000000 gramex-1.94.2/gramex/handlers/formhandler.py
+-rw-rw-rw-   0        0        0     3774 2024-01-29 15:13:34.000000 gramex-1.94.2/gramex/handlers/functionhandler.py
+-rw-rw-rw-   0        0        0     6706 2024-01-29 15:13:34.000000 gramex-1.94.2/gramex/handlers/jsonhandler.py
+-rw-rw-rw-   0        0        0     6838 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/handlers/messagehandler.py
+-rw-rw-rw-   0        0        0    16154 2024-01-29 15:13:34.000000 gramex-1.94.2/gramex/handlers/mlhandler.py
+-rw-rw-rw-   0        0        0     7492 2024-01-29 15:13:34.000000 gramex-1.94.2/gramex/handlers/modelhandler.py
+-rw-rw-rw-   0        0        0     1413 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/handlers/openapiconfig.yaml
+-rw-rw-rw-   0        0        0     7326 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/handlers/openapihandler.py
+-rw-rw-rw-   0        0        0      818 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/handlers/pptxhandler.py
+-rw-rw-rw-   0        0        0     5144 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/handlers/processhandler.py
+-rw-rw-rw-   0        0        0     7882 2024-01-29 15:13:34.000000 gramex-1.94.2/gramex/handlers/proxyhandler.py
+-rw-rw-rw-   0        0        0     1362 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/handlers/queryhandler.template.html
+-rw-rw-rw-   0        0        0    11337 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/handlers/socialhandler.py
+-rw-rw-rw-   0        0        0     9433 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/handlers/uploadhandler.py
+-rw-rw-rw-   0        0        0     2121 2024-01-29 15:13:34.000000 gramex-1.94.2/gramex/handlers/websockethandler.py
+-rw-rw-rw-   0        0        0     1458 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/http.py
+-rw-rw-rw-   0        0        0    35639 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/install.py
+-rw-rw-rw-   0        0        0     2086 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/license.py
+-rw-rw-rw-   0        0        0     2005 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/migrate.py
+-rw-rw-rw-   0        0        0    18682 2024-01-29 15:13:34.000000 gramex-1.94.2/gramex/ml.py
+-rw-rw-rw-   0        0        0    13687 2024-01-29 15:13:34.000000 gramex-1.94.2/gramex/ml_api.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.450153 gramex-1.94.2/gramex/pptgen/
+-rw-rw-rw-   0        0        0    10024 2024-03-02 06:00:42.000000 gramex-1.94.2/gramex/pptgen/__init__.py
+-rw-rw-rw-   0        0        0    18855 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/pptgen/color.py
+-rw-rw-rw-   0        0        0     7779 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/pptgen/colors.json
+-rw-rw-rw-   0        0        0    45627 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/pptgen/commands.py
+-rw-rw-rw-   0        0        0     6351 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/pptgen/fonts.json
+-rw-rw-rw-   0        0        0     1305 2024-03-02 06:00:42.000000 gramex-1.94.2/gramex/pptgen/fontwidth.py
+-rw-rw-rw-   0        0        0    26249 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/pptgen/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.451780 gramex-1.94.2/gramex/pptgen2/
+-rw-rw-rw-   0        0        0    23437 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/pptgen2/__init__.py
+-rw-rw-rw-   0        0        0    34451 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/pptgen2/commands.py
+-rw-rw-rw-   0        0        0    12068 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/pptgen2/config.yaml
+-rw-rw-rw-   0        0        0     4279 2024-03-02 06:00:42.000000 gramex-1.94.2/gramex/pynode.py
+-rw-rw-rw-   0        0        0     2979 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/scale.py
+-rw-rw-rw-   0        0        0     1057 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/secrets.py
+-rw-rw-rw-   0        0        0     2508 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/servicenow.yaml
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.457697 gramex-1.94.2/gramex/services/
+-rw-rw-rw-   0        0        0    39782 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/services/__init__.py
+-rw-rw-rw-   0        0        0    11451 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/services/emailer.py
+-rw-rw-rw-   0        0        0     3721 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/services/rediscache.py
+-rw-rw-rw-   0        0        0     7164 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/services/scheduler.py
+-rw-rw-rw-   0        0        0     3720 2023-10-23 22:11:53.000000 gramex-1.94.2/gramex/services/sms.py
+-rw-rw-rw-   0        0        0     6385 2024-03-02 06:00:42.000000 gramex-1.94.2/gramex/services/ttlcache.py
+-rw-rw-rw-   0        0        0     4520 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/services/urlcache.py
+-rw-rw-rw-   0        0        0     5822 2024-01-29 15:13:34.000000 gramex-1.94.2/gramex/services/watcher.py
+-rw-rw-rw-   0        0        0     3831 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/sm_api.py
+-rw-rw-rw-   0        0        0     8567 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/topcause.py
+-rw-rw-rw-   0        0        0     8709 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/transformers.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.464851 gramex-1.94.2/gramex/transforms/
+-rw-rw-rw-   0        0        0      787 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/transforms/__init__.py
+-rw-rw-rw-   0        0        0     1659 2024-03-02 06:00:42.000000 gramex-1.94.2/gramex/transforms/auth.py
+-rw-rw-rw-   0        0        0     3022 2023-07-31 04:30:40.000000 gramex-1.94.2/gramex/transforms/template.py
+-rw-rw-rw-   0        0        0    32988 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/transforms/transforms.py
+-rw-rw-rw-   0        0        0    10094 2024-05-20 10:32:31.000000 gramex-1.94.2/gramex/transforms/twitterstream.py
+-rw-rw-rw-   0        0        0     6808 2024-01-29 15:13:34.000000 gramex-1.94.2/gramex/winservice.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.493764 gramex-1.94.2/gramex.egg-info/
+-rw-rw-rw-   0        0        0     5875 2024-05-20 10:34:04.000000 gramex-1.94.2/gramex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9713 2024-05-20 10:34:05.000000 gramex-1.94.2/gramex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 10:34:04.000000 gramex-1.94.2/gramex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2024-05-20 10:34:04.000000 gramex-1.94.2/gramex.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      953 2024-05-20 10:34:04.000000 gramex-1.94.2/gramex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-20 10:34:04.000000 gramex-1.94.2/gramex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7166 2024-05-20 10:32:31.000000 gramex-1.94.2/pyproject.toml
+-rw-rw-rw-   0        0        0      214 2024-05-20 10:34:05.506803 gramex-1.94.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 10:34:05.492754 gramex-1.94.2/tests/
+-rw-rw-rw-   0        0        0     5233 2023-07-31 04:30:40.000000 gramex-1.94.2/tests/test_admin.py
+-rw-rw-rw-   0        0        0     9054 2023-07-31 04:30:40.000000 gramex-1.94.2/tests/test_alerts.py
+-rw-rw-rw-   0        0        0     3981 2023-07-31 04:30:40.000000 gramex-1.94.2/tests/test_args.py
+-rw-rw-rw-   0        0        0    39128 2023-07-31 04:30:40.000000 gramex-1.94.2/tests/test_auth.py
+-rw-rw-rw-   0        0        0    14612 2023-07-31 04:30:40.000000 gramex-1.94.2/tests/test_cache.py
+-rw-rw-rw-   0        0        0    15151 2023-09-21 00:20:48.000000 gramex-1.94.2/tests/test_capturehandler.py
+-rw-rw-rw-   0        0        0     1288 2023-07-31 04:30:40.000000 gramex-1.94.2/tests/test_comichandler.py
+-rw-rw-rw-   0        0        0    12571 2023-07-31 04:30:40.000000 gramex-1.94.2/tests/test_drivehandler.py
+-rw-rw-rw-   0        0        0    17308 2023-07-31 04:30:40.000000 gramex-1.94.2/tests/test_filehandler.py
+-rw-rw-rw-   0        0        0     6797 2023-07-31 04:30:40.000000 gramex-1.94.2/tests/test_filterhandler.py
+-rw-rw-rw-   0        0        0    35746 2023-07-31 04:30:40.000000 gramex-1.94.2/tests/test_formhandler.py
+-rw-rw-rw-   0        0        0     8787 2023-09-12 09:13:58.000000 gramex-1.94.2/tests/test_functionhandler.py
+-rw-rw-rw-   0        0        0     3201 2023-07-31 04:30:40.000000 gramex-1.94.2/tests/test_gramexlog.py
+-rw-rw-rw-   0        0        0    19008 2023-07-31 04:30:40.000000 gramex-1.94.2/tests/test_handlers.py
+-rw-rw-rw-   0        0        0     1475 2023-07-31 04:30:40.000000 gramex-1.94.2/tests/test_init.py
+-rw-rw-rw-   0        0        0     8931 2023-07-31 04:30:40.000000 gramex-1.94.2/tests/test_install.py
+-rw-rw-rw-   0        0        0     6361 2023-07-31 04:30:40.000000 gramex-1.94.2/tests/test_jsonhandler.py
+-rw-rw-rw-   0        0        0     3896 2023-07-31 04:30:40.000000 gramex-1.94.2/tests/test_ldapauth.py
+-rw-rw-rw-   0        0        0     7519 2023-07-31 04:30:40.000000 gramex-1.94.2/tests/test_logviewer.py
+-rw-rw-rw-   0        0        0    32874 2024-05-20 10:32:31.000000 gramex-1.94.2/tests/test_mlhandler.py
+-rw-rw-rw-   0        0        0     4745 2023-07-31 04:30:40.000000 gramex-1.94.2/tests/test_modelhandler.py
+-rw-rw-rw-   0        0        0     7082 2023-07-31 04:30:40.000000 gramex-1.94.2/tests/test_openapihandler.py
+-rw-rw-rw-   0        0        0     1411 2023-07-31 04:30:40.000000 gramex-1.94.2/tests/test_pptxhandler.py
+-rw-rw-rw-   0        0        0     3530 2023-07-31 04:30:40.000000 gramex-1.94.2/tests/test_processhandler.py
+-rw-rw-rw-   0        0        0     3834 2023-07-31 04:30:40.000000 gramex-1.94.2/tests/test_proxyhandler.py
+-rw-rw-rw-   0        0        0     1527 2023-07-31 04:30:40.000000 gramex-1.94.2/tests/test_pynode.py
+-rw-rw-rw-   0        0        0     1220 2023-07-31 04:30:40.000000 gramex-1.94.2/tests/test_schedule.py
+-rw-rw-rw-   0        0        0      757 2023-07-31 04:30:40.000000 gramex-1.94.2/tests/test_secrets.py
+-rw-rw-rw-   0        0        0      330 2023-07-31 04:30:41.000000 gramex-1.94.2/tests/test_sms.py
+-rw-rw-rw-   0        0        0      180 2023-07-31 04:30:41.000000 gramex-1.94.2/tests/test_subapp.py
+-rw-rw-rw-   0        0        0     5382 2023-07-31 04:30:41.000000 gramex-1.94.2/tests/test_subprocess.py
+-rw-rw-rw-   0        0        0     2277 2023-07-31 04:30:41.000000 gramex-1.94.2/tests/test_translater.py
+-rw-rw-rw-   0        0        0     2894 2024-05-20 10:32:31.000000 gramex-1.94.2/tests/test_twitterresthandler.py
+-rw-rw-rw-   0        0        0     2352 2023-07-31 04:30:41.000000 gramex-1.94.2/tests/test_ui.py
+-rw-rw-rw-   0        0        0     2359 2023-07-31 04:30:41.000000 gramex-1.94.2/tests/test_update.py
+-rw-rw-rw-   0        0        0     6563 2023-07-31 04:30:41.000000 gramex-1.94.2/tests/test_uploadhandler.py
+-rw-rw-rw-   0        0        0     1966 2023-07-31 04:30:41.000000 gramex-1.94.2/tests/test_watcher.py
+-rw-rw-rw-   0        0        0     2647 2023-07-31 04:30:41.000000 gramex-1.94.2/tests/test_websockethandler.py
```

### Comparing `gramex-1.94.1/.gitignore` & `gramex-1.94.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/LICENSE` & `gramex-1.94.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/MANIFEST.in` & `gramex-1.94.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/PKG-INFO` & `gramex-1.94.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gramex
-Version: 1.94.1
+Version: 1.94.2
 Summary: Gramex: Low Code Data Solutions Platform
 Author-email: Anand S <s.anand@gramener.com>, Pratap Vardhan <pratapapvr@gmail.com>, Jaidev Deshpande <jaidev.deshpande@gramener.com>, Bhanu Kamapantula <talk2kish@gmail.com>, Radheya Kale <radheya.kale@gramener.com>, Karmanya Aggarwal <karmanyaaggarwal@gmail.com>, Sandeep Bhat <sandeep.bhat@gramener.com>, Shraddheya Shrivastava <shraddheya.shrivastava@gramener.com>, Sundeep Reddy Mallu <sundeep.mally@gramener.com>
 License: MIT
 Project-URL: Homepage, https://gramener.com/gramex/
 Project-URL: Documentation, https://gramener.com/gramex/guide/
 Project-URL: Repository, https://github.com/gramener/gramex
 Project-URL: Changelog, https://gramener.com/gramex/guide/release/
```

### Comparing `gramex-1.94.1/README.md` & `gramex-1.94.2/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/__init__.py` & `gramex-1.94.2/gramex/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-'''Parses command line / configuration and runs Gramex.
+"""Parses command line / configuration and runs Gramex.
 
 Running `gramex` on the command line calls:
 
 1. [gramex.commandline][] to parse command line arguments
 2. [gramex.init][] to parse the configuration and start Gramex
 
 This module also has
 
 - [gramex.shutdown][] to shut down Gramex (e.g. on `Ctrl+C`)
 - [gramex.gramex_update][] to check if Gramex is out of date
 - [gramex.log][] to log messages persistently (e.g. on ElasticSearch)
-'''
+"""
 
 import os
 import sys
 import json
 import yaml
 import logging
 import logging.config
 from packaging import version
 from pathlib import Path
 from typing import List
 from orderedattrdict import AttrDict
 from gramex.config import ChainConfig, PathConfig, app_log, variables, setup_variables
 from gramex.config import ioloop_running, prune_keys, setup_secrets
 
-help = '''
+help = """
 Gramex {__version__} Copyright (c) 2017 by Gramener
 Help: https://gramener.com/gramex/guide/
 
 Common startup options
 
 --listen.port=9090            Starts Gramex at port 9090
 --log.level=warning           Accepts debug|info|warning|error|critical
@@ -48,47 +48,47 @@
 Installation commands. For usage, run "gramex <command> --help"
 
 gramex install                Install an app
 gramex update                 Update an app
 gramex setup                  Run make, npm install, bower install etc on app
 gramex run                    Run an installed app
 gramex uninstall              Uninstall an app
-'''
+"""
 
-__version__ = '1.94.1'
+__version__ = "1.94.2"
 
 paths = AttrDict()  # Paths where configurations are stored
 conf = AttrDict()  # Final merged configurations
 config_layers = ChainConfig()  # Loads all configurations. init() updates it
 appconfig = AttrDict()  # Final app configuration
 
-paths['source'] = Path(__file__).absolute().parent  # Where gramex source code is
-paths['base'] = Path('.')  # Where gramex is run from
+paths["source"] = Path(__file__).absolute().parent  # Where gramex source code is
+paths["base"] = Path(".")  # Where gramex is run from
 
 callbacks = {}  # Services callbacks
 _sys_path = list(sys.path)  # Preserve original sys.path
 
 
 # List of URLs to warn about in case of duplicates
 PathConfig.duplicate_warn = [
-    'url.*',
-    'cache.*',
-    'schedule.*',
-    'watch.*',
-    'email.*',
-    'alert.*',
-    'sms.*',
-    'log.loggers.*',
-    'log.handlers.*',
-    'log.formatters.*',
+    "url.*",
+    "cache.*",
+    "schedule.*",
+    "watch.*",
+    "email.*",
+    "alert.*",
+    "sms.*",
+    "log.loggers.*",
+    "log.handlers.*",
+    "log.formatters.*",
 ]
 
 
 def commandline(args: List[str] = None):
-    '''Run Gramex from the command line.
+    """Run Gramex from the command line.
 
     Parameters:
         args: Command line arguments. If not provided, uses `sys.argv`
 
     Gramex can be run in 2 ways, both of which call [gramex.commandline][]:
 
     1. `python -m gramex`, which runs `__main__.py`.
@@ -109,106 +109,106 @@
 
     Keyword arguments with '.' are split into sub-keys, e.g.
     `gramex --listen.port 80` becomes `init(listen={"port": 80})`.
 
     Values are parsed as YAML, e.g. `null` becomes `None`.
 
     If the keyword arguments include `--help`, it prints the usage of that function and exits.
-    '''
+    """
     commands = sys.argv[1:] if args is None else args
 
     # First, setup log: service at INFO to log progress. App's log: may override this later.
-    log_config = (+PathConfig(paths['source'] / 'gramex.yaml')).get('log', AttrDict())
+    log_config = (+PathConfig(paths["source"] / "gramex.yaml")).get("log", AttrDict())
     log_config.loggers.gramex.level = logging.INFO
     from . import services
 
     services.log(log_config)
 
     # kwargs has all optional command line args as a dict of values / lists.
     # args has all positional arguments as a list.
     kwargs = parse_command_line(commands)
-    args = kwargs.pop('_')
+    args = kwargs.pop("_")
 
     # If -V or --version is specified, print a message and end
-    if 'V' in kwargs or 'version' in kwargs:
-        pyver = '{0}.{1}.{2}'.format(*sys.version_info[:3])
+    if "V" in kwargs or "version" in kwargs:
+        pyver = "{0}.{1}.{2}".format(*sys.version_info[:3])
         msg = [
-            f'Gramex version: {__version__}',
+            f"Gramex version: {__version__}",
             f'Gramex path: {paths["source"]}',
-            f'Python version: {pyver}',
-            f'Python path: {sys.executable}',
+            f"Python version: {pyver}",
+            f"Python path: {sys.executable}",
         ]
-        return console(msg='\n'.join(msg))
+        return console(msg="\n".join(msg))
 
     # Any positional argument is treated as a gramex command
     if len(args) > 0:
         base_command = args.pop(0).lower()
-        method = 'install' if base_command == 'update' else base_command
+        method = "install" if base_command == "update" else base_command
         if method in {
-            'install',
-            'uninstall',
-            'setup',
-            'run',
-            'service',
-            'init',
-            'mail',
-            'license',
-            'features',
-            'complexity',
+            "install",
+            "uninstall",
+            "setup",
+            "run",
+            "service",
+            "init",
+            "mail",
+            "license",
+            "features",
+            "complexity",
         }:
             import gramex.install
 
-            if 'help' in kwargs:
+            if "help" in kwargs:
                 return console(msg=gramex.install.show_usage(method))
             return getattr(gramex.install, method)(args=args, kwargs=kwargs)
-        raise NotImplementedError(f'Unknown gramex command: {base_command}')
-    elif 'help' in kwargs:
+        raise NotImplementedError(f"Unknown gramex command: {base_command}")
+    elif "help" in kwargs:
         return console(msg=help.strip().format(**globals()))
 
     # Use current dir as base (where gramex is run from) if there's a gramex.yaml.
-    if not os.path.isfile('gramex.yaml'):
-        return console(msg='No gramex.yaml. See https://gramener.com/gramex/guide/')
+    if not os.path.isfile("gramex.yaml"):
+        return console(msg="No gramex.yaml. See https://gramener.com/gramex/guide/")
 
-    pyver = sys.version.replace('\n', ' ')
-    app_log.info(f'Gramex {__version__} | {os.getcwd()} | Python {pyver}')
+    pyver = sys.version.replace("\n", " ")
+    app_log.info(f"Gramex {__version__} | {os.getcwd()} | Python {pyver}")
 
     # Run gramex.init(cmd={command line arguments like YAML variables})
     # --log.* settings are moved to log.loggers.gramex.*
     #   E.g. --log.level => log.loggers.gramex.level
     # --* remaining settings are moved to app.*
     #   E.g. --watch => app.watch
     config = AttrDict(app=kwargs)
-    if kwargs.get('log'):
-        config.log = AttrDict(loggers=AttrDict(gramex=kwargs.pop('log')))
-        if 'level' in config.log.loggers.gramex:
+    if kwargs.get("log"):
+        config.log = AttrDict(loggers=AttrDict(gramex=kwargs.pop("log")))
+        if "level" in config.log.loggers.gramex:
             config.log.loggers.gramex.level = config.log.loggers.gramex.level.upper()
     return init(cmd=config)
 
 
 def parse_command_line(commands: List[str]):
     # Parse command line arguments.
     # e.g. gramex cmd1 cmd2 --a=1 2 -b x --c --p.q=4
     # returns {"_": ["cmd1", "cmd2"], "a": [1, 2], "b": "x", "c": True, "p": {"q": [4]}}
-    group = '_'
+    group = "_"
     args = AttrDict({group: []})
     for arg in commands:
         # If it's a keyword argument, extract key=value. "--key" becomes key=True
-        if arg.startswith('-'):
-            group, value = arg.lstrip('-'), 'True'
-            if '=' in group:
-                group, value = group.split('=', 1)
+        if arg.startswith("-"):
+            group, value = arg.lstrip("-"), "True"
+            if "=" in group:
+                group, value = group.split("=", 1)
         # If it's a positional argument, leave the key as '_', and get the value
         else:
             value = arg
 
         # Parse values as YAML, e.g. null -> None
         value = yaml.safe_load(value)
         # If there are sub-keys, create a dict for them
         base = args
-        keys = group.split('.')
+        keys = group.split(".")
         for key in keys[:-1]:
             base = base.setdefault(key, AttrDict())
 
         # Make a list where required. `--x=1 --x=2` becomes {x: [1, 2]}
         # If key is present, make it a list.
         # If key is a list, append to it.
         if keys[-1] not in base or base[keys[-1]] is True:
@@ -218,15 +218,15 @@
         else:
             base[keys[-1]].append(value)
 
     return args
 
 
 def init(force_reload: bool = False, **kwargs) -> None:
-    '''Load Gramex configurations and start / restart the Gramex instance.
+    """Load Gramex configurations and start / restart the Gramex instance.
 
     Parameters:
         force_reload (bool): Reload services even config hasn't changed
         **kwargs (dict): Overrides config
 
     `gramex.init()` loads configurations from 3 sources, which override each other:
 
@@ -240,18 +240,18 @@
     configuration has changed or `force_reload=True`.
 
     If a kwarg value is:
 
     - a string, it's loaded as-is
     - a Path pointing to a file, it's loaded as a YAML config file
     - a Path pointing to a directory, it loads a `gramex.yaml` file from that directory
-    '''
+    """
     # Set up secrets from .secrets.yaml, if any
     try:
-        setup_secrets(paths['base'] / '.secrets.yaml')
+        setup_secrets(paths["base"] / ".secrets.yaml")
     except Exception as e:
         app_log.exception(e)
 
     # Add base path locations where config files are found to sys.path.
     # This allows variables: to import files from folder where configs are defined.
     sys.path[:] = _sys_path + [
         str(path.absolute()) for path in paths.values() if isinstance(path, Path)
@@ -263,156 +263,156 @@
 
     # Initialise configuration layers with provided configurations
     # AttrDicts are updated as-is. Paths are converted to PathConfig
     paths.update(kwargs)
     for key, val in paths.items():
         if isinstance(val, Path):
             if val.is_dir():
-                val = val / 'gramex.yaml'
+                val = val / "gramex.yaml"
             val = PathConfig(val)
         config_layers[key] = val
 
     # Locate all config files
     config_files = set()
     for path_config in config_layers.values():
-        if hasattr(path_config, '__info__'):
+        if hasattr(path_config, "__info__"):
             for pathinfo in path_config.__info__.imports:
                 config_files.add(pathinfo.path)
     config_files = list(config_files)
 
     # Add config file folders to sys.path
     sys.path[:] = _sys_path + [str(path.absolute().parent) for path in config_files]
 
     from . import services
 
-    globals()['service'] = services.info  # gramex.service = gramex.services.info
+    globals()["service"] = services.info  # gramex.service = gramex.services.info
 
     # Override final configurations
     appconfig.clear()
     appconfig.update(+config_layers)
     # If --settings.debug, override root and Gramex loggers to show debug messages
-    if appconfig.app.get('settings', {}).get('debug', False):
+    if appconfig.app.get("settings", {}).get("debug", False):
         appconfig.log.root.level = appconfig.log.loggers.gramex.level = logging.DEBUG
 
     # Set up a watch on config files (including imported files)
-    if appconfig.app.get('watch', True):
+    if appconfig.app.get("watch", True):
         from services import watcher
 
-        watcher.watch('gramex-reconfig', paths=config_files, on_modified=lambda event: init())
+        watcher.watch("gramex-reconfig", paths=config_files, on_modified=lambda event: init())
 
     # Run all valid services. (The "+" before config_chain merges the chain)
     # Services may return callbacks to be run at the end
     for key, val in appconfig.items():
         if key not in conf or conf[key] != val or force_reload:
             if hasattr(services, key):
-                app_log.debug(f'Loading service: {key}')
-                conf[key] = prune_keys(val, {'comment'})
+                app_log.debug(f"Loading service: {key}")
+                conf[key] = prune_keys(val, {"comment"})
                 callback = getattr(services, key)(conf[key])
                 if callable(callback):
                     callbacks[key] = callback
             else:
-                app_log.error(f'No service named {key}')
+                app_log.error(f"No service named {key}")
 
     # Run the callbacks. Specifically, the app service starts the Tornado ioloop
     for key in (+config_layers).keys():
         if key in callbacks:
-            app_log.debug(f'Running callback: {key}')
+            app_log.debug(f"Running callback: {key}")
             callbacks[key]()
 
 
 def shutdown():
-    '''Shut down the running Gramex instance.'''
+    """Shut down the running Gramex instance."""
     from . import services
 
     ioloop = services.info.main_ioloop
     if ioloop_running(ioloop):
-        app_log.info('Shutting down Gramex...')
+        app_log.info("Shutting down Gramex...")
         # Shut down Gramex in a thread-safe way. add_callback is the ONLY thread-safe method
         ioloop.add_callback(ioloop.stop)
 
 
 def gramex_update(url: str):
-    '''Check if a newer version of Gramex is available. If yes, log a warning.
+    """Check if a newer version of Gramex is available. If yes, log a warning.
 
     Parameters:
         url: URL to check for new version
 
     Gramex uses <https://gramener.com/gramex-update/> as the URL to check for new versions.
-    '''
+    """
     import time
     import requests
     import platform
     from . import services
 
     if not services.info.eventlog:
-        return app_log.error('eventlog: service is not running. So Gramex update is disabled')
+        return app_log.error("eventlog: service is not running. So Gramex update is disabled")
 
     query = services.info.eventlog.query
     update = query('SELECT * FROM events WHERE event="update" ORDER BY time DESC LIMIT 1')
     delay = 24 * 60 * 60  # Wait for one day before updates
-    if update and time.time() < update[0]['time'] + delay:
-        return app_log.debug('Gramex update ran recently. Deferring check.')
+    if update and time.time() < update[0]["time"] + delay:
+        return app_log.debug("Gramex update ran recently. Deferring check.")
 
     meta = {
-        'dir': variables.get('GRAMEXDATA'),
-        'uname': platform.uname(),
+        "dir": variables.get("GRAMEXDATA"),
+        "uname": platform.uname(),
     }
     if update:
-        events = query('SELECT * FROM events WHERE time > ? ORDER BY time', (update[0]['time'],))
+        events = query("SELECT * FROM events WHERE time > ? ORDER BY time", (update[0]["time"],))
     else:
-        events = query('SELECT * FROM events')
+        events = query("SELECT * FROM events")
     logs = [dict(log, **meta) for log in events]
 
     r = requests.post(url, data=json.dumps(logs), timeout=30)
     r.raise_for_status()
     update = r.json()
-    server_version = update['version']
+    server_version = update["version"]
     if version.parse(server_version) > version.parse(__version__):
-        app_log.error(f'Gramex {server_version} is available. https://gramener.com/gramex/guide/')
+        app_log.error(f"Gramex {server_version} is available. https://gramener.com/gramex/guide/")
     elif version.parse(server_version) < version.parse(__version__):
-        app_log.warning(f'Gramex {__version__} is ahead of stable {server_version}')
+        app_log.warning(f"Gramex {__version__} is ahead of stable {server_version}")
     else:
-        app_log.debug(f'Gramex {__version__} is up to date')
-    services.info.eventlog.add('update', update)
-    return {'logs': logs, 'response': update}
+        app_log.debug(f"Gramex {__version__} is up to date")
+    services.info.eventlog.add("update", update)
+    return {"logs": logs, "response": update}
 
 
 def log(*args, **kwargs):
-    '''Logs structured information for future reference.
+    """Logs structured information for future reference.
 
     Examples:
         >>> gramex.log(level='INFO', x=1, msg='abc')
 
         This logs `{level: INFO, x: 1, msg: abc}` into a logging queue.
 
         If a `gramexlog` service like ElasticSearch has been configured, it will periodically flush
         the logs into the server.
-    '''
+    """
     from . import services
 
     # gramexlog() positional arguments may have a handler and app (in any order)
     # The app defaults to the first gramexlog:
-    handler, app = None, services.info.gramexlog.get('defaultapp')
+    handler, app = None, services.info.gramexlog.get("defaultapp")
     for arg in args:
         # Pretend that anything that has a .args is a handler
-        if hasattr(getattr(arg, 'args', None), 'items'):
+        if hasattr(getattr(arg, "args", None), "items"):
             handler = arg
         # ... and anything that's a string is an index name. The last string overrides all
         elif isinstance(arg, str):
             app = arg
     # If the user logs into an unknown app, stop immediately
     try:
         conf = services.info.gramexlog.apps[app]
     except KeyError:
-        raise ValueError(f'gramexlog: no config for {app}')
+        raise ValueError(f"gramexlog: no config for {app}")
 
     # Add all URL query parameters. In case of multiple values, capture the last
     if handler:
         kwargs.update({key: val[-1] for key, val in handler.args.items()})
     # Add additional keys specified in gramex.yaml via keys:
     kwargs.update(conf.extra_keys(handler))
     conf.queue.append(kwargs)
 
 
 def console(msg):
-    '''Write message to console. An alias for print().'''
+    """Write message to console. An alias for print()."""
     print(msg)  # noqa
```

### Comparing `gramex-1.94.1/gramex/apps/admin2/gramex.yaml` & `gramex-1.94.2/gramex/apps/admin2/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/admin2/gramexadmin.py` & `gramex-1.94.2/gramex/apps/admin2/gramexadmin.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,17 +157,17 @@
     sys.stdout = out
     # Run code and get the result. (Result is None for exec)
     try:
         context = contexts.setdefault(handler.session['id'], {})
         context['handler'] = handler
         # B307:eval B102:exec_used is safe since only admin can run this
         if mode == 'eval':
-            result = eval(co, context)  # nosec B307
+            result = eval(co, context)  # noqa S307
         else:
-            exec(co, context)  # nosec B102
+            exec(co, context)  # noqa S102
             result = None
     except Exception as e:
         result = e
     finally:
         sys.stdout = old_stdout
 
     # Write the stdout (if any), then the returned value (if any)
@@ -213,18 +213,18 @@
     value['git', 'path'] = which('git')
 
     from gramex.cache import Subprocess
 
     apps = {
         # B602:any_other_function_with_shell_equals_true is safe here since the code is
         # constructed entirely in this function. We use shell to pick up the commands' paths.
-        ('node', 'version'): Subprocess('node --version', shell=True),  # nosec 602
-        ('npm', 'version'): Subprocess('npm --version', shell=True),  # nosec 602
-        ('yarn', 'version'): Subprocess('yarn --version', shell=True),  # nosec 602
-        ('git', 'version'): Subprocess('git --version', shell=True),  # nosec 602
+        ('node', 'version'): Subprocess('node --version', shell=True),  # noqa S604
+        ('npm', 'version'): Subprocess('npm --version', shell=True),  # noqa S604
+        ('yarn', 'version'): Subprocess('yarn --version', shell=True),  # noqa S604
+        ('git', 'version'): Subprocess('git --version', shell=True),  # noqa S604
     }
     for key, proc in apps.items():
         stdout, stderr = yield proc.wait_for_exit()
         value[key] = stdout.strip()
         if not value[key]:
             error[key] = stderr.strip()
```

### Comparing `gramex-1.94.1/gramex/apps/admin2/index.html` & `gramex-1.94.2/gramex/apps/admin2/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/admin2/schedule.js` & `gramex-1.94.2/gramex/apps/admin2/schedule.js`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/capture/README.md` & `gramex-1.94.2/gramex/apps/capture/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/capture/capture.js` & `gramex-1.94.2/gramex/apps/capture/capture.js`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/capture/chromecapture.js` & `gramex-1.94.2/gramex/apps/capture/chromecapture.js`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/capture/index.html` & `gramex-1.94.2/gramex/apps/capture/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/capture/package-lock.json` & `gramex-1.94.2/gramex/apps/capture/package-lock.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984748143881209%*

 * *Differences: {"'packages'": "{'node_modules/@babel/code-frame': {'version': '7.24.2', 'resolved': "*

 * *               "'https://registry.npmjs.org/@babel/code-frame/-/code-frame-7.24.2.tgz', "*

 * *               "'integrity': "*

 * *               "'sha512-y5+tLQyV8pg3fsiln67BVLD1P13Eg4lh5RW9mF0zUuvLrv9uIQ4MCL+CRT+FTsBlBjcIan6PGsLcBN0m3ClUyQ==', "*

 * *               "'dependencies': {'@babel/highlight': '^7.24.2', 'picocolors': '^1.0.0', delete: "*

 * *               "['chalk']}}, 'node_modules/@babel/helper-validator-identifier': {'version […]*

```diff
@@ -17,44 +17,45 @@
             "devDependencies": {},
             "license": "ISC",
             "name": "capture",
             "version": "1.0.0"
         },
         "node_modules/@babel/code-frame": {
             "dependencies": {
-                "@babel/highlight": "^7.23.4",
-                "chalk": "^2.4.2"
+                "@babel/highlight": "^7.24.2",
+                "picocolors": "^1.0.0"
             },
             "engines": {
                 "node": ">=6.9.0"
             },
-            "integrity": "sha512-CgH3s1a96LipHCmSUmYFPwY7MNx8C3avkq7i4Wl3cfa662ldtUe4VM1TPXX70pfmrlWTb6jLqTYrZyT2ZTJBgA==",
-            "resolved": "https://registry.npmjs.org/@babel/code-frame/-/code-frame-7.23.5.tgz",
-            "version": "7.23.5"
+            "integrity": "sha512-y5+tLQyV8pg3fsiln67BVLD1P13Eg4lh5RW9mF0zUuvLrv9uIQ4MCL+CRT+FTsBlBjcIan6PGsLcBN0m3ClUyQ==",
+            "resolved": "https://registry.npmjs.org/@babel/code-frame/-/code-frame-7.24.2.tgz",
+            "version": "7.24.2"
         },
         "node_modules/@babel/helper-validator-identifier": {
             "engines": {
                 "node": ">=6.9.0"
             },
-            "integrity": "sha512-Y4OZ+ytlatR8AI+8KZfKuL5urKp7qey08ha31L8b3BwewJAoJamTzyvxPR/5D+KkdJCGPq/+8TukHBlY10FX9A==",
-            "resolved": "https://registry.npmjs.org/@babel/helper-validator-identifier/-/helper-validator-identifier-7.22.20.tgz",
-            "version": "7.22.20"
+            "integrity": "sha512-3q93SSKX2TWCG30M2G2kwaKeTYgEUp5Snjuj8qm729SObL6nbtUldAi37qbxkD5gg3xnBio+f9nqpSepGZMvxA==",
+            "resolved": "https://registry.npmjs.org/@babel/helper-validator-identifier/-/helper-validator-identifier-7.24.5.tgz",
+            "version": "7.24.5"
         },
         "node_modules/@babel/highlight": {
             "dependencies": {
-                "@babel/helper-validator-identifier": "^7.22.20",
+                "@babel/helper-validator-identifier": "^7.24.5",
                 "chalk": "^2.4.2",
-                "js-tokens": "^4.0.0"
+                "js-tokens": "^4.0.0",
+                "picocolors": "^1.0.0"
             },
             "engines": {
                 "node": ">=6.9.0"
             },
-            "integrity": "sha512-acGdbYSfp2WheJoJm/EBBBLh/ID8KDc64ISZ9DYtBmC8/Q204PZJLHyzeB5qMzJ5trcOkybd78M4x2KWsUq++A==",
-            "resolved": "https://registry.npmjs.org/@babel/highlight/-/highlight-7.23.4.tgz",
-            "version": "7.23.4"
+            "integrity": "sha512-8lLmua6AVh/8SLJRRVD6V8p73Hir9w5mJrhE+IPpILG31KKlI9iz5zmBYKcWPS59qSfgP9RaSBQSHHE81WKuEw==",
+            "resolved": "https://registry.npmjs.org/@babel/highlight/-/highlight-7.24.5.tgz",
+            "version": "7.24.5"
         },
         "node_modules/@puppeteer/browsers": {
             "bin": {
                 "browsers": "lib/cjs/main-cli.js"
             },
             "dependencies": {
                 "debug": "4.3.4",
@@ -102,18 +103,18 @@
             "resolved": "https://registry.npmjs.org/ms/-/ms-2.1.2.tgz",
             "version": "2.1.2"
         },
         "node_modules/@types/node": {
             "dependencies": {
                 "undici-types": "~5.26.4"
             },
-            "integrity": "sha512-Kza43ewS3xoLgCEpQrsT+xRo/EJej1y0kVYGiLFE1NEODXGzTfwiC6tXTLMQskn1X4/Rjlh0MQUvx9W+L9long==",
+            "integrity": "sha512-eWLDGF/FOSPtAvEqeRAQ4C8LSA7M1I7i0ky1I8U7kD1J5ITyW3AsRhQrKVoWf5pFKZ2kILsEGJhsI9r93PYnOw==",
             "optional": true,
-            "resolved": "https://registry.npmjs.org/@types/node/-/node-20.11.24.tgz",
-            "version": "20.11.24"
+            "resolved": "https://registry.npmjs.org/@types/node/-/node-20.12.12.tgz",
+            "version": "20.12.12"
         },
         "node_modules/@types/yauzl": {
             "dependencies": {
                 "@types/node": "*"
             },
             "integrity": "sha512-oJoftv0LSuaDZE3Le4DbKX+KS9G36NzOeSap90UIK0yMA/NhKJhqlSGtNDORNRaIbQfzjXDrQa0ytJ6mNRGz/Q==",
             "optional": true,
@@ -683,15 +684,15 @@
         "node_modules/express": {
             "dependencies": {
                 "accepts": "~1.3.8",
                 "array-flatten": "1.1.1",
                 "body-parser": "1.20.2",
                 "content-disposition": "0.5.4",
                 "content-type": "~1.0.4",
-                "cookie": "0.5.0",
+                "cookie": "0.6.0",
                 "cookie-signature": "1.0.6",
                 "debug": "2.6.9",
                 "depd": "2.0.0",
                 "encodeurl": "~1.0.2",
                 "escape-html": "~1.0.3",
                 "etag": "~1.8.1",
                 "finalhandler": "1.2.0",
@@ -713,17 +714,25 @@
                 "type-is": "~1.6.18",
                 "utils-merge": "1.0.1",
                 "vary": "~1.1.2"
             },
             "engines": {
                 "node": ">= 0.10.0"
             },
-            "integrity": "sha512-6VyCijWQ+9O7WuVMTRBTl+cjNNIzD5cY5mQ1WM8r/LEkI2u8EYpOotESNwzNlyCn3g+dmjKYI6BmNneSr/FSRw==",
-            "resolved": "https://registry.npmjs.org/express/-/express-4.18.3.tgz",
-            "version": "4.18.3"
+            "integrity": "sha512-5T6nhjsT+EOMzuck8JjBHARTHfMht0POzlA60WV2pMD3gyXw2LZnZ+ueGdNxG+0calOJcWKbpFcuzLZ91YWq9Q==",
+            "resolved": "https://registry.npmjs.org/express/-/express-4.19.2.tgz",
+            "version": "4.19.2"
+        },
+        "node_modules/express/node_modules/cookie": {
+            "engines": {
+                "node": ">= 0.6"
+            },
+            "integrity": "sha512-U71cyTamuh1CRNCfpGY6to28lxvNwPG4Guz/EVjgf3Jmzv0vlDp1atT9eS5dDjMYHucpHbWns6Lwf3BKz6svdw==",
+            "resolved": "https://registry.npmjs.org/cookie/-/cookie-0.6.0.tgz",
+            "version": "0.6.0"
         },
         "node_modules/extract-zip": {
             "bin": {
                 "extract-zip": "cli.js"
             },
             "dependencies": {
                 "debug": "^4.1.1",
@@ -944,17 +953,17 @@
         "node_modules/hasown": {
             "dependencies": {
                 "function-bind": "^1.1.2"
             },
             "engines": {
                 "node": ">= 0.4"
             },
-            "integrity": "sha512-1/th4MHjnwncwXsIW6QMzlvYL9kG5e/CpVvLRZe4XPa8TOUNbCELqmvhDmnkNsAjwaG4+I8gJJL0JBvTTLO9qA==",
-            "resolved": "https://registry.npmjs.org/hasown/-/hasown-2.0.1.tgz",
-            "version": "2.0.1"
+            "integrity": "sha512-0hJU9SCPvmMzIBdZFqNPXWa6dqh7WdH0cII9y+CyS8rG3nL48Bclra9HmKhVVUHyPWNH5Y7xDwAB7bfgSjkUMQ==",
+            "resolved": "https://registry.npmjs.org/hasown/-/hasown-2.0.2.tgz",
+            "version": "2.0.2"
         },
         "node_modules/http-errors": {
             "dependencies": {
                 "depd": "2.0.0",
                 "inherits": "2.0.4",
                 "setprototypeof": "1.2.0",
                 "statuses": "2.0.1",
@@ -1458,14 +1467,19 @@
             "version": "4.0.0"
         },
         "node_modules/pend": {
             "integrity": "sha512-F3asv42UuXchdzt+xXqfW1OGlVBe+mxa2mqI0pg5yAHZPvFmY3Y6drSf/GQ1A86WgWEN9Kzh/WrgKa6iGcHXLg==",
             "resolved": "https://registry.npmjs.org/pend/-/pend-1.2.0.tgz",
             "version": "1.2.0"
         },
+        "node_modules/picocolors": {
+            "integrity": "sha512-anP1Z8qwhkbmu7MFP5iTt+wQKXgwzf7zTyGlcdzabySa9vd0Xt392U0rVmz9poOaBj0uHJKyyo9/upk0HrEQew==",
+            "resolved": "https://registry.npmjs.org/picocolors/-/picocolors-1.0.1.tgz",
+            "version": "1.0.1"
+        },
         "node_modules/process-nextick-args": {
             "integrity": "sha512-3ouUOpQhtgrbOa17J7+uxOTpITYWaGP7/AhoR3+A+/1e9skrzelGi/dXzEYyvbxubEF6Wn2ypscTKiKJFFn1ag==",
             "resolved": "https://registry.npmjs.org/process-nextick-args/-/process-nextick-args-2.0.1.tgz",
             "version": "2.0.1"
         },
         "node_modules/progress": {
             "engines": {
@@ -1506,15 +1520,15 @@
                 "@puppeteer/browsers": "0.5.0",
                 "cosmiconfig": "8.1.3",
                 "https-proxy-agent": "5.0.1",
                 "progress": "2.0.3",
                 "proxy-from-env": "1.1.0",
                 "puppeteer-core": "19.11.1"
             },
-            "deprecated": "< 21.5.0 is no longer supported",
+            "deprecated": "< 22.5.0 is no longer supported",
             "hasInstallScript": true,
             "integrity": "sha512-39olGaX2djYUdhaQQHDZ0T0GwEp+5f9UB9HmEP0qHfdQHIq0xGQZuAZ5TLnJIc/88SrPLpEflPC+xUqOTv3c5g==",
             "resolved": "https://registry.npmjs.org/puppeteer/-/puppeteer-19.11.1.tgz",
             "version": "19.11.1"
         },
         "node_modules/puppeteer-core": {
             "dependencies": {
@@ -1722,27 +1736,27 @@
             },
             "integrity": "sha512-XGuRDNjXUijsUL0vl6nSD7cwURuzEgglbOaFuZM9g3kwDXOWVTck0jLzjPzGD+TazWbboZYu52/9/XPdUgne9g==",
             "resolved": "https://registry.npmjs.org/serve-static/-/serve-static-1.15.0.tgz",
             "version": "1.15.0"
         },
         "node_modules/set-function-length": {
             "dependencies": {
-                "define-data-property": "^1.1.2",
+                "define-data-property": "^1.1.4",
                 "es-errors": "^1.3.0",
                 "function-bind": "^1.1.2",
-                "get-intrinsic": "^1.2.3",
+                "get-intrinsic": "^1.2.4",
                 "gopd": "^1.0.1",
-                "has-property-descriptors": "^1.0.1"
+                "has-property-descriptors": "^1.0.2"
             },
             "engines": {
                 "node": ">= 0.4"
             },
-            "integrity": "sha512-j4t6ccc+VsKwYHso+kElc5neZpjtq9EnRICFZtWyBsLojhmeF/ZBd/elqm22WJh/BziDe/SBiOeAt0m2mfLD0g==",
-            "resolved": "https://registry.npmjs.org/set-function-length/-/set-function-length-1.2.1.tgz",
-            "version": "1.2.1"
+            "integrity": "sha512-pgRc4hJ4/sNjWCSS9AmnS40x3bNMDTknHgL5UaMBTMyJnU90EgWh1Rz+MC9eFu4BuN/UwZjKQuY/1v3rM7HMfg==",
+            "resolved": "https://registry.npmjs.org/set-function-length/-/set-function-length-1.2.2.tgz",
+            "version": "1.2.2"
         },
         "node_modules/setimmediate": {
             "integrity": "sha512-MATJdZp8sLqDl/68LfQmbP8zKPLQNV6BIZoIgrscFDQ+RsvK/BxeDQOgyxKKoh0y/8h3BqVFnCqQ/gd+reiIXA==",
             "resolved": "https://registry.npmjs.org/setimmediate/-/setimmediate-1.0.5.tgz",
             "version": "1.0.5"
         },
         "node_modules/setprototypeof": {
```

### Comparing `gramex-1.94.1/gramex/apps/capture/package.json` & `gramex-1.94.2/gramex/apps/capture/package.json`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/filemanager/README.html` & `gramex-1.94.2/gramex/apps/filemanager/README.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/filemanager/drivehandler-snippet.html` & `gramex-1.94.2/gramex/apps/filemanager/drivehandler-snippet.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/filemanager/filemanager-snippet.html` & `gramex-1.94.2/gramex/apps/filemanager/filemanager-snippet.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/filemanager/filemanager.html` & `gramex-1.94.2/gramex/apps/filemanager/filemanager.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/filemanager/filemanager.js` & `gramex-1.94.2/gramex/apps/filemanager/filemanager.js`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/filemanager/filemanager.py` & `gramex-1.94.2/gramex/apps/filemanager/filemanager.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/filemanager/gramex.yaml` & `gramex-1.94.2/gramex/apps/filemanager/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/filemanager/index.html` & `gramex-1.94.2/gramex/apps/filemanager/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/filemanager/navbar.html` & `gramex-1.94.2/gramex/apps/filemanager/navbar.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/init/default/.eslintrc.yml` & `gramex-1.94.2/gramex/apps/init/default/.eslintrc.yml`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/init/default/.gitlab-ci.yml` & `gramex-1.94.2/gramex/apps/init/default/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/init/default/.template.gitignore` & `gramex-1.94.2/gramex/apps/init/default/.template.gitignore`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/init/default/assets/README.template.md` & `gramex-1.94.2/gramex/apps/init/default/assets/README.template.md`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/init/default/gramex.template.yaml` & `gramex-1.94.2/gramex/apps/init/default/gramex.template.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/init/default/index.template.html` & `gramex-1.94.2/gramex/apps/init/default/index.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/init/default/js/README.template.md` & `gramex-1.94.2/gramex/apps/init/default/js/README.template.md`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/init/default/login.template.html` & `gramex-1.94.2/gramex/apps/init/default/login.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/init/default/template-navbar.template.html` & `gramex-1.94.2/gramex/apps/init/default/template-navbar.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/init/ide/index.template.html` & `gramex-1.94.2/gramex/apps/init/ide/index.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/init/minimal/index.template.html` & `gramex-1.94.2/gramex/apps/init/minimal/index.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/languagetool/README.md` & `gramex-1.94.2/gramex/apps/languagetool/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/languagetool/gramex.yaml` & `gramex-1.94.2/gramex/apps/languagetool/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/logviewer/config.yaml` & `gramex-1.94.2/gramex/apps/logviewer/config.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/logviewer/gramex.yaml` & `gramex-1.94.2/gramex/apps/logviewer/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/logviewer/index.html` & `gramex-1.94.2/gramex/apps/logviewer/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/logviewer/logviewer.py` & `gramex-1.94.2/gramex/apps/logviewer/logviewer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 import sys
 import os.path
 from glob import glob
 
 # B410:import_lxml lxml.etree is safe on https://github.com/tiran/defusedxml/tree/main/xmltestdata
-from lxml.etree import Element  # nosec B410
-from lxml.html import fromstring, tostring  # nosec B410
+from lxml.etree import Element  # noqa S410
+from lxml.html import fromstring, tostring  # noqa S410
 import numpy as np
 import pandas as pd
 import gramex.data
 import gramex.cache
 from gramex import conf
 from gramex.config import app_log
 from gramex.transforms import build_transform
```

### Comparing `gramex-1.94.1/gramex/apps/logviewer/lv-datepicker.html` & `gramex-1.94.2/gramex/apps/logviewer/lv-datepicker.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/logviewer/package-lock.json` & `gramex-1.94.2/gramex/apps/logviewer/package-lock.json`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/logviewer/render.js` & `gramex-1.94.2/gramex/apps/logviewer/render.js`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/logviewer/script.js` & `gramex-1.94.2/gramex/apps/logviewer/script.js`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/mail/index.html` & `gramex-1.94.2/gramex/apps/mail/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/mlhandler/template.html` & `gramex-1.94.2/gramex/apps/mlhandler/template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/pynode/index.js` & `gramex-1.94.2/gramex/apps/pynode/index.js`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/pynode/package-lock.json` & `gramex-1.94.2/gramex/apps/pynode/package-lock.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974999999999999%*

 * *Differences: {"'packages'": "{'node_modules/ws': {'version': '8.17.0', 'resolved': "*

 * *               "'https://registry.npmjs.org/ws/-/ws-8.17.0.tgz', 'integrity': "*

 * *               "'sha512-uJq6108EgZMAl20KagGkzCKfMEjxmKvZHG7Tlq0Z6nOky7YF7aq4mOx6xK8TJ/i1LeK4Qus7INktacctDgY8Ow=='}}"}*

```diff
@@ -39,27 +39,27 @@
             "resolved": "https://registry.npmjs.org/which/-/which-2.0.2.tgz",
             "version": "2.0.2"
         },
         "node_modules/ws": {
             "engines": {
                 "node": ">=10.0.0"
             },
-            "integrity": "sha512-HS0c//TP7Ina87TfiPUz1rQzMhHrl/SG2guqRcTOIUYD2q8uhUdNHZYJUaQ8aTGPzCh+c6oawMKW35nFl1dxyQ==",
+            "integrity": "sha512-uJq6108EgZMAl20KagGkzCKfMEjxmKvZHG7Tlq0Z6nOky7YF7aq4mOx6xK8TJ/i1LeK4Qus7INktacctDgY8Ow==",
             "peerDependencies": {
                 "bufferutil": "^4.0.1",
                 "utf-8-validate": ">=5.0.2"
             },
             "peerDependenciesMeta": {
                 "bufferutil": {
                     "optional": true
                 },
                 "utf-8-validate": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/ws/-/ws-8.16.0.tgz",
-            "version": "8.16.0"
+            "resolved": "https://registry.npmjs.org/ws/-/ws-8.17.0.tgz",
+            "version": "8.17.0"
         }
     },
     "requires": true,
     "version": "1.0.0"
 }
```

### Comparing `gramex-1.94.1/gramex/apps/ui/.snyk` & `gramex-1.94.2/gramex/apps/ui/.snyk`

 * *Files 18% similar despite different names*

```diff
@@ -19,8 +19,14 @@
 
   SNYK-JS-INFLIGHT-6095116:
     - '*':
         reason: No fix available. Await comicgen > glob upgrade
         expires: 2024-12-31T00:00:00.000Z
         created: 2024-03-02T00:00:00.000Z
 
+  SNYK-JS-BRACES-6838727:
+    - '*':
+        reason: No fix available. Await sass/chokidar/braces upgrade
+        expires: 2024-12-31T00:00:00.000Z
+        created: 2024-05-20T00:00:00.000Z
+
 patch: {}
```

### Comparing `gramex-1.94.1/gramex/apps/ui/__init__.py` & `gramex-1.94.2/gramex/apps/ui/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re
 import os
 import gramex
 import gramex.cache
 import gramex.handlers
 
 # B404:import_subprocess only for JS compilation
-import subprocess  # nosec B404
+import subprocess  # noqa S404
 from hashlib import md5
 from tornado.gen import coroutine, Return
 from functools import partial
 from gramex.config import variables, app_log, merge
 from urllib.parse import urlparse, parse_qs, urlencode
 
 
@@ -59,15 +59,15 @@
     handler.redirect(f'https://cdn.jsdelivr.net/npm/{path}', permanent=handler.get_arg('v', None))
 
 
 def _get_cache_key(state):
     '''Return short string capturing state of object. Used to create unique filenames for state'''
     cache_key = gramex.cache.cache_key(state).encode('utf-8')
     # B303, B324:md5 is safe here - it's not for cryptographic use
-    return md5(cache_key).hexdigest()[:5]  # nosec B303, B324
+    return md5(cache_key).hexdigest()[:5]  # noqa S113
 
 
 @coroutine
 def sass(
     handler: gramex.handlers.FileHandler, template: str = _join(ui_dir, 'bootstrap-theme.scss')
 ):
     '''Return a bootstrap theme based on the custom SASS variables provided.'''
```

### Comparing `gramex-1.94.1/gramex/apps/ui/bootstrap-theme.scss` & `gramex-1.94.2/gramex/apps/ui/bootstrap-theme.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/config.yaml` & `gramex-1.94.2/gramex/apps/ui/config.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/gramex.yaml` & `gramex-1.94.2/gramex/apps/ui/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/gramexui.scss` & `gramex-1.94.2/gramex/apps/ui/gramexui.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/package-lock.json` & `gramex-1.94.2/gramex/apps/ui/package-lock.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965399743291081%*

 * *Differences: {"'packages'": "{'node_modules/@emnapi/runtime': {'version': '1.2.0', 'resolved': "*

 * *               "'https://registry.npmjs.org/@emnapi/runtime/-/runtime-1.2.0.tgz', 'integrity': "*

 * *               "'sha512-bV21/9LQmcQeCPEg3BDFtvwL6cwiTMksYNWQQ4KOxCZikEGalWtenoZ0wCiukJINlGCIi2KXx01g4FoH/LxpzQ=='}, "*

 * *               "'node_modules/@img/sharp-darwin-arm64': {'version': '0.33.4', 'resolved': "*

 * *               "'https://registry.npmjs.org/@img/sharp-darwin-arm64/-/sharp-darwin-arm64-0.33.4.tgz', "*

 * *               "' […]*

```diff
@@ -31,18 +31,18 @@
             "resolved": "https://registry.npmjs.org/@dabh/diagnostics/-/diagnostics-2.0.3.tgz",
             "version": "2.0.3"
         },
         "node_modules/@emnapi/runtime": {
             "dependencies": {
                 "tslib": "^2.4.0"
             },
-            "integrity": "sha512-Txumi3td7J4A/xTTwlssKieHKTGl3j4A1tglBx72auZ49YK7ePY6XZricgIg9mnZT4xPfA+UPCUdnhRuEFDL+w==",
+            "integrity": "sha512-bV21/9LQmcQeCPEg3BDFtvwL6cwiTMksYNWQQ4KOxCZikEGalWtenoZ0wCiukJINlGCIi2KXx01g4FoH/LxpzQ==",
             "optional": true,
-            "resolved": "https://registry.npmjs.org/@emnapi/runtime/-/runtime-0.45.0.tgz",
-            "version": "0.45.0"
+            "resolved": "https://registry.npmjs.org/@emnapi/runtime/-/runtime-1.2.0.tgz",
+            "version": "1.2.0"
         },
         "node_modules/@esbuild/android-arm": {
             "cpu": [
                 "arm"
             ],
             "engines": {
                 "node": ">=12"
@@ -380,24 +380,24 @@
                 "npm": ">=9.6.5",
                 "pnpm": ">=7.1.0",
                 "yarn": ">=3.2.0"
             },
             "funding": {
                 "url": "https://opencollective.com/libvips"
             },
-            "integrity": "sha512-itHBs1rPmsmGF9p4qRe++CzCgd+kFYktnsoR1sbIAfsRMrJZau0Tt1AH9KVnufc2/tU02Gf6Ibujx+15qRE03w==",
+            "integrity": "sha512-p0suNqXufJs9t3RqLBO6vvrgr5OhgbWp76s5gTRvdmxmuv9E1rcaqGUsl3l4mKVmXPkTkTErXediAui4x+8PSA==",
             "optional": true,
             "optionalDependencies": {
-                "@img/sharp-libvips-darwin-arm64": "1.0.1"
+                "@img/sharp-libvips-darwin-arm64": "1.0.2"
             },
             "os": [
                 "darwin"
             ],
-            "resolved": "https://registry.npmjs.org/@img/sharp-darwin-arm64/-/sharp-darwin-arm64-0.33.2.tgz",
-            "version": "0.33.2"
+            "resolved": "https://registry.npmjs.org/@img/sharp-darwin-arm64/-/sharp-darwin-arm64-0.33.4.tgz",
+            "version": "0.33.4"
         },
         "node_modules/@img/sharp-darwin-x64": {
             "cpu": [
                 "x64"
             ],
             "engines": {
                 "glibc": ">=2.26",
@@ -405,192 +405,192 @@
                 "npm": ">=9.6.5",
                 "pnpm": ">=7.1.0",
                 "yarn": ">=3.2.0"
             },
             "funding": {
                 "url": "https://opencollective.com/libvips"
             },
-            "integrity": "sha512-/rK/69Rrp9x5kaWBjVN07KixZanRr+W1OiyKdXcbjQD6KbW+obaTeBBtLUAtbBsnlTTmWthw99xqoOS7SsySDg==",
+            "integrity": "sha512-0l7yRObwtTi82Z6ebVI2PnHT8EB2NxBgpK2MiKJZJ7cz32R4lxd001ecMhzzsZig3Yv9oclvqqdV93jo9hy+Dw==",
             "optional": true,
             "optionalDependencies": {
-                "@img/sharp-libvips-darwin-x64": "1.0.1"
+                "@img/sharp-libvips-darwin-x64": "1.0.2"
             },
             "os": [
                 "darwin"
             ],
-            "resolved": "https://registry.npmjs.org/@img/sharp-darwin-x64/-/sharp-darwin-x64-0.33.2.tgz",
-            "version": "0.33.2"
+            "resolved": "https://registry.npmjs.org/@img/sharp-darwin-x64/-/sharp-darwin-x64-0.33.4.tgz",
+            "version": "0.33.4"
         },
         "node_modules/@img/sharp-libvips-darwin-arm64": {
             "cpu": [
                 "arm64"
             ],
             "engines": {
                 "macos": ">=11",
                 "npm": ">=9.6.5",
                 "pnpm": ">=7.1.0",
                 "yarn": ">=3.2.0"
             },
             "funding": {
                 "url": "https://opencollective.com/libvips"
             },
-            "integrity": "sha512-kQyrSNd6lmBV7O0BUiyu/OEw9yeNGFbQhbxswS1i6rMDwBBSX+e+rPzu3S+MwAiGU3HdLze3PanQ4Xkfemgzcw==",
+            "integrity": "sha512-tcK/41Rq8IKlSaKRCCAuuY3lDJjQnYIW1UXU1kxcEKrfL8WR7N6+rzNoOxoQRJWTAECuKwgAHnPvqXGN8XfkHA==",
             "optional": true,
             "os": [
                 "darwin"
             ],
-            "resolved": "https://registry.npmjs.org/@img/sharp-libvips-darwin-arm64/-/sharp-libvips-darwin-arm64-1.0.1.tgz",
-            "version": "1.0.1"
+            "resolved": "https://registry.npmjs.org/@img/sharp-libvips-darwin-arm64/-/sharp-libvips-darwin-arm64-1.0.2.tgz",
+            "version": "1.0.2"
         },
         "node_modules/@img/sharp-libvips-darwin-x64": {
             "cpu": [
                 "x64"
             ],
             "engines": {
                 "macos": ">=10.13",
                 "npm": ">=9.6.5",
                 "pnpm": ">=7.1.0",
                 "yarn": ">=3.2.0"
             },
             "funding": {
                 "url": "https://opencollective.com/libvips"
             },
-            "integrity": "sha512-eVU/JYLPVjhhrd8Tk6gosl5pVlvsqiFlt50wotCvdkFGf+mDNBJxMh+bvav+Wt3EBnNZWq8Sp2I7XfSjm8siog==",
+            "integrity": "sha512-Ofw+7oaWa0HiiMiKWqqaZbaYV3/UGL2wAPeLuJTx+9cXpCRdvQhCLG0IH8YGwM0yGWGLpsF4Su9vM1o6aer+Fw==",
             "optional": true,
             "os": [
                 "darwin"
             ],
-            "resolved": "https://registry.npmjs.org/@img/sharp-libvips-darwin-x64/-/sharp-libvips-darwin-x64-1.0.1.tgz",
-            "version": "1.0.1"
+            "resolved": "https://registry.npmjs.org/@img/sharp-libvips-darwin-x64/-/sharp-libvips-darwin-x64-1.0.2.tgz",
+            "version": "1.0.2"
         },
         "node_modules/@img/sharp-libvips-linux-arm": {
             "cpu": [
                 "arm"
             ],
             "engines": {
                 "glibc": ">=2.28",
                 "npm": ">=9.6.5",
                 "pnpm": ">=7.1.0",
                 "yarn": ">=3.2.0"
             },
             "funding": {
                 "url": "https://opencollective.com/libvips"
             },
-            "integrity": "sha512-FtdMvR4R99FTsD53IA3LxYGghQ82t3yt0ZQ93WMZ2xV3dqrb0E8zq4VHaTOuLEAuA83oDawHV3fd+BsAPadHIQ==",
+            "integrity": "sha512-iLWCvrKgeFoglQxdEwzu1eQV04o8YeYGFXtfWU26Zr2wWT3q3MTzC+QTCO3ZQfWd3doKHT4Pm2kRmLbupT+sZw==",
             "optional": true,
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@img/sharp-libvips-linux-arm/-/sharp-libvips-linux-arm-1.0.1.tgz",
-            "version": "1.0.1"
+            "resolved": "https://registry.npmjs.org/@img/sharp-libvips-linux-arm/-/sharp-libvips-linux-arm-1.0.2.tgz",
+            "version": "1.0.2"
         },
         "node_modules/@img/sharp-libvips-linux-arm64": {
             "cpu": [
                 "arm64"
             ],
             "engines": {
                 "glibc": ">=2.26",
                 "npm": ">=9.6.5",
                 "pnpm": ">=7.1.0",
                 "yarn": ">=3.2.0"
             },
             "funding": {
                 "url": "https://opencollective.com/libvips"
             },
-            "integrity": "sha512-bnGG+MJjdX70mAQcSLxgeJco11G+MxTz+ebxlz8Y3dxyeb3Nkl7LgLI0mXupoO+u1wRNx/iRj5yHtzA4sde1yA==",
+            "integrity": "sha512-x7kCt3N00ofFmmkkdshwj3vGPCnmiDh7Gwnd4nUwZln2YjqPxV1NlTyZOvoDWdKQVDL911487HOueBvrpflagw==",
             "optional": true,
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@img/sharp-libvips-linux-arm64/-/sharp-libvips-linux-arm64-1.0.1.tgz",
-            "version": "1.0.1"
+            "resolved": "https://registry.npmjs.org/@img/sharp-libvips-linux-arm64/-/sharp-libvips-linux-arm64-1.0.2.tgz",
+            "version": "1.0.2"
         },
         "node_modules/@img/sharp-libvips-linux-s390x": {
             "cpu": [
                 "s390x"
             ],
             "engines": {
                 "glibc": ">=2.28",
                 "npm": ">=9.6.5",
                 "pnpm": ">=7.1.0",
                 "yarn": ">=3.2.0"
             },
             "funding": {
                 "url": "https://opencollective.com/libvips"
             },
-            "integrity": "sha512-3+rzfAR1YpMOeA2zZNp+aYEzGNWK4zF3+sdMxuCS3ey9HhDbJ66w6hDSHDMoap32DueFwhhs3vwooAB2MaK4XQ==",
+            "integrity": "sha512-cmhQ1J4qVhfmS6szYW7RT+gLJq9dH2i4maq+qyXayUSn9/3iY2ZeWpbAgSpSVbV2E1JUL2Gg7pwnYQ1h8rQIog==",
             "optional": true,
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@img/sharp-libvips-linux-s390x/-/sharp-libvips-linux-s390x-1.0.1.tgz",
-            "version": "1.0.1"
+            "resolved": "https://registry.npmjs.org/@img/sharp-libvips-linux-s390x/-/sharp-libvips-linux-s390x-1.0.2.tgz",
+            "version": "1.0.2"
         },
         "node_modules/@img/sharp-libvips-linux-x64": {
             "cpu": [
                 "x64"
             ],
             "engines": {
                 "glibc": ">=2.26",
                 "npm": ">=9.6.5",
                 "pnpm": ">=7.1.0",
                 "yarn": ">=3.2.0"
             },
             "funding": {
                 "url": "https://opencollective.com/libvips"
             },
-            "integrity": "sha512-3NR1mxFsaSgMMzz1bAnnKbSAI+lHXVTqAHgc1bgzjHuXjo4hlscpUxc0vFSAPKI3yuzdzcZOkq7nDPrP2F8Jgw==",
+            "integrity": "sha512-E441q4Qdb+7yuyiADVi5J+44x8ctlrqn8XgkDTwr4qPJzWkaHwD489iZ4nGDgcuya4iMN3ULV6NwbhRZJ9Z7SQ==",
             "optional": true,
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@img/sharp-libvips-linux-x64/-/sharp-libvips-linux-x64-1.0.1.tgz",
-            "version": "1.0.1"
+            "resolved": "https://registry.npmjs.org/@img/sharp-libvips-linux-x64/-/sharp-libvips-linux-x64-1.0.2.tgz",
+            "version": "1.0.2"
         },
         "node_modules/@img/sharp-libvips-linuxmusl-arm64": {
             "cpu": [
                 "arm64"
             ],
             "engines": {
                 "musl": ">=1.2.2",
                 "npm": ">=9.6.5",
                 "pnpm": ">=7.1.0",
                 "yarn": ">=3.2.0"
             },
             "funding": {
                 "url": "https://opencollective.com/libvips"
             },
-            "integrity": "sha512-5aBRcjHDG/T6jwC3Edl3lP8nl9U2Yo8+oTl5drd1dh9Z1EBfzUKAJFUDTDisDjUwc7N4AjnPGfCA3jl3hY8uDg==",
+            "integrity": "sha512-3CAkndNpYUrlDqkCM5qhksfE+qSIREVpyoeHIU6jd48SJZViAmznoQQLAv4hVXF7xyUB9zf+G++e2v1ABjCbEQ==",
             "optional": true,
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@img/sharp-libvips-linuxmusl-arm64/-/sharp-libvips-linuxmusl-arm64-1.0.1.tgz",
-            "version": "1.0.1"
+            "resolved": "https://registry.npmjs.org/@img/sharp-libvips-linuxmusl-arm64/-/sharp-libvips-linuxmusl-arm64-1.0.2.tgz",
+            "version": "1.0.2"
         },
         "node_modules/@img/sharp-libvips-linuxmusl-x64": {
             "cpu": [
                 "x64"
             ],
             "engines": {
                 "musl": ">=1.2.2",
                 "npm": ">=9.6.5",
                 "pnpm": ">=7.1.0",
                 "yarn": ">=3.2.0"
             },
             "funding": {
                 "url": "https://opencollective.com/libvips"
             },
-            "integrity": "sha512-dcT7inI9DBFK6ovfeWRe3hG30h51cBAP5JXlZfx6pzc/Mnf9HFCQDLtYf4MCBjxaaTfjCCjkBxcy3XzOAo5txw==",
+            "integrity": "sha512-VI94Q6khIHqHWNOh6LLdm9s2Ry4zdjWJwH56WoiJU7NTeDwyApdZZ8c+SADC8OH98KWNQXnE01UdJ9CSfZvwZw==",
             "optional": true,
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@img/sharp-libvips-linuxmusl-x64/-/sharp-libvips-linuxmusl-x64-1.0.1.tgz",
-            "version": "1.0.1"
+            "resolved": "https://registry.npmjs.org/@img/sharp-libvips-linuxmusl-x64/-/sharp-libvips-linuxmusl-x64-1.0.2.tgz",
+            "version": "1.0.2"
         },
         "node_modules/@img/sharp-linux-arm": {
             "cpu": [
                 "arm"
             ],
             "engines": {
                 "glibc": ">=2.28",
@@ -598,24 +598,24 @@
                 "npm": ">=9.6.5",
                 "pnpm": ">=7.1.0",
                 "yarn": ">=3.2.0"
             },
             "funding": {
                 "url": "https://opencollective.com/libvips"
             },
-            "integrity": "sha512-Fndk/4Zq3vAc4G/qyfXASbS3HBZbKrlnKZLEJzPLrXoJuipFNNwTes71+Ki1hwYW5lch26niRYoZFAtZVf3EGA==",
+            "integrity": "sha512-RUgBD1c0+gCYZGCCe6mMdTiOFS0Zc/XrN0fYd6hISIKcDUbAW5NtSQW9g/powkrXYm6Vzwd6y+fqmExDuCdHNQ==",
             "optional": true,
             "optionalDependencies": {
-                "@img/sharp-libvips-linux-arm": "1.0.1"
+                "@img/sharp-libvips-linux-arm": "1.0.2"
             },
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@img/sharp-linux-arm/-/sharp-linux-arm-0.33.2.tgz",
-            "version": "0.33.2"
+            "resolved": "https://registry.npmjs.org/@img/sharp-linux-arm/-/sharp-linux-arm-0.33.4.tgz",
+            "version": "0.33.4"
         },
         "node_modules/@img/sharp-linux-arm64": {
             "cpu": [
                 "arm64"
             ],
             "engines": {
                 "glibc": ">=2.26",
@@ -623,49 +623,49 @@
                 "npm": ">=9.6.5",
                 "pnpm": ">=7.1.0",
                 "yarn": ">=3.2.0"
             },
             "funding": {
                 "url": "https://opencollective.com/libvips"
             },
-            "integrity": "sha512-pz0NNo882vVfqJ0yNInuG9YH71smP4gRSdeL09ukC2YLE6ZyZePAlWKEHgAzJGTiOh8Qkaov6mMIMlEhmLdKew==",
+            "integrity": "sha512-2800clwVg1ZQtxwSoTlHvtm9ObgAax7V6MTAB/hDT945Tfyy3hVkmiHpeLPCKYqYR1Gcmv1uDZ3a4OFwkdBL7Q==",
             "optional": true,
             "optionalDependencies": {
-                "@img/sharp-libvips-linux-arm64": "1.0.1"
+                "@img/sharp-libvips-linux-arm64": "1.0.2"
             },
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@img/sharp-linux-arm64/-/sharp-linux-arm64-0.33.2.tgz",
-            "version": "0.33.2"
+            "resolved": "https://registry.npmjs.org/@img/sharp-linux-arm64/-/sharp-linux-arm64-0.33.4.tgz",
+            "version": "0.33.4"
         },
         "node_modules/@img/sharp-linux-s390x": {
             "cpu": [
                 "s390x"
             ],
             "engines": {
-                "glibc": ">=2.28",
+                "glibc": ">=2.31",
                 "node": "^18.17.0 || ^20.3.0 || >=21.0.0",
                 "npm": ">=9.6.5",
                 "pnpm": ">=7.1.0",
                 "yarn": ">=3.2.0"
             },
             "funding": {
                 "url": "https://opencollective.com/libvips"
             },
-            "integrity": "sha512-MBoInDXDppMfhSzbMmOQtGfloVAflS2rP1qPcUIiITMi36Mm5YR7r0ASND99razjQUpHTzjrU1flO76hKvP5RA==",
+            "integrity": "sha512-h3RAL3siQoyzSoH36tUeS0PDmb5wINKGYzcLB5C6DIiAn2F3udeFAum+gj8IbA/82+8RGCTn7XW8WTFnqag4tQ==",
             "optional": true,
             "optionalDependencies": {
-                "@img/sharp-libvips-linux-s390x": "1.0.1"
+                "@img/sharp-libvips-linux-s390x": "1.0.2"
             },
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@img/sharp-linux-s390x/-/sharp-linux-s390x-0.33.2.tgz",
-            "version": "0.33.2"
+            "resolved": "https://registry.npmjs.org/@img/sharp-linux-s390x/-/sharp-linux-s390x-0.33.4.tgz",
+            "version": "0.33.4"
         },
         "node_modules/@img/sharp-linux-x64": {
             "cpu": [
                 "x64"
             ],
             "engines": {
                 "glibc": ">=2.26",
@@ -673,24 +673,24 @@
                 "npm": ">=9.6.5",
                 "pnpm": ">=7.1.0",
                 "yarn": ">=3.2.0"
             },
             "funding": {
                 "url": "https://opencollective.com/libvips"
             },
-            "integrity": "sha512-xUT82H5IbXewKkeF5aiooajoO1tQV4PnKfS/OZtb5DDdxS/FCI/uXTVZ35GQ97RZXsycojz/AJ0asoz6p2/H/A==",
+            "integrity": "sha512-GoR++s0XW9DGVi8SUGQ/U4AeIzLdNjHka6jidVwapQ/JebGVQIpi52OdyxCNVRE++n1FCLzjDovJNozif7w/Aw==",
             "optional": true,
             "optionalDependencies": {
-                "@img/sharp-libvips-linux-x64": "1.0.1"
+                "@img/sharp-libvips-linux-x64": "1.0.2"
             },
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@img/sharp-linux-x64/-/sharp-linux-x64-0.33.2.tgz",
-            "version": "0.33.2"
+            "resolved": "https://registry.npmjs.org/@img/sharp-linux-x64/-/sharp-linux-x64-0.33.4.tgz",
+            "version": "0.33.4"
         },
         "node_modules/@img/sharp-linuxmusl-arm64": {
             "cpu": [
                 "arm64"
             ],
             "engines": {
                 "musl": ">=1.2.2",
@@ -698,24 +698,24 @@
                 "npm": ">=9.6.5",
                 "pnpm": ">=7.1.0",
                 "yarn": ">=3.2.0"
             },
             "funding": {
                 "url": "https://opencollective.com/libvips"
             },
-            "integrity": "sha512-F+0z8JCu/UnMzg8IYW1TMeiViIWBVg7IWP6nE0p5S5EPQxlLd76c8jYemG21X99UzFwgkRo5yz2DS+zbrnxZeA==",
+            "integrity": "sha512-nhr1yC3BlVrKDTl6cO12gTpXMl4ITBUZieehFvMntlCXFzH2bvKG76tBL2Y/OqhupZt81pR7R+Q5YhJxW0rGgQ==",
             "optional": true,
             "optionalDependencies": {
-                "@img/sharp-libvips-linuxmusl-arm64": "1.0.1"
+                "@img/sharp-libvips-linuxmusl-arm64": "1.0.2"
             },
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@img/sharp-linuxmusl-arm64/-/sharp-linuxmusl-arm64-0.33.2.tgz",
-            "version": "0.33.2"
+            "resolved": "https://registry.npmjs.org/@img/sharp-linuxmusl-arm64/-/sharp-linuxmusl-arm64-0.33.4.tgz",
+            "version": "0.33.4"
         },
         "node_modules/@img/sharp-linuxmusl-x64": {
             "cpu": [
                 "x64"
             ],
             "engines": {
                 "musl": ">=1.2.2",
@@ -723,87 +723,87 @@
                 "npm": ">=9.6.5",
                 "pnpm": ">=7.1.0",
                 "yarn": ">=3.2.0"
             },
             "funding": {
                 "url": "https://opencollective.com/libvips"
             },
-            "integrity": "sha512-+ZLE3SQmSL+Fn1gmSaM8uFusW5Y3J9VOf+wMGNnTtJUMUxFhv+P4UPaYEYT8tqnyYVaOVGgMN/zsOxn9pSsO2A==",
+            "integrity": "sha512-uCPTku0zwqDmZEOi4ILyGdmW76tH7dm8kKlOIV1XC5cLyJ71ENAAqarOHQh0RLfpIpbV5KOpXzdU6XkJtS0daw==",
             "optional": true,
             "optionalDependencies": {
-                "@img/sharp-libvips-linuxmusl-x64": "1.0.1"
+                "@img/sharp-libvips-linuxmusl-x64": "1.0.2"
             },
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@img/sharp-linuxmusl-x64/-/sharp-linuxmusl-x64-0.33.2.tgz",
-            "version": "0.33.2"
+            "resolved": "https://registry.npmjs.org/@img/sharp-linuxmusl-x64/-/sharp-linuxmusl-x64-0.33.4.tgz",
+            "version": "0.33.4"
         },
         "node_modules/@img/sharp-wasm32": {
             "cpu": [
                 "wasm32"
             ],
             "dependencies": {
-                "@emnapi/runtime": "^0.45.0"
+                "@emnapi/runtime": "^1.1.1"
             },
             "engines": {
                 "node": "^18.17.0 || ^20.3.0 || >=21.0.0",
                 "npm": ">=9.6.5",
                 "pnpm": ">=7.1.0",
                 "yarn": ">=3.2.0"
             },
             "funding": {
                 "url": "https://opencollective.com/libvips"
             },
-            "integrity": "sha512-fLbTaESVKuQcpm8ffgBD7jLb/CQLcATju/jxtTXR1XCLwbOQt+OL5zPHSDMmp2JZIeq82e18yE0Vv7zh6+6BfQ==",
+            "integrity": "sha512-Bmmauh4sXUsUqkleQahpdNXKvo+wa1V9KhT2pDA4VJGKwnKMJXiSTGphn0gnJrlooda0QxCtXc6RX1XAU6hMnQ==",
             "optional": true,
-            "resolved": "https://registry.npmjs.org/@img/sharp-wasm32/-/sharp-wasm32-0.33.2.tgz",
-            "version": "0.33.2"
+            "resolved": "https://registry.npmjs.org/@img/sharp-wasm32/-/sharp-wasm32-0.33.4.tgz",
+            "version": "0.33.4"
         },
         "node_modules/@img/sharp-win32-ia32": {
             "cpu": [
                 "ia32"
             ],
             "engines": {
                 "node": "^18.17.0 || ^20.3.0 || >=21.0.0",
                 "npm": ">=9.6.5",
                 "pnpm": ">=7.1.0",
                 "yarn": ">=3.2.0"
             },
             "funding": {
                 "url": "https://opencollective.com/libvips"
             },
-            "integrity": "sha512-okBpql96hIGuZ4lN3+nsAjGeggxKm7hIRu9zyec0lnfB8E7Z6p95BuRZzDDXZOl2e8UmR4RhYt631i7mfmKU8g==",
+            "integrity": "sha512-99SJ91XzUhYHbx7uhK3+9Lf7+LjwMGQZMDlO/E/YVJ7Nc3lyDFZPGhjwiYdctoH2BOzW9+TnfqcaMKt0jHLdqw==",
             "optional": true,
             "os": [
                 "win32"
             ],
-            "resolved": "https://registry.npmjs.org/@img/sharp-win32-ia32/-/sharp-win32-ia32-0.33.2.tgz",
-            "version": "0.33.2"
+            "resolved": "https://registry.npmjs.org/@img/sharp-win32-ia32/-/sharp-win32-ia32-0.33.4.tgz",
+            "version": "0.33.4"
         },
         "node_modules/@img/sharp-win32-x64": {
             "cpu": [
                 "x64"
             ],
             "engines": {
                 "node": "^18.17.0 || ^20.3.0 || >=21.0.0",
                 "npm": ">=9.6.5",
                 "pnpm": ">=7.1.0",
                 "yarn": ">=3.2.0"
             },
             "funding": {
                 "url": "https://opencollective.com/libvips"
             },
-            "integrity": "sha512-E4magOks77DK47FwHUIGH0RYWSgRBfGdK56kIHSVeB9uIS4pPFr4N2kIVsXdQQo4LzOsENKV5KAhRlRL7eMAdg==",
+            "integrity": "sha512-3QLocdTRVIrFNye5YocZl+KKpYKP+fksi1QhmOArgx7GyhIbQp/WrJRu176jm8IxromS7RIkzMiMINVdBtC8Aw==",
             "optional": true,
             "os": [
                 "win32"
             ],
-            "resolved": "https://registry.npmjs.org/@img/sharp-win32-x64/-/sharp-win32-x64-0.33.2.tgz",
-            "version": "0.33.2"
+            "resolved": "https://registry.npmjs.org/@img/sharp-win32-x64/-/sharp-win32-x64-0.33.4.tgz",
+            "version": "0.33.4"
         },
         "node_modules/@popperjs/core": {
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/popperjs"
             },
             "integrity": "sha512-P1st0aksCrn9sGZhp8GMYwBnQsbvAWsZAX44oXNNvLHGqAOcoVxmjZiohstwQ7SqKnbR47akdNi+uleWD8+g6A==",
@@ -888,17 +888,20 @@
             "resolved": "https://registry.npmjs.org/base64-js/-/base64-js-1.5.1.tgz",
             "version": "1.5.1"
         },
         "node_modules/binary-extensions": {
             "engines": {
                 "node": ">=8"
             },
-            "integrity": "sha512-jDctJ/IVQbZoJykoeHbhXpOlNBqGNcwXJKJog42E5HDPUwQTSdjCHdihjj0DlnheQ7blbT6dHOafNAiS8ooQKA==",
-            "resolved": "https://registry.npmjs.org/binary-extensions/-/binary-extensions-2.2.0.tgz",
-            "version": "2.2.0"
+            "funding": {
+                "url": "https://github.com/sponsors/sindresorhus"
+            },
+            "integrity": "sha512-Ceh+7ox5qe7LJuLHoY0feh3pHuUDHAcRUeyL2VYghZwfpkNIy/+8Ocg0a3UuSoYzavmylwuLWQOf3hl0jjMMIw==",
+            "resolved": "https://registry.npmjs.org/binary-extensions/-/binary-extensions-2.3.0.tgz",
+            "version": "2.3.0"
         },
         "node_modules/body-parser": {
             "dependencies": {
                 "bytes": "3.1.2",
                 "content-type": "~1.0.5",
                 "debug": "2.6.9",
                 "depd": "2.0.0",
@@ -1231,17 +1234,17 @@
             "resolved": "https://registry.npmjs.org/content-type/-/content-type-1.0.5.tgz",
             "version": "1.0.5"
         },
         "node_modules/cookie": {
             "engines": {
                 "node": ">= 0.6"
             },
-            "integrity": "sha512-YZ3GUyn/o8gfKJlnlX7g7xq4gyO6OSuhGPKaaGssGB2qgDUS0gPgtTvoyZLTt9Ab6dC4hfc9dV5arkvc/OCmrw==",
-            "resolved": "https://registry.npmjs.org/cookie/-/cookie-0.5.0.tgz",
-            "version": "0.5.0"
+            "integrity": "sha512-U71cyTamuh1CRNCfpGY6to28lxvNwPG4Guz/EVjgf3Jmzv0vlDp1atT9eS5dDjMYHucpHbWns6Lwf3BKz6svdw==",
+            "resolved": "https://registry.npmjs.org/cookie/-/cookie-0.6.0.tgz",
+            "version": "0.6.0"
         },
         "node_modules/cookie-signature": {
             "integrity": "sha512-QADzlaHc8icV8I7vbaJXJwod9HWYp8uCqf1xa4OfNu1T7JVxQIrUgOWtHdNDtPiywmFbiS12VjotIXLrKM3orQ==",
             "resolved": "https://registry.npmjs.org/cookie-signature/-/cookie-signature-1.0.6.tgz",
             "version": "1.0.6"
         },
         "node_modules/css-select": {
@@ -1316,17 +1319,17 @@
             "resolved": "https://registry.npmjs.org/destroy/-/destroy-1.2.0.tgz",
             "version": "1.2.0"
         },
         "node_modules/detect-libc": {
             "engines": {
                 "node": ">=8"
             },
-            "integrity": "sha512-UX6sGumvvqSaXgdKGUsgZWqcUyIXZ/vZTrlRT/iobiKhGL0zL4d3osHj3uqllWJK+i+sixDS/3COVEOFbupFyw==",
-            "resolved": "https://registry.npmjs.org/detect-libc/-/detect-libc-2.0.2.tgz",
-            "version": "2.0.2"
+            "integrity": "sha512-bwy0MGW55bG41VqxxypOsdSdGqLwXPI/focwgTYCFMbdUiBAxLg9CFzG08sz2aqzknwiX7Hkl0bQENjg8iLByw==",
+            "resolved": "https://registry.npmjs.org/detect-libc/-/detect-libc-2.0.3.tgz",
+            "version": "2.0.3"
         },
         "node_modules/dfa": {
             "integrity": "sha512-ED3jP8saaweFTjeGX8HQPjeC1YYyZs98jGNZx6IiBvxW7JG5v492kamAQB3m2wop07CvU/RQmzcKr6bgcC5D/Q==",
             "resolved": "https://registry.npmjs.org/dfa/-/dfa-1.2.0.tgz",
             "version": "1.2.0"
         },
         "node_modules/dom-serializer": {
@@ -1477,15 +1480,15 @@
         "node_modules/express": {
             "dependencies": {
                 "accepts": "~1.3.8",
                 "array-flatten": "1.1.1",
                 "body-parser": "1.20.2",
                 "content-disposition": "0.5.4",
                 "content-type": "~1.0.4",
-                "cookie": "0.5.0",
+                "cookie": "0.6.0",
                 "cookie-signature": "1.0.6",
                 "debug": "2.6.9",
                 "depd": "2.0.0",
                 "encodeurl": "~1.0.2",
                 "escape-html": "~1.0.3",
                 "etag": "~1.8.1",
                 "finalhandler": "1.2.0",
@@ -1507,17 +1510,17 @@
                 "type-is": "~1.6.18",
                 "utils-merge": "1.0.1",
                 "vary": "~1.1.2"
             },
             "engines": {
                 "node": ">= 0.10.0"
             },
-            "integrity": "sha512-6VyCijWQ+9O7WuVMTRBTl+cjNNIzD5cY5mQ1WM8r/LEkI2u8EYpOotESNwzNlyCn3g+dmjKYI6BmNneSr/FSRw==",
-            "resolved": "https://registry.npmjs.org/express/-/express-4.18.3.tgz",
-            "version": "4.18.3"
+            "integrity": "sha512-5T6nhjsT+EOMzuck8JjBHARTHfMht0POzlA60WV2pMD3gyXw2LZnZ+ueGdNxG+0calOJcWKbpFcuzLZ91YWq9Q==",
+            "resolved": "https://registry.npmjs.org/express/-/express-4.19.2.tgz",
+            "version": "4.19.2"
         },
         "node_modules/fast-deep-equal": {
             "integrity": "sha512-f3qQ9oQy9j2AhBe/H9VC91wLmKBCCU/gDOnKNAYG5hswO7BLKj09Hc5HYNz9cGI++xlpDCIgDaitVs03ATR84Q==",
             "resolved": "https://registry.npmjs.org/fast-deep-equal/-/fast-deep-equal-3.1.3.tgz",
             "version": "3.1.3"
         },
         "node_modules/fecha": {
@@ -1723,17 +1726,17 @@
         "node_modules/hasown": {
             "dependencies": {
                 "function-bind": "^1.1.2"
             },
             "engines": {
                 "node": ">= 0.4"
             },
-            "integrity": "sha512-1/th4MHjnwncwXsIW6QMzlvYL9kG5e/CpVvLRZe4XPa8TOUNbCELqmvhDmnkNsAjwaG4+I8gJJL0JBvTTLO9qA==",
-            "resolved": "https://registry.npmjs.org/hasown/-/hasown-2.0.1.tgz",
-            "version": "2.0.1"
+            "integrity": "sha512-0hJU9SCPvmMzIBdZFqNPXWa6dqh7WdH0cII9y+CyS8rG3nL48Bclra9HmKhVVUHyPWNH5Y7xDwAB7bfgSjkUMQ==",
+            "resolved": "https://registry.npmjs.org/hasown/-/hasown-2.0.2.tgz",
+            "version": "2.0.2"
         },
         "node_modules/hsluv": {
             "integrity": "sha512-08iL2VyCRbkQKBySkSh6m8zMUa3sADAxGVWs3Z1aPcUkTJeK0ETG4Fc27tEmQBGUAXZjIsXOZqBvacuVNSC/fQ==",
             "resolved": "https://registry.npmjs.org/hsluv/-/hsluv-0.0.3.tgz",
             "version": "0.0.3"
         },
         "node_modules/htmlparser2": {
@@ -1777,17 +1780,17 @@
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-v3MXnZAcvnywkTUEZomIActle7RXXeedOR31wwl7VlyoXO4Qi9arvSenNQWne1TcRwhCL1HwLI21bEqdpj8/rA==",
             "resolved": "https://registry.npmjs.org/iconv-lite/-/iconv-lite-0.4.24.tgz",
             "version": "0.4.24"
         },
         "node_modules/immutable": {
-            "integrity": "sha512-8eabxkth9gZatlwl5TBuJnCsoTADlL6ftEr7A4qgdaTsPyreilDSnUk57SO+jfKcNtxPa22U5KK6DSeAYhpBJw==",
-            "resolved": "https://registry.npmjs.org/immutable/-/immutable-4.3.5.tgz",
-            "version": "4.3.5"
+            "integrity": "sha512-Ju0+lEMyzMVZarkTn/gqRpdqd5dOPaz1mCZ0SH3JV6iFw81PldE/PEB1hWVEA288HPt4WXW8O7AWxB10M+03QQ==",
+            "resolved": "https://registry.npmjs.org/immutable/-/immutable-4.3.6.tgz",
+            "version": "4.3.6"
         },
         "node_modules/inflight": {
             "dependencies": {
                 "once": "^1.3.0",
                 "wrappy": "1"
             },
             "integrity": "sha512-k92I/b08q4wvFscXCLvqfsHCrjrF7yiXsQuIVvVE7N82W3+aqpzuUdBbfhWcy/FZR3/4IgflMgKLOsvPDrGCJA==",
@@ -1908,25 +1911,14 @@
             "version": "2.6.0"
         },
         "node_modules/logform/node_modules/ms": {
             "integrity": "sha512-6FlzubTLZG3J2a/NVCAleEhjzq5oxgHyaCU9yYXvcLsvoVaHJq/s5xXI6/XXP6tz7R9xAOtHnSO/tXtF3WRTlA==",
             "resolved": "https://registry.npmjs.org/ms/-/ms-2.1.3.tgz",
             "version": "2.1.3"
         },
-        "node_modules/lru-cache": {
-            "dependencies": {
-                "yallist": "^4.0.0"
-            },
-            "engines": {
-                "node": ">=10"
-            },
-            "integrity": "sha512-Jo6dJ04CmSjuznwJSS3pUeWmd/H0ffTlkXXgwZi+eq1UCmqQwCh+eLsYOYCwY991i2Fah4h1BEMCx4qThGbsiA==",
-            "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-6.0.0.tgz",
-            "version": "6.0.0"
-        },
         "node_modules/media-typer": {
             "engines": {
                 "node": ">= 0.6"
             },
             "integrity": "sha512-dq+qelQ9akHpcOl/gUVRTxVIOkAJ1wR3QAvb4RsVjS8oVoFjDGTc679wJYmUmknUF5HwMLOgb5O+a3KxfWapPQ==",
             "resolved": "https://registry.npmjs.org/media-typer/-/media-typer-0.3.0.tgz",
             "version": "0.3.0"
@@ -2234,17 +2226,17 @@
                 "node": ">=8.10.0"
             },
             "integrity": "sha512-hOS089on8RduqdbhvQ5Z37A0ESjsqz6qnRcffsMU3495FuTdqSm+7bhJ29JvIOsBDEEnan5DPu9t3To9VRlMzA==",
             "resolved": "https://registry.npmjs.org/readdirp/-/readdirp-3.6.0.tgz",
             "version": "3.6.0"
         },
         "node_modules/restructure": {
-            "integrity": "sha512-Xj8/MEIhhfj9X2rmD9iJ4Gga9EFqVlpMj3vfLnV2r/Mh5jRMryNV+6lWh9GdJtDBcBSPIqzRdfBQ3wDtNFv/uw==",
-            "resolved": "https://registry.npmjs.org/restructure/-/restructure-3.0.0.tgz",
-            "version": "3.0.0"
+            "integrity": "sha512-6neDpI/yE9eogQo22qmWwKIA9wFPRyYjQleDEh6zaNAf2ZPqLJYUvNBJBWEWNoBlCeQMQkvIOe2YI/K2GOag+g==",
+            "resolved": "https://registry.npmjs.org/restructure/-/restructure-3.0.1.tgz",
+            "version": "3.0.1"
         },
         "node_modules/rimraf": {
             "bin": {
                 "rimraf": "bin.js"
             },
             "dependencies": {
                 "glob": "^7.1.3"
@@ -2346,31 +2338,28 @@
                 "chokidar": ">=3.0.0 <4.0.0",
                 "immutable": "^4.0.0",
                 "source-map-js": ">=0.6.2 <2.0.0"
             },
             "engines": {
                 "node": ">=14.0.0"
             },
-            "integrity": "sha512-wovtnV2PxzteLlfNzbgm1tFXPLoZILYAMJtvoXXkD7/+1uP41eKkIt1ypWq5/q2uT94qHjXehEYfmjKOvjL9sg==",
-            "resolved": "https://registry.npmjs.org/sass/-/sass-1.71.1.tgz",
-            "version": "1.71.1"
+            "integrity": "sha512-eb4GZt1C3avsX3heBNlrc7I09nyT00IUuo4eFhAbeXWU2fvA7oXI53SxODVAA+zgZCk9aunAZgO+losjR3fAwA==",
+            "resolved": "https://registry.npmjs.org/sass/-/sass-1.77.2.tgz",
+            "version": "1.77.2"
         },
         "node_modules/semver": {
             "bin": {
                 "semver": "bin/semver.js"
             },
-            "dependencies": {
-                "lru-cache": "^6.0.0"
-            },
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-EnwXhrlwXMk9gKu5/flx5sv/an57AkRplG3hTK68W7FRDN+k+OWBj65M7719OkA82XLBxrcX0KSHj+X5COhOVg==",
-            "resolved": "https://registry.npmjs.org/semver/-/semver-7.6.0.tgz",
-            "version": "7.6.0"
+            "integrity": "sha512-FNAIBWCx9qcRhoHcgcJ0gvU7SN1lYU2ZXuSfl04bSC5OpvDHFyJCjdNHomPXxjQlCBU67YW64PzY7/VIEH7F2w==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.6.2.tgz",
+            "version": "7.6.2"
         },
         "node_modules/send": {
             "dependencies": {
                 "debug": "2.6.9",
                 "depd": "2.0.0",
                 "destroy": "1.2.0",
                 "encodeurl": "~1.0.2",
@@ -2408,71 +2397,71 @@
             },
             "integrity": "sha512-XGuRDNjXUijsUL0vl6nSD7cwURuzEgglbOaFuZM9g3kwDXOWVTck0jLzjPzGD+TazWbboZYu52/9/XPdUgne9g==",
             "resolved": "https://registry.npmjs.org/serve-static/-/serve-static-1.15.0.tgz",
             "version": "1.15.0"
         },
         "node_modules/set-function-length": {
             "dependencies": {
-                "define-data-property": "^1.1.2",
+                "define-data-property": "^1.1.4",
                 "es-errors": "^1.3.0",
                 "function-bind": "^1.1.2",
-                "get-intrinsic": "^1.2.3",
+                "get-intrinsic": "^1.2.4",
                 "gopd": "^1.0.1",
-                "has-property-descriptors": "^1.0.1"
+                "has-property-descriptors": "^1.0.2"
             },
             "engines": {
                 "node": ">= 0.4"
             },
-            "integrity": "sha512-j4t6ccc+VsKwYHso+kElc5neZpjtq9EnRICFZtWyBsLojhmeF/ZBd/elqm22WJh/BziDe/SBiOeAt0m2mfLD0g==",
-            "resolved": "https://registry.npmjs.org/set-function-length/-/set-function-length-1.2.1.tgz",
-            "version": "1.2.1"
+            "integrity": "sha512-pgRc4hJ4/sNjWCSS9AmnS40x3bNMDTknHgL5UaMBTMyJnU90EgWh1Rz+MC9eFu4BuN/UwZjKQuY/1v3rM7HMfg==",
+            "resolved": "https://registry.npmjs.org/set-function-length/-/set-function-length-1.2.2.tgz",
+            "version": "1.2.2"
         },
         "node_modules/setprototypeof": {
             "integrity": "sha512-E5LDX7Wrp85Kil5bhZv46j8jOeboKq5JMmYM3gVGdGH8xFpPWXUMsNrlODCrkoxMEeNi/XZIwuRvY4XNwYMJpw==",
             "resolved": "https://registry.npmjs.org/setprototypeof/-/setprototypeof-1.2.0.tgz",
             "version": "1.2.0"
         },
         "node_modules/sharp": {
             "dependencies": {
                 "color": "^4.2.3",
-                "detect-libc": "^2.0.2",
-                "semver": "^7.5.4"
+                "detect-libc": "^2.0.3",
+                "semver": "^7.6.0"
             },
             "engines": {
-                "libvips": ">=8.15.1",
+                "libvips": ">=8.15.2",
                 "node": "^18.17.0 || ^20.3.0 || >=21.0.0"
             },
             "funding": {
                 "url": "https://opencollective.com/libvips"
             },
             "hasInstallScript": true,
-            "integrity": "sha512-WlYOPyyPDiiM07j/UO+E720ju6gtNtHjEGg5vovUk1Lgxyjm2LFO+37Nt/UI3MMh2l6hxTWQWi7qk3cXJTutcQ==",
+            "integrity": "sha512-7i/dt5kGl7qR4gwPRD2biwD2/SvBn3O04J77XKFgL2OnZtQw+AG9wnuS/csmu80nPRHLYE9E41fyEiG8nhH6/Q==",
             "optionalDependencies": {
-                "@img/sharp-darwin-arm64": "0.33.2",
-                "@img/sharp-darwin-x64": "0.33.2",
-                "@img/sharp-libvips-darwin-arm64": "1.0.1",
-                "@img/sharp-libvips-darwin-x64": "1.0.1",
-                "@img/sharp-libvips-linux-arm": "1.0.1",
-                "@img/sharp-libvips-linux-arm64": "1.0.1",
-                "@img/sharp-libvips-linux-s390x": "1.0.1",
-                "@img/sharp-libvips-linux-x64": "1.0.1",
-                "@img/sharp-libvips-linuxmusl-arm64": "1.0.1",
-                "@img/sharp-libvips-linuxmusl-x64": "1.0.1",
-                "@img/sharp-linux-arm": "0.33.2",
-                "@img/sharp-linux-arm64": "0.33.2",
-                "@img/sharp-linux-s390x": "0.33.2",
-                "@img/sharp-linux-x64": "0.33.2",
-                "@img/sharp-linuxmusl-arm64": "0.33.2",
-                "@img/sharp-linuxmusl-x64": "0.33.2",
-                "@img/sharp-wasm32": "0.33.2",
-                "@img/sharp-win32-ia32": "0.33.2",
-                "@img/sharp-win32-x64": "0.33.2"
+                "@img/sharp-darwin-arm64": "0.33.4",
+                "@img/sharp-darwin-x64": "0.33.4",
+                "@img/sharp-libvips-darwin-arm64": "1.0.2",
+                "@img/sharp-libvips-darwin-x64": "1.0.2",
+                "@img/sharp-libvips-linux-arm": "1.0.2",
+                "@img/sharp-libvips-linux-arm64": "1.0.2",
+                "@img/sharp-libvips-linux-s390x": "1.0.2",
+                "@img/sharp-libvips-linux-x64": "1.0.2",
+                "@img/sharp-libvips-linuxmusl-arm64": "1.0.2",
+                "@img/sharp-libvips-linuxmusl-x64": "1.0.2",
+                "@img/sharp-linux-arm": "0.33.4",
+                "@img/sharp-linux-arm64": "0.33.4",
+                "@img/sharp-linux-s390x": "0.33.4",
+                "@img/sharp-linux-x64": "0.33.4",
+                "@img/sharp-linuxmusl-arm64": "0.33.4",
+                "@img/sharp-linuxmusl-x64": "0.33.4",
+                "@img/sharp-wasm32": "0.33.4",
+                "@img/sharp-win32-ia32": "0.33.4",
+                "@img/sharp-win32-x64": "0.33.4"
             },
-            "resolved": "https://registry.npmjs.org/sharp/-/sharp-0.33.2.tgz",
-            "version": "0.33.2"
+            "resolved": "https://registry.npmjs.org/sharp/-/sharp-0.33.4.tgz",
+            "version": "0.33.4"
         },
         "node_modules/side-channel": {
             "dependencies": {
                 "call-bind": "^1.0.7",
                 "es-errors": "^1.3.0",
                 "get-intrinsic": "^1.2.4",
                 "object-inspect": "^1.13.1"
@@ -2495,17 +2484,17 @@
             "resolved": "https://registry.npmjs.org/simple-swizzle/-/simple-swizzle-0.2.2.tgz",
             "version": "0.2.2"
         },
         "node_modules/source-map-js": {
             "engines": {
                 "node": ">=0.10.0"
             },
-            "integrity": "sha512-R0XvVJ9WusLiqTCEiGCmICCMplcCkIwwR11mOSD9CR5u+IXYdiseeEuXCVAjS54zqwkLcPNnmU4OeJ6tUrWhDw==",
-            "resolved": "https://registry.npmjs.org/source-map-js/-/source-map-js-1.0.2.tgz",
-            "version": "1.0.2"
+            "integrity": "sha512-itJW8lvSA0TXEphiRoawsCksnlf8SyvmFzIhltqAHluXd88pkCd+cXJVHTDwdCr0IzwptSm035IHQktUu1QUMg==",
+            "resolved": "https://registry.npmjs.org/source-map-js/-/source-map-js-1.2.0.tgz",
+            "version": "1.2.0"
         },
         "node_modules/stack-trace": {
             "engines": {
                 "node": "*"
             },
             "integrity": "sha512-KGzahc7puUKkzyMt+IqAep+TVNbKP+k2Lmwhub39m1AsTSkaDutx56aDCo+HLDzf/D26BIHTJWNiTG1KAJiQCg==",
             "resolved": "https://registry.npmjs.org/stack-trace/-/stack-trace-0.0.10.tgz",
@@ -2636,22 +2625,22 @@
                 "is-stream": "^2.0.0",
                 "logform": "^2.4.0",
                 "one-time": "^1.0.0",
                 "readable-stream": "^3.4.0",
                 "safe-stable-stringify": "^2.3.1",
                 "stack-trace": "0.0.x",
                 "triple-beam": "^1.3.0",
-                "winston-transport": "^4.5.0"
+                "winston-transport": "^4.7.0"
             },
             "engines": {
                 "node": ">= 12.0.0"
             },
-            "integrity": "sha512-L3yR6/MzZAOl0DsysUXHVjOwv8mKZ71TrA/41EIduGpOOV5LQVodqN+QdQ6BS6PJ/RdIshZhq84P/fStEZkk7g==",
-            "resolved": "https://registry.npmjs.org/winston/-/winston-3.11.0.tgz",
-            "version": "3.11.0"
+            "integrity": "sha512-rwidmA1w3SE4j0E5MuIufFhyJPBDG7Nu71RkZor1p2+qHvJSZ9GYDA81AyleQcZbh/+V6HjeBdfnTZJm9rSeQQ==",
+            "resolved": "https://registry.npmjs.org/winston/-/winston-3.13.0.tgz",
+            "version": "3.13.0"
         },
         "node_modules/winston-daily-rotate-file": {
             "dependencies": {
                 "file-stream-rotator": "^0.6.1",
                 "object-hash": "^2.0.1",
                 "triple-beam": "^1.3.0",
                 "winston-transport": "^4.4.0"
@@ -2679,16 +2668,11 @@
             "resolved": "https://registry.npmjs.org/winston-transport/-/winston-transport-4.7.0.tgz",
             "version": "4.7.0"
         },
         "node_modules/wrappy": {
             "integrity": "sha512-l4Sp/DRseor9wL6EvV2+TuQn63dMkPjZ/sp9XkghTEbV9KlPS1xUsZ3u7/IQO4wxtcFB4bgpQPRcR3QCvezPcQ==",
             "resolved": "https://registry.npmjs.org/wrappy/-/wrappy-1.0.2.tgz",
             "version": "1.0.2"
-        },
-        "node_modules/yallist": {
-            "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
-            "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
-            "version": "4.0.0"
         }
     },
     "requires": true
 }
```

### Comparing `gramex-1.94.1/gramex/apps/ui/setup.js` & `gramex-1.94.2/gramex/apps/ui/setup.js`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/bootstrap5.scss` & `gramex-1.94.2/gramex/apps/ui/theme/bootstrap5.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/bootswatch/cerulean.png` & `gramex-1.94.2/gramex/apps/ui/theme/bootswatch/cerulean.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/bootswatch/cosmo.png` & `gramex-1.94.2/gramex/apps/ui/theme/bootswatch/cosmo.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/bootswatch/cyborg.png` & `gramex-1.94.2/gramex/apps/ui/theme/bootswatch/cyborg.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/bootswatch/darkly.png` & `gramex-1.94.2/gramex/apps/ui/theme/bootswatch/darkly.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/bootswatch/flatly.png` & `gramex-1.94.2/gramex/apps/ui/theme/bootswatch/flatly.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/bootswatch/journal.png` & `gramex-1.94.2/gramex/apps/ui/theme/bootswatch/journal.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/bootswatch/litera.png` & `gramex-1.94.2/gramex/apps/ui/theme/bootswatch/litera.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/bootswatch/lumen.png` & `gramex-1.94.2/gramex/apps/ui/theme/bootswatch/lumen.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/bootswatch/lux.png` & `gramex-1.94.2/gramex/apps/ui/theme/bootswatch/lux.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/bootswatch/materia.png` & `gramex-1.94.2/gramex/apps/ui/theme/bootswatch/materia.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/bootswatch/minty.png` & `gramex-1.94.2/gramex/apps/ui/theme/bootswatch/minty.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/bootswatch/pulse.png` & `gramex-1.94.2/gramex/apps/ui/theme/bootswatch/pulse.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/bootswatch/sandstone.png` & `gramex-1.94.2/gramex/apps/ui/theme/bootswatch/sandstone.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/bootswatch/simplex.png` & `gramex-1.94.2/gramex/apps/ui/theme/bootswatch/simplex.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/bootswatch/sketchy.png` & `gramex-1.94.2/gramex/apps/ui/theme/bootswatch/sketchy.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/bootswatch/slate.png` & `gramex-1.94.2/gramex/apps/ui/theme/bootswatch/slate.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/bootswatch/solar.png` & `gramex-1.94.2/gramex/apps/ui/theme/bootswatch/solar.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/bootswatch/spacelab.png` & `gramex-1.94.2/gramex/apps/ui/theme/bootswatch/spacelab.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/bootswatch/superhero.png` & `gramex-1.94.2/gramex/apps/ui/theme/bootswatch/superhero.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/bootswatch/united.png` & `gramex-1.94.2/gramex/apps/ui/theme/bootswatch/united.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/bootswatch/yeti.png` & `gramex-1.94.2/gramex/apps/ui/theme/bootswatch/yeti.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/default.png` & `gramex-1.94.2/gramex/apps/ui/theme/default.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/index.html` & `gramex-1.94.2/gramex/apps/ui/theme/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/sample.html` & `gramex-1.94.2/gramex/apps/ui/theme/sample.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/themes-guide/blue_voltage.png` & `gramex-1.94.2/gramex/apps/ui/theme/themes-guide/blue_voltage.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/themes-guide/blue_voltage.scss` & `gramex-1.94.2/gramex/apps/ui/theme/themes-guide/blue_voltage.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/themes-guide/boldstrap.png` & `gramex-1.94.2/gramex/apps/ui/theme/themes-guide/boldstrap.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/themes-guide/bootstrap_purple.png` & `gramex-1.94.2/gramex/apps/ui/theme/themes-guide/bootstrap_purple.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/themes-guide/darkster.png` & `gramex-1.94.2/gramex/apps/ui/theme/themes-guide/darkster.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/themes-guide/darkster.scss` & `gramex-1.94.2/gramex/apps/ui/theme/themes-guide/darkster.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/themes-guide/fresca.png` & `gramex-1.94.2/gramex/apps/ui/theme/themes-guide/fresca.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/themes-guide/greyson.png` & `gramex-1.94.2/gramex/apps/ui/theme/themes-guide/greyson.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/themes-guide/greyson.scss` & `gramex-1.94.2/gramex/apps/ui/theme/themes-guide/greyson.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/themes-guide/hello_kiddie.png` & `gramex-1.94.2/gramex/apps/ui/theme/themes-guide/hello_kiddie.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/themes-guide/hello_kiddie.scss` & `gramex-1.94.2/gramex/apps/ui/theme/themes-guide/hello_kiddie.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/themes-guide/herbie.png` & `gramex-1.94.2/gramex/apps/ui/theme/themes-guide/herbie.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/themes-guide/hootstrap.png` & `gramex-1.94.2/gramex/apps/ui/theme/themes-guide/hootstrap.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/themes-guide/lovey.png` & `gramex-1.94.2/gramex/apps/ui/theme/themes-guide/lovey.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/themes-guide/monotony.png` & `gramex-1.94.2/gramex/apps/ui/theme/themes-guide/monotony.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/themes-guide/poypull.png` & `gramex-1.94.2/gramex/apps/ui/theme/themes-guide/poypull.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/themes-guide/poypull.scss` & `gramex-1.94.2/gramex/apps/ui/theme/themes-guide/poypull.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/themes-guide/signal.png` & `gramex-1.94.2/gramex/apps/ui/theme/themes-guide/signal.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/themes-guide/signal.scss` & `gramex-1.94.2/gramex/apps/ui/theme/themes-guide/signal.scss`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/themes-guide/tequila.png` & `gramex-1.94.2/gramex/apps/ui/theme/themes-guide/tequila.png`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/ui/theme/themes.json` & `gramex-1.94.2/gramex/apps/ui/theme/themes.json`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/update/README.md` & `gramex-1.94.2/gramex/apps/update/README.md`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/update/gramex.yaml` & `gramex-1.94.2/gramex/apps/update/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/update/gramexupdate.py` & `gramex-1.94.2/gramex/apps/update/gramexupdate.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/apps/update/index.html` & `gramex-1.94.2/gramex/apps/update/index.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/cache.py` & `gramex-1.94.2/gramex/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 import os
 import pandas as pd
 import re
 import requests
 import sqlalchemy as sa
 
 # B404:import_subprocess only developers can access this, not users
-import subprocess  # nosec B404
+import subprocess  # noqa B404
 import sys
 import tempfile
 import time
 import tornado.ioloop
 import tornado.template
 from gramex.config import PathConfig
 from gramex.config import app_log, merge, used_kwargs, CustomJSONDecoder, CustomJSONEncoder
 from orderedattrdict import AttrDict
 from queue import Queue
 from threading import Thread
 from tornado.concurrent import Future
 from types import ModuleType
-from typing import Any, List, Tuple, Union, Dict, Callable, BinaryIO
+from typing import Optional, Any, List, Tuple, Union, Dict, Callable, BinaryIO
 from typing_extensions import Literal
 from urllib.parse import urlparse
 
 
 MILLISECOND = 0.001  # in seconds
 _opener_defaults = {
     'mode': 'r',
@@ -66,18 +66,18 @@
 
 
 atexit.register(_delete_temp_files)
 
 
 def open(
     path: str,
-    callback: Union[str, Callable] = None,
-    transform: Callable = None,
+    callback: Optional[Union[str, Callable]] = None,
+    transform: Optional[Callable] = None,
     rel: bool = False,
-    **kwargs: dict,
+    **kwargs,
 ) -> Any:
     '''Reads a file, processes it via a callback, caches the result and returns it.
 
     When called again, returns the cached result unless the file has updated.
 
     Examples:
         >>> gramex.cache.open('data.yaml')
@@ -213,20 +213,20 @@
     result = cached['data']
     return (result, reloaded) if _reload_status else result
 
 
 def read_excel(
     io: Union[str, BinaryIO],
     sheet_name: Union[str, int] = 0,
-    table: str = None,
-    name: str = None,
-    range: str = None,
-    links: Union[Dict[str, str], bool] = None,
+    table: Optional[str] = None,
+    name: Optional[str] = None,
+    range: Optional[str] = None,
+    links: Optional[Union[Dict[str, str], bool]] = None,
     header: Union[None, int, List[int]] = ...,
-    **kwargs: dict,
+    **kwargs,
 ) -> pd.DataFrame:
     '''Read data from an XLSX as a DataFrame using `openpyxl`.
 
     Examples:
         >>> gramex.cache.read_excel('data.xlsx', sheet_name='Sheet1')
         >>> gramex.cache.read_excel('data.xlsx', sheet_name=0)
         >>> gramex.cache.read_excel('data.xlsx', table='Table1')
@@ -570,15 +570,15 @@
     if urlparts.scheme not in {'http', 'https'}:  # url is a filepath
         if info:
             ext = os.path.splitext(url)[1]
             content_type = mimetypes.guess_type(url, strict=True)[0]
             return {'name': url, 'r': None, 'url': None, 'ext': ext, 'content_type': content_type}
         else:
             return url
-    r = requests.get(url, **kwargs)  # nosec B113 - timeout is controlled by kwargs
+    r = requests.get(url, **kwargs)  # noqa S113 - timeout is controlled by kwargs
     if 'Content-Type' in r.headers:
         content_type = r.headers['Content-Type'].split(';')[0]
         ext = mimetypes.guess_extension(content_type, strict=False)
     else:
         ext = os.path.splitext(urlparts.path)[1]
     with tempfile.NamedTemporaryFile(suffix=ext, delete=False) as handle:
         for chunk in r.iter_content(chunk_size=16384):
@@ -684,15 +684,15 @@
 
         # On UNIX, close all file descriptors except 0, 1, 2 before child
         # process is executed. I've no idea why. Copied from
         # http://stackoverflow.com/a/4896288/100904
         kwargs['close_fds'] = 'posix' in sys.builtin_module_names
 
         # B603:subprocess_without_shell_equals_true: only developers can access this, not users
-        self.proc = subprocess.Popen(args, **kwargs)  # nosec B603
+        self.proc = subprocess.Popen(args, **kwargs)  # noqa S603
         self.thread = {}  # Has the running threads
         self.future = {}  # Stores the futures indicating stream close
         self.loop = _get_current_ioloop()
 
         # Buffering has 2 modes. buffer_size='line' reads and writes line by line
         # buffer_size=<number> reads in byte chunks. Define the appropriate method
         if hasattr(buffer_size, 'lower') and 'line' in buffer_size.lower():
@@ -868,23 +868,23 @@
     kwargs['buffer_size'] = buffer_size
     # started is set if we actually call Subprocess as part of this function
     started = False
 
     # If process was never started, start it
     if key not in _daemons:
         # B404:import_subprocess only developers can access this, not users
-        started = _daemons[key] = Subprocess(args, **kwargs)  # nosec B404
+        started = _daemons[key] = Subprocess(args, **kwargs)  # noqa S404
 
     # Ensure that process is running. Restart if required
     proc = _daemons[key]
     restart = int(restart)
     while proc.proc.returncode is not None and restart > 0:
         restart -= 1
         # B404:import_subprocess only developers can access this, not users
-        proc = started = _daemons[key] = Subprocess(args, **kwargs)  # nosec B404
+        proc = started = _daemons[key] = Subprocess(args, **kwargs)  # noqa S404
     if proc.proc.returncode is not None:
         raise RuntimeError(f'Error {proc.proc.returncode} starting {arg_str}')
     if started:
         app_log.info(f'Started: {arg_str}')
 
     future = Future()
     # If process was started, wait until it has initialized. Else just return the proc
@@ -1328,15 +1328,15 @@
 
 @opener
 def _yaml(handle, **kwargs):
     import yaml
 
     kwargs.setdefault('Loader', yaml.SafeLoader)
     # B506:yaml_load we load safely using SafeLoader
-    return yaml.load(handle.read(), **kwargs)  # nosec B506
+    return yaml.load(handle.read(), **kwargs)  # noqa S506
 
 
 def _template(path, **kwargs):
     root, name = os.path.split(path)
     return tornado.template.Loader(root, **kwargs).load(name)
 
 
@@ -1445,28 +1445,28 @@
         # bandit security note: We use string substitution for DB and table names.
         # But these are validated via gramex.data._sql_safe, so we're fine.
         if dialect == 'mysql':
             # https://dev.mysql.com/doc/refman/8.0/en/information-schema-tables-table.html
             # Works only on MySQL 5.7 and above
             # B608:hardcoded_sql_expressions only used internally
             w = _wheres('table_schema', 'table_name', db, tables)
-            q = 'SELECT update_time FROM information_schema.tables WHERE ' + w  # nosec B608
+            q = 'SELECT update_time FROM information_schema.tables WHERE ' + w  # noqa S608
         elif dialect == 'snowflake':
             # https://docs.snowflake.com/en/sql-reference/info-schema/tables.html
             w = _wheres('table_schema', 'table_name', db, tables)
-            q = 'SELECT last_altered FROM information_schema.tables WHERE ' + w  # nosec B608
+            q = 'SELECT last_altered FROM information_schema.tables WHERE ' + w  # noqa S608
         elif dialect == 'mssql':
             # https://goo.gl/b4aL9m
             w = _wheres('database_id', 'object_id', db, tables, fn=['DB_ID', 'OBJECT_ID'])
-            q = 'SELECT last_user_update FROM sys.dm_db_index_usage_stats WHERE ' + w  # nosec B608
+            q = 'SELECT last_user_update FROM sys.dm_db_index_usage_stats WHERE ' + w  # noqa S608
         elif dialect == 'postgresql':
             # https://www.postgresql.org/docs/9.6/static/monitoring-stats.html
             w = _wheres('schemaname', 'relname', 'public', tables)
             q = (
-                'SELECT n_tup_ins, n_tup_upd, n_tup_del FROM pg_stat_all_tables '  # nosec B608
+                'SELECT n_tup_ins, n_tup_upd, n_tup_del FROM pg_stat_all_tables '  # noqa S608
                 + 'WHERE '
                 + w
             )
         elif dialect == 'sqlite':
             if not db:
                 raise KeyError(f'gramex.cache.query: does not support memory sqlite "{dialect}"')
             q = db
```

### Comparing `gramex-1.94.1/gramex/config.py` & `gramex-1.94.2/gramex/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,15 +283,15 @@
 
 _valid_key_chars = string.ascii_letters + string.digits
 
 
 def random_string(size, chars=_valid_key_chars):
     '''Return random string of length size using chars (which defaults to alphanumeric)'''
     # B311:random random() is safe since it's for non-cryptographic use
-    return ''.join(choice(chars) for index in range(size))  # nosec B311
+    return ''.join(choice(chars) for index in range(size))  # noqa S311
 
 
 class PathConfig(AttrDict):
     '''
     An `AttrDict` that is loaded from a path as a YAML file. For e.g.,
     `conf = PathConfig(path)` loads the YAML file at `path` as an AttrDict.
     `+conf` reloads the path if required.
@@ -557,15 +557,15 @@
             app_log.warning(f'Missing config: {path}')
             _warned_paths.add(path)
         return default
     app_log.debug(f'Loading config: {path}')
     with path.open(encoding='utf-8') as handle:
         try:
             # B506:yaml_load we use a safe loader
-            result = yaml.load(handle, Loader=ConfigYAMLLoader)  # nosec B506
+            result = yaml.load(handle, Loader=ConfigYAMLLoader)  # noqa S506
         except Exception:
             app_log.exception(f'Config error: {path}')
             return default
     if not isinstance(result, AttrDict):
         if result is not None:
             app_log.warning(f'Config is not a dict: {path}')
         return default
@@ -606,15 +606,15 @@
     frozen_vars = dict(variables)
     for key, _value, node in walk(result):
         if isinstance(key, str) and ' if ' in key:
             # Evaluate conditional
             base, expr = key.split(' if ', 2)
             try:
                 # B307:eval this is safe since `expr` is written by app developer
-                condition = eval(expr, globals(), frozen_vars)  # nosec B307
+                condition = eval(expr, globals(), frozen_vars)  # noqa S307
             except Exception:
                 condition = False
                 app_log.exception(f'Failed condition evaluation: {key}')
             if condition:
                 replace.append((node, key, base))
             else:
                 remove.append((node, key))
@@ -893,15 +893,15 @@
     if secrets_url and secrets_key:
         from urllib.request import urlopen
         from tornado.web import decode_signed_value
 
         app_log.info(f'Fetching remote secrets from {secrets_url}')
         # Load string from the URL -- but ignore comments. file:// URLs are fine too
         # B310:urllib_urlopen secrets can be local files or URLs
-        value = yaml.safe_load(urlopen(secrets_url))  # nosec B310
+        value = yaml.safe_load(urlopen(secrets_url))  # noqa S310
         value = decode_signed_value(secrets_key, '', value, max_age_days=max_age_days)
         result.update(loads(value.decode('utf-8')))
     # If SECRETS_IMPORT: is set, fetch secrets from those file(s) as well.
     # SECRETS_IMPORT: can be a file pattern, or a list/dict of file patterns
     secrets_import = result.pop('SECRETS_IMPORT', None)
     if secrets_import:
         # Create a list of file patterns to import from
```

### Comparing `gramex-1.94.1/gramex/data.py` & `gramex-1.94.2/gramex/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1196,22 +1196,23 @@
         app_log.info(f'alter() not required for schema-less DB {engine.driver}')
         return engine
     try:
         db_table = get_table(engine, table, extend_existing=True)
     except sa.exc.NoSuchTableError:
         # If the table's not in the DB, create it
         cols = []
+        table_kwargs = {"extend_existing": True}
         for name, row in columns.items():
             row = dict({'type': row} if isinstance(row, str) else row, name=name)
             col_type = row.get('type', 'text')
             if isinstance(col_type, str):
                 # Use eval() to handle direct types like INTEGER *and* expressions like VARCHAR(3)
                 # eval() is safe here since `col_type` is written by app developer
                 # B307:eval is safe here since `col_type` is written by app developer
-                row['type'] = eval(col_type.upper(), vars(sa.types))  # nosec B307
+                row['type'] = eval(col_type.upper(), vars(sa.types))  # noqa S307
             row['type_'] = row.pop('type')
             if 'default' in row:
                 from inspect import isclass
 
                 default = row.pop('default')
                 # default: can be a string like `'sa.func.now()'` or `'func.now()'`
                 if isinstance(default, dict):
@@ -1221,16 +1222,18 @@
                     )(**libs)
                 # default can be an SQLAlchemy function, e.g. sa.func.now()
                 elif isclass(default) and issubclass(default, sa.func.Function):
                     row['server_default'] = default
                 # default can also be a static value, e.g. `0`
                 else:
                     row['server_default'] = str(default)
+            if scheme in {'sqlite'} and row.get('autoincrement'):
+                table_kwargs['sqlite_autoincrement'] = True
             cols.append(sa.Column(**row))
-        sa.Table(table, _METADATA_CACHE[engine], *cols, extend_existing=True).create(engine)
+        sa.Table(table, _METADATA_CACHE[engine], *cols, **table_kwargs).create(engine)
     else:
         quote = engine.dialect.identifier_preparer.quote_identifier
         # If the table's already in the DB, add new columns. We can't change column types
         with engine.connect() as conn, conn.begin():
             for name, row in columns.items():
                 if name in db_table.columns:
                     continue
@@ -2072,15 +2075,15 @@
     columns: Dict[str, Union[str, dict]] = None,
     query: str = None,
     queryfile: str = None,
     **kwargs,
 ):
     table = _mongodb_collection(url, database, collection, **kwargs)
     result = table.insert_many([_mongodb_json(row) for row in rows.to_dict(orient='records')])
-    meta['inserted'] = [{'id': str(id) for id in result.inserted_ids}]  # noqa: B035
+    meta['inserted'] = [{'id': str(id) for id in result.inserted_ids}]  # noqa B035
     return len(result.inserted_ids)
 
 
 # InfluxDB Operations
 # ----------------------------------------
```

### Comparing `gramex-1.94.1/gramex/debug.py` & `gramex-1.94.2/gramex/debug.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/deploy.yaml` & `gramex-1.94.2/gramex/deploy.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/download.vega.js` & `gramex-1.94.2/gramex/download.vega.js`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/favicon.ico` & `gramex-1.94.2/gramex/favicon.ico`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/gramex.yaml` & `gramex-1.94.2/gramex/gramex.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/gramexfeatures.csv` & `gramex-1.94.2/gramex/gramexfeatures.csv`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/gramexsize.csv` & `gramex-1.94.2/gramex/gramexsize.csv`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 gramex.cache.SQLiteStore.*,app.session.type=sqlite,5
 gramex.cache.SQLiteStore.*,url.*.kwargs.store.type=sqlite,5
 gramex.cache.HDF5Store.*,app.session.type=hdf5,18
 gramex.cache.HDF5Store.*,url.*.kwargs.store.type=hdf5,18
 gramex.cache.JSONStore.*,app.session.type=json,15
 gramex.cache.JSONStore.*,url.*.kwargs.store.type=json,15
 gramex.config.*,*,158
-gramex.data.*,url.*.handler=FormHandler|FilterHandler|MLHandler|DriverHandler,347
+gramex.data.*,url.*.handler=FormHandler|FilterHandler|MLHandler|DriverHandler,348
 gramex.debug.*,TODO - if any PY code uses gramex.debug,32
 gramex.install.*,TODO - Gramex app installation & management,164
 gramex.license.*,TODO - Gramex enterprise license management,9
 gramex.migrate.*,url.*.handler=GoogleAuth|SimpleAuth|OAuth2|FacebookAuth|TwitterAuth|SAMLAuth|SAMLAuth2|LDAPAuth|DBAuth|IntegratedAuth|SMSAuth|EmailAuth,3
 gramex.ml.Classifier.*,url.*.handler=ModelHandler,15
 gramex.ml._conda_r_home,TODO - if any PY code uses gramex.ml.r,4
 gramex.ml.r,TODO - if any PY code uses gramex.ml.r,11
@@ -50,15 +50,14 @@
 gramex.winservice.*,TODO - if app is deployed on Windows server,22
 gramex.__init__.*,*,49
 gramex.apps.admin2.*,import.*.path=$GRAMEXAPPS/admin2/gramex.yaml,54
 gramex.apps.filemanager.*,import.*.path=$GRAMEXAPPS/filemanager/gramex.yaml,7
 gramex.apps.logviewer.*,import.*.path=$GRAMEXAPPS/logviewer/gramex.yaml,61
 gramex.apps.mail.*,import.*.path=$GRAMEXAPPS/mail/gramex.yaml,2
 gramex.apps.ui.*,import.*.path=$GRAMEXAPPS/ui/gramex.yaml,32
-gramex.apps.uifactory.*,import.*.path=$GRAMEXAPPS/uifactory/gramex.yaml,21
 gramex.apps.update.*,import.*.path=$GRAMEXAPPS/update/gramex.yaml,14
 gramex.handlers.authhandler.AuthHandler.*,url.*.handler=GoogleAuth|SimpleAuth|OAuth2|FacebookAuth|TwitterAuth|SAMLAuth|SAMLAuth2|LDAPAuth|DBAuth|IntegratedAuth|SMSAuth|EmailAuth,35
 gramex.handlers.authhandler.LogoutHandler.*,url.*.handler=LogoutHandler,4
 gramex.handlers.authhandler.GoogleAuth.*,url.*.handler=GoogleAuth,5
 gramex.handlers.authhandler.SimpleAuth.*,url.*.handler=SimpleAuth,5
 gramex.handlers.basehandler.BaseMixin.setup,url,2
 gramex.handlers.basehandler.BaseMixin.clear_special_keys,url,3
```

### Comparing `gramex-1.94.1/gramex/handlers/400.html` & `gramex-1.94.2/gramex/handlers/400.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/handlers/401.html` & `gramex-1.94.2/gramex/handlers/401.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/handlers/403.html` & `gramex-1.94.2/gramex/handlers/403.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/handlers/404.html` & `gramex-1.94.2/gramex/handlers/404.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/handlers/500.html` & `gramex-1.94.2/gramex/handlers/500.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/handlers/__init__.py` & `gramex-1.94.2/gramex/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/handlers/auth.recaptcha.template.html` & `gramex-1.94.2/gramex/handlers/auth.recaptcha.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/handlers/auth.template.html` & `gramex-1.94.2/gramex/handlers/auth.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/handlers/authhandler.py` & `gramex-1.94.2/gramex/handlers/authhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/handlers/basehandler.py` & `gramex-1.94.2/gramex/handlers/basehandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -783,15 +783,15 @@
                 self.add_header(name, value)
             else:
                 self.set_header(name, value)
                 headers_written.add(name)
 
     def debug_exception(self, typ, value, tb):
         super(BaseHandler, self).log_exception(typ, value, tb)
-        import pdb  # noqa: T100
+        import pdb  # noqa T100
 
         pdb.post_mortem(tb)
 
     def _write_custom_error(self, status_code, **kwargs):
         if status_code in self.error:
             try:
                 result = self.error[status_code]['function'](
```

### Comparing `gramex-1.94.1/gramex/handlers/capturehandler.py` & `gramex-1.94.2/gramex/handlers/capturehandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import psutil
 import requests
 import tornado.gen
 from orderedattrdict import AttrDict
 from threading import Thread, Lock
 
 # B404:import_subprocess only for JS compilation
-from subprocess import Popen, PIPE, STDOUT  # nosec B404
+from subprocess import Popen, PIPE, STDOUT  # noqa S404
 from urllib.parse import urlencode, urljoin
 from tornado.web import HTTPError
 from tornado.httpclient import AsyncHTTPClient
 from gramex.config import app_log, variables
 from gramex.cache import cache_key
 from gramex.http import OK, BAD_REQUEST, GATEWAY_TIMEOUT, BAD_GATEWAY, CLIENT_TIMEOUT
 from .basehandler import BaseHandler
@@ -131,15 +131,15 @@
             app_log.error(f'url: {self.url} timed out')
         except requests.ConnectionError:
             # Try starting the process again
             app_log.info(f'Starting {script} via {self.cmd}')
             self.close()
             # B603:subprocess_without_shell_equals_true is safe since self.cmd is taken from
             # the YAML configuration (from developers)
-            self.proc = Popen(shlex.split(self.cmd), stdout=PIPE, stderr=STDOUT)  # nosec B603
+            self.proc = Popen(shlex.split(self.cmd), stdout=PIPE, stderr=STDOUT)  # noqa S603
             self.proc.poll()
             atexit.register(self.close)
             # TODO: what if readline() does not return quickly?
             line = self.proc.stdout.readline().strip()
             if not self.first_line_re.search(line):
                 return app_log.error(f'cmd: {self.cmd} invalid. Returned "{line}"')
             app_log.info(f'Pinging {script} at {self.url}')
```

### Comparing `gramex-1.94.1/gramex/handlers/chatgpthandler.py` & `gramex-1.94.2/gramex/handlers/chatgpthandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/handlers/comichandler.py` & `gramex-1.94.2/gramex/handlers/comichandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/handlers/drivehandler.py` & `gramex-1.94.2/gramex/handlers/drivehandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             self.args[key] = self.args[key][:n]
         for i, upload in enumerate(uploads):
             file = os.path.basename(upload.get('filename', ''))
             ext = os.path.splitext(file)[1]
             path = slug.filename(file)
             # B311:random random() is safe since it's for non-cryptographic use
             while self.fs.exists(path):
-                randomletter = choice(digits + ascii_lowercase)  # nosec B311
+                randomletter = choice(digits + ascii_lowercase)  # noqa S311
                 path = os.path.splitext(path)[0] + randomletter + ext
             self.args['file'][i] = file
             self.args['ext'][i] = ext.lower()
             self.args['path'][i] = path
             self.args['size'][i] = len(upload['body'])
             self.args['date'][i] = int(time.time())
             # Guess MIME type from filename if it's unknown
```

### Comparing `gramex-1.94.1/gramex/handlers/filehandler.py` & `gramex-1.94.2/gramex/handlers/filehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/handlers/filehandler.template.html` & `gramex-1.94.2/gramex/handlers/filehandler.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/handlers/formhandler.py` & `gramex-1.94.2/gramex/handlers/formhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/handlers/functionhandler.py` & `gramex-1.94.2/gramex/handlers/functionhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/handlers/jsonhandler.py` & `gramex-1.94.2/gramex/handlers/jsonhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/handlers/messagehandler.py` & `gramex-1.94.2/gramex/handlers/messagehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/handlers/mlhandler.py` & `gramex-1.94.2/gramex/handlers/mlhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/handlers/modelhandler.py` & `gramex-1.94.2/gramex/handlers/modelhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/handlers/openapiconfig.yaml` & `gramex-1.94.2/gramex/handlers/openapiconfig.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/handlers/openapihandler.py` & `gramex-1.94.2/gramex/handlers/openapihandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/handlers/pptxhandler.py` & `gramex-1.94.2/gramex/handlers/pptxhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/handlers/processhandler.py` & `gramex-1.94.2/gramex/handlers/processhandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         for header_name, header_value in self.headers.items():
             self.set_header(header_name, header_value)
 
         proc = Subprocess(
             self.cmdargs,
             # NOTE: developer should sanitize args if shell=True
             # B604 any_other_function_with_shell_equals_true
-            shell=self.shell,  # nosec B604
+            shell=self.shell,  # noqa S604
             cwd=self.cwd,
             stream_stdout=self.stream_stdout,
             stream_stderr=self.stream_stderr,
             buffer_size=self.buffer_size,
         )
         yield proc.wait_for_exit()
         # Wait for process to finish
```

### Comparing `gramex-1.94.1/gramex/handlers/proxyhandler.py` & `gramex-1.94.2/gramex/handlers/proxyhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/handlers/queryhandler.template.html` & `gramex-1.94.2/gramex/handlers/queryhandler.template.html`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/handlers/socialhandler.py` & `gramex-1.94.2/gramex/handlers/socialhandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
         If after all of this, we don't have a token, raise an exception.
         '''
         info = self.session.get(self.user_info, {})
         token = self.kwargs.get(key, None)  # Get from config
         session_token = fetch(info, key, None)
         # B105:hardcoded_password_string: 'persist' is not a password
-        if token == 'persist':  # nosec B105
+        if token == 'persist':  # noqa S105
             token = self.read_store().get(key, None)  # If persist, use store
             if token is None and session_token:  # Or persist from session
                 self.write_store(info)
         if token is None:
             token = session_token  # Use session token
         if token is None:  # Ensure token is present
             raise HTTPError(BAD_REQUEST, f'token {key} missing')
```

### Comparing `gramex-1.94.1/gramex/handlers/uploadhandler.py` & `gramex-1.94.2/gramex/handlers/uploadhandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         return filemeta
 
     def deletefiles(self, handler):
         status = []
         for delete_key in self.keys.get('delete', []):
             for key in handler.args.get(delete_key, []):
                 stat = {'success': False, 'key': key}
-                if key in self.store.keys():  # noqa: SIM118 self.store is not iterable
+                if key in self.store.keys():  # noqa SIM118 self.store is not iterable
                     path = os.path.join(self.path, key)
                     if os.path.exists(path):
                         os.remove(path)
                         self.store.dump(key, None)
                         stat['success'] = True
                 status.append(stat)
         return status
```

### Comparing `gramex-1.94.1/gramex/handlers/websockethandler.py` & `gramex-1.94.2/gramex/handlers/websockethandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/http.py` & `gramex-1.94.2/gramex/http.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/install.py` & `gramex-1.94.2/gramex/install.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from pathlib import Path
 from collections import Counter
 
 from orderedattrdict import AttrDict
 from orderedattrdict.yamlutils import AttrDictYAMLLoader
 
 # B404:import_subprocess only developers can access this, not users
-from subprocess import Popen, check_output, CalledProcessError  # nosec B404
+from subprocess import Popen, check_output, CalledProcessError  # noqa S404
 from textwrap import dedent
 from tornado.template import Template
 from zipfile import ZipFile
 import gramex
 import gramex.license
 from gramex.config import ChainConfig, PathConfig, variables, app_log, slug
 
@@ -527,15 +527,15 @@
     import ast
     import fnmatch
     import mccabe
     import pandas as pd
     import re
 
     # B404:import_subprocess only used for internal Gramex scripts
-    from subprocess import check_output  # nosec B404
+    from subprocess import check_output  # noqa S404
 
     project_path = os.getcwd() if len(args) == 0 else args[0]
     project_yaml = _gramex_yaml_path(project_path, kwargs)
     if project_yaml is None:
         return
 
     def walk(node: dict, parents: tuple = ()):
@@ -568,15 +568,15 @@
             for node in visitor.graphs.values():
                 py_complexity += node.complexity()
 
     base = gramex.config.PathConfig(os.path.join(os.path.dirname(gramex.__file__), 'gramex.yaml'))
     try:
         app = gramex.config.PathConfig(project_yaml)
         conf = +gramex.config.ChainConfig([('base', base), ('app', app)])
-    except Exception as e:  # noqa: B902 capture load errors as a "feature"
+    except Exception as e:  # noqa B902 capture load errors as a "feature"
         app_log.exception(str(e))
         return
     yamlpaths = {'.'.join(key): val for key, val in walk(conf)}
     used = set()
     gramexsize = gramex.cache.open('gramexsize.csv', rel=True)
     for _index, gramex_code in gramexsize.iterrows():
         # TODO: fnmatch.filter() is the slowest part. Optimize it
@@ -590,15 +590,17 @@
                 if yamlpaths[key] in yaml_value.split('|'):
                     used.add(gramex_code['codepath'])
     gramex_complexity = gramexsize.set_index('codepath')['complexity'][list(used)].sum()
 
     # Calculate JS complexity
     # B602:subprocess_popen_with_shell_equals_true and
     # B607:start_process_with_partial_path are safe to skip since this is a Gramex internal cmd
-    output = check_output('npx --yes @gramex/escomplexity', cwd=project_path, shell=True)  # nosec
+    output = check_output(
+        'npx --yes @gramex/escomplexity', cwd=project_path, shell=True  # noqa S607
+    )  # noqa S602
     es_complexity = int(output.decode('utf-8').split('\n')[-2].strip())
     return pd.DataFrame(
         {
             'py': [py_complexity],
             'js': [es_complexity],
             'gramex': [gramex_complexity],
         }
@@ -770,30 +772,29 @@
     if isinstance(appcmd, str):
         appcmd = shlex.split(appcmd)
     # If the app is a Cygwin app, TARGET should be a Cygwin path too.
     target = config.target
     cygwin, cygpath, kwargs = which('cygcheck'), which('cygpath'), {'universal_newlines': True}
     if cygwin is not None and cygpath is not None:
         # subprocess.check_output is safe here since these are developer-initiated
-        # B404:import_subprocess check_output is safe here since these are developer-initiated
-        path = check_output([cygpath, '-au', which(appcmd[0])], **kwargs).strip()  # nosec 404
-        is_cygwin_app = check_output([cygwin, '-f', path], **kwargs).strip()  # nosec 404
+        path = check_output([cygpath, '-au', which(appcmd[0])], **kwargs).strip()  # noqa S603
+        is_cygwin_app = check_output([cygwin, '-f', path], **kwargs).strip()  # noqa S603
         if is_cygwin_app:
-            target = check_output([cygpath, '-au', target], **kwargs).strip()  # nosec 404
+            target = check_output([cygpath, '-au', target], **kwargs).strip()  # noqa S603
     # Replace TARGET with the actual target
     if 'TARGET' in appcmd:
         appcmd = [target if arg == 'TARGET' else arg for arg in appcmd]
     else:
         appcmd.append(target)
     app_log.info(f'Running {" ".join(appcmd)}')
     if not safe_rmtree(config.target):
         app_log.error(f'Cannot delete target {config.target}. Aborting installation')
         return
     # B603:subprocess_without_shell_equals_true is safe since this is developer-initiated
-    proc = Popen(appcmd, bufsize=-1, **kwargs)  # nosec 603
+    proc = Popen(appcmd, bufsize=-1, **kwargs)  # noqa S603
     proc.communicate()
     return proc.returncode
 
 
 # Setup file configurations. If {file} exists, then if {exe} exists, run {cmd}.
 setup_paths = [
     [{'file': 'Makefile', 'exe': 'make', 'cmd': '"{exe}"'}],
@@ -869,26 +870,26 @@
 
 def save_user_config(appname, value):
     user_config = AttrDict()
     if user_conf_file.exists():
         with user_conf_file.open(encoding='utf-8') as handle:
             # If app.yaml is empty, yaml.safe_load returns None. Use the AttrDict() instead
             # B506:yaml_load is safe since this object is internally created
-            user_config = yaml.load(handle, Loader=AttrDictYAMLLoader) or user_config  # nosec
+            user_config = yaml.load(handle, Loader=AttrDictYAMLLoader) or user_config  # noqa S506
     if value is None:
         if appname in user_config:
             del user_config[appname]
     else:
         app_config = user_config.setdefault(appname, AttrDict())
         app_config.update({key: value[key] for key in app_keys if key in value})
 
     with user_conf_file.open(mode='w', encoding='utf-8') as handle:
         # Use yaml.dump (not .safe_dump) to serialize the AttrDicts
         # B506:yaml_load is safe since this object is internally created
-        yaml.dump(user_config, handle, indent=4, default_flow_style=False)  # nosec
+        yaml.dump(user_config, handle, indent=4, default_flow_style=False)  # noqa S506
 
 
 def get_app_config(appname, kwargs):
     '''
     Get the stored configuration for appname, and override it with kwargs.
     `.target` defaults to $GRAMEXDATA/apps/<appname>.
     '''
@@ -914,27 +915,27 @@
     return usage[command].format(apps='\n'.join('- ' + app for app in sorted(apps)))
 
 
 def _check_output(cmd, default=b'', **kwargs):
     '''Run cmd and return output. Return default in case the command fails'''
     try:
         # B603:subprocess_without_shell_equals_true is safe since this is developer-initiated
-        return check_output(shlex.split(cmd), **kwargs).strip()  # nosec B603
+        return check_output(shlex.split(cmd), **kwargs).strip()  # noqa S603
     # OSError is raised if the cmd is not found.
     # CalledProcessError is raised if the cmd returns an error.
     except (OSError, CalledProcessError):
         return default
 
 
 def _run_console(cmd, **kwargs):
     '''Run cmd and pipe output to console. Log and raise error if cmd is not found'''
     cmd = shlex.split(cmd)
     try:
         # B603:subprocess_without_shell_equals_true is safe since this is developer-initiated
-        proc = Popen(cmd, bufsize=-1, universal_newlines=True, **kwargs)  # nosec B603
+        proc = Popen(cmd, bufsize=-1, universal_newlines=True, **kwargs)  # noqa S603
     except OSError:
         app_log.error(f'Cannot find command: {cmd[0]}')
         raise
     proc.communicate()
 
 
 def _mkdir(path):
```

### Comparing `gramex-1.94.1/gramex/license.py` & `gramex-1.94.2/gramex/license.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/migrate.py` & `gramex-1.94.2/gramex/migrate.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/ml.py` & `gramex-1.94.2/gramex/ml.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/ml_api.py` & `gramex-1.94.2/gramex/ml_api.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/pptgen/__init__.py` & `gramex-1.94.2/gramex/pptgen/__init__.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/pptgen/color.py` & `gramex-1.94.2/gramex/pptgen/color.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         'dark_1': 9,
     }
 
     def __init__(self, *values):
         self.values = values
 
     def __getitem__(self, key):
-        if isinstance(key, slice) or type(key) is int:
+        if isinstance(key, (slice, int)):
             return self.values.__getitem__(key)
         elif key in self._lookup:
             return self.values[self._lookup[key]]
 
     def __getattr__(self, key):
         if key in self._lookup:
             return self.values[self._lookup[key]]
```

### Comparing `gramex-1.94.1/gramex/pptgen/colors.json` & `gramex-1.94.2/gramex/pptgen/colors.json`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/pptgen/commands.py` & `gramex-1.94.2/gramex/pptgen/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import collections
 import numpy as np
 import pandas as pd
 import matplotlib.cm
 import matplotlib.colors
 
 # B410:import_lxml lxml.etree is safe on https://github.com/tiran/defusedxml/tree/main/xmltestdata
-from lxml.etree import fromstring  # nosec B410
+from lxml.etree import fromstring  # noqa S410
 from tornado.template import Template
 from tornado.escape import to_unicode
 from pptx.chart import data as pptxcd
 from pptx.dml.color import RGBColor
 from pptx.enum.shapes import MSO_SHAPE
 from pptx.oxml.xmlchemy import OxmlElement
 from urllib.parse import urlparse
@@ -72,15 +72,15 @@
         default_css['font-size'] = paragraph.runs[0].font.size / pixel_inch
     default_css['text-align'] = paragraph.alignment
     default_css['font-family'] = paragraph.runs[0].font.name
     # Updating default css with css from config.
     default_css.update(style)
     default_css['color'] = default_css.get('color', '#0000000')
     # B320: lxml.etree is safe on https://github.com/tiran/defusedxml/tree/main/xmltestdata
-    update_text = fromstring('<root>{}</root>'.format(template(spec['text'], data)))  # nosec B320
+    update_text = fromstring('<root>{}</root>'.format(template(spec['text'], data)))  # noqa S320
     paragraph.runs[0].text = update_text.text if update_text.text else ''
     utils.apply_text_css(shape, paragraph.runs[0], paragraph, **default_css)
     index = 1
     for child in update_text.getchildren():
         if not child.tag == 'text':
             raise ValueError('XML elemet must contain only "text" tag.')
         # Adding runs for each text item
@@ -415,18 +415,18 @@
                     elif isinstance(style[key], (dict)):
                         point_css[key] = style[key].get(args['name'], '#cccccc')
                 # Evaluatinig line and shape color format
                 for series_point in {'point', 'series'}:
                     # Replacing point with series to change color in legend
                     fillpoint = color_mapping[chart_name].replace('point', series_point)
                     # B307:eval this is safe since `expr` is written by app developer
-                    chart_css(eval(fillpoint).fill, point_css, point_css['color'])  # nosec B307
+                    chart_css(eval(fillpoint).fill, point_css, point_css['color'])  # noqa S307
                     # Will apply on outer line of chart shape line(like stroke in html)
                     _stroke = point_css.get('stroke', point_css['color'])
-                    chart_css(eval(fillpoint).line.fill, point_css, _stroke)  # nosec B307
+                    chart_css(eval(fillpoint).line.fill, point_css, _stroke)  # noqa S307
 
 
 # Custom Charts Functions below(Sankey, Treemap, Calendarmap).
 
 
 def sankey(shape, spec, data):
     '''Draw sankey in PPT.'''
```

### Comparing `gramex-1.94.1/gramex/pptgen/fonts.json` & `gramex-1.94.2/gramex/pptgen/fonts.json`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/pptgen/fontwidth.py` & `gramex-1.94.2/gramex/pptgen/fontwidth.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/pptgen/utils.py` & `gramex-1.94.2/gramex/pptgen/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import ast
 import copy
 import platform
 import numpy as np
 import pandas as pd
 
 # B410:import_lxml lxml.etree is safe on https://github.com/tiran/defusedxml/tree/main/xmltestdata
-from lxml import objectify  # nosec B410
-from lxml.builder import ElementMaker  # nosec B410
+from lxml import objectify  # noqa S410
+from lxml.builder import ElementMaker  # noqa S410
 from pptx.util import Inches
 from pptx.dml.color import RGBColor
 from pptx.enum.base import EnumValue
 from pptx.enum.text import PP_ALIGN, MSO_ANCHOR
 from gramex.transforms import build_transform
```

### Comparing `gramex-1.94.1/gramex/pptgen2/__init__.py` & `gramex-1.94.2/gramex/pptgen2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -521,8 +521,8 @@
     sys.path.append('.')
     # Generate output
     gramex.pptgen2.pptgen(**rules)
     # If --no-open is specified, or the OS doesn't have startfile (e.g. Linux), stop here.
     # Otherwise, open the output PPTX created
     if not rules.get('no-open', False) and hasattr(os, 'startfile'):
         # B606:start_process_with_no_shell is safe -- it's a file we've explicitly created
-        os.startfile(rules['target'])  # nosec B606
+        os.startfile(rules['target'])  # noqa S606
```

### Comparing `gramex-1.94.1/gramex/pptgen2/commands.py` & `gramex-1.94.2/gramex/pptgen2/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from PIL import Image
 from functools import partial
 from gramex import console
 from gramex.config import app_log, objectpath
 from gramex.transforms import build_transform
 
 # B410:import_lxml lxml.etree is safe on https://github.com/tiran/defusedxml/tree/main/xmltestdata
-from lxml.html import fragments_fromstring, builder, HtmlElement  # nosec B410
+from lxml.html import fragments_fromstring, builder, HtmlElement  # noqa S410
 from orderedattrdict import AttrDict
 from pptx.chart import data as pptxchartdata
 from pptx.dml.color import RGBColor
 from pptx.dml.fill import FillFormat
 from pptx.enum.base import EnumValue
 from pptx.enum.dml import MSO_THEME_COLOR, MSO_FILL
 from pptx.enum.text import PP_ALIGN, MSO_VERTICAL_ANCHOR
```

### Comparing `gramex-1.94.1/gramex/pptgen2/config.yaml` & `gramex-1.94.2/gramex/pptgen2/config.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/pynode.py` & `gramex-1.94.2/gramex/pynode.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/scale.py` & `gramex-1.94.2/gramex/scale.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/secrets.py` & `gramex-1.94.2/gramex/secrets.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/servicenow.yaml` & `gramex-1.94.2/gramex/servicenow.yaml`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/services/__init__.py` & `gramex-1.94.2/gramex/services/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 
                 def check_exit():
                     if exit[0] is True:
                         shutdown()
                     # If Ctrl-D is pressed, run the Python debugger
                     char = debug.getch()
                     if char == b'\x04':
-                        breakpoint()  # noqa: T100
+                        breakpoint()  # noqa T100
                     # If Ctrl-B is pressed, start the browser
                     if char == b'\x02':
                         browser = webbrowser.get()
                         browser.open(url)
 
                 def signal_handler(signum, frame):
                     exit[0] = True
@@ -958,15 +958,15 @@
     method += '\trequest = handler.request\n'
     method += f'\treturn ({", ".join(key_getters)})'
     context = {
         'missing': '~',
         'argsep': ', ',  # join args using comma
     }
     # B102:exec_used is safe since the code is constructed entirely in this function
-    exec(method, context)  # nosec B102
+    exec(method, context)  # noqa S102
     return context['cache_key']
 
 
 def _cache_generator(conf, name):
     '''
     The `url:` section of `gramex.yaml` can specify a `cache:` section.
```

### Comparing `gramex-1.94.1/gramex/services/emailer.py` & `gramex-1.94.2/gramex/services/emailer.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/services/rediscache.py` & `gramex-1.94.2/gramex/services/rediscache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # B403:import_public we only pickle Gramex internal objects
-import pickle  # nosec B403
+import pickle  # noqa S403
 from redis import StrictRedis
 
 
 def get_redis(path: str, **kwargs):
     host, port, db, redis_kwargs = 'localhost', 6379, 0, {}
     if isinstance(path, str):
         parts = path.split(':')
@@ -51,15 +51,15 @@
             self.store.config_set('maxmemory', maxsize)
             self.store.config_set('maxmemory-policy', 'allkeys-lru')  # Approximate LRU cache
 
     def __getitem__(self, key):
         key = pickle.dumps(key, pickle.HIGHEST_PROTOCOL)
         result = self.store.get(key)
         # B301:pickle key is set by developers and safe to pickle
-        return None if result is None else pickle.loads(result)  # nosec B301
+        return None if result is None else pickle.loads(result)  # noqa S301
 
     def __setitem__(self, key, value, expire=None):
         key = pickle.dumps(key, pickle.HIGHEST_PROTOCOL)
         value = pickle.dumps(value, pickle.HIGHEST_PROTOCOL)
         if expire and expire <= 0:
             expire = None
         self.store.set(key, value, ex=expire)
@@ -68,15 +68,15 @@
         self.size = self.store.dbsize()
         return self.size
 
     def __iter__(self):
         for key in self.store.scan_iter():
             try:
                 # B301:pickle key is set by developers and safe to pickle
-                yield pickle.loads(key)  # nosec B301
+                yield pickle.loads(key)  # noqa S301
             except pickle.UnpicklingError:
                 # If redis already has keys created by other apps, yield them as-is
                 yield key
 
     @property
     def currsize(self):
         '''The current size of cache in bytes'''
```

### Comparing `gramex-1.94.1/gramex/services/scheduler.py` & `gramex-1.94.2/gramex/services/scheduler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/services/sms.py` & `gramex-1.94.2/gramex/services/sms.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/services/ttlcache.py` & `gramex-1.94.2/gramex/services/ttlcache.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/services/urlcache.py` & `gramex-1.94.2/gramex/services/urlcache.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 Each type of store has a separate CacheFile. (MemoryCacheFile, DiskCacheFile,
 etc.) The parent CacheFile implements the no-caching behaviour.
 
 See gramex.handlers.BaseHandler for examples on how to use these objects.
 '''
 
 # B403:import_public we only pickle Gramex internal objects
-import pickle  # nosec B403
+import pickle  # noqa S403
 from diskcache import Cache as DiskCache
 from .ttlcache import TTLCache as MemoryCache
 from .rediscache import RedisCache
 from gramex.config import app_log
 from gramex.http import OK, NOT_MODIFIED
 
 # HTTP Headers that should not be cached
@@ -64,15 +64,15 @@
         return handler
 
 
 class MemoryCacheFile(CacheFile):
     def get(self):
         result = self.store.get(self.key)
         # B301:pickle key is an internal state string and safe to pickle
-        return None if result is None else pickle.loads(result)  # nosec B301
+        return None if result is None else pickle.loads(result)  # noqa S301
 
     def wrap(self, handler):
         self._finish = handler.finish
 
         def finish(chunk=None):
             # Save the headers and body originally written
             headers = [
```

### Comparing `gramex-1.94.1/gramex/services/watcher.py` & `gramex-1.94.2/gramex/services/watcher.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/sm_api.py` & `gramex-1.94.2/gramex/sm_api.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/topcause.py` & `gramex-1.94.2/gramex/topcause.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
         Returns
         -------
         self : object
             Returns the instance itself.
         '''
         if not isinstance(X, pd.DataFrame):
-            X = pd.DataFrame(X)  # noqa: N806 X can be in uppercase
+            X = pd.DataFrame(X)  # noqa N806 X can be in uppercase
         if not isinstance(y, pd.Series):
             y = pd.Series(y)
         if X.shape[0] != y.shape[0]:
             raise ValueError(f'X has {X.shape[0]} rows, but y has {y.shape[0]} rows')
 
         # If values contain ±Inf treat it an NaN
         with pd.option_context('mode.use_inf_as_na', True):
```

### Comparing `gramex-1.94.1/gramex/transformers.py` & `gramex-1.94.2/gramex/transformers.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         self.post_train(model_path)
 
     def predict(self, text, **kwargs):
         text = text.tolist()
         predictions = self.pipeline(text)
         return [k["label"] for k in predictions]
 
-    def score(self, X, y_true, **kwargs):  # noqa: N803
+    def score(self, X, y_true, **kwargs):  # noqa N803
         y_true = [self.model.config.label2id[x] for x in y_true]
         y_pred = self.predict(X.squeeze("columns"))
         y_pred = [self.model.config.label2id[x] for x in y_pred]
         return roc_auc_score(y_true, y_pred)
 
 
 class NER(BaseTransformer):
```

### Comparing `gramex-1.94.1/gramex/transforms/__init__.py` & `gramex-1.94.2/gramex/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/transforms/auth.py` & `gramex-1.94.2/gramex/transforms/auth.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/transforms/template.py` & `gramex-1.94.2/gramex/transforms/template.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex/transforms/transforms.py` & `gramex-1.94.2/gramex/transforms/transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,15 +308,15 @@
         GeneratorType=GeneratorType,
         Return=tornado.gen.Return,
         AttrDict=AttrDict,
         **{key: getattr(gramex.transforms, key) for key in gramex.transforms.__all__},
     )
     code = compile(''.join(body), filename=filename, mode='exec')
     # B102:exec_used is safe since the code is written by app developer
-    exec(code, context)  # nosec B102
+    exec(code, context)  # noqa S102
 
     # Return the transformed function
     result = context['transform']
     result.__name__ = str(function_name or filename)
     result.__doc__ = str(doc)
     result.__func__ = function
 
@@ -494,15 +494,15 @@
     if len(args) == 1 and isinstance(args[0], dict):
         pairs = args[0].items()
     else:
         pairs = zip(args[0::2], args[1::2])
     for cond, val in pairs:
         if isinstance(cond, str):
             # B307:eval is safe here since `cond` is written by app developer
-            if eval(Template(cond).substitute(var_defaults)):  # nosec B307
+            if eval(Template(cond).substitute(var_defaults)):  # noqa S307
                 return val
         elif cond:
             return val
 
     # If none of the conditions matched, we'll be here.
     # If there are an odd number of arguments and there's at least one condition,
     # treat the last as a default.
@@ -564,15 +564,15 @@
         else:
             app_log.error(f'flattener:{filename}: value {source} is not a str/int')
             continue
     body.append('\treturn r')
     code = compile(''.join(body), filename=f'flattener:{filename}', mode='exec')
     context = {'AttrDict': AttrDict, 'default': default}
     # B307:eval is safe here since the code is constructed entirely in this function
-    eval(code, context)  # nosec B307
+    eval(code, context)  # noqa S307
     return context[filename]
 
 
 _once_info = {}
 
 
 def once(*args, **kwargs):
@@ -843,15 +843,15 @@
     code = compile(
         'def fn(handler, %s):\n\treturn {%s}' % (', '.join(vars), ' '.join(vals)),
         filename='log',
         mode='exec',
     )
     context = {'os': os, 'time': time, 'datetime': datetime, 'conf': conf, 'AttrDict': AttrDict}
     # B102:exec_used is safe here since the code is constructed entirely in this function
-    exec(code, context)  # nosec B102
+    exec(code, context)  # noqa S102
     return context['fn']
 
 
 def time_key(format, offset=None, freq=None):
     import pandas as pd
 
     result = {'function': lambda *args, **kwargs: pd.Timestamp.utcnow().strftime(format)}
```

### Comparing `gramex-1.94.1/gramex/transforms/twitterstream.py` & `gramex-1.94.2/gramex/transforms/twitterstream.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,15 +243,15 @@
         if path != self.stream_path:
             if self.stream is not None:
                 self.stream.close()
             self.stream_path = path
             folder = os.path.dirname(os.path.abspath(path))
             if not os.path.exists(folder):
                 os.makedirs(folder)
-            self.stream = open(path, 'ab')  # noqa: SIM115
+            self.stream = open(path, 'ab')  # noqa SIM115
             app_log.debug(f'StreamWriter writing to {path}')
 
         # Schedule the next call after a minute
         ioloop = gramex.service.info.main_ioloop or tornado.ioloop.IOLoop.current()
         ioloop.call_later(60, self.rotate)
 
     def write(self, data):
```

### Comparing `gramex-1.94.1/gramex/winservice.py` & `gramex-1.94.2/gramex/winservice.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/gramex.egg-info/PKG-INFO` & `gramex-1.94.2/gramex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gramex
-Version: 1.94.1
+Version: 1.94.2
 Summary: Gramex: Low Code Data Solutions Platform
 Author-email: Anand S <s.anand@gramener.com>, Pratap Vardhan <pratapapvr@gmail.com>, Jaidev Deshpande <jaidev.deshpande@gramener.com>, Bhanu Kamapantula <talk2kish@gmail.com>, Radheya Kale <radheya.kale@gramener.com>, Karmanya Aggarwal <karmanyaaggarwal@gmail.com>, Sandeep Bhat <sandeep.bhat@gramener.com>, Shraddheya Shrivastava <shraddheya.shrivastava@gramener.com>, Sundeep Reddy Mallu <sundeep.mally@gramener.com>
 License: MIT
 Project-URL: Homepage, https://gramener.com/gramex/
 Project-URL: Documentation, https://gramener.com/gramex/guide/
 Project-URL: Repository, https://github.com/gramener/gramex
 Project-URL: Changelog, https://gramener.com/gramex/guide/release/
```

### Comparing `gramex-1.94.1/gramex.egg-info/requires.txt` & `gramex-1.94.2/gramex.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/pyproject.toml` & `gramex-1.94.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gramex"
-version = "1.94.1"
+version = "1.94.2"
 description = "Gramex: Low Code Data Solutions Platform"
 # People with 2+ contributions on https://github.com/gramener/gramex/graphs/contributors
 authors = [
     {name = "Anand S", email = "s.anand@gramener.com"},
     {name = "Pratap Vardhan", email = "pratapapvr@gmail.com"},
     {name = "Jaidev Deshpande", email = "jaidev.deshpande@gramener.com"},
     {name = "Bhanu Kamapantula", email = "talk2kish@gmail.com"},
@@ -89,14 +89,36 @@
 [tool.setuptools.packages.find]
 include = ["gramex*"]
 
 [tool.black]
 # pytest/complexity_error/invalid.py has non-parseable Python code
 force-exclude = "complexity_error"
 
+[tool.ruff]
+exclude = ["build", "dist", "docs", ".eggs", "node_modules", ".vscode"]
+line-length = 99
+# E203 allows whitespace before :. Black needs this
+# E911 allows use of str(). Required for pathlib.Path to string conversions
+# N802 ignores "function name should be in lowercase". Required for
+#   tearDownModule(), extendMarkdown, etc where function name is pre-defined
+# B902 ignores "blind except Exception:". We trap broad errors often
+lint.ignore = ["E203", "N802", "B006", "B007", "B008", "S101"]
+
+[tool.ruff.lint.per-file-ignores]
+# ML libraries use capital "X" as a function argument or a variable. That's OK
+"gramex/ml_api.py" = ["N803", "N806"]
+"gramex/sm_api.py" = ["N803", "N806"]
+"gramex/transformers.py" = ["N803", "N806"]
+# requests.post infers filename from open(...) handle, so avoid context handler (flake8-simplify)
+"tests/test_uploadhandler.py" = ["SIM115"]
+# Ignore bandit checks for test cases
+"pytest/**/*.py" = ["S"]
+"testlib/**/*.py" = ["S"]
+"tests/**/*.py" = ["S"]
+
 [tool.pytest.ini_options]
 testpaths = "pytest"
 
 [project.optional-dependencies]
 # pip install "gramex[full]" for better debugging and ML support
 full = [
     "boto3",  # for gramex.services.sns.AmazonSNS
```

### Comparing `gramex-1.94.1/tests/test_admin.py` & `gramex-1.94.2/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_alerts.py` & `gramex-1.94.2/tests/test_alerts.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_args.py` & `gramex-1.94.2/tests/test_args.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_auth.py` & `gramex-1.94.2/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_cache.py` & `gramex-1.94.2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_capturehandler.py` & `gramex-1.94.2/tests/test_capturehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_comichandler.py` & `gramex-1.94.2/tests/test_comichandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_drivehandler.py` & `gramex-1.94.2/tests/test_drivehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_filehandler.py` & `gramex-1.94.2/tests/test_filehandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_filterhandler.py` & `gramex-1.94.2/tests/test_filterhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_formhandler.py` & `gramex-1.94.2/tests/test_formhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_functionhandler.py` & `gramex-1.94.2/tests/test_functionhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_gramexlog.py` & `gramex-1.94.2/tests/test_gramexlog.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_handlers.py` & `gramex-1.94.2/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_init.py` & `gramex-1.94.2/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_install.py` & `gramex-1.94.2/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_jsonhandler.py` & `gramex-1.94.2/tests/test_jsonhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_ldapauth.py` & `gramex-1.94.2/tests/test_ldapauth.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_logviewer.py` & `gramex-1.94.2/tests/test_logviewer.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_mlhandler.py` & `gramex-1.94.2/tests/test_mlhandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     from statsmodels.datasets.interest_inflation import load as infl_load
 
     STATSMODELS_INSTALLED = True
 except ImportError:
     STATSMODELS_INSTALLED = False
 try:
     logging.getLogger("tensorflow").disabled = True
-    import transformers as trf  # NOQA: F401
+    import transformers as trf  # noqa F401
 
     TRANSFORMERS_INSTALLED = True
 except ImportError:
     TRANSFORMERS_INSTALLED = False
 
 
 op = os.path
@@ -547,15 +547,15 @@
     def test_post_after_delete_custom_model(self):
         org_clf = joblib.load(self.model_path)
         try:
             r = self.get("/mlhandler?delete=model", method="delete")
             self.assertEqual(r.status_code, OK)
             self.assertFalse(op.exists(self.model_path))
             # recreate the model
-            X, y = make_classification()  # NOQA: N806
+            X, y = make_classification()  # noqa N806
             xtrain, xtest, ytrain, ytest = train_test_split(X, y, stratify=y, test_size=0.25)
             df = pd.DataFrame(xtrain)
             df["target"] = ytrain
             r = self.get("/mlhandler?class=GaussianNB", method="put")
             self.assertEqual(r.status_code, OK)
             r = self.get(
                 "/mlhandler?_action=train&target_col=target",
@@ -573,15 +573,15 @@
     def test_post_after_delete_default_model(self):
         clf = joblib.load(self.model_path)
         try:
             r = self.get("/mlhandler?delete=model", method="delete")
             self.assertEqual(r.status_code, OK)
             self.assertFalse(op.exists(self.model_path))
             # recreate the model
-            X, y = make_classification()  # NOQA: N806
+            X, y = make_classification()  # noqa N806
             xtrain, xtest, ytrain, ytest = train_test_split(X, y, stratify=y, test_size=0.25)
             df = pd.DataFrame(xtrain)
             df["target"] = ytrain
             r = self.get(
                 "/mlhandler?_action=train&target_col=target",
                 method="post",
                 data=df.to_json(orient="records"),
@@ -667,15 +667,15 @@
         # Try getting predictions
         self.test_get_predictions(target_col="target")
         self.test_get_bulk_predictions("target")
 
     def test_train(self):
         # backup the original model
         clf = joblib.load(self.model_path)
-        X, y = make_classification()  # NOQA: N806
+        X, y = make_classification()  # noqa N806
         xtrain, xtest, ytrain, ytest = train_test_split(X, y, stratify=y, test_size=0.25)
         df = pd.DataFrame(xtrain)
         df["target"] = ytrain
         try:
             resp = self.get(
                 "/mlhandler?_action=train&target_col=target",
                 method="post",
```

### Comparing `gramex-1.94.1/tests/test_modelhandler.py` & `gramex-1.94.2/tests/test_modelhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_openapihandler.py` & `gramex-1.94.2/tests/test_openapihandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_pptxhandler.py` & `gramex-1.94.2/tests/test_pptxhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_processhandler.py` & `gramex-1.94.2/tests/test_processhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_proxyhandler.py` & `gramex-1.94.2/tests/test_proxyhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_pynode.py` & `gramex-1.94.2/tests/test_pynode.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_schedule.py` & `gramex-1.94.2/tests/test_schedule.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_secrets.py` & `gramex-1.94.2/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_subprocess.py` & `gramex-1.94.2/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_translater.py` & `gramex-1.94.2/tests/test_translater.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_twitterresthandler.py` & `gramex-1.94.2/tests/test_twitterresthandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from . import server, TestGramex
 
 threadpool = concurrent.futures.ThreadPoolExecutor(8)
 
 
 def async_fetch(name, path, method='post', url='/api/twitter/', **kwargs):
     future = threadpool.submit(getattr(requests, method), server.base_url + url + path, **kwargs)
-    setattr(future, 'name', name)  # noqa: B010 future.name doesn't exist, so create it
+    setattr(future, 'name', name)  # noqa B010 future.name doesn't exist, so create it
     return future
 
 
 class TestTwitterRESTHandler(TestGramex):
     def test_twitter(self):
         search = {'q': 'gramener', 'count': 2}
         tweets = {'screen_name': 'gramener', 'count': 2}
```

### Comparing `gramex-1.94.1/tests/test_ui.py` & `gramex-1.94.2/tests/test_ui.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_update.py` & `gramex-1.94.2/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_uploadhandler.py` & `gramex-1.94.2/tests/test_uploadhandler.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_watcher.py` & `gramex-1.94.2/tests/test_watcher.py`

 * *Files identical despite different names*

### Comparing `gramex-1.94.1/tests/test_websockethandler.py` & `gramex-1.94.2/tests/test_websockethandler.py`

 * *Files identical despite different names*

