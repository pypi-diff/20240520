# Comparing `tmp/plone_sphinx_theme-0.0.2.tar.gz` & `tmp/plone_sphinx_theme-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone_sphinx_theme-0.0.2.tar", last modified: Mon May  6 09:54:36 2024, max compression
+gzip compressed data, was "plone_sphinx_theme-0.0.3.tar", last modified: Sun May 19 22:31:31 2024, max compression
```

## Comparing `plone_sphinx_theme-0.0.2.tar` & `plone_sphinx_theme-0.0.3.tar`

### file list

```diff
@@ -1,108 +1,112 @@
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.993795 plone_sphinx_theme-0.0.2/
--rw-r--r--   0 stevepiercy   (501) staff       (20)      531 2024-05-06 09:54:35.818419 plone_sphinx_theme-0.0.2/CHANGES.md
--rw-r--r--   0 stevepiercy   (501) staff       (20)    18091 2024-05-06 09:54:35.818697 plone_sphinx_theme-0.0.2/LICENSE
--rw-r--r--   0 stevepiercy   (501) staff       (20)       18 2024-05-06 09:54:35.818900 plone_sphinx_theme-0.0.2/MANIFEST.in
--rw-r--r--   0 stevepiercy   (501) staff       (20)     8253 2024-05-06 09:54:35.819099 plone_sphinx_theme-0.0.2/Makefile
--rw-r--r--   0 stevepiercy   (501) staff       (20)      749 2024-05-06 09:54:35.819278 plone_sphinx_theme-0.0.2/README.md
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.823037 plone_sphinx_theme-0.0.2/docs/
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.819625 plone_sphinx_theme-0.0.2/docs/_static/
--rw-r--r--   0 stevepiercy   (501) staff       (20)     5430 2024-05-06 09:54:35.819588 plone_sphinx_theme-0.0.2/docs/_static/favicon.ico
--rw-r--r--   0 stevepiercy   (501) staff       (20)     3775 2024-05-06 09:54:35.819800 plone_sphinx_theme-0.0.2/docs/_static/logo.svg
--rw-r--r--   0 stevepiercy   (501) staff       (20)    15651 2024-05-06 09:54:35.820112 plone_sphinx_theme-0.0.2/docs/conf.py
--rw-r--r--   0 stevepiercy   (501) staff       (20)     2568 2024-05-06 09:54:35.820255 plone_sphinx_theme-0.0.2/docs/glossary.md
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.820730 plone_sphinx_theme-0.0.2/docs/guides/
--rw-r--r--   0 stevepiercy   (501) staff       (20)     3887 2024-05-06 09:54:35.820427 plone_sphinx_theme-0.0.2/docs/guides/contribute.md
--rw-r--r--   0 stevepiercy   (501) staff       (20)     2177 2024-05-06 09:54:35.820569 plone_sphinx_theme-0.0.2/docs/guides/contributing-policies.md
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1173 2024-05-06 09:54:35.820701 plone_sphinx_theme-0.0.2/docs/guides/develop.md
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1911 2024-05-06 09:54:35.820822 plone_sphinx_theme-0.0.2/docs/guides/usage.md
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1583 2024-05-06 09:54:35.820944 plone_sphinx_theme-0.0.2/docs/index.md
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.822909 plone_sphinx_theme-0.0.2/docs/reference/
--rw-r--r--   0 stevepiercy   (501) staff       (20)     5113 2024-05-06 09:54:35.821103 plone_sphinx_theme-0.0.2/docs/reference/extensions.md
--rw-r--r--   0 stevepiercy   (501) staff       (20)     3212 2024-05-06 09:54:35.821224 plone_sphinx_theme-0.0.2/docs/reference/file-system-structure.md
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.822771 plone_sphinx_theme-0.0.2/docs/reference/kitchen-sink/
--rw-r--r--   0 stevepiercy   (501) staff       (20)     3208 2024-05-06 09:54:35.821381 plone_sphinx_theme-0.0.2/docs/reference/kitchen-sink/admonitions.rst
--rw-r--r--   0 stevepiercy   (501) staff       (20)      980 2024-05-06 09:54:35.821509 plone_sphinx_theme-0.0.2/docs/reference/kitchen-sink/api.rst
--rw-r--r--   0 stevepiercy   (501) staff       (20)     8114 2024-05-06 09:54:35.821653 plone_sphinx_theme-0.0.2/docs/reference/kitchen-sink/blocks.rst
--rw-r--r--   0 stevepiercy   (501) staff       (20)     8597 2024-05-06 09:54:35.821883 plone_sphinx_theme-0.0.2/docs/reference/kitchen-sink/generic.rst
--rw-r--r--   0 stevepiercy   (501) staff       (20)     3070 2024-05-06 09:54:35.822114 plone_sphinx_theme-0.0.2/docs/reference/kitchen-sink/images.rst
--rw-r--r--   0 stevepiercy   (501) staff       (20)      576 2024-05-06 09:54:35.822232 plone_sphinx_theme-0.0.2/docs/reference/kitchen-sink/index.rst
--rw-r--r--   0 stevepiercy   (501) staff       (20)     6150 2024-05-06 09:54:35.822363 plone_sphinx_theme-0.0.2/docs/reference/kitchen-sink/lists.rst
--rw-r--r--   0 stevepiercy   (501) staff       (20)    13453 2024-05-06 09:54:35.822482 plone_sphinx_theme-0.0.2/docs/reference/kitchen-sink/really-long.rst
--rw-r--r--   0 stevepiercy   (501) staff       (20)     6375 2024-05-06 09:54:35.822616 plone_sphinx_theme-0.0.2/docs/reference/kitchen-sink/structure.rst
--rw-r--r--   0 stevepiercy   (501) staff       (20)     6705 2024-05-06 09:54:35.822742 plone_sphinx_theme-0.0.2/docs/reference/kitchen-sink/tables.rst
--rw-r--r--   0 stevepiercy   (501) staff       (20)     2669 2024-05-06 09:54:35.822871 plone_sphinx_theme-0.0.2/docs/reference/kitchen-sink/typography.rst
--rw-r--r--   0 stevepiercy   (501) staff       (20)     2507 2024-05-06 09:54:35.823009 plone_sphinx_theme-0.0.2/docs/reference/special-theme-elements.md
--rw-r--r--   0 stevepiercy   (501) staff       (20)      236 2024-05-06 09:54:35.823189 plone_sphinx_theme-0.0.2/docs/robots.txt
--rw-r--r--   0 stevepiercy   (501) staff       (20)      622 2024-05-06 09:54:35.823300 plone_sphinx_theme-0.0.2/package.json
--rw-r--r--   0 stevepiercy   (501) staff       (20)     3404 2024-05-06 09:54:35.823408 plone_sphinx_theme-0.0.2/pyproject.toml
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.823670 plone_sphinx_theme-0.0.2/scripts/
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1195 2024-05-06 09:54:35.823638 plone_sphinx_theme-0.0.2/scripts/kitchen_sink_update.py
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1655 2024-05-06 09:54:35.823757 plone_sphinx_theme-0.0.2/scripts/sbt_styles_update.py
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.823822 plone_sphinx_theme-0.0.2/src/
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.829146 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/
--rw-r--r--   0 stevepiercy   (501) staff       (20)     2894 2024-05-06 09:54:35.823933 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/__init__.py
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.824278 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.824044 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/scripts/
--rw-r--r--   0 stevepiercy   (501) staff       (20)     6353 2024-05-06 09:54:35.824251 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/scripts/index.js
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.825619 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.824574 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/abstracts/
--rw-r--r--   0 stevepiercy   (501) staff       (20)      600 2024-05-06 09:54:35.824543 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/abstracts/_mixins.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1950 2024-05-06 09:54:35.824690 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/abstracts/_variables.scss
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.824956 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/base/
--rw-r--r--   0 stevepiercy   (501) staff       (20)      933 2024-05-06 09:54:35.824924 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/base/_base.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1880 2024-05-06 09:54:35.825147 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/base/_print.scss
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.825207 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/components/
--rw-r--r--   0 stevepiercy   (501) staff       (20)      124 2024-05-06 09:54:35.825297 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/components/_title.scss
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.825364 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/content/
--rw-r--r--   0 stevepiercy   (501) staff       (20)      197 2024-05-06 09:54:35.825456 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/content/_margin.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)      287 2024-05-06 09:54:35.825585 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/index.scss
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.828046 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.825791 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/abstracts/
--rw-r--r--   0 stevepiercy   (501) staff       (20)      600 2024-05-06 09:54:35.825760 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/abstracts/_mixins.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1950 2024-05-06 09:54:35.825860 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/abstracts/_variables.scss
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.826130 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/
--rw-r--r--   0 stevepiercy   (501) staff       (20)      933 2024-05-06 09:54:35.825987 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/_base.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1880 2024-05-06 09:54:35.826098 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/_print.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)      517 2024-05-06 09:54:35.826312 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/_typography.scss
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.826800 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/components/
--rw-r--r--   0 stevepiercy   (501) staff       (20)      325 2024-05-06 09:54:35.826509 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/components/_back-to-top.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)      455 2024-05-06 09:54:35.826631 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/components/_icon-links.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)      461 2024-05-06 09:54:35.826763 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/components/_logo.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1059 2024-05-06 09:54:35.826894 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/components/_search.scss
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.827457 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/
--rw-r--r--   0 stevepiercy   (501) staff       (20)      128 2024-05-06 09:54:35.827046 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_code.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)      824 2024-05-06 09:54:35.827165 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_images.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)     4767 2024-05-06 09:54:35.827297 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_margin.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)      250 2024-05-06 09:54:35.827425 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_notebooks.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)      364 2024-05-06 09:54:35.827551 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_quotes.scss
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.827750 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/extensions/
--rw-r--r--   0 stevepiercy   (501) staff       (20)      308 2024-05-06 09:54:35.827719 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/extensions/_comments.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)      431 2024-05-06 09:54:35.827836 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/extensions/_thebe.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1262 2024-05-06 09:54:35.828019 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/index.scss
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.829018 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/
--rw-r--r--   0 stevepiercy   (501) staff       (20)       94 2024-05-06 09:54:35.828162 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_announcement.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)      746 2024-05-06 09:54:35.828278 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_article-container.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)      113 2024-05-06 09:54:35.828390 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_article.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)      150 2024-05-06 09:54:35.828501 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_footer-article.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)      436 2024-05-06 09:54:35.828613 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_footer-content.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)     4365 2024-05-06 09:54:35.828745 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_header-article.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)      233 2024-05-06 09:54:35.828867 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_header-primary.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1266 2024-05-06 09:54:35.828987 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_sidebar-primary.scss
--rw-r--r--   0 stevepiercy   (501) staff       (20)     2585 2024-05-06 09:54:35.829116 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_sidebar-secondary.scss
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.829181 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/theme/
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.829800 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/theme/plone-sphinx-theme/
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1305 2024-05-06 09:54:35.829371 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/theme/plone-sphinx-theme/404.html
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.829635 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/theme/plone-sphinx-theme/components/
--rw-r--r--   0 stevepiercy   (501) staff       (20)      142 2024-05-06 09:54:35.829599 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/theme/plone-sphinx-theme/components/chapter-title.html
--rw-r--r--   0 stevepiercy   (501) staff       (20)       13 2024-05-06 09:54:35.829765 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/theme/plone-sphinx-theme/components/version.html
--rw-r--r--   0 stevepiercy   (501) staff       (20)      349 2024-05-06 09:54:35.829982 plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/theme/plone-sphinx-theme/theme.conf
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.830068 plone_sphinx_theme-0.0.2/styles/
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.830348 plone_sphinx_theme-0.0.2/styles/Vocab/
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.830261 plone_sphinx_theme-0.0.2/styles/Vocab/Base/
--rw-r--r--   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.830164 plone_sphinx_theme-0.0.2/styles/Vocab/Base/accept.txt
--rw-r--r--   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.830258 plone_sphinx_theme-0.0.2/styles/Vocab/Base/reject.txt
-drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-06 09:54:35.830615 plone_sphinx_theme-0.0.2/styles/Vocab/Plone/
--rw-r--r--   0 stevepiercy   (501) staff       (20)      564 2024-05-06 09:54:35.830578 plone_sphinx_theme-0.0.2/styles/Vocab/Plone/accept.txt
--rw-r--r--   0 stevepiercy   (501) staff       (20)       14 2024-05-06 09:54:35.830784 plone_sphinx_theme-0.0.2/styles/Vocab/Plone/reject.txt
--rw-r--r--   0 stevepiercy   (501) staff       (20)     1628 2024-05-06 09:54:35.830937 plone_sphinx_theme-0.0.2/webpack.config.js
--rw-r--r--   0        0        0    23841 1970-01-01 00:00:00.000000 plone_sphinx_theme-0.0.2/PKG-INFO
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.330340 plone_sphinx_theme-0.0.3/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1336 2024-05-19 22:31:31.152678 plone_sphinx_theme-0.0.3/CHANGES.md
+-rw-r--r--   0 stevepiercy   (501) staff       (20)    18091 2024-05-19 22:31:31.152958 plone_sphinx_theme-0.0.3/LICENSE
+-rw-r--r--   0 stevepiercy   (501) staff       (20)       33 2024-05-19 22:31:31.153073 plone_sphinx_theme-0.0.3/MANIFEST.in
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     7914 2024-05-19 22:31:31.153321 plone_sphinx_theme-0.0.3/Makefile
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      888 2024-05-19 22:31:31.153412 plone_sphinx_theme-0.0.3/README.md
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.157188 plone_sphinx_theme-0.0.3/docs/
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.153771 plone_sphinx_theme-0.0.3/docs/_static/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     5430 2024-05-19 22:31:31.153740 plone_sphinx_theme-0.0.3/docs/_static/favicon.ico
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     3775 2024-05-19 22:31:31.153953 plone_sphinx_theme-0.0.3/docs/_static/logo.svg
+-rw-r--r--   0 stevepiercy   (501) staff       (20)    16098 2024-05-19 22:31:31.154119 plone_sphinx_theme-0.0.3/docs/conf.py
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     2620 2024-05-19 22:31:31.154234 plone_sphinx_theme-0.0.3/docs/glossary.md
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.154778 plone_sphinx_theme-0.0.3/docs/guides/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     3887 2024-05-19 22:31:31.154478 plone_sphinx_theme-0.0.3/docs/guides/contribute.md
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     2177 2024-05-19 22:31:31.154629 plone_sphinx_theme-0.0.3/docs/guides/contributing-policies.md
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1173 2024-05-19 22:31:31.154747 plone_sphinx_theme-0.0.3/docs/guides/develop.md
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1885 2024-05-19 22:31:31.154847 plone_sphinx_theme-0.0.3/docs/guides/usage.md
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1588 2024-05-19 22:31:31.154949 plone_sphinx_theme-0.0.3/docs/index.md
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.157047 plone_sphinx_theme-0.0.3/docs/reference/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     5113 2024-05-19 22:31:31.155104 plone_sphinx_theme-0.0.3/docs/reference/extensions.md
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     3212 2024-05-19 22:31:31.155233 plone_sphinx_theme-0.0.3/docs/reference/file-system-structure.md
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.156905 plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     3208 2024-05-19 22:31:31.155420 plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/admonitions.rst
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      980 2024-05-19 22:31:31.155549 plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/api.rst
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     8114 2024-05-19 22:31:31.155692 plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/blocks.rst
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     8597 2024-05-19 22:31:31.156005 plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/generic.rst
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     3070 2024-05-19 22:31:31.156219 plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/images.rst
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      576 2024-05-19 22:31:31.156346 plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/index.rst
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     6150 2024-05-19 22:31:31.156484 plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/lists.rst
+-rw-r--r--   0 stevepiercy   (501) staff       (20)    13453 2024-05-19 22:31:31.156613 plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/really-long.rst
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     6375 2024-05-19 22:31:31.156742 plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/structure.rst
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     6705 2024-05-19 22:31:31.156870 plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/tables.rst
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     2669 2024-05-19 22:31:31.157006 plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/typography.rst
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     2507 2024-05-19 22:31:31.157158 plone_sphinx_theme-0.0.3/docs/reference/special-theme-elements.md
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      260 2024-05-19 22:31:31.157257 plone_sphinx_theme-0.0.3/docs/robots.txt
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.157320 plone_sphinx_theme-0.0.3/news/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.157318 plone_sphinx_theme-0.0.3/news/.gitkeep
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      622 2024-05-19 22:31:31.157706 plone_sphinx_theme-0.0.3/package.json
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     3498 2024-05-19 22:31:31.157812 plone_sphinx_theme-0.0.3/pyproject.toml
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      302 2024-05-19 22:31:31.157918 plone_sphinx_theme-0.0.3/requirements-docs.txt
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      133 2024-05-19 22:31:31.158039 plone_sphinx_theme-0.0.3/requirements-initial.txt
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.158362 plone_sphinx_theme-0.0.3/scripts/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1195 2024-05-19 22:31:31.158330 plone_sphinx_theme-0.0.3/scripts/kitchen_sink_update.py
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1655 2024-05-19 22:31:31.158448 plone_sphinx_theme-0.0.3/scripts/sbt_styles_update.py
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.158515 plone_sphinx_theme-0.0.3/src/
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.163955 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     2894 2024-05-19 22:31:31.158631 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/__init__.py
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.159004 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.158750 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/scripts/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     6353 2024-05-19 22:31:31.158973 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/scripts/index.js
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.160436 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.159321 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/abstracts/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      600 2024-05-19 22:31:31.159284 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/abstracts/_mixins.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1950 2024-05-19 22:31:31.159472 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/abstracts/_variables.scss
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.159767 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/base/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      933 2024-05-19 22:31:31.159732 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/base/_base.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1880 2024-05-19 22:31:31.159955 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/base/_print.scss
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.160032 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/components/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      124 2024-05-19 22:31:31.160124 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/components/_title.scss
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.160206 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/content/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      197 2024-05-19 22:31:31.160294 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/content/_margin.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      287 2024-05-19 22:31:31.160405 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/index.scss
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.162799 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.160650 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/abstracts/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      600 2024-05-19 22:31:31.160603 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/abstracts/_mixins.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1950 2024-05-19 22:31:31.160722 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/abstracts/_variables.scss
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.160981 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      933 2024-05-19 22:31:31.160859 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/_base.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1880 2024-05-19 22:31:31.160951 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/_print.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      517 2024-05-19 22:31:31.161156 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/_typography.scss
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.161636 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/components/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      325 2024-05-19 22:31:31.161352 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/components/_back-to-top.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      455 2024-05-19 22:31:31.161476 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/components/_icon-links.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      461 2024-05-19 22:31:31.161605 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/components/_logo.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1059 2024-05-19 22:31:31.161732 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/components/_search.scss
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.162249 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      128 2024-05-19 22:31:31.161876 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_code.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      824 2024-05-19 22:31:31.161990 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_images.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     4767 2024-05-19 22:31:31.162113 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_margin.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      250 2024-05-19 22:31:31.162218 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_notebooks.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      364 2024-05-19 22:31:31.162332 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_quotes.scss
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.162554 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/extensions/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      308 2024-05-19 22:31:31.162519 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/extensions/_comments.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      431 2024-05-19 22:31:31.162648 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/extensions/_thebe.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1262 2024-05-19 22:31:31.162767 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/index.scss
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.163830 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)       94 2024-05-19 22:31:31.162937 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_announcement.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      746 2024-05-19 22:31:31.163066 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_article-container.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      113 2024-05-19 22:31:31.163170 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_article.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      150 2024-05-19 22:31:31.163287 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_footer-article.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      436 2024-05-19 22:31:31.163412 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_footer-content.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     4365 2024-05-19 22:31:31.163557 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_header-article.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      233 2024-05-19 22:31:31.163682 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_header-primary.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1266 2024-05-19 22:31:31.163799 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_sidebar-primary.scss
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     2585 2024-05-19 22:31:31.163926 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_sidebar-secondary.scss
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.163996 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/theme/
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.164637 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/theme/plone-sphinx-theme/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1305 2024-05-19 22:31:31.164246 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/theme/plone-sphinx-theme/404.html
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.164526 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/theme/plone-sphinx-theme/components/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      142 2024-05-19 22:31:31.164489 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/theme/plone-sphinx-theme/components/chapter-title.html
+-rw-r--r--   0 stevepiercy   (501) staff       (20)       13 2024-05-19 22:31:31.164606 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/theme/plone-sphinx-theme/components/version.html
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      349 2024-05-19 22:31:31.164795 plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/theme/plone-sphinx-theme/theme.conf
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.164870 plone_sphinx_theme-0.0.3/styles/
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.165105 plone_sphinx_theme-0.0.3/styles/Vocab/
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.165034 plone_sphinx_theme-0.0.3/styles/Vocab/Base/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.164947 plone_sphinx_theme-0.0.3/styles/Vocab/Base/accept.txt
+-rw-r--r--   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.165032 plone_sphinx_theme-0.0.3/styles/Vocab/Base/reject.txt
+drwxr-xr-x   0 stevepiercy   (501) staff       (20)        0 2024-05-19 22:31:31.165271 plone_sphinx_theme-0.0.3/styles/Vocab/Plone/
+-rw-r--r--   0 stevepiercy   (501) staff       (20)      564 2024-05-19 22:31:31.165238 plone_sphinx_theme-0.0.3/styles/Vocab/Plone/accept.txt
+-rw-r--r--   0 stevepiercy   (501) staff       (20)       14 2024-05-19 22:31:31.165427 plone_sphinx_theme-0.0.3/styles/Vocab/Plone/reject.txt
+-rw-r--r--   0 stevepiercy   (501) staff       (20)     1628 2024-05-19 22:31:31.165545 plone_sphinx_theme-0.0.3/webpack.config.js
+-rw-r--r--   0        0        0    23980 1970-01-01 00:00:00.000000 plone_sphinx_theme-0.0.3/PKG-INFO
```

### Comparing `plone_sphinx_theme-0.0.2/LICENSE` & `plone_sphinx_theme-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/Makefile` & `plone_sphinx_theme-0.0.3/Makefile`

 * *Files 13% similar despite different names*

```diff
@@ -208,22 +208,13 @@
 sbt-styles-update:  ## Copy Sphinx Book Theme styles to Plone Sphinx Theme
 	bin/python scripts/sbt_styles_update.py
 
 .PHONY: kitchen-sink-update
 kitchen-sink-update:  ## Copy Kitchen Sink documentation files to Plone Sphinx Theme
 	bin/python scripts/kitchen_sink_update.py
 
-.PHONY: netlify
-netlify:
-	pip install -r requirements-initial.txt
-	pip install -r requirements.txt
-	pip install -r requirements-netlify.txt
-	git submodule init; \
-	git submodule update; \
-	pip install -e submodules/plone.api[test]; \
-	ln -s ../submodules/volto/docs/source ./docs/volto
-	ln -s ../submodules/plone.restapi ./docs/plone.restapi
-	ln -s ../submodules/plone.api/docs ./docs/plone.api
-	cd $(DOCS_DIR) && sphinx-build -b html $(ALLSPHINXOPTS) $(BUILDDIR)/html && cp ./netlify_robots.txt $(BUILDDIR)/html/robots.txt
+.PHONY: rtd-pr-preview
+rtd-pr-preview: bin/python  ## Build pull request preview on Read the Docs
+	cd $(DOCS_DIR) && $(SPHINXBUILD) -b html $(ALLSPHINXOPTS) ${READTHEDOCS_OUTPUT}/html/
 
 .PHONY: all
 all: clean vale linkcheck html  ## Clean docs build, then run vale and linkcheck, and build html
```

### Comparing `plone_sphinx_theme-0.0.2/README.md` & `plone_sphinx_theme-0.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,21 +3,28 @@
 plone-sphinx-theme is a Sphinx theme for [Plone 6 Documentation](https://6.docs.plone.org/), [Plone Conference Training](https://training.plone.org/), and documentation of various Plone packages.
 
 It is based on [`sphinx-book-theme`](https://sphinx-book-theme.readthedocs.io/en/latest/), which in turn is based on [`pydata-sphinx-theme`](https://pydata-sphinx-theme.readthedocs.io/en/stable/).
 
 
 ## Requirements
 
--   Python 3.10, 3.11, or 3.12
+-   Python 3.9, 3.10, 3.11, or 3.12
 -   GNU Make is required only for contributing to or development of this theme.
 
 
-## Documentation and demonstration
+## Documentation
 
-TODO:
+Documentation is hosted on Read the Docs.
+
+https://plone-sphinx-theme.readthedocs.io/
+
+
+## Demonstration
+
+TODO: Add reference to documentation permanent URL.
 
 To build documentation and a demonstration of this project, you can use `make` commands.
 
 
 ## Releasing
 
 Run the following command.
```

### Comparing `plone_sphinx_theme-0.0.2/docs/_static/favicon.ico` & `plone_sphinx_theme-0.0.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/docs/_static/logo.svg` & `plone_sphinx_theme-0.0.3/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/docs/conf.py` & `plone_sphinx_theme-0.0.3/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -167,17 +167,15 @@
     "article_header_start": ["toggle-primary-sidebar"],
     # "extra_navbar": """
     # <p class="ploneorglink">
     #     <a href="https://plone.org">
     #         <img src="/_static/logo.svg" alt="plone.org" /> plone.org</a>
     # </p>""",
     "extra_footer": """<p>The text and illustrations in this website are licensed by the Plone Foundation under a Creative Commons Attribution 4.0 International license. Plone and the Plone® logo are registered trademarks of the Plone Foundation, registered in the United States and other countries. For guidelines on the permitted uses of the Plone trademarks, see <a href="https://plone.org/foundation/logo">https://plone.org/foundation/logo</a>. All other trademarks are owned by their respective owners.</p>
-    <p><a href="https://www.netlify.com">
-  <img src="https://www.netlify.com/img/global/badges/netlify-color-bg.svg" alt="Deploys by Netlify">
-</a></p>""",
+    <p>Pull request previews by <a href="https://readthedocs.org/">Read the Docs</a>.</p>""",
     # "navbar_center": ["chapter-title.html"],
     "footer_end": ["version.html"],
     "icon_links": [
         {
             "name": "GitHub",
             "url": "https://github.com/plone/documentation",
             "icon": "fa-brands fa-square-github",
@@ -213,33 +211,33 @@
     ],
     "logo": {
         "text": "Plone Sphinx Theme",
     },
     "navigation_with_keys": True,
     "path_to_docs": "docs",
     "repository_branch": "main",
-    "repository_url": "https://github.com/plone/documentation",
+    "repository_url": "https://github.com/plone/plone-sphinx-theme",
     "search_bar_text": "Search",  # TODO: Confirm usage of search_bar_text
     "switcher": {
         "json_url": "/_static/switcher.json",
         "version_match": version,
     },
     "use_edit_page_button": True,
     "use_issues_button": True,
     "use_repository_button": True,
 }
 # suggest edit link
 # remark: {{ file_name }} is mandatory in "edit_page_url_template"
-html_context = {  # TODO: verify html_context usage in theme
-    "edit_page_url_template": "https://6.docs.plone.org/contributing/index.html?{{ file_name }}#making-contributions-on-github",
+html_context = {  # TODO: verify html_context usage in plone-sphinx-theme
+    "edit_page_url_template": "https://github.com/plone/plone-sphinx-theme/edit/main/docs/{{ file_name }}",
 }
 
 # Announce that we have an opensearch plugin
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_use_opensearch
-html_use_opensearch = "https://6.docs.plone.org"  # TODO: Confirm usage of opensearch in theme
+html_use_opensearch = "https://plone-sphinx-theme.readthedocs.io"  # TODO: Confirm usage of opensearch in theme
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
 html_title = "%(project)s v%(release)s" % {"project": project, "release": release}
 
 # If false, no index is generated.
 html_use_index = True
@@ -257,19 +255,33 @@
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = [
     "_static",  # Last path wins. See https://github.com/plone/documentation/pull/1442
 ]
 
+
+# -- Options for autodoc ----------------------------------------------------
+
+# https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#configuration
+# Automatically extract typehints when specified and place them in
+# descriptions of the relevant function/method.
+# autodoc_typehints = "description"
+
+# Don't show class signature with the class' name.
+autodoc_class_signature = "separated"
+
+
 # -- Options for sphinx_sitemap to html -----------------------------
+
 # Used by sphinx_sitemap to generate a sitemap
-html_baseurl = "https://6.docs.plone.org/"
+html_baseurl = "https://plone-sphinx-theme.readthedocs.io/"
 # https://sphinx-sitemap.readthedocs.io/en/latest/advanced-configuration.html#customizing-the-url-scheme
 sitemap_url_scheme = "{link}"
+sitemap_filename = "sitemap-custom.xml"
 
 # -- Options for myST markdown conversion to html -----------------------------
 
 # For more information see:
 # https://myst-parser.readthedocs.io/en/latest/syntax/optional.html
 myst_enable_extensions = [
     "deflist",  # Support definition lists.
@@ -316,17 +328,17 @@
 
 
 # -- GraphViz configuration ----------------------------------
 graphviz_output_format = "svg"
 
 
 # -- OpenGraph configuration ----------------------------------
-ogp_site_url = "https://6.docs.plone.org/"
+ogp_site_url = "https://plone-sphinx-theme.readthedocs.io/"
 ogp_description_length = 200
-ogp_image = "https://6.docs.plone.org/_static/Plone_logo_square.png"
+ogp_image = "https://plone-sphinx-theme.readthedocs.io/_static/Plone_logo_square.png"
 ogp_site_name = "Plone Sphinx Theme Documentation"
 ogp_type = "website"
 ogp_custom_meta_tags = [
     '<meta property="og:locale" content="en_US" />',
 ]
 
 
@@ -383,15 +395,15 @@
     for key in app.config.source_replacements:
         result = result.replace(key, app.config.source_replacements[key])
     source[0] = result
 
 # Dict of replacements.
 source_replacements = {
     "{PLONE_BACKEND_MINOR_VERSION}": "6.0",
-    "{PLONE_BACKEND_PATCH_VERSION}": "6.0.10.1",
+    "{PLONE_BACKEND_PATCH_VERSION}": "6.0.11",
     "{NVM_VERSION}": "0.39.5",
     "{SUPPORTED_PYTHON_VERSIONS}": "3.8, 3.9, 3.10, 3.11, or 3.12",
 }
 
 
 # Finally, configure app attributes.
 def setup(app):
```

### Comparing `plone_sphinx_theme-0.0.2/docs/glossary.md` & `plone_sphinx_theme-0.0.3/docs/glossary.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,21 @@
   html_meta:
     "description": "Terms and definitions used throughout the Plone Sphinx Theme documentation."
     "property=og:description": "Terms and definitions used throughout the Plone Sphinx Theme documentation."
     "property=og:title": "Glossary"
     "keywords": "Plone, documentation, glossary, term, definition"
 ---
 
+(glossary-label)=
+
 # Glossary
 
+```{glossary}
+:sorted: true
+
 Sphinx
     [Sphinx](https://www.sphinx-doc.org/en/master/) is a tool that makes it easy to create intelligent and beautiful documentation.
     It was originally created for Python documentation, and it has excellent facilities for the documentation of software projects in a range of languages.
     Sphinx uses {term}`reStructuredText` as its markup language, and many of its strengths come from the power and straightforwardness of reStructuredText and its parsing and translating suite, {term}`Docutils`.
 
 Docutils
     [Docutils](https://docutils.sourceforge.io/) is an open-source text processing system for processing plain text documentation into useful formats, such as HTML, LaTeX, man-pages, OpenDocument, or XML.
@@ -49,7 +54,8 @@
     ```
     ````
 
 Open Graph
     The [Open Graph protocol](https://ogp.me/) enables any web page to become a rich object in a social graph.
     For instance, this is used on Facebook to allow any web page to have the same functionality as any other object on Facebook.
 
+```
```

### Comparing `plone_sphinx_theme-0.0.2/docs/guides/contribute.md` & `plone_sphinx_theme-0.0.3/docs/guides/contribute.md`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/docs/guides/contributing-policies.md` & `plone_sphinx_theme-0.0.3/docs/guides/contributing-policies.md`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/docs/guides/develop.md` & `plone_sphinx_theme-0.0.3/docs/guides/develop.md`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/docs/guides/usage.md` & `plone_sphinx_theme-0.0.3/docs/guides/usage.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "property=og:title": "Plone Sphinx Theme usage guide"
     "keywords": "Plone, Sphinx, Theme, plone-sphinx-theme, usage, guide"
 ---
 
 # Usage
 
 This guide describes how to use Plone Sphinx Theme for documentation of your project.
-By following this guide, you can consistently reproduce results in any environment, including to Read the Docs, Netlify, or GitHub Pages.
+By following this guide, you can consistently reproduce results in any environment, including to Read the Docs.
 
 ```{seealso}
 To contribute code to Plone Sphinx Theme, first follow the {doc}`contributing-policies`, then {doc}`contribute`.
 To develop your own theme based upon Plone Sphinx Theme, see {doc}`develop`.
 ```
```

### Comparing `plone_sphinx_theme-0.0.2/docs/index.md` & `plone_sphinx_theme-0.0.3/docs/index.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # Plone Sphinx Theme
 
 [Plone Sphinx Theme](https://github.com/plone/plone-sphinx-theme) is the official Sphinx theme for [documentation of Plone 6](https://6.docs.plone.org/), [Plone Conference trainings](https://training.plone.org/), and documentation of various Plone packages.
 
 It uses [Markedly Structured Text (MyST)](https://myst-parser.readthedocs.io/en/latest/), a rich and extensible flavor of Markdown for authoring documentation that combines the simplicity of CommonMark with the features of reStructuredText.
 
-Plone Sphinx Theme requires Python 3.10, 3.11, or 3.12.
+Plone Sphinx Theme requires Python 3.9, 3.10, 3.11, or 3.12.
 
 
 ```{todo}
 `plone/cookie-documentation` generates a customized project based on `plone/plone-sphinx-theme`.
 ```
 
  ```{toctree}
```

### Comparing `plone_sphinx_theme-0.0.2/docs/reference/extensions.md` & `plone_sphinx_theme-0.0.3/docs/reference/extensions.md`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/docs/reference/file-system-structure.md` & `plone_sphinx_theme-0.0.3/docs/reference/file-system-structure.md`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/docs/reference/kitchen-sink/admonitions.rst` & `plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/admonitions.rst`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/docs/reference/kitchen-sink/api.rst` & `plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/api.rst`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/docs/reference/kitchen-sink/blocks.rst` & `plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/blocks.rst`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/docs/reference/kitchen-sink/generic.rst` & `plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/generic.rst`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/docs/reference/kitchen-sink/images.rst` & `plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/images.rst`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/docs/reference/kitchen-sink/index.rst` & `plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/index.rst`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/docs/reference/kitchen-sink/lists.rst` & `plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/lists.rst`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/docs/reference/kitchen-sink/really-long.rst` & `plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/really-long.rst`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/docs/reference/kitchen-sink/structure.rst` & `plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/structure.rst`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/docs/reference/kitchen-sink/tables.rst` & `plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/tables.rst`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/docs/reference/kitchen-sink/typography.rst` & `plone_sphinx_theme-0.0.3/docs/reference/kitchen-sink/typography.rst`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/docs/reference/special-theme-elements.md` & `plone_sphinx_theme-0.0.3/docs/reference/special-theme-elements.md`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/package.json` & `plone_sphinx_theme-0.0.3/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -6,16 +6,16 @@
     },
     "devDependencies": {
         "css-loader": "^3.4.2",
         "dedent": "^0.7.0",
         "extract-loader": "^4.0.3",
         "file-loader": "^5.0.2",
         "html-webpack-plugin": "^4.3.0",
-        "sass": "^1.75.0",
         "optimize-css-assets-webpack-plugin": "^5.0.3",
+        "sass": "^1.75.0",
         "sass-loader": "^10.1.1",
         "style-loader": "^1.1.3",
         "webpack": "^4.41.6",
         "webpack-cli": "^3.3.11",
         "webpack-dev-server": "^3.10.3"
     },
     "dependencies": {
```

### Comparing `plone_sphinx_theme-0.0.2/pyproject.toml` & `plone_sphinx_theme-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
   "pip==24.0",
   "setuptools==69.5.1",
   "wheel==0.43.0",
 ]
 doc = [
   "graphviz",
   "linkify-it-py",
-  "myst_parser",
+  "myst-parser",
   "sphinx-autobuild",
   "sphinx-copybutton",
   "sphinx-design",
   "sphinx-examples",
   "sphinx-notfound-page",
   "sphinx-reredirects",
   "sphinx-sitemap",
@@ -120,14 +120,19 @@
 directory = "news/"
 title_format = "{version} ({project_date})"
 # First underline is used for version/date header.
 # Second underline is used for the type names (like 'Bug fixes:').
 underlines = ["-", ""]
 
 [[tool.towncrier.type]]
+directory = "internal"
+name = "Internal changes:"
+showcontent = true
+
+[[tool.towncrier.type]]
 directory = "breaking"
 name = "Breaking changes:"
 showcontent = true
 
 [[tool.towncrier.type]]
 directory = "feature"
 name = "New features:"
```

### Comparing `plone_sphinx_theme-0.0.2/scripts/kitchen_sink_update.py` & `plone_sphinx_theme-0.0.3/scripts/kitchen_sink_update.py`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/scripts/sbt_styles_update.py` & `plone_sphinx_theme-0.0.3/scripts/sbt_styles_update.py`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/__init__.py` & `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 import os
 from pathlib import Path
 
 from sphinx.application import Sphinx
 from sphinx.util import logging
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 from sphinx_book_theme import update_context_with_repository_info, update_sourcename
 
 logger = logging.getLogger(__name__)
 
 
 def get_html_theme_path():
```

### Comparing `plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/scripts/index.js` & `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/scripts/index.js`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/abstracts/_mixins.scss` & `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/abstracts/_mixins.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/abstracts/_variables.scss` & `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/abstracts/_variables.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/base/_base.scss` & `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/base/_base.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/base/_print.scss` & `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/base/_print.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/abstracts/_mixins.scss` & `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/abstracts/_mixins.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/abstracts/_variables.scss` & `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/abstracts/_variables.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/_base.scss` & `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/_base.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/_print.scss` & `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/_print.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/_typography.scss` & `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/base/_typography.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/components/_search.scss` & `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/components/_search.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_images.scss` & `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_images.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_margin.scss` & `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/content/_margin.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/index.scss` & `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/index.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_article-container.scss` & `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_article-container.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_header-article.scss` & `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_header-article.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_sidebar-primary.scss` & `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_sidebar-primary.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_sidebar-secondary.scss` & `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/assets/styles/sphinx-book-theme/sections/_sidebar-secondary.scss`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/src/plone_sphinx_theme/theme/plone-sphinx-theme/404.html` & `plone_sphinx_theme-0.0.3/src/plone_sphinx_theme/theme/plone-sphinx-theme/404.html`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/styles/Vocab/Plone/accept.txt` & `plone_sphinx_theme-0.0.3/styles/Vocab/Plone/accept.txt`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/webpack.config.js` & `plone_sphinx_theme-0.0.3/webpack.config.js`

 * *Files identical despite different names*

### Comparing `plone_sphinx_theme-0.0.2/PKG-INFO` & `plone_sphinx_theme-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone-sphinx-theme
-Version: 0.0.2
+Version: 0.0.3
 Summary: Plone Sphinx Theme is the official Sphinx theme for Plone 6 Documentation, Plone Conference Training, and documentation of various Plone packages.
 Keywords: Plone,Sphinx,Theme,documentation,training,Diátaxis
 Author-Email: Steve Piercy <spiercy@plone.org>
 Maintainer-Email: Steve Piercy <spiercy@plone.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
@@ -361,15 +361,15 @@
 Requires-Dist: sphinx>=7
 Requires-Dist: sphinx-book-theme>=1.1.2
 Requires-Dist: pip==24.0; extra == "initial"
 Requires-Dist: setuptools==69.5.1; extra == "initial"
 Requires-Dist: wheel==0.43.0; extra == "initial"
 Requires-Dist: graphviz; extra == "doc"
 Requires-Dist: linkify-it-py; extra == "doc"
-Requires-Dist: myst_parser; extra == "doc"
+Requires-Dist: myst-parser; extra == "doc"
 Requires-Dist: sphinx-autobuild; extra == "doc"
 Requires-Dist: sphinx-copybutton; extra == "doc"
 Requires-Dist: sphinx-design; extra == "doc"
 Requires-Dist: sphinx-examples; extra == "doc"
 Requires-Dist: sphinx-notfound-page; extra == "doc"
 Requires-Dist: sphinx-reredirects; extra == "doc"
 Requires-Dist: sphinx-sitemap; extra == "doc"
@@ -391,21 +391,28 @@
 plone-sphinx-theme is a Sphinx theme for [Plone 6 Documentation](https://6.docs.plone.org/), [Plone Conference Training](https://training.plone.org/), and documentation of various Plone packages.
 
 It is based on [`sphinx-book-theme`](https://sphinx-book-theme.readthedocs.io/en/latest/), which in turn is based on [`pydata-sphinx-theme`](https://pydata-sphinx-theme.readthedocs.io/en/stable/).
 
 
 ## Requirements
 
--   Python 3.10, 3.11, or 3.12
+-   Python 3.9, 3.10, 3.11, or 3.12
 -   GNU Make is required only for contributing to or development of this theme.
 
 
-## Documentation and demonstration
+## Documentation
 
-TODO:
+Documentation is hosted on Read the Docs.
+
+https://plone-sphinx-theme.readthedocs.io/
+
+
+## Demonstration
+
+TODO: Add reference to documentation permanent URL.
 
 To build documentation and a demonstration of this project, you can use `make` commands.
 
 
 ## Releasing
 
 Run the following command.
```

