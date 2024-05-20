# Comparing `tmp/protein_turnover_website-0.4.0.tar.gz` & `tmp/protein_turnover_website-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protein_turnover_website-0.4.0.tar", max compression
+gzip compressed data, was "protein_turnover_website-0.4.1.tar", max compression
```

## Comparing `protein_turnover_website-0.4.0.tar` & `protein_turnover_website-0.4.1.tar`

### file list

```diff
@@ -1,86 +1,87 @@
--rw-r--r--   0        0        0     1068 2024-05-17 07:06:31.689753 protein_turnover_website-0.4.0/LICENSE
--rw-r--r--   0        0        0       54 2024-05-17 06:43:03.102172 protein_turnover_website-0.4.0/prerelease.md
--rw-r--r--   0        0        0        0 2022-07-26 04:07:22.266032 protein_turnover_website-0.4.0/protein_turnover_website/__init__.py
--rw-r--r--   0        0        0     2703 2024-04-30 05:50:34.065016 protein_turnover_website-0.4.0/protein_turnover_website/app.py
--rw-r--r--   0        0        0     3093 2023-11-02 07:02:15.299192 protein_turnover_website-0.4.0/protein_turnover_website/cdn.toml
--rw-r--r--   0        0        0     2348 2024-05-13 17:45:54.986841 protein_turnover_website-0.4.0/protein_turnover_website/commands.py
--rw-r--r--   0        0        0     2326 2024-05-19 05:48:07.744329 protein_turnover_website-0.4.0/protein_turnover_website/config.py
--rw-r--r--   0        0        0        0 2022-07-26 22:24:13.364615 protein_turnover_website-0.4.0/protein_turnover_website/explorer/__init__.py
--rw-r--r--   0        0        0    11154 2024-05-19 02:18:48.498784 protein_turnover_website-0.4.0/protein_turnover_website/explorer/explorer.py
--rw-r--r--   0        0        0     1973 2024-02-09 01:57:57.957617 protein_turnover_website-0.4.0/protein_turnover_website/explorer/explorer_view.py
--rw-r--r--   0        0        0     1402 2022-10-04 02:27:11.831477 protein_turnover_website-0.4.0/protein_turnover_website/explorer/templates/explorer-test.html
--rw-r--r--   0        0        0      684 2022-10-02 08:18:42.820693 protein_turnover_website-0.4.0/protein_turnover_website/explorer/templates/explorer.css
--rw-r--r--   0        0        0     2707 2024-02-09 05:14:34.573665 protein_turnover_website-0.4.0/protein_turnover_website/explorer/templates/explorer.html
--rw-r--r--   0        0        0     4743 2024-05-17 09:19:50.799202 protein_turnover_website-0.4.0/protein_turnover_website/explorer/templates/explorer.js
--rw-r--r--   0        0        0     5554 2024-02-09 02:01:08.107049 protein_turnover_website-0.4.0/protein_turnover_website/explorer/templates/explorer.ts
--rw-r--r--   0        0        0     5042 2024-05-19 03:27:01.503075 protein_turnover_website-0.4.0/protein_turnover_website/flask_utils.py
--rw-r--r--   0        0        0      618 2024-04-28 01:18:02.953935 protein_turnover_website-0.4.0/protein_turnover_website/index_view.py
--rw-r--r--   0        0        0    14385 2024-04-26 00:38:41.221557 protein_turnover_website-0.4.0/protein_turnover_website/inspect.py
--rw-r--r--   0        0        0     7914 2024-05-18 20:07:47.125646 protein_turnover_website-0.4.0/protein_turnover_website/inspect_view.py
--rw-r--r--   0        0        0     6632 2024-05-19 02:41:27.270572 protein_turnover_website-0.4.0/protein_turnover_website/jobs.py
--rw-r--r--   0        0        0     9560 2024-05-19 02:41:18.226491 protein_turnover_website-0.4.0/protein_turnover_website/jobs_view.py
--rw-r--r--   0        0        0    11506 2024-05-19 02:09:12.917842 protein_turnover_website-0.4.0/protein_turnover_website/jobsmanager.py
--rw-r--r--   0        0        0     2982 2024-05-19 03:34:25.959094 protein_turnover_website-0.4.0/protein_turnover_website/logger.py
--rw-r--r--   0        0        0        0 2022-08-17 09:28:39.309757 protein_turnover_website-0.4.0/protein_turnover_website/login/__init__.py
--rw-r--r--   0        0        0     4024 2024-04-16 00:47:38.985633 protein_turnover_website-0.4.0/protein_turnover_website/login/login_view.py
--rw-r--r--   0        0        0     1609 2022-10-04 02:27:11.839478 protein_turnover_website-0.4.0/protein_turnover_website/login/templates/login.html
--rw-r--r--   0        0        0      808 2024-05-17 09:19:50.803202 protein_turnover_website-0.4.0/protein_turnover_website/login/templates/login.js
--rw-r--r--   0        0        0      842 2023-11-02 07:02:15.299192 protein_turnover_website-0.4.0/protein_turnover_website/login/templates/login.ts
--rw-r--r--   0        0        0        0 2022-11-08 03:47:29.541934 protein_turnover_website-0.4.0/protein_turnover_website/sqla/__init__.py
--rw-r--r--   0        0        0     5657 2024-05-19 02:10:05.778296 protein_turnover_website-0.4.0/protein_turnover_website/sqla/export.py
--rw-r--r--   0        0        0      963 2024-03-11 07:57:30.587258 protein_turnover_website-0.4.0/protein_turnover_website/sqla/export.toml
--rw-r--r--   0        0        0    10772 2024-03-31 22:43:01.586988 protein_turnover_website-0.4.0/protein_turnover_website/sqla/inspect.py
--rw-r--r--   0        0        0      679 2024-03-28 12:14:06.794706 protein_turnover_website-0.4.0/protein_turnover_website/sqla/peptides.toml
--rw-r--r--   0        0        0      588 2023-11-13 22:21:06.788496 protein_turnover_website-0.4.0/protein_turnover_website/sqla/proteins.toml
--rw-r--r--   0        0        0    15025 2022-07-26 04:49:46.758869 protein_turnover_website-0.4.0/protein_turnover_website/static/img/UWA-Full-Hor-CMYK-wt-opt.svgz
--rw-r--r--   0        0        0    62042 2022-08-23 03:32:47.883547 protein_turnover_website-0.4.0/protein_turnover_website/static/img/about/eics.png
--rw-r--r--   0        0        0    43312 2022-08-23 03:28:30.649979 protein_turnover_website-0.4.0/protein_turnover_website/static/img/about/isotopeEnvelopes.png
--rw-r--r--   0        0        0     9576 2022-08-23 23:23:37.063505 protein_turnover_website-0.4.0/protein_turnover_website/static/img/about/labelledEnvelope.png
--rw-r--r--   0        0        0    32813 2023-03-14 02:49:15.755245 protein_turnover_website-0.4.0/protein_turnover_website/static/img/about/plotFittedEnvelopes.png
--rw-r--r--   0        0        0     2383 2022-07-26 04:50:41.527162 protein_turnover_website-0.4.0/protein_turnover_website/static/img/email-white.svgz
--rw-r--r--   0        0        0    32928 2022-08-12 06:39:23.045191 protein_turnover_website-0.4.0/protein_turnover_website/static/img/enrichment.png
--rw-r--r--   0        0        0    13430 2023-02-16 08:46:20.525798 protein_turnover_website-0.4.0/protein_turnover_website/static/img/nnls_residuals.png
--rw-r--r--   0        0        0    17346 2022-07-26 05:06:40.732228 protein_turnover_website-0.4.0/protein_turnover_website/static/img/turnover.png
--rw-r--r--   0        0        0   503303 2023-03-13 08:45:49.226525 protein_turnover_website-0.4.0/protein_turnover_website/static/img/wheat4.jpg
--rw-r--r--   0        0        0     9509 2024-05-13 18:00:04.667209 protein_turnover_website-0.4.0/protein_turnover_website/templates/about-frag.html
--rw-r--r--   0        0        0    14425 2024-05-13 12:39:23.043947 protein_turnover_website-0.4.0/protein_turnover_website/templates/about-orig.html
--rw-r--r--   0        0        0     1192 2024-05-13 17:57:38.180718 protein_turnover_website-0.4.0/protein_turnover_website/templates/about.html
--rw-r--r--   0        0        0     8911 2024-05-13 18:01:38.003934 protein_turnover_website-0.4.0/protein_turnover_website/templates/about.md.tplt
--rw-r--r--   0        0        0      291 2024-04-28 00:43:05.728911 protein_turnover_website-0.4.0/protein_turnover_website/templates/bad-file.html
--rw-r--r--   0        0        0     3571 2024-05-17 04:28:41.885275 protein_turnover_website-0.4.0/protein_turnover_website/templates/configuration.html
--rw-r--r--   0        0        0     1473 2024-04-28 00:40:29.487698 protein_turnover_website-0.4.0/protein_turnover_website/templates/errors/404.html
--rw-r--r--   0        0        0     5516 2024-04-08 03:50:35.047582 protein_turnover_website-0.4.0/protein_turnover_website/templates/filter-frag.html
--rw-r--r--   0        0        0      287 2023-11-03 03:27:24.219728 protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/beta.html
--rw-r--r--   0        0        0     7311 2022-07-26 04:16:32.500682 protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/email.svg
--rw-r--r--   0        0        0      485 2022-10-04 02:27:11.839478 protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/google.html
--rw-r--r--   0        0        0     1738 2023-11-03 22:30:22.219226 protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/macros.html
--rw-r--r--   0        0        0      885 2023-11-03 03:27:36.311873 protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/meta.html
--rw-r--r--   0        0        0      307 2022-07-26 04:16:32.500682 protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/offsite.svg
--rw-r--r--   0        0        0     3672 2024-02-14 06:31:18.938538 protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/range.css
--rw-r--r--   0        0        0      602 2024-02-14 07:36:27.479208 protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/range.html
--rw-r--r--   0        0        0     4011 2024-05-17 09:19:50.839203 protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/range.js
--rw-r--r--   0        0        0     4206 2024-02-20 02:42:42.591329 protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/range.ts
--rw-r--r--   0        0        0     1486 2022-10-04 02:27:11.835478 protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/theme.html
--rw-r--r--   0        0        0      446 2022-10-04 02:27:11.835478 protein_turnover_website-0.4.0/protein_turnover_website/templates/index.html
--rw-r--r--   0        0        0     2527 2024-05-17 09:19:50.807202 protein_turnover_website-0.4.0/protein_turnover_website/templates/inspect-download.js
--rw-r--r--   0        0        0     2755 2023-11-02 07:02:15.299192 protein_turnover_website-0.4.0/protein_turnover_website/templates/inspect-download.ts
--rw-r--r--   0        0        0     8373 2024-04-28 04:43:51.155619 protein_turnover_website-0.4.0/protein_turnover_website/templates/inspect.html
--rw-r--r--   0        0        0    12482 2024-05-17 09:19:50.823202 protein_turnover_website-0.4.0/protein_turnover_website/templates/inspect.js
--rw-r--r--   0        0        0    14319 2024-05-17 09:02:50.406196 protein_turnover_website-0.4.0/protein_turnover_website/templates/inspect.ts
--rw-r--r--   0        0        0     4614 2024-05-19 02:36:25.783854 protein_turnover_website-0.4.0/protein_turnover_website/templates/job-frag.html
--rw-r--r--   0        0        0     2789 2024-05-19 02:37:23.800371 protein_turnover_website-0.4.0/protein_turnover_website/templates/job-index.html
--rw-r--r--   0        0        0     3525 2024-05-17 09:19:50.827202 protein_turnover_website-0.4.0/protein_turnover_website/templates/job-index.js
--rw-r--r--   0        0        0     4153 2024-05-17 09:19:47.319160 protein_turnover_website-0.4.0/protein_turnover_website/templates/job-index.ts
--rw-r--r--   0        0        0    11736 2024-04-26 07:55:01.842002 protein_turnover_website-0.4.0/protein_turnover_website/templates/jobs.html
--rw-r--r--   0        0        0    12544 2024-05-17 09:19:50.835202 protein_turnover_website-0.4.0/protein_turnover_website/templates/jobs.js
--rw-r--r--   0        0        0    13944 2024-04-11 02:21:23.908714 protein_turnover_website-0.4.0/protein_turnover_website/templates/jobs.ts
--rw-r--r--   0        0        0     2517 2022-08-14 23:50:39.361001 protein_turnover_website-0.4.0/protein_turnover_website/templates/macros/spinner.html
--rw-r--r--   0        0        0      388 2024-04-29 01:16:09.377432 protein_turnover_website-0.4.0/protein_turnover_website/templates/print.css
--rw-r--r--   0        0        0    12753 2024-05-17 03:59:53.237173 protein_turnover_website-0.4.0/protein_turnover_website/templates/raw.html
--rw-r--r--   0        0        0     6508 2023-03-13 08:09:04.609138 protein_turnover_website-0.4.0/protein_turnover_website/templates/table_meta.html
--rw-r--r--   0        0        0      135 2024-04-29 00:49:29.828093 protein_turnover_website-0.4.0/protein_turnover_website/templates/view.html
--rw-r--r--   0        0        0     3945 2024-04-26 06:37:44.451865 protein_turnover_website-0.4.0/protein_turnover_website/utils.py
--rw-r--r--   0        0        0      261 2024-04-11 11:43:50.588696 protein_turnover_website-0.4.0/protein_turnover_website/wsgi.py
--rw-r--r--   0        0        0      123 2024-04-29 01:02:58.914559 protein_turnover_website-0.4.0/protein_turnover_website/wsgi_view.py
--rw-r--r--   0        0        0     1587 2024-05-19 09:01:03.011450 protein_turnover_website-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1304 1970-01-01 00:00:00.000000 protein_turnover_website-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-17 07:06:31.689753 protein_turnover_website-0.4.1/LICENSE
+-rw-r--r--   0        0        0       88 2024-05-20 06:23:33.667243 protein_turnover_website-0.4.1/prerelease.md
+-rw-r--r--   0        0        0        0 2022-07-26 04:07:22.266032 protein_turnover_website-0.4.1/protein_turnover_website/__init__.py
+-rw-r--r--   0        0        0     2703 2024-05-20 01:17:11.024519 protein_turnover_website-0.4.1/protein_turnover_website/app.py
+-rw-r--r--   0        0        0     3093 2023-11-02 07:02:15.299192 protein_turnover_website-0.4.1/protein_turnover_website/cdn.toml
+-rw-r--r--   0        0        0     2348 2024-05-13 17:45:54.986841 protein_turnover_website-0.4.1/protein_turnover_website/commands.py
+-rw-r--r--   0        0        0     1823 2024-05-20 01:20:59.904165 protein_turnover_website-0.4.1/protein_turnover_website/config.py
+-rw-r--r--   0        0        0        0 2022-07-26 22:24:13.364615 protein_turnover_website-0.4.1/protein_turnover_website/explorer/__init__.py
+-rw-r--r--   0        0        0    11154 2024-05-19 02:18:48.498784 protein_turnover_website-0.4.1/protein_turnover_website/explorer/explorer.py
+-rw-r--r--   0        0        0     1973 2024-02-09 01:57:57.957617 protein_turnover_website-0.4.1/protein_turnover_website/explorer/explorer_view.py
+-rw-r--r--   0        0        0     1402 2022-10-04 02:27:11.831477 protein_turnover_website-0.4.1/protein_turnover_website/explorer/templates/explorer-test.html
+-rw-r--r--   0        0        0      684 2022-10-02 08:18:42.820693 protein_turnover_website-0.4.1/protein_turnover_website/explorer/templates/explorer.css
+-rw-r--r--   0        0        0     2707 2024-02-09 05:14:34.573665 protein_turnover_website-0.4.1/protein_turnover_website/explorer/templates/explorer.html
+-rw-r--r--   0        0        0     4743 2024-05-17 09:19:50.799202 protein_turnover_website-0.4.1/protein_turnover_website/explorer/templates/explorer.js
+-rw-r--r--   0        0        0     5554 2024-02-09 02:01:08.107049 protein_turnover_website-0.4.1/protein_turnover_website/explorer/templates/explorer.ts
+-rw-r--r--   0        0        0     5098 2024-05-20 01:18:14.445598 protein_turnover_website-0.4.1/protein_turnover_website/flask_utils.py
+-rw-r--r--   0        0        0      618 2024-04-28 01:18:02.953935 protein_turnover_website-0.4.1/protein_turnover_website/index_view.py
+-rw-r--r--   0        0        0    14385 2024-04-26 00:38:41.221557 protein_turnover_website-0.4.1/protein_turnover_website/inspect.py
+-rw-r--r--   0        0        0     7914 2024-05-18 20:07:47.125646 protein_turnover_website-0.4.1/protein_turnover_website/inspect_view.py
+-rw-r--r--   0        0        0     6620 2024-05-20 00:17:43.302973 protein_turnover_website-0.4.1/protein_turnover_website/jobs.py
+-rw-r--r--   0        0        0     9560 2024-05-19 02:41:18.226491 protein_turnover_website-0.4.1/protein_turnover_website/jobs_view.py
+-rw-r--r--   0        0        0    11506 2024-05-19 02:09:12.917842 protein_turnover_website-0.4.1/protein_turnover_website/jobsmanager.py
+-rw-r--r--   0        0        0     2982 2024-05-19 03:34:25.959094 protein_turnover_website-0.4.1/protein_turnover_website/logger.py
+-rw-r--r--   0        0        0        0 2022-08-17 09:28:39.309757 protein_turnover_website-0.4.1/protein_turnover_website/login/__init__.py
+-rw-r--r--   0        0        0     4024 2024-04-16 00:47:38.985633 protein_turnover_website-0.4.1/protein_turnover_website/login/login_view.py
+-rw-r--r--   0        0        0     1609 2022-10-04 02:27:11.839478 protein_turnover_website-0.4.1/protein_turnover_website/login/templates/login.html
+-rw-r--r--   0        0        0      808 2024-05-17 09:19:50.803202 protein_turnover_website-0.4.1/protein_turnover_website/login/templates/login.js
+-rw-r--r--   0        0        0      842 2023-11-02 07:02:15.299192 protein_turnover_website-0.4.1/protein_turnover_website/login/templates/login.ts
+-rw-r--r--   0        0        0      607 2024-05-20 06:22:00.302711 protein_turnover_website-0.4.1/protein_turnover_website/non_user_config.py
+-rw-r--r--   0        0        0        0 2022-11-08 03:47:29.541934 protein_turnover_website-0.4.1/protein_turnover_website/sqla/__init__.py
+-rw-r--r--   0        0        0     5657 2024-05-19 02:10:05.778296 protein_turnover_website-0.4.1/protein_turnover_website/sqla/export.py
+-rw-r--r--   0        0        0      963 2024-03-11 07:57:30.587258 protein_turnover_website-0.4.1/protein_turnover_website/sqla/export.toml
+-rw-r--r--   0        0        0    10772 2024-03-31 22:43:01.586988 protein_turnover_website-0.4.1/protein_turnover_website/sqla/inspect.py
+-rw-r--r--   0        0        0      679 2024-03-28 12:14:06.794706 protein_turnover_website-0.4.1/protein_turnover_website/sqla/peptides.toml
+-rw-r--r--   0        0        0      588 2023-11-13 22:21:06.788496 protein_turnover_website-0.4.1/protein_turnover_website/sqla/proteins.toml
+-rw-r--r--   0        0        0    15025 2022-07-26 04:49:46.758869 protein_turnover_website-0.4.1/protein_turnover_website/static/img/UWA-Full-Hor-CMYK-wt-opt.svgz
+-rw-r--r--   0        0        0    62042 2022-08-23 03:32:47.883547 protein_turnover_website-0.4.1/protein_turnover_website/static/img/about/eics.png
+-rw-r--r--   0        0        0    43312 2022-08-23 03:28:30.649979 protein_turnover_website-0.4.1/protein_turnover_website/static/img/about/isotopeEnvelopes.png
+-rw-r--r--   0        0        0     9576 2022-08-23 23:23:37.063505 protein_turnover_website-0.4.1/protein_turnover_website/static/img/about/labelledEnvelope.png
+-rw-r--r--   0        0        0    32813 2023-03-14 02:49:15.755245 protein_turnover_website-0.4.1/protein_turnover_website/static/img/about/plotFittedEnvelopes.png
+-rw-r--r--   0        0        0     2383 2022-07-26 04:50:41.527162 protein_turnover_website-0.4.1/protein_turnover_website/static/img/email-white.svgz
+-rw-r--r--   0        0        0    32928 2022-08-12 06:39:23.045191 protein_turnover_website-0.4.1/protein_turnover_website/static/img/enrichment.png
+-rw-r--r--   0        0        0    13430 2023-02-16 08:46:20.525798 protein_turnover_website-0.4.1/protein_turnover_website/static/img/nnls_residuals.png
+-rw-r--r--   0        0        0    17346 2022-07-26 05:06:40.732228 protein_turnover_website-0.4.1/protein_turnover_website/static/img/turnover.png
+-rw-r--r--   0        0        0   503303 2023-03-13 08:45:49.226525 protein_turnover_website-0.4.1/protein_turnover_website/static/img/wheat4.jpg
+-rw-r--r--   0        0        0     9562 2024-05-19 20:34:14.819633 protein_turnover_website-0.4.1/protein_turnover_website/templates/about-frag.html
+-rw-r--r--   0        0        0    14425 2024-05-13 12:39:23.043947 protein_turnover_website-0.4.1/protein_turnover_website/templates/about-orig.html
+-rw-r--r--   0        0        0     1192 2024-05-13 17:57:38.180718 protein_turnover_website-0.4.1/protein_turnover_website/templates/about.html
+-rw-r--r--   0        0        0     8999 2024-05-19 20:34:06.783560 protein_turnover_website-0.4.1/protein_turnover_website/templates/about.md.tplt
+-rw-r--r--   0        0        0      291 2024-04-28 00:43:05.728911 protein_turnover_website-0.4.1/protein_turnover_website/templates/bad-file.html
+-rw-r--r--   0        0        0     3571 2024-05-20 00:45:07.287534 protein_turnover_website-0.4.1/protein_turnover_website/templates/configuration.html
+-rw-r--r--   0        0        0     1473 2024-04-28 00:40:29.487698 protein_turnover_website-0.4.1/protein_turnover_website/templates/errors/404.html
+-rw-r--r--   0        0        0     5516 2024-04-08 03:50:35.047582 protein_turnover_website-0.4.1/protein_turnover_website/templates/filter-frag.html
+-rw-r--r--   0        0        0      287 2023-11-03 03:27:24.219728 protein_turnover_website-0.4.1/protein_turnover_website/templates/fragments/beta.html
+-rw-r--r--   0        0        0     7311 2022-07-26 04:16:32.500682 protein_turnover_website-0.4.1/protein_turnover_website/templates/fragments/email.svg
+-rw-r--r--   0        0        0      485 2022-10-04 02:27:11.839478 protein_turnover_website-0.4.1/protein_turnover_website/templates/fragments/google.html
+-rw-r--r--   0        0        0     1738 2023-11-03 22:30:22.219226 protein_turnover_website-0.4.1/protein_turnover_website/templates/fragments/macros.html
+-rw-r--r--   0        0        0      885 2023-11-03 03:27:36.311873 protein_turnover_website-0.4.1/protein_turnover_website/templates/fragments/meta.html
+-rw-r--r--   0        0        0      307 2022-07-26 04:16:32.500682 protein_turnover_website-0.4.1/protein_turnover_website/templates/fragments/offsite.svg
+-rw-r--r--   0        0        0     3672 2024-02-14 06:31:18.938538 protein_turnover_website-0.4.1/protein_turnover_website/templates/fragments/range.css
+-rw-r--r--   0        0        0      602 2024-02-14 07:36:27.479208 protein_turnover_website-0.4.1/protein_turnover_website/templates/fragments/range.html
+-rw-r--r--   0        0        0     4011 2024-05-17 09:19:50.839203 protein_turnover_website-0.4.1/protein_turnover_website/templates/fragments/range.js
+-rw-r--r--   0        0        0     4206 2024-02-20 02:42:42.591329 protein_turnover_website-0.4.1/protein_turnover_website/templates/fragments/range.ts
+-rw-r--r--   0        0        0     1486 2022-10-04 02:27:11.835478 protein_turnover_website-0.4.1/protein_turnover_website/templates/fragments/theme.html
+-rw-r--r--   0        0        0      446 2022-10-04 02:27:11.835478 protein_turnover_website-0.4.1/protein_turnover_website/templates/index.html
+-rw-r--r--   0        0        0     2527 2024-05-17 09:19:50.807202 protein_turnover_website-0.4.1/protein_turnover_website/templates/inspect-download.js
+-rw-r--r--   0        0        0     2755 2023-11-02 07:02:15.299192 protein_turnover_website-0.4.1/protein_turnover_website/templates/inspect-download.ts
+-rw-r--r--   0        0        0     8373 2024-04-28 04:43:51.155619 protein_turnover_website-0.4.1/protein_turnover_website/templates/inspect.html
+-rw-r--r--   0        0        0    12482 2024-05-17 09:19:50.823202 protein_turnover_website-0.4.1/protein_turnover_website/templates/inspect.js
+-rw-r--r--   0        0        0    14319 2024-05-17 09:02:50.406196 protein_turnover_website-0.4.1/protein_turnover_website/templates/inspect.ts
+-rw-r--r--   0        0        0     4614 2024-05-19 02:36:25.783854 protein_turnover_website-0.4.1/protein_turnover_website/templates/job-frag.html
+-rw-r--r--   0        0        0     2789 2024-05-19 02:37:23.800371 protein_turnover_website-0.4.1/protein_turnover_website/templates/job-index.html
+-rw-r--r--   0        0        0     3525 2024-05-17 09:19:50.827202 protein_turnover_website-0.4.1/protein_turnover_website/templates/job-index.js
+-rw-r--r--   0        0        0     4153 2024-05-17 09:19:47.319160 protein_turnover_website-0.4.1/protein_turnover_website/templates/job-index.ts
+-rw-r--r--   0        0        0    11736 2024-04-26 07:55:01.842002 protein_turnover_website-0.4.1/protein_turnover_website/templates/jobs.html
+-rw-r--r--   0        0        0    12544 2024-05-17 09:19:50.835202 protein_turnover_website-0.4.1/protein_turnover_website/templates/jobs.js
+-rw-r--r--   0        0        0    13944 2024-04-11 02:21:23.908714 protein_turnover_website-0.4.1/protein_turnover_website/templates/jobs.ts
+-rw-r--r--   0        0        0     2517 2022-08-14 23:50:39.361001 protein_turnover_website-0.4.1/protein_turnover_website/templates/macros/spinner.html
+-rw-r--r--   0        0        0      388 2024-04-29 01:16:09.377432 protein_turnover_website-0.4.1/protein_turnover_website/templates/print.css
+-rw-r--r--   0        0        0    12753 2024-05-17 03:59:53.237173 protein_turnover_website-0.4.1/protein_turnover_website/templates/raw.html
+-rw-r--r--   0        0        0     6508 2023-03-13 08:09:04.609138 protein_turnover_website-0.4.1/protein_turnover_website/templates/table_meta.html
+-rw-r--r--   0        0        0      135 2024-04-29 00:49:29.828093 protein_turnover_website-0.4.1/protein_turnover_website/templates/view.html
+-rw-r--r--   0        0        0     3945 2024-04-26 06:37:44.451865 protein_turnover_website-0.4.1/protein_turnover_website/utils.py
+-rw-r--r--   0        0        0      261 2024-04-11 11:43:50.588696 protein_turnover_website-0.4.1/protein_turnover_website/wsgi.py
+-rw-r--r--   0        0        0      123 2024-04-29 01:02:58.914559 protein_turnover_website-0.4.1/protein_turnover_website/wsgi_view.py
+-rw-r--r--   0        0        0     1587 2024-05-20 01:35:24.459898 protein_turnover_website-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 protein_turnover_website-0.4.1/PKG-INFO
```

### Comparing `protein_turnover_website-0.4.0/LICENSE` & `protein_turnover_website-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/app.py` & `protein_turnover_website-0.4.1/protein_turnover_website/app.py`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/cdn.toml` & `protein_turnover_website-0.4.1/protein_turnover_website/cdn.toml`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/commands.py` & `protein_turnover_website-0.4.1/protein_turnover_website/commands.py`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/explorer/explorer.py` & `protein_turnover_website-0.4.1/protein_turnover_website/explorer/explorer.py`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/explorer/explorer_view.py` & `protein_turnover_website-0.4.1/protein_turnover_website/explorer/explorer_view.py`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/explorer/templates/explorer-test.html` & `protein_turnover_website-0.4.1/protein_turnover_website/explorer/templates/explorer-test.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/explorer/templates/explorer.css` & `protein_turnover_website-0.4.1/protein_turnover_website/explorer/templates/explorer.css`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/explorer/templates/explorer.html` & `protein_turnover_website-0.4.1/protein_turnover_website/explorer/templates/explorer.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/explorer/templates/explorer.js` & `protein_turnover_website-0.4.1/protein_turnover_website/explorer/templates/explorer.js`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/explorer/templates/explorer.ts` & `protein_turnover_website-0.4.1/protein_turnover_website/explorer/templates/explorer.ts`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/flask_utils.py` & `protein_turnover_website-0.4.1/protein_turnover_website/flask_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,20 @@
 
 
 def oktokill() -> bool:
     if current_user.is_authenticated:
         return True
     if current_app.config.get("WEBSITE_STATE", "multi_user") == "single_user":
         return True
-    return current_app.config.get("KILL_OK", False)
+    return current_app.config.get("CAN_KILL_JOBS", False)
 
 
 def config_app(config: Config) -> Config:
     config.from_object(f"{NAME}.config")
+    config.from_object(f"{NAME}.non_user_config")
     config.from_pyfile("turnover-web.cfg", silent=True)
     # we are running in embbed mode...
     # config.from_envvar("TURNOVER_SETTINGS", silent=True)
     if "TURNOVER_SETTINGS" in os.environ:
         config.from_file(os.environ["TURNOVER_SETTINGS"], load=tomllib.load, text=False)  # type: ignore
 
     return config
```

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/index_view.py` & `protein_turnover_website-0.4.1/protein_turnover_website/index_view.py`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/inspect.py` & `protein_turnover_website-0.4.1/protein_turnover_website/inspect.py`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/inspect_view.py` & `protein_turnover_website-0.4.1/protein_turnover_website/inspect_view.py`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/jobs.py` & `protein_turnover_website-0.4.1/protein_turnover_website/jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from protein_turnover.jobs import PeptideSettings
 from protein_turnover.jobs import TurnoverJob
 
 from .explorer.explorer import find_mountpoint_for
 from .explorer.explorer import get_mountpoints
 from .explorer.explorer import logger
 from .explorer.explorer import safe_repr
-from .flask_utils import oktokill as oktokill
+from .flask_utils import oktokill
 from .jobsmanager import JobsManager
 from .jobsmanager import PersonalJobsManager
 
 
 def oktokill_abort() -> None:
     if not oktokill():
         abort(404)
```

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/jobs_view.py` & `protein_turnover_website-0.4.1/protein_turnover_website/jobs_view.py`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/jobsmanager.py` & `protein_turnover_website-0.4.1/protein_turnover_website/jobsmanager.py`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/logger.py` & `protein_turnover_website-0.4.1/protein_turnover_website/logger.py`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/login/login_view.py` & `protein_turnover_website-0.4.1/protein_turnover_website/login/login_view.py`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/login/templates/login.html` & `protein_turnover_website-0.4.1/protein_turnover_website/login/templates/login.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/login/templates/login.js` & `protein_turnover_website-0.4.1/protein_turnover_website/login/templates/login.js`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/login/templates/login.ts` & `protein_turnover_website-0.4.1/protein_turnover_website/login/templates/login.ts`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/sqla/export.py` & `protein_turnover_website-0.4.1/protein_turnover_website/sqla/export.py`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/sqla/export.toml` & `protein_turnover_website-0.4.1/protein_turnover_website/sqla/export.toml`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/sqla/inspect.py` & `protein_turnover_website-0.4.1/protein_turnover_website/sqla/inspect.py`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/sqla/peptides.toml` & `protein_turnover_website-0.4.1/protein_turnover_website/sqla/peptides.toml`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/sqla/proteins.toml` & `protein_turnover_website-0.4.1/protein_turnover_website/sqla/proteins.toml`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/static/img/UWA-Full-Hor-CMYK-wt-opt.svgz` & `protein_turnover_website-0.4.1/protein_turnover_website/static/img/UWA-Full-Hor-CMYK-wt-opt.svgz`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/static/img/about/eics.png` & `protein_turnover_website-0.4.1/protein_turnover_website/static/img/about/eics.png`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/static/img/about/isotopeEnvelopes.png` & `protein_turnover_website-0.4.1/protein_turnover_website/static/img/about/isotopeEnvelopes.png`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/static/img/about/labelledEnvelope.png` & `protein_turnover_website-0.4.1/protein_turnover_website/static/img/about/labelledEnvelope.png`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/static/img/about/plotFittedEnvelopes.png` & `protein_turnover_website-0.4.1/protein_turnover_website/static/img/about/plotFittedEnvelopes.png`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/static/img/email-white.svgz` & `protein_turnover_website-0.4.1/protein_turnover_website/static/img/email-white.svgz`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/static/img/enrichment.png` & `protein_turnover_website-0.4.1/protein_turnover_website/static/img/enrichment.png`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/static/img/nnls_residuals.png` & `protein_turnover_website-0.4.1/protein_turnover_website/static/img/nnls_residuals.png`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/static/img/turnover.png` & `protein_turnover_website-0.4.1/protein_turnover_website/static/img/turnover.png`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/static/img/wheat4.jpg` & `protein_turnover_website-0.4.1/protein_turnover_website/static/img/wheat4.jpg`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/about-frag.html` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/about-frag.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <h2>Calculations</h2>
 <p>We are hunting for peptides that may have taken up heavy atom isotopes such
 as <sup>15</sup><code>N</code>. Since there can be anywhere from <code>0</code> to
 <code>maxIso</code> uptake of heavy atoms we need to search for a range
 of <code>mz</code>'s for each peptide.</p>
-<p><img alt="" src="/static/img/about/eics.png" /></p>
+<p><img alt="eics" src="/static/img/about/eics.png" /></p>
 <p>We try and fit a gaussian to the intensities of the peptide <em>without</em> isotopic enrichment</p>
 <p>$$\begin{equation}
 \text{monoFitParams} \equiv \text{minimize}[\mu,\sigma, k, b]
 = \sum_i \left(k \times
- e^{-( \text{retention-time}_i - \mu)^2/2 \sigma^2}
+e^{-( \text{retention-time}_i - \mu)^2/2 \sigma^2}
 + b - \text{intensity}^{o}_i \right)^2
 \end{equation}$$</p>
 <p>where $`\text{intensity}^{o}_{i}`$ are the intensities found for the peptide with no isotopic
 enrichment. (Actually we fit to a smoothed version of the intensities)</p>
 <p>We use quadrature to estimate the area under this curve.</p>
 <p>$$\begin{equation}
 A_{\text{o}} = \int_{l_b=\max(\mu_{opt} - 2 * \sigma_{opt} , rt_0)}^{u_b=\min(\mu_{opt} + 2 *
@@ -28,15 +28,15 @@
 \end{equation}$$</p>
 <p>$`A_o`$ is stored as <code>monoPeakArea</code>.</p>
 <h4>Estimating intensities of EICs</h4>
 <p>We now linearly fit the scatter plots of the heavy peptides with the base peptide.</p>
 <p>$$\begin{equation}
 I^{\text{[eic]}}_{rt} \sim \alpha^{\text{[eic]}} + \beta^{\text{[eic]}} I^{\text{mono}}_{rt}
 \end{equation}$$</p>
-<p><img alt="" src="/static/img/about/isotopeEnvelopes.png" /></p>
+<p><img alt="isotope envelopes" src="/static/img/about/isotopeEnvelopes.png" /></p>
 <p>Note that the <em>first</em> value of <code>isotopeEnvelopes</code> is based on an mz that
 has <em>negative</em> enrichment (at least theorectically!) as a check. (See
 the blue <span
     style="background-color:#1E90FF; width:1em; height: 1em; display:inline-block; opacity:1.0; border:0px"></span> line in the plot at top.)</p>
 <p>If we integrate this relationship on both sides over the retention time range
 we get an intensity relationship:</p>
 <p>$$\begin{equation}
@@ -119,15 +119,15 @@
 \begin{array}{c} \; \\ \times \mathbf{w} \end{array}
 \begin{array}{c} \; \\ \quad = \end{array}
 \begin{array}{c} \; \\ \quad \mathbf{A} \times \mathbf{w} \end{array}
 \begin{array}{c}  \; \\ \quad \sim \end{array}
 \begin{array}{c} \; \\ \quad \mathbf{I}^{exp} \end{array}
 \end{equation}$$</p>
 <p>With $`\mathbf{w} \ge 0`$ and $`\text{labelledEnvelopes} \equiv \mathbf{w}`$</p>
-<p><img alt="" src="/static/img/about/labelledEnvelope.png" /></p>
+<p><img alt="labeled envolopes" src="/static/img/about/labelledEnvelope.png" /></p>
 <p>If we turn the positive weights $`\mathbf{\hat{w}}`$ into fractions
 $`f_i = w_i / \sum_{i=0}^{N} w_i`$ then
 <code>LPF</code> $`\equiv \text{relativeIsotopeAbundance}`$ (an estimate of the fraction of
 <em>this peptide</em> that include some/any heavy atoms)
 $$\begin{equation}
 \text{relativeIsotopeAbundance} = 1 - f_0 = \sum_{i=1}^N f_i
 \end{equation}$$</p>
@@ -174,8 +174,8 @@
 <li><code>isotopeEnvelopes</code> is plotted as <span
     style="background-color:turquoise; width:1em; height: 1em; display:inline-block; opacity:0.4; border:1px solid
         black"></span></li>
 <li>the negative enrichment value <span
     style="background-color:red; width:1em; height: 1em; display:inline-block; opacity:0.4; border:0px"></span> is used to filter hits
         $`\frac{\text{isotopeEnvelopes}[0]}{\text{isotopeEnvelopes}[-1]} \ge \text{monoMinus1MinRatio}`$</li>
 </ul>
-<p><img alt="" src="/static/img/about/plotFittedEnvelopes.png" /></p>
+<p><img alt="fitted envelopes" src="/static/img/about/plotFittedEnvelopes.png" /></p>
```

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/about-orig.html` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/about-orig.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/about.html` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/about.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/about.md.tplt` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/about.md.tplt`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
 {%- macro colorbox(col, opacity=1.0, border='0px') -%}
 <span
     style="background-color:{{col}}; width:1em; height: 1em; display:inline-block; opacity:{{opacity}}; border:{{border}}"></span>
 {%- endmacro -%}
 
 
-{%- macro image(img) %}
-![]({{image_prefix}}/static/img/about/{{img}})
+{%- macro image(img,title='') %}
+![{{title}}]({{image_prefix}}/static/img/about/{{img}})
 {% endmacro -%}
 
 {%- if no_github -%}
 {% macro eqn() -%}
 $$\begin{equation}{{caller()}}\end{equation}$$
 {%- endmacro -%}
 {%- else -%}
@@ -25,15 +25,15 @@
 ## Calculations
 
 We are hunting for peptides that may have taken up heavy atom isotopes such
 as <sup>15</sup>`N`. Since there can be anywhere from `0` to
 `maxIso` uptake of heavy atoms we need to search for a range
 of `mz`'s for each peptide.
 
-{{ image('eics.png') }}
+{{ image('eics.png', "eics") }}
 
 We try and fit a gaussian to the intensities of the peptide *without* isotopic enrichment
 
 {% call eqn() %}
 \text{monoFitParams} \equiv \text{minimize}[\mu,\sigma, k, b]
 = \sum_i \left(k \times
 e^{-( \text{retention-time}_i - \mu)^2/2 \sigma^2}
@@ -65,15 +65,15 @@
 #### Estimating intensities of EICs
 We now linearly fit the scatter plots of the heavy peptides with the base peptide.
 
 {% call eqn() %}
 I^{\text{[eic]}}_{rt} \sim \alpha^{\text{[eic]}} + \beta^{\text{[eic]}} I^{\text{mono}}_{rt}
 {% endcall %}
 
-{{ image('isotopeEnvelopes.png') }}
+{{ image('isotopeEnvelopes.png', 'isotope envelopes') }}
 
 Note that the *first* value of `isotopeEnvelopes` is based on an mz that
 has *negative* enrichment (at least theorectically!) as a check. (See
 the blue {{colorbox("#1E90FF")}} line in the plot at top.)
 {# {% call eqn() %}
 \text{isotopeEnvelopes} = I^{\text{exp}}_i = A_{\text{o}} \times \max(0, \text{slope}_i)
 {% endcall %} #}
@@ -183,15 +183,15 @@
 \begin{array}{c} \; \\ \quad \mathbf{A} \times \mathbf{w} \end{array}
 \begin{array}{c}  \; \\ \quad \sim \end{array}
 \begin{array}{c} \; \\ \quad \mathbf{I}^{exp} \end{array}
 {% endcall %}
 
 With $`\mathbf{w} \ge 0`$ and $`\text{labelledEnvelopes} \equiv \mathbf{w}`$
 
-{{ image('labelledEnvelope.png') }}
+{{ image('labelledEnvelope.png', 'labeled envolopes') }}
 
 If we turn the positive weights $`\mathbf{\hat{w}}`$ into fractions
 $`f_i = w_i / \sum_{i=0}^{N} w_i`$ then
 `LPF` $`\equiv \text{relativeIsotopeAbundance}`$ (an estimate of the fraction of
 *this peptide* that include some/any heavy atoms)
 {% call eqn() %}
 \text{relativeIsotopeAbundance} = 1 - f_0 = \sum_{i=1}^N f_i
@@ -244,11 +244,11 @@
         is plotted as {{colorbox("#2c9cde", opacity=1)}}''
 * `isotopeEnvelopes` is plotted as {{colorbox("turquoise", opacity=0.4, border="1px solid
         black")}}
 * the negative enrichment value {{colorbox('red', opacity=0.4)}} is used to filter hits
         $`\frac{\text{isotopeEnvelopes}[0]}{\text{isotopeEnvelopes}[-1]} \ge \text{monoMinus1MinRatio}`$
 
 
-{{ image('plotFittedEnvelopes.png') }}
+{{ image('plotFittedEnvelopes.png', 'fitted envelopes') }}
 
 
 {% endblock content %}
```

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/configuration.html` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/configuration.html`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 <a id="configuration"></a>
 <h2 class="text-center">Configuring this Website</h2>
 <div class="w-75 mx-auto">
     <p>
         You should read the comments in <code>protein_turnover_website/config.py</code>.
         These should be set in
-        <code><a href="https://flask.palletsprojects.com/en/3.0.x/config/#instance-folders">instance/turnover_web.cfg</a></code>
+        <code><a href="https://flask.palletsprojects.com/en/3.0.x/config/#instance-folders">instance/turnover-web.cfg</a></code>
         if running a multi user website or <code>~/.turnover-web.cfg</code> if running as
         a single user site (e.g. as <code>turnover web</code>).
     <ul>
         <li>
             <code>JOBSDIR</code> = <code>"/path/to/jobs-directory"</code>
             <b>[required]</b> where job files live.
         </li>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {% extends base_template %} {% block title %}Configuration::{{config.APP_NAME}}
 {% endblock %} {% block content %}
 ********** CCoonnffiigguurriinngg tthhiiss WWeebbssiittee **********
 You should read the comments in protein_turnover_website/config.py. These
-should be set in _i_n_s_t_a_n_c_e_/_t_u_r_n_o_v_e_r___w_e_b_._c_f_g if running a multi user website or
+should be set in _i_n_s_t_a_n_c_e_/_t_u_r_n_o_v_e_r_-_w_e_b_._c_f_g if running a multi user website or
 ~/.turnover-web.cfg if running as a single user site (e.g. as turnover web).
     * JOBSDIR = "/path/to/jobs-directory" [[rreeqquuiirreedd]] where job files live.
     * CACHEDIR = "/path/to/cachedir" [[rreeqquuiirreedd]] where cache files live.
     * MOUNTPOINTS [[rreeqquuiirreedd]]. A list of directories visible to users of this
       website. Represented as a tuple of (/full/path/to/directory, nickname,
       optional regex *string* to restrict visible files). e.g.
       MOUNTPOINTS = [("/path/to/protein_turnover_data", "Turnover", r"^.*\.
```

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/errors/404.html` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/errors/404.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/filter-frag.html` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/filter-frag.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/email.svg` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/fragments/email.svg`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/macros.html` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/fragments/macros.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/meta.html` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/fragments/meta.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/range.css` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/fragments/range.css`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/range.html` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/fragments/range.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/range.js` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/fragments/range.js`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/range.ts` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/fragments/range.ts`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/fragments/theme.html` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/fragments/theme.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/inspect-download.js` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/inspect-download.js`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/inspect-download.ts` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/inspect-download.ts`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/inspect.html` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/inspect.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/inspect.js` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/inspect.js`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/inspect.ts` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/inspect.ts`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/job-frag.html` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/job-frag.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/job-index.html` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/job-index.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/job-index.js` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/job-index.js`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/job-index.ts` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/job-index.ts`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/jobs.html` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/jobs.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/jobs.js` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/jobs.js`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/jobs.ts` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/jobs.ts`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/macros/spinner.html` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/macros/spinner.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/raw.html` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/raw.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/templates/table_meta.html` & `protein_turnover_website-0.4.1/protein_turnover_website/templates/table_meta.html`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/protein_turnover_website/utils.py` & `protein_turnover_website-0.4.1/protein_turnover_website/utils.py`

 * *Files identical despite different names*

### Comparing `protein_turnover_website-0.4.0/pyproject.toml` & `protein_turnover_website-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "protein-turnover-website"
-version = "0.4.0"
+version = "0.4.1"
 description = "Protein Turnover web pipeline"
 authors = ["Ian Castleden <ian.castleden@uwa.edu.au>"]
 license = "MIT"
 readme = "prerelease.md"
 exclude = ["tests/**"]
 packages = [{ include = "protein_turnover_website" }]
 repository = "https://github.com/arabidopsis/protein_turnover_website.git"
@@ -24,15 +24,15 @@
 # for background job in protein_turnover
 psutil = ">=5.9"
 unidecode = "^1.3.8"
 
 # protein-turnover = { path = "../protein_turnover", develop = true }
 # poetry add git+ssh://git@github.com:arabidopsis/protein_turnover.git
 # protein-turnover = {git = "git@github.com:arabidopsis/protein_turnover.git"}
-protein-turnover = "^0.4.0"
+protein-turnover = "^0.4.1"
 typing-extensions = "^4.8"
 # these dependencies of protein_turnover
 tomli-w = ">=1.0.0"
 # for inspect
 tomli = ">=2.0.1"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `protein_turnover_website-0.4.0/PKG-INFO` & `protein_turnover_website-0.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protein-turnover-website
-Version: 0.4.0
+Version: 0.4.1
 Summary: Protein Turnover web pipeline
 Home-page: https://github.com/arabidopsis/protein_turnover_website.git
 License: MIT
 Author: Ian Castleden
 Author-email: ian.castleden@uwa.edu.au
 Requires-Python: >=3.10
 Classifier: Development Status :: 4 - Beta
@@ -15,21 +15,27 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Dist: Flask (>=3.0,<4.0)
 Requires-Dist: Flask-Login (>=0.6)
 Requires-Dist: openpyxl (>=3.0.10)
-Requires-Dist: protein-turnover (>=0.4.0,<0.5.0)
+Requires-Dist: protein-turnover (>=0.4.1,<0.5.0)
 Requires-Dist: psutil (>=5.9)
 Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
 Requires-Dist: tomli (>=2.0.1)
 Requires-Dist: tomli-w (>=1.0.0)
 Requires-Dist: typing-extensions (>=4.8,<5.0)
 Requires-Dist: unidecode (>=1.3.8,<2.0.0)
 Project-URL: Repository, https://github.com/arabidopsis/protein_turnover_website.git
 Description-Content-Type: text/markdown
 
 # Protein Turnover Pipeline
 
 More documentation soon.
 
+```math
+\lambda
+```
+
+$$\lambda$$
+
```

