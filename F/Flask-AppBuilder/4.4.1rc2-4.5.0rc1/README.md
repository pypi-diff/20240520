# Comparing `tmp/Flask-AppBuilder-4.4.1rc2.tar.gz` & `tmp/Flask-AppBuilder-4.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-AppBuilder-4.4.1rc2.tar", last modified: Fri Feb 23 13:58:21 2024, max compression
+gzip compressed data, was "Flask-AppBuilder-4.5.0rc1.tar", last modified: Mon May 20 14:54:24 2024, max compression
```

## Comparing `Flask-AppBuilder-4.4.1rc2.tar` & `Flask-AppBuilder-4.5.0rc1.tar`

### file list

```diff
@@ -1,1191 +1,1191 @@
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.386926 Flask-AppBuilder-4.4.1rc2/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       97 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/.coveragerc
--rw-r--r--   0 dpgaspar   (501) staff       (20)      113 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/.env
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.399242 Flask-AppBuilder-4.4.1rc2/.github/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      642 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 dpgaspar   (501) staff       (20)      681 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 dpgaspar   (501) staff       (20)      202 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/.github/prlint.json
--rw-r--r--   0 dpgaspar   (501) staff       (20)      709 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/.github/stale.yml
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.401272 Flask-AppBuilder-4.4.1rc2/.github/workflows/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8377 2024-02-19 10:55:30.000000 Flask-AppBuilder-4.4.1rc2/.github/workflows/ci.yml
--rw-r--r--   0 dpgaspar   (501) staff       (20)      137 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/.github/workflows/odbcinst.ini
--rw-r--r--   0 dpgaspar   (501) staff       (20)      951 2024-02-19 10:55:30.000000 Flask-AppBuilder-4.4.1rc2/.github/workflows/ptlint.yml
--rw-r--r--   0 dpgaspar   (501) staff       (20)      147 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/.gitignore
--rw-r--r--   0 dpgaspar   (501) staff       (20)    68631 2024-02-23 13:42:48.000000 Flask-AppBuilder-4.4.1rc2/CHANGELOG.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1926 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/CONTRIBUTING.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.405689 Flask-AppBuilder-4.4.1rc2/Flask_AppBuilder.egg-info/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7854 2024-02-23 13:58:20.000000 Flask-AppBuilder-4.4.1rc2/Flask_AppBuilder.egg-info/PKG-INFO
--rw-r--r--   0 dpgaspar   (501) staff       (20)    36584 2024-02-23 13:58:20.000000 Flask-AppBuilder-4.4.1rc2/Flask_AppBuilder.egg-info/SOURCES.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2024-02-23 13:58:20.000000 Flask-AppBuilder-4.4.1rc2/Flask_AppBuilder.egg-info/dependency_links.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)      109 2024-02-23 13:58:20.000000 Flask-AppBuilder-4.4.1rc2/Flask_AppBuilder.egg-info/entry_points.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-12 08:40:39.000000 Flask-AppBuilder-4.4.1rc2/Flask_AppBuilder.egg-info/not-zip-safe
--rw-r--r--   0 dpgaspar   (501) staff       (20)      571 2024-02-23 13:58:20.000000 Flask-AppBuilder-4.4.1rc2/Flask_AppBuilder.egg-info/requires.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)       17 2024-02-23 13:58:20.000000 Flask-AppBuilder-4.4.1rc2/Flask_AppBuilder.egg-info/top_level.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1493 2023-04-05 15:10:33.000000 Flask-AppBuilder-4.4.1rc2/LICENSE
--rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/MANIFEST.in
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7854 2024-02-23 13:58:21.387078 Flask-AppBuilder-4.4.1rc2/PKG-INFO
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6717 2023-11-20 09:17:41.000000 Flask-AppBuilder-4.4.1rc2/README.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)      506 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/RELEASE.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.406924 Flask-AppBuilder-4.4.1rc2/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)    36590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/babel/messages.pot
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.396713 Flask-AppBuilder-4.4.1rc2/bin/
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      176 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/bin/babel_extract.sh
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      104 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/bin/babel_init.sh
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      422 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/bin/bootswatch_update.sh
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1632 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/bin/config.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      493 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/bin/db_create.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      840 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/bin/db_migrate.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      309 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/bin/db_upgrade.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1419 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/bin/hash_db_password.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/bin/migrate_db_0.7.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)     4001 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/bin/migrate_db_1.3.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1917 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/bin/sqlite_upgrade_1.3.sql
--rw-r--r--   0 dpgaspar   (501) staff       (20)      999 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/docker-compose.yml
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.429542 Flask-AppBuilder-4.4.1rc2/docs/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6802 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/Makefile
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.430805 Flask-AppBuilder-4.4.1rc2/docs/_static/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    18838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/_static/Flask-AppBuilder.png
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.431826 Flask-AppBuilder-4.4.1rc2/docs/_templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      727 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/_templates/layout.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.433791 Flask-AppBuilder-4.4.1rc2/docs/_themes/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1789 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/_themes/LICENSE
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1093 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/_themes/README
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.435674 Flask-AppBuilder-4.4.1rc2/docs/_themes/flask/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      954 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/_themes/flask/layout.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/_themes/flask/relations.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.437002 Flask-AppBuilder-4.4.1rc2/docs/_themes/flask/static/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    18838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/_themes/flask/static/Flask-AppBuilder.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9062 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/_themes/flask/static/flasky.css_t
--rw-r--r--   0 dpgaspar   (501) staff       (20)      181 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/_themes/flask/theme.conf
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.438292 Flask-AppBuilder-4.4.1rc2/docs/_themes/flask_small/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      683 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/_themes/flask_small/layout.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.438908 Flask-AppBuilder-4.4.1rc2/docs/_themes/flask_small/static/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4609 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/_themes/flask_small/static/flasky.css_t
--rw-r--r--   0 dpgaspar   (501) staff       (20)      184 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/_themes/flask_small/theme.conf
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4875 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/_themes/flask_theme_support.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2277 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/actions.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3828 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/addons.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10881 2022-09-05 09:07:43.000000 Flask-AppBuilder-4.4.1rc2/docs/advanced.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4209 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/api.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4614 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/cli.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8834 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/conf.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)    33985 2024-02-12 14:22:00.000000 Flask-AppBuilder-4.4.1rc2/docs/config.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10806 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/customizing.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4109 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/diagrams.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3803 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/generic_datasource.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3835 2024-02-15 13:58:31.000000 Flask-AppBuilder-4.4.1rc2/docs/i18n.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.459523 Flask-AppBuilder-4.4.1rc2/docs/images/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   190476 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/images/ListThumbnail.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    63609 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/images/chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    33854 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/images/chart_time1.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    41838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/images/chart_time2.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    65563 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/images/charts.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   275455 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/images/contact_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    52500 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/images/contacts.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    32505 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/images/direct_chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2591 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/images/fab.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   144592 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/images/group_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    35236 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/images/grouped_chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    16975 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/images/groups.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   173978 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/images/images_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    13590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/images/list_cascade.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10792 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/images/list_cascade_block.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    51248 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/images/list_compact_inline.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    70360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/images/list_master_detail.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15868 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/images/login.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    86223 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/images/login_db.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    31562 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/images/login_oid.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    82437 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/images/oauth_login.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    48690 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/images/oauth_login_one_provider.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    42827 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/images/security.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15977 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/images/simpleview2.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    41274 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/images/swagger001.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    26185 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/images/swagger002.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1389 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.4.1rc2/docs/index.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4377 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.4.1rc2/docs/installation.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2634 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/intro.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6721 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/make.bat
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1464 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/multipledbs.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    11789 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/quickcharts.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/quickfiles.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    17711 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/quickhowto.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4829 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/quickhowto_mongo.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1676 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/quickminimal.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8990 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/relations.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    47345 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/docs/rest_api.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    39051 2024-02-15 13:58:31.000000 Flask-AppBuilder-4.4.1rc2/docs/security.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    17032 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/templates.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4335 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/user_registration.rst
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)    12302 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/versionmigration.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9036 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/docs/views.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.460212 Flask-AppBuilder-4.4.1rc2/examples/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2036 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.461428 Flask-AppBuilder-4.4.1rc2/examples/base_api/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      209 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/base_api/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.462635 Flask-AppBuilder-4.4.1rc2/examples/base_api/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      380 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/base_api/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3789 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/base_api/app/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1809 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/base_api/config.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.465710 Flask-AppBuilder-4.4.1rc2/examples/basefilter/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/basefilter/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      429 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/basefilter/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.467638 Flask-AppBuilder-4.4.1rc2/examples/basefilter/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      358 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/basefilter/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1458 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/basefilter/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.336648 Flask-AppBuilder-4.4.1rc2/examples/basefilter/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.336700 Flask-AppBuilder-4.4.1rc2/examples/basefilter/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.468886 Flask-AppBuilder-4.4.1rc2/examples/basefilter/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1413 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/basefilter/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.470735 Flask-AppBuilder-4.4.1rc2/examples/basefilter/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/basefilter/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/basefilter/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/basefilter/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1906 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/basefilter/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2423 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/basefilter/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.472636 Flask-AppBuilder-4.4.1rc2/examples/composite_keys/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      254 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/composite_keys/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.474673 Flask-AppBuilder-4.4.1rc2/examples/composite_keys/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      358 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/composite_keys/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1464 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/composite_keys/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1842 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/composite_keys/app/views.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2182 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/composite_keys/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1477 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/composite_keys/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.477857 Flask-AppBuilder-4.4.1rc2/examples/crud_rest_api/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/crud_rest_api/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      295 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/crud_rest_api/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.480179 Flask-AppBuilder-4.4.1rc2/examples/crud_rest_api/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/crud_rest_api/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2061 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/examples/crud_rest_api/app/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1804 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/examples/crud_rest_api/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.337163 Flask-AppBuilder-4.4.1rc2/examples/crud_rest_api/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.337217 Flask-AppBuilder-4.4.1rc2/examples/crud_rest_api/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.481775 Flask-AppBuilder-4.4.1rc2/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.483045 Flask-AppBuilder-4.4.1rc2/examples/crud_rest_api/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/crud_rest_api/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/crud_rest_api/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2460 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/examples/crud_rest_api/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2253 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/examples/crud_rest_api/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.485631 Flask-AppBuilder-4.4.1rc2/examples/dash/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      291 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/dash/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.487028 Flask-AppBuilder-4.4.1rc2/examples/dash/app/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.489786 Flask-AppBuilder-4.4.1rc2/examples/dash/app/Dashboard/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      797 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/dash/app/Dashboard/Dash_App1.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1256 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/dash/app/Dashboard/Dash_App2.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1568 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/dash/app/Dashboard/Dash_fun.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/dash/app/Dashboard/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      509 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/dash/app/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.490388 Flask-AppBuilder-4.4.1rc2/examples/dash/app/templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      701 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/dash/app/templates/dash.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1031 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/dash/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.491907 Flask-AppBuilder-4.4.1rc2/examples/dash/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/dash/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/dash/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/dash/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/dash/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.493570 Flask-AppBuilder-4.4.1rc2/examples/employees/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      276 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/employees/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.496522 Flask-AppBuilder-4.4.1rc2/examples/employees/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      711 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/employees/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/employees/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      574 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/employees/app/security.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1972 2022-09-05 09:07:43.000000 Flask-AppBuilder-4.4.1rc2/examples/employees/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.497462 Flask-AppBuilder-4.4.1rc2/examples/employees/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/employees/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1324 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/employees/config.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.500775 Flask-AppBuilder-4.4.1rc2/examples/enums/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/enums/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/enums/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.503143 Flask-AppBuilder-4.4.1rc2/examples/enums/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      358 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/enums/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1158 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/enums/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.338109 Flask-AppBuilder-4.4.1rc2/examples/enums/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.338177 Flask-AppBuilder-4.4.1rc2/examples/enums/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.504581 Flask-AppBuilder-4.4.1rc2/examples/enums/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/enums/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/enums/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3436 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/enums/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.505933 Flask-AppBuilder-4.4.1rc2/examples/enums/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/enums/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/enums/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2226 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/enums/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1841 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/enums/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.509633 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      614 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.514351 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      519 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2607 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      453 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/app/sec.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      880 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/app/sec_forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1923 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/app/sec_views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.338521 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.338572 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.515787 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1589 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.517942 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1961 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2977 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.521382 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      560 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.525637 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      435 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2831 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      453 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/app/sec.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      880 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/app/sec_forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1929 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/app/sec_views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.338910 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.338958 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.527071 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2133 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.528682 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1906 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2930 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.533309 Flask-AppBuilder-4.4.1rc2/examples/factoryapp/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/factoryapp/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      432 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.4.1rc2/examples/factoryapp/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.535573 Flask-AppBuilder-4.4.1rc2/examples/factoryapp/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.4.1rc2/examples/factoryapp/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/factoryapp/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.339316 Flask-AppBuilder-4.4.1rc2/examples/factoryapp/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.339371 Flask-AppBuilder-4.4.1rc2/examples/factoryapp/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.537175 Flask-AppBuilder-4.4.1rc2/examples/factoryapp/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2121 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.4.1rc2/examples/factoryapp/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.540446 Flask-AppBuilder-4.4.1rc2/examples/factoryapp/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/factoryapp/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/factoryapp/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/factoryapp/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1904 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.4.1rc2/examples/factoryapp/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1862 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/factoryapp/config2.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1867 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.4.1rc2/examples/factoryapp/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.542690 Flask-AppBuilder-4.4.1rc2/examples/issue_789/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1610 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/issue_789/README.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4740 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/issue_789/app.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.546684 Flask-AppBuilder-4.4.1rc2/examples/masterdetail/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/masterdetail/NAMES.DIC
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.550122 Flask-AppBuilder-4.4.1rc2/examples/masterdetail/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      351 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/masterdetail/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1164 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/masterdetail/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.339784 Flask-AppBuilder-4.4.1rc2/examples/masterdetail/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.339835 Flask-AppBuilder-4.4.1rc2/examples/masterdetail/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.552281 Flask-AppBuilder-4.4.1rc2/examples/masterdetail/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2711 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/masterdetail/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.555500 Flask-AppBuilder-4.4.1rc2/examples/masterdetail/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/masterdetail/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/masterdetail/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/masterdetail/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1870 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/masterdetail/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1519 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/masterdetail/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.560261 Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      251 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.564563 Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      573 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1803 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2531 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/app/mysecurity.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.340173 Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.340226 Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.566678 Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2988 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.568797 Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1652 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1396 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.574907 Flask-AppBuilder-4.4.1rc2/examples/mongoengine/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongoengine/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      251 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongoengine/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.578096 Flask-AppBuilder-4.4.1rc2/examples/mongoengine/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      508 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongoengine/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1613 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongoengine/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.340552 Flask-AppBuilder-4.4.1rc2/examples/mongoengine/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.340607 Flask-AppBuilder-4.4.1rc2/examples/mongoengine/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.580248 Flask-AppBuilder-4.4.1rc2/examples/mongoengine/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2623 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongoengine/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.583429 Flask-AppBuilder-4.4.1rc2/examples/mongoengine/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongoengine/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongoengine/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongoengine/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1652 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongoengine/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongoengine/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1396 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongoengine/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.589024 Flask-AppBuilder-4.4.1rc2/examples/mongoimages/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongoimages/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      296 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongoimages/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.592367 Flask-AppBuilder-4.4.1rc2/examples/mongoimages/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      508 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongoimages/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2732 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongoimages/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.340978 Flask-AppBuilder-4.4.1rc2/examples/mongoimages/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.341031 Flask-AppBuilder-4.4.1rc2/examples/mongoimages/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.594456 Flask-AppBuilder-4.4.1rc2/examples/mongoimages/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4050 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongoimages/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.597718 Flask-AppBuilder-4.4.1rc2/examples/mongoimages/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongoimages/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongoimages/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongoimages/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1906 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongoimages/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongoimages/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/mongoimages/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.602256 Flask-AppBuilder-4.4.1rc2/examples/oauth/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       67 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/oauth/.gitignore
--rw-r--r--   0 dpgaspar   (501) staff       (20)      531 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/oauth/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.607874 Flask-AppBuilder-4.4.1rc2/examples/oauth/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      743 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/oauth/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      399 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/oauth/app/forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      256 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/oauth/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      928 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.4.1rc2/examples/oauth/app/security.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2395 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.4.1rc2/examples/oauth/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.610194 Flask-AppBuilder-4.4.1rc2/examples/oauth/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/oauth/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/oauth/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8914 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/examples/oauth/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/oauth/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.613401 Flask-AppBuilder-4.4.1rc2/examples/productsale/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      192 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/productsale/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.616873 Flask-AppBuilder-4.4.1rc2/examples/productsale/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      628 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/productsale/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1755 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/productsale/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.341713 Flask-AppBuilder-4.4.1rc2/examples/productsale/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.341640 Flask-AppBuilder-4.4.1rc2/examples/productsale/app/translations/es/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.619379 Flask-AppBuilder-4.4.1rc2/examples/productsale/app/translations/es/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/productsale/app/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/productsale/app/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.341768 Flask-AppBuilder-4.4.1rc2/examples/productsale/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.622049 Flask-AppBuilder-4.4.1rc2/examples/productsale/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/productsale/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/productsale/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1304 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/productsale/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.623243 Flask-AppBuilder-4.4.1rc2/examples/productsale/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/productsale/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1667 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/productsale/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/productsale/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.626693 Flask-AppBuilder-4.4.1rc2/examples/quickactions/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.630071 Flask-AppBuilder-4.4.1rc2/examples/quickactions/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      554 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickactions/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      263 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickactions/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.342412 Flask-AppBuilder-4.4.1rc2/examples/quickactions/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.342222 Flask-AppBuilder-4.4.1rc2/examples/quickactions/app/translations/es/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.632291 Flask-AppBuilder-4.4.1rc2/examples/quickactions/app/translations/es/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickactions/app/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickactions/app/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.342475 Flask-AppBuilder-4.4.1rc2/examples/quickactions/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.634592 Flask-AppBuilder-4.4.1rc2/examples/quickactions/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1067 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickactions/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.635799 Flask-AppBuilder-4.4.1rc2/examples/quickactions/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickactions/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1945 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickactions/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickactions/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      279 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickactions/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.638069 Flask-AppBuilder-4.4.1rc2/examples/quickcharts/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickcharts/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.642551 Flask-AppBuilder-4.4.1rc2/examples/quickcharts/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickcharts/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1646 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/examples/quickcharts/app/data.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1342 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickcharts/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.342920 Flask-AppBuilder-4.4.1rc2/examples/quickcharts/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.342985 Flask-AppBuilder-4.4.1rc2/examples/quickcharts/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.644946 Flask-AppBuilder-4.4.1rc2/examples/quickcharts/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2928 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickcharts/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.648206 Flask-AppBuilder-4.4.1rc2/examples/quickcharts/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickcharts/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickcharts/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickcharts/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1775 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickcharts/config.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.650508 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.653859 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      352 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1342 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.343340 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.343394 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.656230 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5034 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.659750 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/babel/messages.pot~
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.343748 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/build/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.343627 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/build/bdist.linux-i686/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.343677 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/build/bdist.linux-i686/egg/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.663106 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/build/bdist.linux-i686/egg/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      356 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/build/bdist.linux-i686/egg/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1322 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/build/bdist.linux-i686/egg/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5082 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/build/bdist.linux-i686/egg/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.343797 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/build/lib/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.666368 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/build/lib/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      356 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/build/lib/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1322 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/build/lib/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5082 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/build/lib/app/views.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1726 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.669629 Flask-AppBuilder-4.4.1rc2/examples/quickfiles/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      225 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickfiles/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.672865 Flask-AppBuilder-4.4.1rc2/examples/quickfiles/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      351 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickfiles/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1188 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickfiles/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.673919 Flask-AppBuilder-4.4.1rc2/examples/quickfiles/app/translations/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickfiles/app/translations/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.344119 Flask-AppBuilder-4.4.1rc2/examples/quickfiles/app/translations/es/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.677279 Flask-AppBuilder-4.4.1rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)    16804 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po~
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.344238 Flask-AppBuilder-4.4.1rc2/examples/quickfiles/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.680828 Flask-AppBuilder-4.4.1rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)    16794 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1395 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickfiles/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.683054 Flask-AppBuilder-4.4.1rc2/examples/quickfiles/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickfiles/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickfiles/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1795 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickfiles/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickfiles/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.687949 Flask-AppBuilder-4.4.1rc2/examples/quickhowto/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.691650 Flask-AppBuilder-4.4.1rc2/examples/quickhowto/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2023-11-20 09:32:40.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-07-29 16:17:15.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.344557 Flask-AppBuilder-4.4.1rc2/examples/quickhowto/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.344608 Flask-AppBuilder-4.4.1rc2/examples/quickhowto/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.694128 Flask-AppBuilder-4.4.1rc2/examples/quickhowto/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3166 2023-10-24 12:30:27.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.697565 Flask-AppBuilder-4.4.1rc2/examples/quickhowto/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2758 2024-02-23 12:47:08.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2119 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.702527 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/NAMES.DIC
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.711177 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      574 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      556 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      105 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/indexview.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3024 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      300 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/sec.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      177 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/sec_models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2047 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/sec_views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.345131 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.723338 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/angularAssets/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      177 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/angularAssets/abBtnAdd.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      171 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/angularAssets/abBtnDelete.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      177 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/angularAssets/abBtnEdit.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      179 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/angularAssets/abBtnShow.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      186 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/angularAssets/abDate.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      437 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/angularAssets/abMenuPageSize.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      548 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/angularAssets/abModalOkCancel.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1633 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/angularAssets/abModelSearch.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2033 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/angularAssets/abModelTable.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      737 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/angularAssets/abPagination.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      216 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/angularAssets/abSelect.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.725502 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/css/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7059 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/css/clean-blog.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1446 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/css/scrolling-nav.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.727635 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/img/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      783 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/img/brand.jpg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3208 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/img/loading.gif
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.732403 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/js/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.735652 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/js/Controllers/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1781 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/js/Controllers/alertsCtrl.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)      240 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/js/Controllers/searchCtrl.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3803 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/js/Controllers/tableCtrl.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.737843 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/js/Directives/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3764 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/js/Directives/bigDirectives.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9587 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/js/Directives/btnDirectives.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.739049 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/js/Services/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2825 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/js/Services/apiService.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)   125321 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/js/angular.min.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/js/app.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    17294 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/js/clean-blog.min.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)      612 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/js/scrolling-nav.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.747038 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/templates/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.748197 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/templates/appbuilder/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/templates/appbuilder/index.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      132 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/templates/index.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10245 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/templates/list_angulajs.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      332 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/templates/list_contacts.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2251 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/templates/list_json.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      199 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/templates/mylist.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      324 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/templates/new_base.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      371 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/templates/show_contacts.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.750346 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/templates/widgets/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2549 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/templates/widgets/list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      280 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/templates/widgets/list_override.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.345853 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.345924 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.752477 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2511 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8249 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.755909 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2387 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2327 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1533 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.768275 Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    92965 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/.coverage
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      220 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.774190 Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      753 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1151 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.346374 Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.346440 Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.778165 Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3115 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.784124 Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1942 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/migrate_db_0.7.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1397 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.788070 Flask-AppBuilder-4.4.1rc2/examples/quickimages/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickimages/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.794176 Flask-AppBuilder-4.4.1rc2/examples/quickimages/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      628 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickimages/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2636 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickimages/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.347456 Flask-AppBuilder-4.4.1rc2/examples/quickimages/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.347332 Flask-AppBuilder-4.4.1rc2/examples/quickimages/app/translations/es/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.799409 Flask-AppBuilder-4.4.1rc2/examples/quickimages/app/translations/es/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickimages/app/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickimages/app/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.347532 Flask-AppBuilder-4.4.1rc2/examples/quickimages/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.806880 Flask-AppBuilder-4.4.1rc2/examples/quickimages/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4155 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickimages/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.810601 Flask-AppBuilder-4.4.1rc2/examples/quickimages/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickimages/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1704 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickimages/config.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.826485 Flask-AppBuilder-4.4.1rc2/examples/quickmigrate/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickmigrate/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      444 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickmigrate/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.837586 Flask-AppBuilder-4.4.1rc2/examples/quickmigrate/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      418 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickmigrate/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickmigrate/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.348063 Flask-AppBuilder-4.4.1rc2/examples/quickmigrate/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.348189 Flask-AppBuilder-4.4.1rc2/examples/quickmigrate/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.845007 Flask-AppBuilder-4.4.1rc2/examples/quickmigrate/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3627 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickmigrate/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.852214 Flask-AppBuilder-4.4.1rc2/examples/quickmigrate/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickmigrate/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickmigrate/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2226 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickmigrate/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2119 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickmigrate/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.855913 Flask-AppBuilder-4.4.1rc2/examples/quickminimal/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      430 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quickminimal/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.871412 Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.890158 Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/.idea/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      159 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/.idea/encodings.xml
--rw-r--r--   0 dpgaspar   (501) staff       (20)      679 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/.idea/misc.xml
--rw-r--r--   0 dpgaspar   (501) staff       (20)      278 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/.idea/modules.xml
--rw-r--r--   0 dpgaspar   (501) staff       (20)      284 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/.idea/quicksqlviews.iml
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1846 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/.idea/workspace.xml
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      271 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.901580 Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.348989 Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.349054 Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.909155 Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2792 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.916716 Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2045 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2095 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.941269 Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      257 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.962854 Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      386 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.349499 Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/app/static/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.970038 Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/app/static/css/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2891 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/app/static/css/landing-page.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.977115 Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/app/templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3347 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/app/templates/mybase.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.349750 Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.349810 Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.991576 Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3658 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.012565 Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1862 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1490 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.042202 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      295 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.064106 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1553 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.108391 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       66 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/.babelrc
--rw-r--r--   0 dpgaspar   (501) staff       (20)      398 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/README.md
--rw-r--r--   0 dpgaspar   (501) staff       (20)   838924 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/package-lock.json
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3522 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/package.json
--rw-r--r--   0 dpgaspar   (501) staff       (20)      746 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/package.json.react-original
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.129888 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/public/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3870 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/public/favicon.ico
--rw-r--r--   0 dpgaspar   (501) staff       (20)      283 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/public/index.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      317 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/public/manifest.json
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.144247 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/src/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      375 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/src/App.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.146794 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/src/api/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      959 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/src/api/Api.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.147485 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/src/components/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3602 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/src/components/CRUDButtons.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4478 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/src/components/Forms.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15937 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/src/components/Table.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)      349 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/src/index.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)      285 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/webpack.config.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.152669 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      856 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/templates/base.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      125 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/templates/react.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.350790 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.350874 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.153105 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.153490 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2462 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.154547 Flask-AppBuilder-4.4.1rc2/examples/related_fields/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/related_fields/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      221 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/related_fields/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.154992 Flask-AppBuilder-4.4.1rc2/examples/related_fields/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/related_fields/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2649 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/related_fields/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.351286 Flask-AppBuilder-4.4.1rc2/examples/related_fields/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.351359 Flask-AppBuilder-4.4.1rc2/examples/related_fields/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.155775 Flask-AppBuilder-4.4.1rc2/examples/related_fields/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5713 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/examples/related_fields/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.156132 Flask-AppBuilder-4.4.1rc2/examples/related_fields/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/related_fields/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/related_fields/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2045 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/related_fields/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/related_fields/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2739 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/related_fields/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.156767 Flask-AppBuilder-4.4.1rc2/examples/simpleform/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       67 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/simpleform/.gitignore
--rw-r--r--   0 dpgaspar   (501) staff       (20)      286 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/simpleform/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.157217 Flask-AppBuilder-4.4.1rc2/examples/simpleform/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/simpleform/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      507 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/simpleform/app/forms.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.157379 Flask-AppBuilder-4.4.1rc2/examples/simpleform/app/templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      125 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/simpleform/app/templates/404.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.351767 Flask-AppBuilder-4.4.1rc2/examples/simpleform/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.351818 Flask-AppBuilder-4.4.1rc2/examples/simpleform/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.157663 Flask-AppBuilder-4.4.1rc2/examples/simpleform/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      483 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      727 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)      940 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/simpleform/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.157949 Flask-AppBuilder-4.4.1rc2/examples/simpleform/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/simpleform/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      662 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/simpleform/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3697 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/simpleform/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/simpleform/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.158364 Flask-AppBuilder-4.4.1rc2/examples/simpleview1/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      173 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/simpleview1/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.158635 Flask-AppBuilder-4.4.1rc2/examples/simpleview1/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/simpleview1/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      601 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/simpleview1/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.163581 Flask-AppBuilder-4.4.1rc2/examples/simpleview1/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/simpleview1/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/simpleview1/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/simpleview1/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/simpleview1/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.163875 Flask-AppBuilder-4.4.1rc2/examples/simpleview2/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.164187 Flask-AppBuilder-4.4.1rc2/examples/simpleview2/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      381 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/simpleview2/app/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.164339 Flask-AppBuilder-4.4.1rc2/examples/simpleview2/app/templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      108 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/simpleview2/app/templates/method3.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1198 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/simpleview2/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.164820 Flask-AppBuilder-4.4.1rc2/examples/simpleview2/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/simpleview2/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/simpleview2/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/simpleview2/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/simpleview2/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.166682 Flask-AppBuilder-4.4.1rc2/examples/user_registration/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/user_registration/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      267 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/user_registration/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.167164 Flask-AppBuilder-4.4.1rc2/examples/user_registration/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/user_registration/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1639 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/user_registration/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.352752 Flask-AppBuilder-4.4.1rc2/examples/user_registration/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.352813 Flask-AppBuilder-4.4.1rc2/examples/user_registration/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.172145 Flask-AppBuilder-4.4.1rc2/examples/user_registration/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3965 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/examples/user_registration/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.172716 Flask-AppBuilder-4.4.1rc2/examples/user_registration/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/user_registration/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/user_registration/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/user_registration/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2499 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/user_registration/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/user_registration/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1490 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/user_registration/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.173794 Flask-AppBuilder-4.4.1rc2/examples/widgets/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/widgets/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      229 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/widgets/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.174266 Flask-AppBuilder-4.4.1rc2/examples/widgets/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/widgets/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/widgets/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.353276 Flask-AppBuilder-4.4.1rc2/examples/widgets/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.353323 Flask-AppBuilder-4.4.1rc2/examples/widgets/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.179170 Flask-AppBuilder-4.4.1rc2/examples/widgets/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/widgets/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/widgets/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4839 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/widgets/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.179606 Flask-AppBuilder-4.4.1rc2/examples/widgets/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/widgets/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/widgets/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/widgets/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1862 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/widgets/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/widgets/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1491 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/examples/widgets/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.187193 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      737 2024-02-23 13:42:48.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1969 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/_compat.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1177 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/actions.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.188665 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/api/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    76068 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/api/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9871 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/api/convert.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3366 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/api/manager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/api/schemas.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.189371 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-05-19 13:25:49.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/babel/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2310 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/babel/manager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      506 2023-05-19 13:25:49.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/babel/views.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    26023 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/base.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      342 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/basemanager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    48965 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/baseviews.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.190045 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/charts/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/charts/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1315 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/charts/jsontools.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    17437 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/charts/views.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/charts/widgets.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14981 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/cli.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14071 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/console.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8591 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/const.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1382 2024-02-15 13:58:31.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/exceptions.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9328 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/fields.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6058 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/fieldwidgets.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8452 2024-02-15 11:02:41.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/filemanager.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)     6164 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/filters.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    11025 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3003 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/hooks.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7636 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/menu.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      290 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/messages.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.191109 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9580 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/base.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      794 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/decorators.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10262 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/filters.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.191594 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/generic/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    12948 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/generic/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2641 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/generic/filters.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2247 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/generic/interface.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10808 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/group.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2593 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/mixins.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.199170 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/mongoengine/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/mongoengine/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1757 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/mongoengine/fields.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4176 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/mongoengine/filters.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9952 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/mongoengine/interface.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.199815 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/sqla/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4073 2023-10-24 12:30:27.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/sqla/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    11046 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/sqla/filters.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    39115 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/sqla/interface.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.202182 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5219 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10558 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/decorators.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4162 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    79392 2024-02-15 13:58:31.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/manager.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.202959 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/mongoengine/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/mongoengine/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15221 2024-02-15 10:47:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/mongoengine/manager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3219 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/mongoengine/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10519 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/registerviews.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1359 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/schemas.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.203750 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.204060 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/apis/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      435 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/apis/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.204647 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/apis/permission/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       45 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/apis/permission/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      624 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/apis/permission/api.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.204991 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/apis/permission_view_menu/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       53 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/apis/permission_view_menu/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      647 2023-07-10 13:48:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/apis/permission_view_menu/api.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.205609 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/apis/role/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       39 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/apis/role/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5053 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/apis/role/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      390 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/apis/role/schema.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.206948 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/apis/user/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       39 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/apis/user/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6695 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/apis/user/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2481 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/apis/user/schema.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1095 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/apis/user/validator.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.212047 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/apis/view_menu/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       43 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/apis/view_menu/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      569 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/apis/view_menu/api.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)    26476 2023-10-24 12:30:27.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/manager.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)     5307 2024-02-23 12:47:16.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      247 2022-10-27 13:03:01.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/utils.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    26342 2024-02-23 13:42:27.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.212243 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6148 2023-08-24 13:59:42.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/.DS_Store
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.212596 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6148 2023-08-24 13:59:42.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/.DS_Store
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.216163 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      643 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/ab.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.217693 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/bootstrap-datepicker/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    21102 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/bootstrap-datepicker/bootstrap-datepicker3.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   121457 2023-10-23 09:56:13.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/bootstrap.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   540434 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/bootstrap.min.css.map
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.217921 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/flags/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10904 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/flags/flags16.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.223315 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/fontawesome/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   101894 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/fontawesome/all.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)    18594 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/fontawesome/brands.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)    80761 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/fontawesome/fontawesome.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)      580 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/fontawesome/regular.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)      572 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/fontawesome/solid.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)    16771 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/fontawesome/svg-with-js.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1736 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/fontawesome/v4-font-face.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)    27593 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/fontawesome/v4-shims.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)      794 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/fontawesome/v5-font-face.min.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.223473 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/images/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    51306 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/images/flags16.png
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.224069 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/select2/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    16792 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/select2/select2-bootstrap.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14966 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/select2/select2.min.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.224309 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/swagger/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   151211 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/swagger/swagger-ui.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.240697 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   105250 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/amelia.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   120090 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/cerulean.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   119768 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/cosmo.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   119799 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/cyborg.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   121625 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/darkly.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   121354 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/flatly.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   118666 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/journal.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   124431 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/lumen.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   132318 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/paper.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   118678 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/readable.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   118965 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/sandstone.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   120186 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/simplex.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   129014 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/slate.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   125030 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/solar.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   121499 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/spacelab.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   120731 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/superhero.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   117016 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/united.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   121865 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/yeti.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.255095 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/webfonts/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   186124 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/webfonts/fa-brands-400.ttf
--rw-r--r--   0 dpgaspar   (501) staff       (20)   107656 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/webfonts/fa-brands-400.woff2
--rw-r--r--   0 dpgaspar   (501) staff       (20)    62320 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/webfonts/fa-regular-400.ttf
--rw-r--r--   0 dpgaspar   (501) staff       (20)    25236 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/webfonts/fa-regular-400.woff2
--rw-r--r--   0 dpgaspar   (501) staff       (20)   397420 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/webfonts/fa-solid-900.ttf
--rw-r--r--   0 dpgaspar   (501) staff       (20)   150516 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/webfonts/fa-solid-900.woff2
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10140 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4568 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/webfonts/fa-v4compatibility.woff2
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.257106 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/fonts/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20127 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 dpgaspar   (501) staff       (20)   108738 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 dpgaspar   (501) staff       (20)    45404 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 dpgaspar   (501) staff       (20)    23424 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 dpgaspar   (501) staff       (20)    18028 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.258503 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/img/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2483 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/img/aol.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2591 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/img/fab.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1595 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/img/flickr.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8777 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/img/glyphicons-halflings-white.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    12799 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/img/glyphicons-halflings.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2558 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/img/google.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2882 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/img/myopenid.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2842 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/img/yahoo.png
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.265657 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/js/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3380 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/js/ab.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4228 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/js/ab_actions.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5275 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/js/ab_filters.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1526 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/js/ab_keep_tab.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.272070 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/js/bootstrap-datepicker/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    33871 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/js/bootstrap-datepicker/bootstrap-datepicker.min.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    39680 2023-10-23 09:56:13.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/js/bootstrap.min.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    46151 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/js/google_charts.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    89501 2023-10-23 09:56:13.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/js/jquery-latest.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    21233 2023-10-19 08:31:50.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/js/popper.min.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.273431 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/js/select2/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    70851 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/js/select2/select2.min.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)  1385226 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/js/swagger-ui-bundle.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.356956 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.280202 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/_formhelpers.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)       28 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/base.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      874 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/baselayout.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4588 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/baselib.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      486 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/flash.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      143 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/footer.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.283102 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      444 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/alert.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.286035 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/charts/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      778 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/charts/chart.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      890 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/charts/chart_time.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      670 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/charts/jsonchart.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      717 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/confirm.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14587 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/lib.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.294694 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/model/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      271 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/model/add.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1181 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/model/edit.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      813 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/model/edit_cascade.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      653 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/model/left_master_detail.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      496 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/model/list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      517 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/model/multiple_views.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      501 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/model/search.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1207 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/model/show.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      784 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/model/show_cascade.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.310176 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/security/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      216 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/security/activation.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2949 2023-01-10 15:41:47.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/security/login_db.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1996 2022-10-27 13:03:01.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/security/login_ldap.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1595 2024-02-16 14:58:39.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/security/login_oauth.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6396 2024-02-12 14:21:56.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/security/login_oid.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      230 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/security/register_mail.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1057 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/security/register_oauth.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.318077 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1153 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/base_list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2981 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/chart.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2613 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/direct_chart.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2016 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/form.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/form_horizontal.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1326 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/form_inline.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1328 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/form_vertical.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      247 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/group_form_list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2745 2023-10-23 07:52:14.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1331 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_block.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2038 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_carousel.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1317 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_item.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2843 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_link.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      572 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_master.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1167 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_thumbnail.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1631 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/multiple_chart.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.318369 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/roles/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3249 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/roles/list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2132 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/roles/show.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1087 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/search.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1738 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/show.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1833 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/show_block.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1544 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/show_vertical.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      145 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/index.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3048 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/init.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1299 2023-10-23 07:52:14.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/navbar.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1247 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/navbar_menu.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1564 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/navbar_right.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.318518 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/swagger/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      896 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/swagger/swagger.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.318665 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.323380 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/__pycache__/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      181 2023-07-05 19:34:38.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.361039 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/de/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.324108 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/de/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9681 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    26578 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.361984 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/el/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.324898 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/el/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    11017 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    22936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.362915 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/es/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.330390 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/es/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8468 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20079 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.363850 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/fr/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.330791 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/fr/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8504 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20065 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.364835 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/it/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.331396 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/it/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9121 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    24545 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.365812 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/ja_JP/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.332237 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/ja_JP/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9412 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20790 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.366753 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/ko/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.332747 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/ko/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9513 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/ko/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    39930 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/ko/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.367689 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/nl/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.333185 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/nl/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8252 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/nl/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19648 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/nl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.368611 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/pl/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.338096 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/pl/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8136 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20115 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.369565 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.338767 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8441 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20002 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20509 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po~
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.370524 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/pt_BR/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.339182 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8336 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20517 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.371502 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/ru/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.339603 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/ru/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10674 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    22035 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.372444 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/sl/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.340004 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/sl/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9682 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/sl/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20841 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/sl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.373390 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/tr/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.345089 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/tr/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10336 2024-02-15 10:47:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    40132 2024-02-15 10:47:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.374297 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/zh/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.345793 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/zh/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7528 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/zh/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19095 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/zh/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:20.375273 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/zh_HK/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.346163 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/zh_HK/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7493 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19104 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7537 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/upload.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3178 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/urltools.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.346617 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/utils/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/utils/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2284 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/utils/base.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      734 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/utils/limit.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3359 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/validators.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    31374 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/views.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4815 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/flask_appbuilder/widgets.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.364038 Flask-AppBuilder-4.4.1rc2/images/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   190476 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/images/ListThumbnail.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    63609 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/images/chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    33854 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/images/chart_time1.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    41838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/images/chart_time2.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    65563 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/images/charts.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   275455 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/images/contact_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    52500 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/images/contacts.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    32505 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/images/direct_chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2591 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/images/fab.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   144592 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/images/group_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    35236 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/images/grouped_chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    16975 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/images/groups.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   173978 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/images/images_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    13590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/images/list_cascade.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10792 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/images/list_cascade_block.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    51248 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/images/list_compact_inline.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    70360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/images/list_master_detail.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15868 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/images/login.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    86223 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/images/login_db.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    84309 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/images/login_oauth.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    31562 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/images/login_oid.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   417827 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/images/security.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15977 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/images/simpleview2.png
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      193 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/release.sh
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.365167 Flask-AppBuilder-4.4.1rc2/scripts/
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      217 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/scripts/babel_extract.sh
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.4.1rc2/scripts/babel_init.sh
--rw-r--r--   0 dpgaspar   (501) staff       (20)      908 2024-02-23 13:58:21.387452 Flask-AppBuilder-4.4.1rc2/setup.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2901 2024-02-15 15:43:33.000000 Flask-AppBuilder-4.4.1rc2/setup.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.376057 Flask-AppBuilder-4.4.1rc2/tests/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tests/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5453 2024-02-12 14:21:56.000000 Flask-AppBuilder-4.4.1rc2/tests/base.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      463 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tests/config_api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1029 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tests/config_oauth.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      479 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tests/config_security.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      515 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tests/config_security_api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      250 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tests/const.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.376939 Flask-AppBuilder-4.4.1rc2/tests/fixtures/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tests/fixtures/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      370 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tests/fixtures/addon_manager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9430 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tests/fixtures/data_models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1113 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tests/fixtures/users.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.377199 Flask-AppBuilder-4.4.1rc2/tests/mongoengine/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tests/mongoengine/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1006 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tests/mongoengine/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.383925 Flask-AppBuilder-4.4.1rc2/tests/security/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tests/security/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    35649 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tests/security/test_auth_ldap.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    39385 2024-02-15 13:58:31.000000 Flask-AppBuilder-4.4.1rc2/tests/security/test_auth_oauth.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2431 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tests/security/test_base_security_manager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19586 2024-02-12 14:21:56.000000 Flask-AppBuilder-4.4.1rc2/tests/security/test_mvc_security.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1715 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tests/security/test_password_complexity.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2956 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tests/security/test_rate_limiter.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-02-23 13:58:21.386673 Flask-AppBuilder-4.4.1rc2/tests/sqla/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tests/sqla/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5815 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tests/sqla/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1264 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tests/test_addon.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)   129559 2023-11-20 13:11:44.000000 Flask-AppBuilder-4.4.1rc2/tests/test_api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1211 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tests/test_custom_indexview.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8814 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tests/test_fab_cli.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6521 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tests/test_menu.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    24813 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tests/test_mongoengine.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    72216 2024-02-23 12:47:16.000000 Flask-AppBuilder-4.4.1rc2/tests/test_mvc.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5017 2024-02-12 14:21:56.000000 Flask-AppBuilder-4.4.1rc2/tests/test_mvc_oauth.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1986 2024-02-15 10:47:53.000000 Flask-AppBuilder-4.4.1rc2/tests/test_mvc_oid.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    44662 2024-02-12 14:21:56.000000 Flask-AppBuilder-4.4.1rc2/tests/test_security_api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6022 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tests/test_security_permissions.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      661 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tests/test_sqlalchemy.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2506 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tests/test_urltools.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1577 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.4.1rc2/tox.ini
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:24.097581 Flask-AppBuilder-4.5.0rc1/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       97 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/.coveragerc
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      113 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/.env
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.000355 Flask-AppBuilder-4.5.0rc1/.github/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      642 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      681 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      202 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/.github/prlint.json
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      709 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/.github/stale.yml
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.004028 Flask-AppBuilder-4.5.0rc1/.github/workflows/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8377 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/.github/workflows/ci.yml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      137 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/.github/workflows/odbcinst.ini
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      951 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/.github/workflows/ptlint.yml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      147 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/.gitignore
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    69088 2024-05-20 14:47:01.000000 Flask-AppBuilder-4.5.0rc1/CHANGELOG.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1926 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/CONTRIBUTING.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.011892 Flask-AppBuilder-4.5.0rc1/Flask_AppBuilder.egg-info/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9357 2024-05-20 14:54:22.000000 Flask-AppBuilder-4.5.0rc1/Flask_AppBuilder.egg-info/PKG-INFO
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    36584 2024-05-20 14:54:22.000000 Flask-AppBuilder-4.5.0rc1/Flask_AppBuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2024-05-20 14:54:22.000000 Flask-AppBuilder-4.5.0rc1/Flask_AppBuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      110 2024-05-20 14:54:22.000000 Flask-AppBuilder-4.5.0rc1/Flask_AppBuilder.egg-info/entry_points.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-12 08:40:39.000000 Flask-AppBuilder-4.5.0rc1/Flask_AppBuilder.egg-info/not-zip-safe
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      571 2024-05-20 14:54:22.000000 Flask-AppBuilder-4.5.0rc1/Flask_AppBuilder.egg-info/requires.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       17 2024-05-20 14:54:22.000000 Flask-AppBuilder-4.5.0rc1/Flask_AppBuilder.egg-info/top_level.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1493 2023-04-05 15:10:33.000000 Flask-AppBuilder-4.5.0rc1/LICENSE
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/MANIFEST.in
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9357 2024-05-20 14:54:24.097749 Flask-AppBuilder-4.5.0rc1/PKG-INFO
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6717 2023-11-20 09:17:41.000000 Flask-AppBuilder-4.5.0rc1/README.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      506 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/RELEASE.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.014093 Flask-AppBuilder-4.5.0rc1/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    36590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/babel/messages.pot
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.995859 Flask-AppBuilder-4.5.0rc1/bin/
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      176 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/bin/babel_extract.sh
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      104 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/bin/babel_init.sh
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      422 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/bin/bootswatch_update.sh
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1632 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/bin/config.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      493 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/bin/db_create.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      840 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/bin/db_migrate.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      309 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/bin/db_upgrade.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1419 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/bin/hash_db_password.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/bin/migrate_db_0.7.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)     4001 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/bin/migrate_db_1.3.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1917 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/bin/sqlite_upgrade_1.3.sql
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      999 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/docker-compose.yml
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.079486 Flask-AppBuilder-4.5.0rc1/docs/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6802 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/Makefile
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.083249 Flask-AppBuilder-4.5.0rc1/docs/_static/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    18838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/_static/Flask-AppBuilder.png
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.087190 Flask-AppBuilder-4.5.0rc1/docs/_templates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      727 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/_templates/layout.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.098372 Flask-AppBuilder-4.5.0rc1/docs/_themes/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1789 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/_themes/LICENSE
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1093 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/_themes/README
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.109501 Flask-AppBuilder-4.5.0rc1/docs/_themes/flask/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      954 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/_themes/flask/layout.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/_themes/flask/relations.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.117071 Flask-AppBuilder-4.5.0rc1/docs/_themes/flask/static/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    18838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/_themes/flask/static/Flask-AppBuilder.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9062 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/_themes/flask/static/flasky.css_t
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      181 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/_themes/flask/theme.conf
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.124635 Flask-AppBuilder-4.5.0rc1/docs/_themes/flask_small/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      683 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/_themes/flask_small/layout.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.128782 Flask-AppBuilder-4.5.0rc1/docs/_themes/flask_small/static/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4609 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/_themes/flask_small/static/flasky.css_t
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      184 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/_themes/flask_small/theme.conf
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4875 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/_themes/flask_theme_support.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2277 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/actions.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3828 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/addons.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10881 2022-09-05 09:07:43.000000 Flask-AppBuilder-4.5.0rc1/docs/advanced.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4209 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/api.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4614 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/cli.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8834 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/conf.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)    33985 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/docs/config.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10806 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/customizing.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4109 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/diagrams.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3803 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/generic_datasource.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3835 2024-02-15 13:58:31.000000 Flask-AppBuilder-4.5.0rc1/docs/i18n.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.263011 Flask-AppBuilder-4.5.0rc1/docs/images/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   190476 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/images/ListThumbnail.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    63609 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/images/chart.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    33854 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/images/chart_time1.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    41838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/images/chart_time2.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    65563 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/images/charts.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   275455 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/images/contact_list.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    52500 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/images/contacts.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    32505 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/images/direct_chart.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2591 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/images/fab.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   144592 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/images/group_list.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    35236 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/images/grouped_chart.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    16975 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/images/groups.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   173978 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/images/images_list.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    13590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/images/list_cascade.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10792 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/images/list_cascade_block.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    51248 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/images/list_compact_inline.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    70360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/images/list_master_detail.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    15868 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/images/login.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    86223 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/images/login_db.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    31562 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/images/login_oid.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    82437 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/images/oauth_login.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    48690 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/images/oauth_login_one_provider.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    42827 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/images/security.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    15977 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/images/simpleview2.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    41274 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/images/swagger001.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    26185 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/images/swagger002.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1389 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.5.0rc1/docs/index.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4377 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.5.0rc1/docs/installation.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2634 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/intro.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6721 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/make.bat
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1464 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/multipledbs.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    11789 2024-05-13 08:09:13.000000 Flask-AppBuilder-4.5.0rc1/docs/quickcharts.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/quickfiles.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    17711 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/quickhowto.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4829 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/quickhowto_mongo.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1676 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/quickminimal.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8990 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/relations.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    47345 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/docs/rest_api.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    39051 2024-02-15 13:58:31.000000 Flask-AppBuilder-4.5.0rc1/docs/security.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    17032 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/templates.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4335 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/user_registration.rst
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)    12302 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/versionmigration.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9036 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/docs/views.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.270232 Flask-AppBuilder-4.5.0rc1/examples/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2036 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.284653 Flask-AppBuilder-4.5.0rc1/examples/base_api/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      209 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/base_api/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.299391 Flask-AppBuilder-4.5.0rc1/examples/base_api/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      380 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/base_api/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3789 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/base_api/app/api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1809 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/base_api/config.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.328865 Flask-AppBuilder-4.5.0rc1/examples/basefilter/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/basefilter/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      429 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/basefilter/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.350312 Flask-AppBuilder-4.5.0rc1/examples/basefilter/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      358 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/basefilter/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1458 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/basefilter/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.784013 Flask-AppBuilder-4.5.0rc1/examples/basefilter/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.784071 Flask-AppBuilder-4.5.0rc1/examples/basefilter/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.364547 Flask-AppBuilder-4.5.0rc1/examples/basefilter/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1413 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/basefilter/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.385780 Flask-AppBuilder-4.5.0rc1/examples/basefilter/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/basefilter/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/basefilter/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/basefilter/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1906 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/basefilter/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2423 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/basefilter/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.406905 Flask-AppBuilder-4.5.0rc1/examples/composite_keys/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      254 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/composite_keys/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.428319 Flask-AppBuilder-4.5.0rc1/examples/composite_keys/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      358 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/composite_keys/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1464 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/composite_keys/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1842 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/composite_keys/app/views.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2182 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/composite_keys/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1477 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/composite_keys/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.450387 Flask-AppBuilder-4.5.0rc1/examples/crud_rest_api/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/crud_rest_api/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      295 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/crud_rest_api/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.451470 Flask-AppBuilder-4.5.0rc1/examples/crud_rest_api/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      355 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/crud_rest_api/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2061 2024-05-20 14:44:49.000000 Flask-AppBuilder-4.5.0rc1/examples/crud_rest_api/app/api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1804 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/crud_rest_api/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.786683 Flask-AppBuilder-4.5.0rc1/examples/crud_rest_api/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.787030 Flask-AppBuilder-4.5.0rc1/examples/crud_rest_api/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.452299 Flask-AppBuilder-4.5.0rc1/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.453014 Flask-AppBuilder-4.5.0rc1/examples/crud_rest_api/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/crud_rest_api/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/crud_rest_api/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2460 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/examples/crud_rest_api/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2253 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/crud_rest_api/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.453887 Flask-AppBuilder-4.5.0rc1/examples/dash/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      291 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/dash/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.454547 Flask-AppBuilder-4.5.0rc1/examples/dash/app/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.455688 Flask-AppBuilder-4.5.0rc1/examples/dash/app/Dashboard/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      797 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/dash/app/Dashboard/Dash_App1.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1256 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/dash/app/Dashboard/Dash_App2.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1568 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/dash/app/Dashboard/Dash_fun.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/dash/app/Dashboard/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      509 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/dash/app/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.455844 Flask-AppBuilder-4.5.0rc1/examples/dash/app/templates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      701 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/dash/app/templates/dash.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1031 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/dash/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.456328 Flask-AppBuilder-4.5.0rc1/examples/dash/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/dash/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/dash/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/dash/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/dash/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.456917 Flask-AppBuilder-4.5.0rc1/examples/employees/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      276 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/employees/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.457994 Flask-AppBuilder-4.5.0rc1/examples/employees/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      711 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/employees/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/employees/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      574 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/employees/app/security.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1972 2022-09-05 09:07:43.000000 Flask-AppBuilder-4.5.0rc1/examples/employees/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.458315 Flask-AppBuilder-4.5.0rc1/examples/employees/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/employees/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1324 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/employees/config.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.459385 Flask-AppBuilder-4.5.0rc1/examples/enums/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/enums/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/enums/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.459951 Flask-AppBuilder-4.5.0rc1/examples/enums/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      358 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/enums/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1158 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/enums/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.794118 Flask-AppBuilder-4.5.0rc1/examples/enums/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.794493 Flask-AppBuilder-4.5.0rc1/examples/enums/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.460455 Flask-AppBuilder-4.5.0rc1/examples/enums/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/enums/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/enums/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3436 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/enums/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.460800 Flask-AppBuilder-4.5.0rc1/examples/enums/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/enums/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/enums/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2226 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/enums/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1841 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/enums/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.462550 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      614 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.463748 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      519 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2607 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      453 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/app/sec.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      880 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/app/sec_forms.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1923 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/app/sec_views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.797181 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.797558 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.464146 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1589 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.464690 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1961 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2977 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.465764 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      560 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.466924 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      435 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2831 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      453 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/app/sec.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      880 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/app/sec_forms.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1929 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/app/sec_views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.800709 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.801086 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.467287 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2133 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.467635 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1906 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2930 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.477911 Flask-AppBuilder-4.5.0rc1/examples/factoryapp/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/factoryapp/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      432 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/factoryapp/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.478793 Flask-AppBuilder-4.5.0rc1/examples/factoryapp/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/factoryapp/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/factoryapp/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.803649 Flask-AppBuilder-4.5.0rc1/examples/factoryapp/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.804030 Flask-AppBuilder-4.5.0rc1/examples/factoryapp/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.479881 Flask-AppBuilder-4.5.0rc1/examples/factoryapp/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2121 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/factoryapp/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.481241 Flask-AppBuilder-4.5.0rc1/examples/factoryapp/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/factoryapp/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/factoryapp/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2024-05-20 11:09:10.000000 Flask-AppBuilder-4.5.0rc1/examples/factoryapp/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1904 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/factoryapp/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1862 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/factoryapp/config2.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1867 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/factoryapp/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.488992 Flask-AppBuilder-4.5.0rc1/examples/issue_789/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1610 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/issue_789/README.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4740 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/issue_789/app.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.497885 Flask-AppBuilder-4.5.0rc1/examples/masterdetail/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/masterdetail/NAMES.DIC
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.498636 Flask-AppBuilder-4.5.0rc1/examples/masterdetail/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      351 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/masterdetail/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1164 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/masterdetail/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.807223 Flask-AppBuilder-4.5.0rc1/examples/masterdetail/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.807627 Flask-AppBuilder-4.5.0rc1/examples/masterdetail/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.499045 Flask-AppBuilder-4.5.0rc1/examples/masterdetail/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2711 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/masterdetail/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.499738 Flask-AppBuilder-4.5.0rc1/examples/masterdetail/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/masterdetail/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/masterdetail/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/masterdetail/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1870 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/masterdetail/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1519 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/masterdetail/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.501119 Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      251 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.502139 Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      573 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1803 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2531 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/app/mysecurity.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.810351 Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.810752 Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.502592 Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2988 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.503019 Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1652 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1396 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.504871 Flask-AppBuilder-4.5.0rc1/examples/mongoengine/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongoengine/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      251 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongoengine/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.505503 Flask-AppBuilder-4.5.0rc1/examples/mongoengine/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      508 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongoengine/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1613 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongoengine/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.813484 Flask-AppBuilder-4.5.0rc1/examples/mongoengine/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.813855 Flask-AppBuilder-4.5.0rc1/examples/mongoengine/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.505884 Flask-AppBuilder-4.5.0rc1/examples/mongoengine/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2623 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongoengine/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.506474 Flask-AppBuilder-4.5.0rc1/examples/mongoengine/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongoengine/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongoengine/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongoengine/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1652 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongoengine/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongoengine/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1396 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongoengine/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.507578 Flask-AppBuilder-4.5.0rc1/examples/mongoimages/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongoimages/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      296 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongoimages/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.508278 Flask-AppBuilder-4.5.0rc1/examples/mongoimages/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      508 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongoimages/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2732 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongoimages/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.816428 Flask-AppBuilder-4.5.0rc1/examples/mongoimages/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.816807 Flask-AppBuilder-4.5.0rc1/examples/mongoimages/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.508711 Flask-AppBuilder-4.5.0rc1/examples/mongoimages/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4050 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongoimages/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.509267 Flask-AppBuilder-4.5.0rc1/examples/mongoimages/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongoimages/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongoimages/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongoimages/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1906 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongoimages/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongoimages/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/mongoimages/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.510147 Flask-AppBuilder-4.5.0rc1/examples/oauth/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       67 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/oauth/.gitignore
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      531 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/oauth/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.511279 Flask-AppBuilder-4.5.0rc1/examples/oauth/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      743 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/oauth/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      399 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/oauth/app/forms.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      256 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/oauth/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      928 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.5.0rc1/examples/oauth/app/security.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2395 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.5.0rc1/examples/oauth/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.511795 Flask-AppBuilder-4.5.0rc1/examples/oauth/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/oauth/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/oauth/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8914 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/examples/oauth/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/oauth/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.512477 Flask-AppBuilder-4.5.0rc1/examples/productsale/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      192 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/productsale/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.520007 Flask-AppBuilder-4.5.0rc1/examples/productsale/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      628 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/productsale/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1755 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/productsale/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.822172 Flask-AppBuilder-4.5.0rc1/examples/productsale/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.821583 Flask-AppBuilder-4.5.0rc1/examples/productsale/app/translations/es/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.520443 Flask-AppBuilder-4.5.0rc1/examples/productsale/app/translations/es/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/productsale/app/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/productsale/app/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.822549 Flask-AppBuilder-4.5.0rc1/examples/productsale/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.521062 Flask-AppBuilder-4.5.0rc1/examples/productsale/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/productsale/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/productsale/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1304 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/productsale/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.526000 Flask-AppBuilder-4.5.0rc1/examples/productsale/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/productsale/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1667 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/productsale/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/productsale/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.526835 Flask-AppBuilder-4.5.0rc1/examples/quickactions/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.527521 Flask-AppBuilder-4.5.0rc1/examples/quickactions/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      554 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickactions/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      263 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickactions/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.826314 Flask-AppBuilder-4.5.0rc1/examples/quickactions/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.825700 Flask-AppBuilder-4.5.0rc1/examples/quickactions/app/translations/es/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.527916 Flask-AppBuilder-4.5.0rc1/examples/quickactions/app/translations/es/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickactions/app/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickactions/app/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.826710 Flask-AppBuilder-4.5.0rc1/examples/quickactions/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.528323 Flask-AppBuilder-4.5.0rc1/examples/quickactions/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1067 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickactions/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.528534 Flask-AppBuilder-4.5.0rc1/examples/quickactions/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickactions/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1945 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickactions/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickactions/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      279 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickactions/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.528852 Flask-AppBuilder-4.5.0rc1/examples/quickcharts/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickcharts/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.529567 Flask-AppBuilder-4.5.0rc1/examples/quickcharts/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickcharts/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1646 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/examples/quickcharts/app/data.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1342 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickcharts/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.829506 Flask-AppBuilder-4.5.0rc1/examples/quickcharts/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.829913 Flask-AppBuilder-4.5.0rc1/examples/quickcharts/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.530005 Flask-AppBuilder-4.5.0rc1/examples/quickcharts/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2928 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickcharts/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.530506 Flask-AppBuilder-4.5.0rc1/examples/quickcharts/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickcharts/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickcharts/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickcharts/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1775 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickcharts/config.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.530875 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.531398 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      352 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1342 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.832633 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.833026 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.532014 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5034 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.532729 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/babel/messages.pot~
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.836039 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/build/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.835101 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/build/bdist.linux-i686/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.835473 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/build/bdist.linux-i686/egg/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.533426 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/build/bdist.linux-i686/egg/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      356 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/build/bdist.linux-i686/egg/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1322 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/build/bdist.linux-i686/egg/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5082 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/build/bdist.linux-i686/egg/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.836405 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/build/lib/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.533999 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/build/lib/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      356 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/build/lib/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1322 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/build/lib/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5082 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/build/lib/app/views.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1726 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.534671 Flask-AppBuilder-4.5.0rc1/examples/quickfiles/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      225 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickfiles/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.535215 Flask-AppBuilder-4.5.0rc1/examples/quickfiles/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      351 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickfiles/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1188 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickfiles/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.535385 Flask-AppBuilder-4.5.0rc1/examples/quickfiles/app/translations/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickfiles/app/translations/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.839161 Flask-AppBuilder-4.5.0rc1/examples/quickfiles/app/translations/es/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.536093 Flask-AppBuilder-4.5.0rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    16804 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po~
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.840097 Flask-AppBuilder-4.5.0rc1/examples/quickfiles/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.536816 Flask-AppBuilder-4.5.0rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    16794 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1395 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickfiles/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.537307 Flask-AppBuilder-4.5.0rc1/examples/quickfiles/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickfiles/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickfiles/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1795 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickfiles/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickfiles/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.538937 Flask-AppBuilder-4.5.0rc1/examples/quickhowto/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.540336 Flask-AppBuilder-4.5.0rc1/examples/quickhowto/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.842785 Flask-AppBuilder-4.5.0rc1/examples/quickhowto/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.843149 Flask-AppBuilder-4.5.0rc1/examples/quickhowto/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.540795 Flask-AppBuilder-4.5.0rc1/examples/quickhowto/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3166 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.541705 Flask-AppBuilder-4.5.0rc1/examples/quickhowto/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2758 2024-02-23 12:47:08.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2119 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.543201 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/NAMES.DIC
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.544739 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      574 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      556 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/forms.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      105 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/indexview.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3024 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      300 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/sec.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      177 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/sec_models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2047 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/sec_views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.847547 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.561292 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/angularAssets/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      177 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/angularAssets/abBtnAdd.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      171 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/angularAssets/abBtnDelete.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      177 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/angularAssets/abBtnEdit.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      179 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/angularAssets/abBtnShow.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      186 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/angularAssets/abDate.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      437 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/angularAssets/abMenuPageSize.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      548 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/angularAssets/abModalOkCancel.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1633 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/angularAssets/abModelSearch.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2033 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/angularAssets/abModelTable.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      737 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/angularAssets/abPagination.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      216 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/angularAssets/abSelect.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.561740 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/css/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     7059 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/css/clean-blog.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1446 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/css/scrolling-nav.css
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.562107 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/img/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      783 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/img/brand.jpg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3208 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/img/loading.gif
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.563209 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/js/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.563947 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/js/Controllers/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1781 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/js/Controllers/alertsCtrl.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      240 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/js/Controllers/searchCtrl.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3803 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/js/Controllers/tableCtrl.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.564395 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/js/Directives/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3764 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/js/Directives/bigDirectives.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9587 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/js/Directives/btnDirectives.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.569092 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/js/Services/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2825 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/js/Services/apiService.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   125321 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/js/angular.min.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/js/app.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    17294 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/js/clean-blog.min.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      612 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/js/scrolling-nav.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.570711 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/templates/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.575495 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/templates/appbuilder/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/templates/appbuilder/index.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      132 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/templates/index.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10245 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/templates/list_angulajs.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      332 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/templates/list_contacts.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2251 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/templates/list_json.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      199 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/templates/mylist.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      324 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/templates/new_base.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      371 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/templates/show_contacts.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.575947 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/templates/widgets/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2549 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/templates/widgets/list.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      280 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/templates/widgets/list_override.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.851978 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.852380 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.576350 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2511 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8249 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.576883 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2387 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2327 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1533 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.581950 Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    92965 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/.coverage
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      220 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.582806 Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      753 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1151 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.855033 Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.855435 Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.583360 Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3115 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.584881 Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1942 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/migrate_db_0.7.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1397 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.585554 Flask-AppBuilder-4.5.0rc1/examples/quickimages/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickimages/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.586670 Flask-AppBuilder-4.5.0rc1/examples/quickimages/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      628 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickimages/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2636 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickimages/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.859262 Flask-AppBuilder-4.5.0rc1/examples/quickimages/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.858621 Flask-AppBuilder-4.5.0rc1/examples/quickimages/app/translations/es/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.587723 Flask-AppBuilder-4.5.0rc1/examples/quickimages/app/translations/es/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickimages/app/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickimages/app/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.859648 Flask-AppBuilder-4.5.0rc1/examples/quickimages/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.593301 Flask-AppBuilder-4.5.0rc1/examples/quickimages/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4155 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickimages/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.593545 Flask-AppBuilder-4.5.0rc1/examples/quickimages/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickimages/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1704 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickimages/config.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.594550 Flask-AppBuilder-4.5.0rc1/examples/quickmigrate/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickmigrate/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      444 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickmigrate/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.595672 Flask-AppBuilder-4.5.0rc1/examples/quickmigrate/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      418 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickmigrate/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickmigrate/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.862535 Flask-AppBuilder-4.5.0rc1/examples/quickmigrate/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.862943 Flask-AppBuilder-4.5.0rc1/examples/quickmigrate/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.603077 Flask-AppBuilder-4.5.0rc1/examples/quickmigrate/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3627 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickmigrate/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.603429 Flask-AppBuilder-4.5.0rc1/examples/quickmigrate/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickmigrate/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickmigrate/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2226 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickmigrate/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2119 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickmigrate/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.608260 Flask-AppBuilder-4.5.0rc1/examples/quickminimal/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      430 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quickminimal/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.609678 Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.610741 Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/.idea/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      159 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/.idea/encodings.xml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      679 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/.idea/misc.xml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      278 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/.idea/modules.xml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      284 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/.idea/quicksqlviews.iml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1846 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/.idea/workspace.xml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      271 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.611205 Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.866853 Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.867226 Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.613849 Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2792 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.625529 Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2045 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2095 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.626706 Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      257 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.634049 Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      386 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.870015 Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/app/static/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.634235 Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/app/static/css/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2891 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/app/static/css/landing-page.css
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.634400 Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/app/templates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3347 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/app/templates/mybase.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.871562 Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.872038 Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.634803 Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3658 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.635348 Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1862 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1490 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.636691 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      295 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.637441 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1553 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.644763 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       66 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/.babelrc
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      398 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/README.md
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   838924 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/package-lock.json
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3522 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/package.json
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      746 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/package.json.react-original
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.645418 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/public/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3870 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/public/favicon.ico
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      283 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/public/index.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      317 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/public/manifest.json
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.645766 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/src/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      375 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/src/App.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.645931 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/src/api/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      959 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/src/api/Api.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.646877 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/src/components/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3602 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/src/components/CRUDButtons.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4478 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/src/components/Forms.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    15937 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/src/components/Table.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      349 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/src/index.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      285 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/webpack.config.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.647247 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/templates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      856 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/templates/base.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      125 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/templates/react.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.878504 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.878866 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.647648 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.647948 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2462 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.649362 Flask-AppBuilder-4.5.0rc1/examples/related_fields/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/related_fields/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      221 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/related_fields/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.649862 Flask-AppBuilder-4.5.0rc1/examples/related_fields/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/related_fields/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2649 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/related_fields/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.881600 Flask-AppBuilder-4.5.0rc1/examples/related_fields/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.882019 Flask-AppBuilder-4.5.0rc1/examples/related_fields/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.650374 Flask-AppBuilder-4.5.0rc1/examples/related_fields/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5713 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/examples/related_fields/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.650801 Flask-AppBuilder-4.5.0rc1/examples/related_fields/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/related_fields/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/related_fields/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2045 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/related_fields/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/related_fields/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2739 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/related_fields/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.651635 Flask-AppBuilder-4.5.0rc1/examples/simpleform/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       67 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/simpleform/.gitignore
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      286 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/simpleform/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.659291 Flask-AppBuilder-4.5.0rc1/examples/simpleform/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/simpleform/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      507 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/simpleform/app/forms.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.659572 Flask-AppBuilder-4.5.0rc1/examples/simpleform/app/templates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      125 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/simpleform/app/templates/404.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.885320 Flask-AppBuilder-4.5.0rc1/examples/simpleform/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.885707 Flask-AppBuilder-4.5.0rc1/examples/simpleform/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.659964 Flask-AppBuilder-4.5.0rc1/examples/simpleform/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      483 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      727 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      940 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/simpleform/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.660285 Flask-AppBuilder-4.5.0rc1/examples/simpleform/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/simpleform/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      662 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/simpleform/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3697 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/simpleform/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/simpleform/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.667804 Flask-AppBuilder-4.5.0rc1/examples/simpleview1/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      173 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/simpleview1/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.668161 Flask-AppBuilder-4.5.0rc1/examples/simpleview1/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/simpleview1/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      601 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/simpleview1/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.668504 Flask-AppBuilder-4.5.0rc1/examples/simpleview1/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/simpleview1/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/simpleview1/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/simpleview1/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/simpleview1/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.668897 Flask-AppBuilder-4.5.0rc1/examples/simpleview2/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.669271 Flask-AppBuilder-4.5.0rc1/examples/simpleview2/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      381 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/simpleview2/app/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.669472 Flask-AppBuilder-4.5.0rc1/examples/simpleview2/app/templates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      108 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/simpleview2/app/templates/method3.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1198 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/simpleview2/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.669992 Flask-AppBuilder-4.5.0rc1/examples/simpleview2/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/simpleview2/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/simpleview2/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/simpleview2/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/simpleview2/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.671769 Flask-AppBuilder-4.5.0rc1/examples/user_registration/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/user_registration/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      267 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/user_registration/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.672474 Flask-AppBuilder-4.5.0rc1/examples/user_registration/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/user_registration/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1639 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/user_registration/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.892549 Flask-AppBuilder-4.5.0rc1/examples/user_registration/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.892954 Flask-AppBuilder-4.5.0rc1/examples/user_registration/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.672987 Flask-AppBuilder-4.5.0rc1/examples/user_registration/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3965 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/examples/user_registration/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.673434 Flask-AppBuilder-4.5.0rc1/examples/user_registration/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/user_registration/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/user_registration/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/user_registration/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2499 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/user_registration/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/user_registration/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1490 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/user_registration/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.681352 Flask-AppBuilder-4.5.0rc1/examples/widgets/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/widgets/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      229 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/widgets/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.681843 Flask-AppBuilder-4.5.0rc1/examples/widgets/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/widgets/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/widgets/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.895778 Flask-AppBuilder-4.5.0rc1/examples/widgets/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.896171 Flask-AppBuilder-4.5.0rc1/examples/widgets/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.684508 Flask-AppBuilder-4.5.0rc1/examples/widgets/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/widgets/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/widgets/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4839 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/widgets/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.702971 Flask-AppBuilder-4.5.0rc1/examples/widgets/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/widgets/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/widgets/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/widgets/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1862 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/widgets/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/widgets/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1491 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/examples/widgets/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.724001 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      737 2024-05-20 14:46:48.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1969 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/_compat.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1177 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/actions.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.739276 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/api/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    76738 2024-05-20 14:44:57.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/api/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9871 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/api/convert.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3366 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/api/manager.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4906 2024-05-20 14:44:57.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/api/schemas.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.739808 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-05-19 13:25:49.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/babel/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2310 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/babel/manager.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      506 2023-05-19 13:25:49.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/babel/views.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    26023 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/base.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      342 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/basemanager.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    48965 2024-05-13 08:09:08.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/baseviews.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.741113 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/charts/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/charts/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1315 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/charts/jsontools.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    17437 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/charts/views.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/charts/widgets.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14981 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/cli.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14071 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/console.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8641 2024-05-20 14:44:57.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/const.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1382 2024-02-15 13:58:31.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/exceptions.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9328 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/fields.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6058 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/fieldwidgets.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8452 2024-02-15 11:02:41.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/filemanager.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)     6164 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/filters.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    11025 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/forms.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3003 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/hooks.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     7636 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/menu.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      290 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/messages.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.749667 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9580 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/base.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      794 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/decorators.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10262 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/filters.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.750537 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/generic/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    12948 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/generic/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2641 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/generic/filters.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2247 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/generic/interface.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10808 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/group.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2593 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/mixins.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.751289 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/mongoengine/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/mongoengine/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1757 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/mongoengine/fields.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4176 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/mongoengine/filters.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9952 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/mongoengine/interface.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.751938 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/sqla/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4073 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/sqla/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    11046 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/sqla/filters.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    39115 2024-05-20 14:44:50.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/sqla/interface.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.759626 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5219 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10558 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/decorators.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4162 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/forms.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    79610 2024-05-16 13:08:48.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/manager.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.760747 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/mongoengine/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/mongoengine/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    15221 2024-02-15 10:47:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/mongoengine/manager.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3219 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/mongoengine/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10519 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/registerviews.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1359 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/schemas.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.761608 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.768826 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/apis/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      435 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/apis/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.769367 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/apis/permission/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       45 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/apis/permission/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      624 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/apis/permission/api.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.770073 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/apis/permission_view_menu/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       53 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/apis/permission_view_menu/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      647 2023-07-10 13:48:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/apis/permission_view_menu/api.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.775265 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/apis/role/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       39 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/apis/role/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5053 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/apis/role/api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      390 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/apis/role/schema.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.776174 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/apis/user/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       39 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/apis/user/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6695 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/apis/user/api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2481 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/apis/user/schema.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1095 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/apis/user/validator.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.776748 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/apis/view_menu/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       43 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/apis/view_menu/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      569 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/apis/view_menu/api.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)    26476 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/manager.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)     5307 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      247 2022-10-27 13:03:01.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/utils.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    26342 2024-02-23 13:42:27.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.776909 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6148 2023-08-24 13:59:42.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/.DS_Store
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.777402 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6148 2023-08-24 13:59:42.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/.DS_Store
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.781382 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      643 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/ab.css
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.785090 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/bootstrap-datepicker/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    21102 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/bootstrap-datepicker/bootstrap-datepicker3.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   121457 2023-10-23 09:56:13.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/bootstrap.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   540434 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/bootstrap.min.css.map
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.785370 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/flags/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10904 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/flags/flags16.css
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.795005 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/fontawesome/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   101894 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/fontawesome/all.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    18594 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/fontawesome/brands.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    80761 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/fontawesome/fontawesome.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      580 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/fontawesome/regular.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      572 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/fontawesome/solid.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    16771 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/fontawesome/svg-with-js.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1736 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/fontawesome/v4-font-face.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    27593 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/fontawesome/v4-shims.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      794 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/fontawesome/v5-font-face.min.css
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.795274 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/images/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    51306 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/images/flags16.png
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.795706 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/select2/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    16792 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/select2/select2-bootstrap.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14966 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/select2/select2.min.css
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.798181 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/swagger/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   151211 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/swagger/swagger-ui.css
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.832976 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   105250 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/amelia.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   120090 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/cerulean.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   119768 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/cosmo.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   119799 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/cyborg.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   121625 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/darkly.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   121354 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/flatly.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   118666 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/journal.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   124431 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/lumen.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   132318 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/paper.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   118678 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/readable.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   118965 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/sandstone.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   120186 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/simplex.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   129014 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/slate.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   125030 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/solar.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   121499 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/spacelab.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   120731 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/superhero.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   117016 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/united.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   121865 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/yeti.css
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.848309 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/webfonts/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   186124 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   107656 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    62320 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    25236 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   397420 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   150516 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10140 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4568 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/webfonts/fa-v4compatibility.woff2
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.851784 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/fonts/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20127 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   108738 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    45404 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    23424 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    18028 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.853836 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/img/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2483 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/img/aol.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2591 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/img/fab.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1595 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/img/flickr.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8777 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/img/glyphicons-halflings-white.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    12799 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/img/glyphicons-halflings.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2558 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/img/google.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2882 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/img/myopenid.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2842 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/img/yahoo.png
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.864189 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/js/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3380 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/js/ab.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4228 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/js/ab_actions.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5275 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/js/ab_filters.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1526 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/js/ab_keep_tab.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.866857 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/js/bootstrap-datepicker/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    33871 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/js/bootstrap-datepicker/bootstrap-datepicker.min.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    39680 2023-10-23 09:56:13.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/js/bootstrap.min.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    46151 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/js/google_charts.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    89501 2023-10-23 09:56:13.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/js/jquery-latest.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    21233 2023-10-19 08:31:50.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/js/popper.min.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.867158 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/js/select2/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    70851 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/js/select2/select2.min.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)  1385226 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/js/swagger-ui-bundle.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.919663 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.871052 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/_formhelpers.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       28 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/base.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      874 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/baselayout.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4588 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/baselib.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      486 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/flash.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      143 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/footer.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.876414 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      444 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/alert.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.877221 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/charts/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      778 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/charts/chart.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      890 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/charts/chart_time.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      670 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/charts/jsonchart.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      717 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/confirm.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14587 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/lib.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.892926 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/model/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      271 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/model/add.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1181 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/model/edit.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      813 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/model/edit_cascade.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      653 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/model/left_master_detail.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      496 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/model/list.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      517 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/model/multiple_views.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      501 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/model/search.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1207 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/model/show.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      784 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/model/show_cascade.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.894619 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/security/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      216 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/security/activation.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2949 2023-01-10 15:41:47.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/security/login_db.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1996 2022-10-27 13:03:01.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/security/login_ldap.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1595 2024-02-16 14:58:39.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/security/login_oauth.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6396 2024-02-12 14:21:56.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/security/login_oid.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      230 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/security/register_mail.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1057 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/security/register_oauth.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.902572 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1153 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/base_list.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2981 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/chart.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2613 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/direct_chart.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2016 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/form.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/form_horizontal.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1326 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/form_inline.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1328 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/form_vertical.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      247 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/group_form_list.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2745 2023-10-23 07:52:14.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/list.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1331 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_block.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2038 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_carousel.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1317 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_item.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2843 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_link.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      572 2024-03-18 10:14:10.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_master.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1167 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_thumbnail.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1631 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/multiple_chart.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.902918 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/roles/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3249 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/roles/list.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2132 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/roles/show.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1087 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/search.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1738 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/show.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1833 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/show_block.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1544 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/show_vertical.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      145 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/index.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3048 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/init.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1299 2023-10-23 07:52:14.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/navbar.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1247 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/navbar_menu.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1564 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/navbar_right.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.903101 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/swagger/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      896 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/swagger/swagger.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.903279 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.903389 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/__pycache__/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      181 2023-07-05 19:34:38.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.930490 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/de/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.903996 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/de/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9681 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    26578 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.932214 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/el/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.909240 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/el/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    11017 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    22936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.933927 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/es/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.910256 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/es/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8468 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20079 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.935571 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/fr/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.915248 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8504 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20065 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.937399 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/it/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.917981 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/it/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9121 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    24545 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.939072 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/ja_JP/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.918723 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9412 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20790 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.940776 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/ko/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.919109 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/ko/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9513 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/ko/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    39930 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/ko/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.942550 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/nl/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.919496 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/nl/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8252 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/nl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19648 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/nl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.944183 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/pl/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.919850 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8136 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20115 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.945798 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.920441 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8441 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20002 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20509 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po~
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.947461 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/pt_BR/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.920958 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8336 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20517 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.949225 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/ru/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.926261 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10674 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    22035 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.951001 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/sl/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.926754 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/sl/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9682 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/sl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20841 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/sl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.952714 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/tr/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.927711 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10336 2024-02-15 10:47:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    40132 2024-02-15 10:47:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.954439 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/zh/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.928617 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/zh/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     7528 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/zh/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19095 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/zh/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:22.956141 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/zh_HK/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.929013 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/zh_HK/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     7493 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19104 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     7537 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/upload.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3178 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/urltools.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:23.929515 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/utils/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/utils/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2284 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/utils/base.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      734 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/utils/limit.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3359 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/validators.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    31374 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/views.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4815 2024-03-18 09:52:07.000000 Flask-AppBuilder-4.5.0rc1/flask_appbuilder/widgets.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:24.010485 Flask-AppBuilder-4.5.0rc1/images/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   190476 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/images/ListThumbnail.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    63609 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/images/chart.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    33854 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/images/chart_time1.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    41838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/images/chart_time2.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    65563 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/images/charts.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   275455 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/images/contact_list.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    52500 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/images/contacts.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    32505 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/images/direct_chart.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2591 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/images/fab.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   144592 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/images/group_list.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    35236 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/images/grouped_chart.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    16975 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/images/groups.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   173978 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/images/images_list.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    13590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/images/list_cascade.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10792 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/images/list_cascade_block.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    51248 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/images/list_compact_inline.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    70360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/images/list_master_detail.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    15868 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/images/login.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    86223 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/images/login_db.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    84309 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/images/login_oauth.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    31562 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/images/login_oid.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   417827 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/images/security.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    15977 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/images/simpleview2.png
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      193 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/release.sh
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:24.011406 Flask-AppBuilder-4.5.0rc1/scripts/
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      217 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/scripts/babel_extract.sh
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.5.0rc1/scripts/babel_init.sh
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      908 2024-05-20 14:54:24.098277 Flask-AppBuilder-4.5.0rc1/setup.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2901 2024-05-20 11:09:53.000000 Flask-AppBuilder-4.5.0rc1/setup.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:24.073256 Flask-AppBuilder-4.5.0rc1/tests/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tests/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5453 2024-02-12 14:21:56.000000 Flask-AppBuilder-4.5.0rc1/tests/base.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      463 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tests/config_api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1029 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tests/config_oauth.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      479 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tests/config_security.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      515 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tests/config_security_api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      250 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tests/const.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:24.080935 Flask-AppBuilder-4.5.0rc1/tests/fixtures/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tests/fixtures/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      370 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tests/fixtures/addon_manager.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9430 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tests/fixtures/data_models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1113 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tests/fixtures/users.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:24.081247 Flask-AppBuilder-4.5.0rc1/tests/mongoengine/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tests/mongoengine/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1006 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tests/mongoengine/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:24.083420 Flask-AppBuilder-4.5.0rc1/tests/security/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tests/security/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    35649 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tests/security/test_auth_ldap.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    39385 2024-02-15 13:58:31.000000 Flask-AppBuilder-4.5.0rc1/tests/security/test_auth_oauth.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2431 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tests/security/test_base_security_manager.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19586 2024-02-12 14:21:56.000000 Flask-AppBuilder-4.5.0rc1/tests/security/test_mvc_security.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1715 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tests/security/test_password_complexity.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2956 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tests/security/test_rate_limiter.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2024-05-20 14:54:24.095081 Flask-AppBuilder-4.5.0rc1/tests/sqla/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tests/sqla/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5815 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tests/sqla/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1264 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tests/test_addon.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   130740 2024-05-20 14:44:57.000000 Flask-AppBuilder-4.5.0rc1/tests/test_api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1211 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tests/test_custom_indexview.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8814 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tests/test_fab_cli.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6521 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tests/test_menu.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    24813 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tests/test_mongoengine.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    72216 2024-02-23 12:47:16.000000 Flask-AppBuilder-4.5.0rc1/tests/test_mvc.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5017 2024-02-12 14:21:56.000000 Flask-AppBuilder-4.5.0rc1/tests/test_mvc_oauth.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1986 2024-02-15 10:47:53.000000 Flask-AppBuilder-4.5.0rc1/tests/test_mvc_oid.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    44662 2024-02-12 14:21:56.000000 Flask-AppBuilder-4.5.0rc1/tests/test_security_api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6022 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tests/test_security_permissions.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      661 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tests/test_sqlalchemy.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2506 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tests/test_urltools.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1577 2023-10-23 14:39:53.000000 Flask-AppBuilder-4.5.0rc1/tox.ini
```

### Comparing `Flask-AppBuilder-4.4.1rc2/.github/ISSUE_TEMPLATE.md` & `Flask-AppBuilder-4.5.0rc1/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/.github/PULL_REQUEST_TEMPLATE.md` & `Flask-AppBuilder-4.5.0rc1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/.github/stale.yml` & `Flask-AppBuilder-4.5.0rc1/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/.github/workflows/ci.yml` & `Flask-AppBuilder-4.5.0rc1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/.github/workflows/ptlint.yml` & `Flask-AppBuilder-4.5.0rc1/.github/workflows/ptlint.yml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/CHANGELOG.rst` & `Flask-AppBuilder-4.5.0rc1/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 Flask-AppBuilder ChangeLog
 ==========================
 
-Improvements and Bug fixes on 4.4.1rc2
+Improvements and Bug fixes on 4.5.0
+-----------------------------------
+
+- feat: REST API new select columns query param (#2242) [Daniel Vaz Gaspar]
+- chore: bump werkzeug to 3.0.3 (#2237) [Daniel Vaz Gaspar]
+- fix: Keycloak OAuth2, get groups as role_keys per default (#2235) [Andreas 'count' Kotes]
+- fix: Check if Oauth login with OKTA is correct (#1926) [Hojjat Ali Mohammadi]
+- docs: Update quickcharts.rst for typo gold to goal (#2217) [Abhinav Pareek]
+
+Improvements and Bug fixes on 4.4.1
 -----------------------------------
 
 - fix: user search list on stats (#2211) [Daniel Vaz Gaspar]
 - fix: performance issues on user and roles list (#2209) [Daniel Vaz Gaspar]
 
 Improvements and Bug fixes on 4.4.0
 -----------------------------------
```

### Comparing `Flask-AppBuilder-4.4.1rc2/CONTRIBUTING.rst` & `Flask-AppBuilder-4.5.0rc1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/Flask_AppBuilder.egg-info/PKG-INFO` & `Flask-AppBuilder-4.5.0rc1/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,7 @@
-Metadata-Version: 2.1
-Name: Flask-AppBuilder
-Version: 4.4.1rc2
-Summary: Simple and rapid application development framework, built on top of Flask. includes detailed security, auto CRUD generation for your models, google charts and much more.
-Home-page: https://github.com/dpgaspar/flask-appbuilder/
-Author: Daniel Vaz Gaspar
-Author-email: danielvazgaspar@gmail.com
-License: BSD
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: ~=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: jmespath
-Provides-Extra: oauth
-Provides-Extra: openid
-Provides-Extra: talisman
-License-File: LICENSE
-
 Flask App Builder
 =================
 
 .. image:: https://github.com/dpgaspar/Flask-AppBuilder/workflows/Python/badge.svg
         :target: https://github.com/dpgaspar/Flask-AppBuilder/actions
 
 .. image:: https://img.shields.io/pypi/v/Flask-AppBuilder.svg
```

### Comparing `Flask-AppBuilder-4.4.1rc2/Flask_AppBuilder.egg-info/SOURCES.txt` & `Flask-AppBuilder-4.5.0rc1/Flask_AppBuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/Flask_AppBuilder.egg-info/requires.txt` & `Flask-AppBuilder-4.5.0rc1/Flask_AppBuilder.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/LICENSE` & `Flask-AppBuilder-4.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/PKG-INFO` & `Flask-AppBuilder-4.5.0rc1/Flask_AppBuilder.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,205 @@
 Metadata-Version: 2.1
 Name: Flask-AppBuilder
-Version: 4.4.1rc2
+Version: 4.5.0rc1
 Summary: Simple and rapid application development framework, built on top of Flask. includes detailed security, auto CRUD generation for your models, google charts and much more.
 Home-page: https://github.com/dpgaspar/flask-appbuilder/
 Author: Daniel Vaz Gaspar
 Author-email: danielvazgaspar@gmail.com
 License: BSD
+Description: Flask App Builder
+        =================
+        
+        .. image:: https://github.com/dpgaspar/Flask-AppBuilder/workflows/Python/badge.svg
+                :target: https://github.com/dpgaspar/Flask-AppBuilder/actions
+        
+        .. image:: https://img.shields.io/pypi/v/Flask-AppBuilder.svg
+                :alt: PyPI
+                :target: https://pypi.org/project/Flask-AppBuilder/
+        
+        .. image:: https://img.shields.io/badge/pyversions-3.8%2C%203.9%2C%203.10%2C%203.11%2C%203.12-blue.svg
+                :target: https://www.python.org/
+        
+        .. image:: https://codecov.io/github/dpgaspar/Flask-AppBuilder/coverage.svg?branch=master
+                :target: https://codecov.io/github/dpgaspar/Flask-AppBuilder
+        
+        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+            :target: https://github.com/psf/black
+        
+        
+        Simple and rapid application development framework, built on top of `Flask <http://flask.pocoo.org/>`_.
+        includes detailed security, auto CRUD generation for your models, google charts and much more.
+        
+        Extensive configuration of all functionality, easily integrate with normal Flask/Jinja2 development.
+        
+        - Documentation: `Documentation <http://flask-appbuilder.readthedocs.org/en/latest/>`_
+        
+        - Mailing list: `Google group <https://groups.google.com/forum/#!forum/flask-appbuilder>`_
+        
+        - Chat: `Gitter <https://gitter.im/dpgaspar/Flask-AppBuilder>`_
+        
+        - Examples: `examples <https://github.com/dpgaspar/Flask-AppBuilder/tree/master/examples>`_
+        
+        Checkout installation video on `YouTube <http://youtu.be/xvum4vfwldg>`_
+        
+        Quick how to `Demo from the docs <http://flaskappbuilder.pythonanywhere.com/>`_ (login has guest/welcome).
+        
+        Change Log
+        ----------
+        
+        `Versions <https://github.com/dpgaspar/Flask-AppBuilder/tree/master/CHANGELOG.rst>`_ for further detail on what changed.
+        
+        Fixes, Bugs and contributions
+        -----------------------------
+        
+        You're welcome to report bugs, propose new features, or even better contribute to this project.
+        
+        `Issues, bugs and new features <https://github.com/dpgaspar/Flask-AppBuilder/issues/new>`_
+        
+        `Contribute <https://github.com/dpgaspar/Flask-AppBuilder/fork>`_
+        
+        Includes:
+        ---------
+        
+          - Database
+              - SQLAlchemy, multiple database support: sqlite, MySQL, ORACLE, MSSQL, DB2 etc.
+              - Partial support for MongoDB using MongoEngine.
+              - Multiple database connections support (Vertical partitioning).
+              - Easy mixin audit to models (created/changed by user, and timestamps).
+          - Security
+              - Automatic permissions lookup, based on exposed methods. It will grant all permissions to the Admin Role.
+              - Inserts on the Database all the detailed permissions possible on your application.
+              - Public (no authentication needed) and Private permissions.
+              - Role based permissions.
+              - Authentication support for OAuth, OpenID, Database, LDAP and REMOTE_USER environ var.
+              - Support for self user registration.
+          - Views and Widgets
+              - Automatic menu generation.
+              - Automatic CRUD generation.
+              - Multiple actions on db records.
+              - Big variety of filters for your lists.
+              - Various view widgets: lists, master-detail, list of thumbnails etc
+              - Select2, Datepicker, DateTimePicker
+              - Related Select2 fields.
+              - Google charts with automatic group by or direct values and filters.
+              - AddOn system, write your own and contribute.
+          - CRUD REST API
+              - Automatic CRUD RESTful APIs.
+              - Internationalization
+              - Integration with flask-jwt-extended extension to protect your endpoints.
+              - Metadata for dynamic rendering.
+              - Selectable columns and metadata keys.
+              - Automatic and configurable data validation.
+          - Forms
+              - Automatic, Add, Edit and Show from Database Models
+              - Labels and descriptions for each field.
+              - Automatic base validators from model's definition.
+              - Custom validators, extra fields, custom filters for related dropdown lists.
+              - Image and File support for upload and database field association. It will handle everything for you.
+              - Field sets for Form's (Django style).
+          - i18n
+              - Support for multi-language via Babel
+          - Bootstrap 3.1.1 CSS and js, with Select2 and DatePicker
+          - Font-Awesome icons, for menu icons and actions.
+        
+        
+        Some pictures
+        -------------
+        
+        Login page (with AUTH_DB)
+        
+        .. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/login_db.png
+            :width: 480px
+            :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/login_db.png
+        
+        
+        Login page (with AUTH_OAUTH)
+        
+        .. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/login_oauth.png
+            :width: 480px
+            :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/login_oauth.png
+        
+        
+        Security
+        
+        .. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/security.png
+            :width: 480px
+            :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/security.png
+        
+        
+        Lists:
+        
+        List contacts example
+        
+        .. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/contact_list.png
+            :width: 480px
+            :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/contact_list.png
+        
+        
+        List Group example with search
+        
+        .. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/group_list.png
+            :width: 480px
+            :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/group_list.png
+        
+        
+        
+        Charts:
+        
+        Group by pie chart
+        
+        .. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/grouped_chart.png
+            :width: 480px
+            :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/grouped_chart.png
+        
+        Direct time chart
+        
+        .. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/direct_chart.png
+            :width: 480px
+            :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/chart_time1.png
+        
+        Group by time chart
+        
+        .. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/chart_time2.png
+            :width: 480px
+            :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/chart_time2.png
+        
+        
+        Projects/Organizations using FAB
+        --------------------------------
+        
+        If you would like to share your project, or let everyone know that you're using FAB
+        on your organization please submit a PR or send me an email with the details.
+        
+        Projects:
+        
+        - `Superset <https://github.com/apache/incubator-superset>`_ - a data exploration platform designed to be visual, intuitive, and interactive
+        
+        - `Airflow <https://github.com/apache/airflow>`_ - a platform to programmatically author, schedule, and monitor workflows.
+        
+        
+        Organizations:
+        
+        - Miniclip
+        - EuroBIC
+        - `On Beat Digital <https://onbeat.digital/>`_
+        
+        
+        Depends on:
+        -----------
+        
+        - flask
+        - click
+        - colorama
+        - flask-sqlalchemy
+        - flask-login
+        - flask-openid
+        - flask-wtform
+        - flask-Babel
+        
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
@@ -20,198 +210,7 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: ~=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: jmespath
 Provides-Extra: oauth
 Provides-Extra: openid
 Provides-Extra: talisman
-License-File: LICENSE
-
-Flask App Builder
-=================
-
-.. image:: https://github.com/dpgaspar/Flask-AppBuilder/workflows/Python/badge.svg
-        :target: https://github.com/dpgaspar/Flask-AppBuilder/actions
-
-.. image:: https://img.shields.io/pypi/v/Flask-AppBuilder.svg
-        :alt: PyPI
-        :target: https://pypi.org/project/Flask-AppBuilder/
-
-.. image:: https://img.shields.io/badge/pyversions-3.8%2C%203.9%2C%203.10%2C%203.11%2C%203.12-blue.svg
-        :target: https://www.python.org/
-
-.. image:: https://codecov.io/github/dpgaspar/Flask-AppBuilder/coverage.svg?branch=master
-        :target: https://codecov.io/github/dpgaspar/Flask-AppBuilder
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
-
-
-Simple and rapid application development framework, built on top of `Flask <http://flask.pocoo.org/>`_.
-includes detailed security, auto CRUD generation for your models, google charts and much more.
-
-Extensive configuration of all functionality, easily integrate with normal Flask/Jinja2 development.
-
-- Documentation: `Documentation <http://flask-appbuilder.readthedocs.org/en/latest/>`_
-
-- Mailing list: `Google group <https://groups.google.com/forum/#!forum/flask-appbuilder>`_
-
-- Chat: `Gitter <https://gitter.im/dpgaspar/Flask-AppBuilder>`_
-
-- Examples: `examples <https://github.com/dpgaspar/Flask-AppBuilder/tree/master/examples>`_
-
-Checkout installation video on `YouTube <http://youtu.be/xvum4vfwldg>`_
-
-Quick how to `Demo from the docs <http://flaskappbuilder.pythonanywhere.com/>`_ (login has guest/welcome).
-
-Change Log
-----------
-
-`Versions <https://github.com/dpgaspar/Flask-AppBuilder/tree/master/CHANGELOG.rst>`_ for further detail on what changed.
-
-Fixes, Bugs and contributions
------------------------------
-
-You're welcome to report bugs, propose new features, or even better contribute to this project.
-
-`Issues, bugs and new features <https://github.com/dpgaspar/Flask-AppBuilder/issues/new>`_
-
-`Contribute <https://github.com/dpgaspar/Flask-AppBuilder/fork>`_
-
-Includes:
----------
-
-  - Database
-      - SQLAlchemy, multiple database support: sqlite, MySQL, ORACLE, MSSQL, DB2 etc.
-      - Partial support for MongoDB using MongoEngine.
-      - Multiple database connections support (Vertical partitioning).
-      - Easy mixin audit to models (created/changed by user, and timestamps).
-  - Security
-      - Automatic permissions lookup, based on exposed methods. It will grant all permissions to the Admin Role.
-      - Inserts on the Database all the detailed permissions possible on your application.
-      - Public (no authentication needed) and Private permissions.
-      - Role based permissions.
-      - Authentication support for OAuth, OpenID, Database, LDAP and REMOTE_USER environ var.
-      - Support for self user registration.
-  - Views and Widgets
-      - Automatic menu generation.
-      - Automatic CRUD generation.
-      - Multiple actions on db records.
-      - Big variety of filters for your lists.
-      - Various view widgets: lists, master-detail, list of thumbnails etc
-      - Select2, Datepicker, DateTimePicker
-      - Related Select2 fields.
-      - Google charts with automatic group by or direct values and filters.
-      - AddOn system, write your own and contribute.
-  - CRUD REST API
-      - Automatic CRUD RESTful APIs.
-      - Internationalization
-      - Integration with flask-jwt-extended extension to protect your endpoints.
-      - Metadata for dynamic rendering.
-      - Selectable columns and metadata keys.
-      - Automatic and configurable data validation.
-  - Forms
-      - Automatic, Add, Edit and Show from Database Models
-      - Labels and descriptions for each field.
-      - Automatic base validators from model's definition.
-      - Custom validators, extra fields, custom filters for related dropdown lists.
-      - Image and File support for upload and database field association. It will handle everything for you.
-      - Field sets for Form's (Django style).
-  - i18n
-      - Support for multi-language via Babel
-  - Bootstrap 3.1.1 CSS and js, with Select2 and DatePicker
-  - Font-Awesome icons, for menu icons and actions.
-
-
-Some pictures
--------------
-
-Login page (with AUTH_DB)
-
-.. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/login_db.png
-    :width: 480px
-    :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/login_db.png
-
-
-Login page (with AUTH_OAUTH)
-
-.. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/login_oauth.png
-    :width: 480px
-    :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/login_oauth.png
-
-
-Security
-
-.. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/security.png
-    :width: 480px
-    :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/security.png
-
-
-Lists:
-
-List contacts example
-
-.. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/contact_list.png
-    :width: 480px
-    :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/contact_list.png
-
-
-List Group example with search
-
-.. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/group_list.png
-    :width: 480px
-    :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/group_list.png
-
-
-
-Charts:
-
-Group by pie chart
-
-.. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/grouped_chart.png
-    :width: 480px
-    :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/grouped_chart.png
-
-Direct time chart
-
-.. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/direct_chart.png
-    :width: 480px
-    :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/chart_time1.png
-
-Group by time chart
-
-.. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/chart_time2.png
-    :width: 480px
-    :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/chart_time2.png
-
-
-Projects/Organizations using FAB
---------------------------------
-
-If you would like to share your project, or let everyone know that you're using FAB
-on your organization please submit a PR or send me an email with the details.
-
-Projects:
-
-- `Superset <https://github.com/apache/incubator-superset>`_ - a data exploration platform designed to be visual, intuitive, and interactive
-
-- `Airflow <https://github.com/apache/airflow>`_ - a platform to programmatically author, schedule, and monitor workflows.
-
-
-Organizations:
-
-- Miniclip
-- EuroBIC
-- `On Beat Digital <https://onbeat.digital/>`_
-
-
-Depends on:
------------
-
-- flask
-- click
-- colorama
-- flask-sqlalchemy
-- flask-login
-- flask-openid
-- flask-wtform
-- flask-Babel
```

### Comparing `Flask-AppBuilder-4.4.1rc2/README.rst` & `Flask-AppBuilder-4.5.0rc1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,189 +1,216 @@
-Flask App Builder
-=================
-
-.. image:: https://github.com/dpgaspar/Flask-AppBuilder/workflows/Python/badge.svg
-        :target: https://github.com/dpgaspar/Flask-AppBuilder/actions
-
-.. image:: https://img.shields.io/pypi/v/Flask-AppBuilder.svg
-        :alt: PyPI
-        :target: https://pypi.org/project/Flask-AppBuilder/
-
-.. image:: https://img.shields.io/badge/pyversions-3.8%2C%203.9%2C%203.10%2C%203.11%2C%203.12-blue.svg
-        :target: https://www.python.org/
-
-.. image:: https://codecov.io/github/dpgaspar/Flask-AppBuilder/coverage.svg?branch=master
-        :target: https://codecov.io/github/dpgaspar/Flask-AppBuilder
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
-
-
-Simple and rapid application development framework, built on top of `Flask <http://flask.pocoo.org/>`_.
-includes detailed security, auto CRUD generation for your models, google charts and much more.
-
-Extensive configuration of all functionality, easily integrate with normal Flask/Jinja2 development.
-
-- Documentation: `Documentation <http://flask-appbuilder.readthedocs.org/en/latest/>`_
-
-- Mailing list: `Google group <https://groups.google.com/forum/#!forum/flask-appbuilder>`_
-
-- Chat: `Gitter <https://gitter.im/dpgaspar/Flask-AppBuilder>`_
-
-- Examples: `examples <https://github.com/dpgaspar/Flask-AppBuilder/tree/master/examples>`_
-
-Checkout installation video on `YouTube <http://youtu.be/xvum4vfwldg>`_
-
-Quick how to `Demo from the docs <http://flaskappbuilder.pythonanywhere.com/>`_ (login has guest/welcome).
-
-Change Log
-----------
-
-`Versions <https://github.com/dpgaspar/Flask-AppBuilder/tree/master/CHANGELOG.rst>`_ for further detail on what changed.
-
-Fixes, Bugs and contributions
------------------------------
-
-You're welcome to report bugs, propose new features, or even better contribute to this project.
-
-`Issues, bugs and new features <https://github.com/dpgaspar/Flask-AppBuilder/issues/new>`_
-
-`Contribute <https://github.com/dpgaspar/Flask-AppBuilder/fork>`_
-
-Includes:
----------
-
-  - Database
-      - SQLAlchemy, multiple database support: sqlite, MySQL, ORACLE, MSSQL, DB2 etc.
-      - Partial support for MongoDB using MongoEngine.
-      - Multiple database connections support (Vertical partitioning).
-      - Easy mixin audit to models (created/changed by user, and timestamps).
-  - Security
-      - Automatic permissions lookup, based on exposed methods. It will grant all permissions to the Admin Role.
-      - Inserts on the Database all the detailed permissions possible on your application.
-      - Public (no authentication needed) and Private permissions.
-      - Role based permissions.
-      - Authentication support for OAuth, OpenID, Database, LDAP and REMOTE_USER environ var.
-      - Support for self user registration.
-  - Views and Widgets
-      - Automatic menu generation.
-      - Automatic CRUD generation.
-      - Multiple actions on db records.
-      - Big variety of filters for your lists.
-      - Various view widgets: lists, master-detail, list of thumbnails etc
-      - Select2, Datepicker, DateTimePicker
-      - Related Select2 fields.
-      - Google charts with automatic group by or direct values and filters.
-      - AddOn system, write your own and contribute.
-  - CRUD REST API
-      - Automatic CRUD RESTful APIs.
-      - Internationalization
-      - Integration with flask-jwt-extended extension to protect your endpoints.
-      - Metadata for dynamic rendering.
-      - Selectable columns and metadata keys.
-      - Automatic and configurable data validation.
-  - Forms
-      - Automatic, Add, Edit and Show from Database Models
-      - Labels and descriptions for each field.
-      - Automatic base validators from model's definition.
-      - Custom validators, extra fields, custom filters for related dropdown lists.
-      - Image and File support for upload and database field association. It will handle everything for you.
-      - Field sets for Form's (Django style).
-  - i18n
-      - Support for multi-language via Babel
-  - Bootstrap 3.1.1 CSS and js, with Select2 and DatePicker
-  - Font-Awesome icons, for menu icons and actions.
-
-
-Some pictures
--------------
-
-Login page (with AUTH_DB)
-
-.. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/login_db.png
-    :width: 480px
-    :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/login_db.png
-
-
-Login page (with AUTH_OAUTH)
-
-.. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/login_oauth.png
-    :width: 480px
-    :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/login_oauth.png
-
-
-Security
-
-.. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/security.png
-    :width: 480px
-    :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/security.png
-
-
-Lists:
-
-List contacts example
-
-.. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/contact_list.png
-    :width: 480px
-    :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/contact_list.png
-
-
-List Group example with search
-
-.. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/group_list.png
-    :width: 480px
-    :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/group_list.png
-
-
-
-Charts:
-
-Group by pie chart
-
-.. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/grouped_chart.png
-    :width: 480px
-    :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/grouped_chart.png
-
-Direct time chart
-
-.. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/direct_chart.png
-    :width: 480px
-    :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/chart_time1.png
-
-Group by time chart
-
-.. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/chart_time2.png
-    :width: 480px
-    :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/chart_time2.png
-
-
-Projects/Organizations using FAB
---------------------------------
-
-If you would like to share your project, or let everyone know that you're using FAB
-on your organization please submit a PR or send me an email with the details.
-
-Projects:
-
-- `Superset <https://github.com/apache/incubator-superset>`_ - a data exploration platform designed to be visual, intuitive, and interactive
-
-- `Airflow <https://github.com/apache/airflow>`_ - a platform to programmatically author, schedule, and monitor workflows.
-
-
-Organizations:
-
-- Miniclip
-- EuroBIC
-- `On Beat Digital <https://onbeat.digital/>`_
-
-
-Depends on:
------------
-
-- flask
-- click
-- colorama
-- flask-sqlalchemy
-- flask-login
-- flask-openid
-- flask-wtform
-- flask-Babel
+Metadata-Version: 2.1
+Name: Flask-AppBuilder
+Version: 4.5.0rc1
+Summary: Simple and rapid application development framework, built on top of Flask. includes detailed security, auto CRUD generation for your models, google charts and much more.
+Home-page: https://github.com/dpgaspar/flask-appbuilder/
+Author: Daniel Vaz Gaspar
+Author-email: danielvazgaspar@gmail.com
+License: BSD
+Description: Flask App Builder
+        =================
+        
+        .. image:: https://github.com/dpgaspar/Flask-AppBuilder/workflows/Python/badge.svg
+                :target: https://github.com/dpgaspar/Flask-AppBuilder/actions
+        
+        .. image:: https://img.shields.io/pypi/v/Flask-AppBuilder.svg
+                :alt: PyPI
+                :target: https://pypi.org/project/Flask-AppBuilder/
+        
+        .. image:: https://img.shields.io/badge/pyversions-3.8%2C%203.9%2C%203.10%2C%203.11%2C%203.12-blue.svg
+                :target: https://www.python.org/
+        
+        .. image:: https://codecov.io/github/dpgaspar/Flask-AppBuilder/coverage.svg?branch=master
+                :target: https://codecov.io/github/dpgaspar/Flask-AppBuilder
+        
+        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+            :target: https://github.com/psf/black
+        
+        
+        Simple and rapid application development framework, built on top of `Flask <http://flask.pocoo.org/>`_.
+        includes detailed security, auto CRUD generation for your models, google charts and much more.
+        
+        Extensive configuration of all functionality, easily integrate with normal Flask/Jinja2 development.
+        
+        - Documentation: `Documentation <http://flask-appbuilder.readthedocs.org/en/latest/>`_
+        
+        - Mailing list: `Google group <https://groups.google.com/forum/#!forum/flask-appbuilder>`_
+        
+        - Chat: `Gitter <https://gitter.im/dpgaspar/Flask-AppBuilder>`_
+        
+        - Examples: `examples <https://github.com/dpgaspar/Flask-AppBuilder/tree/master/examples>`_
+        
+        Checkout installation video on `YouTube <http://youtu.be/xvum4vfwldg>`_
+        
+        Quick how to `Demo from the docs <http://flaskappbuilder.pythonanywhere.com/>`_ (login has guest/welcome).
+        
+        Change Log
+        ----------
+        
+        `Versions <https://github.com/dpgaspar/Flask-AppBuilder/tree/master/CHANGELOG.rst>`_ for further detail on what changed.
+        
+        Fixes, Bugs and contributions
+        -----------------------------
+        
+        You're welcome to report bugs, propose new features, or even better contribute to this project.
+        
+        `Issues, bugs and new features <https://github.com/dpgaspar/Flask-AppBuilder/issues/new>`_
+        
+        `Contribute <https://github.com/dpgaspar/Flask-AppBuilder/fork>`_
+        
+        Includes:
+        ---------
+        
+          - Database
+              - SQLAlchemy, multiple database support: sqlite, MySQL, ORACLE, MSSQL, DB2 etc.
+              - Partial support for MongoDB using MongoEngine.
+              - Multiple database connections support (Vertical partitioning).
+              - Easy mixin audit to models (created/changed by user, and timestamps).
+          - Security
+              - Automatic permissions lookup, based on exposed methods. It will grant all permissions to the Admin Role.
+              - Inserts on the Database all the detailed permissions possible on your application.
+              - Public (no authentication needed) and Private permissions.
+              - Role based permissions.
+              - Authentication support for OAuth, OpenID, Database, LDAP and REMOTE_USER environ var.
+              - Support for self user registration.
+          - Views and Widgets
+              - Automatic menu generation.
+              - Automatic CRUD generation.
+              - Multiple actions on db records.
+              - Big variety of filters for your lists.
+              - Various view widgets: lists, master-detail, list of thumbnails etc
+              - Select2, Datepicker, DateTimePicker
+              - Related Select2 fields.
+              - Google charts with automatic group by or direct values and filters.
+              - AddOn system, write your own and contribute.
+          - CRUD REST API
+              - Automatic CRUD RESTful APIs.
+              - Internationalization
+              - Integration with flask-jwt-extended extension to protect your endpoints.
+              - Metadata for dynamic rendering.
+              - Selectable columns and metadata keys.
+              - Automatic and configurable data validation.
+          - Forms
+              - Automatic, Add, Edit and Show from Database Models
+              - Labels and descriptions for each field.
+              - Automatic base validators from model's definition.
+              - Custom validators, extra fields, custom filters for related dropdown lists.
+              - Image and File support for upload and database field association. It will handle everything for you.
+              - Field sets for Form's (Django style).
+          - i18n
+              - Support for multi-language via Babel
+          - Bootstrap 3.1.1 CSS and js, with Select2 and DatePicker
+          - Font-Awesome icons, for menu icons and actions.
+        
+        
+        Some pictures
+        -------------
+        
+        Login page (with AUTH_DB)
+        
+        .. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/login_db.png
+            :width: 480px
+            :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/login_db.png
+        
+        
+        Login page (with AUTH_OAUTH)
+        
+        .. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/login_oauth.png
+            :width: 480px
+            :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/login_oauth.png
+        
+        
+        Security
+        
+        .. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/security.png
+            :width: 480px
+            :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/security.png
+        
+        
+        Lists:
+        
+        List contacts example
+        
+        .. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/contact_list.png
+            :width: 480px
+            :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/contact_list.png
+        
+        
+        List Group example with search
+        
+        .. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/group_list.png
+            :width: 480px
+            :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/group_list.png
+        
+        
+        
+        Charts:
+        
+        Group by pie chart
+        
+        .. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/grouped_chart.png
+            :width: 480px
+            :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/grouped_chart.png
+        
+        Direct time chart
+        
+        .. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/direct_chart.png
+            :width: 480px
+            :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/chart_time1.png
+        
+        Group by time chart
+        
+        .. image:: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/chart_time2.png
+            :width: 480px
+            :target: https://raw.github.com/dpgaspar/flask-AppBuilder/master/images/chart_time2.png
+        
+        
+        Projects/Organizations using FAB
+        --------------------------------
+        
+        If you would like to share your project, or let everyone know that you're using FAB
+        on your organization please submit a PR or send me an email with the details.
+        
+        Projects:
+        
+        - `Superset <https://github.com/apache/incubator-superset>`_ - a data exploration platform designed to be visual, intuitive, and interactive
+        
+        - `Airflow <https://github.com/apache/airflow>`_ - a platform to programmatically author, schedule, and monitor workflows.
+        
+        
+        Organizations:
+        
+        - Miniclip
+        - EuroBIC
+        - `On Beat Digital <https://onbeat.digital/>`_
+        
+        
+        Depends on:
+        -----------
+        
+        - flask
+        - click
+        - colorama
+        - flask-sqlalchemy
+        - flask-login
+        - flask-openid
+        - flask-wtform
+        - flask-Babel
+        
+Platform: any
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: ~=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: jmespath
+Provides-Extra: oauth
+Provides-Extra: openid
+Provides-Extra: talisman
```

### Comparing `Flask-AppBuilder-4.4.1rc2/babel/messages.pot` & `Flask-AppBuilder-4.5.0rc1/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/bin/config.py` & `Flask-AppBuilder-4.5.0rc1/bin/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/bin/db_migrate.py` & `Flask-AppBuilder-4.5.0rc1/bin/db_migrate.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/bin/hash_db_password.py` & `Flask-AppBuilder-4.5.0rc1/bin/hash_db_password.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/bin/migrate_db_0.7.py` & `Flask-AppBuilder-4.5.0rc1/bin/migrate_db_0.7.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/bin/migrate_db_1.3.py` & `Flask-AppBuilder-4.5.0rc1/bin/migrate_db_1.3.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/bin/sqlite_upgrade_1.3.sql` & `Flask-AppBuilder-4.5.0rc1/bin/sqlite_upgrade_1.3.sql`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docker-compose.yml` & `Flask-AppBuilder-4.5.0rc1/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/Makefile` & `Flask-AppBuilder-4.5.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/_static/Flask-AppBuilder.png` & `Flask-AppBuilder-4.5.0rc1/docs/_static/Flask-AppBuilder.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/_templates/layout.html` & `Flask-AppBuilder-4.5.0rc1/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/_themes/LICENSE` & `Flask-AppBuilder-4.5.0rc1/docs/_themes/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/_themes/README` & `Flask-AppBuilder-4.5.0rc1/docs/_themes/README`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/_themes/flask/layout.html` & `Flask-AppBuilder-4.5.0rc1/docs/_themes/flask/layout.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/_themes/flask/relations.html` & `Flask-AppBuilder-4.5.0rc1/docs/_themes/flask/relations.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/_themes/flask/static/Flask-AppBuilder.png` & `Flask-AppBuilder-4.5.0rc1/docs/_themes/flask/static/Flask-AppBuilder.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/_themes/flask/static/flasky.css_t` & `Flask-AppBuilder-4.5.0rc1/docs/_themes/flask/static/flasky.css_t`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/_themes/flask_small/layout.html` & `Flask-AppBuilder-4.5.0rc1/docs/_themes/flask_small/layout.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/_themes/flask_small/static/flasky.css_t` & `Flask-AppBuilder-4.5.0rc1/docs/_themes/flask_small/static/flasky.css_t`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/_themes/flask_theme_support.py` & `Flask-AppBuilder-4.5.0rc1/docs/_themes/flask_theme_support.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/actions.rst` & `Flask-AppBuilder-4.5.0rc1/docs/actions.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/addons.rst` & `Flask-AppBuilder-4.5.0rc1/docs/addons.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/advanced.rst` & `Flask-AppBuilder-4.5.0rc1/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/api.rst` & `Flask-AppBuilder-4.5.0rc1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/cli.rst` & `Flask-AppBuilder-4.5.0rc1/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/conf.py` & `Flask-AppBuilder-4.5.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/config.rst` & `Flask-AppBuilder-4.5.0rc1/docs/config.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/customizing.rst` & `Flask-AppBuilder-4.5.0rc1/docs/customizing.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/diagrams.rst` & `Flask-AppBuilder-4.5.0rc1/docs/diagrams.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/generic_datasource.rst` & `Flask-AppBuilder-4.5.0rc1/docs/generic_datasource.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/i18n.rst` & `Flask-AppBuilder-4.5.0rc1/docs/i18n.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/images/ListThumbnail.png` & `Flask-AppBuilder-4.5.0rc1/docs/images/ListThumbnail.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/images/chart.png` & `Flask-AppBuilder-4.5.0rc1/docs/images/chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/images/chart_time1.png` & `Flask-AppBuilder-4.5.0rc1/docs/images/chart_time1.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/images/chart_time2.png` & `Flask-AppBuilder-4.5.0rc1/docs/images/chart_time2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/images/charts.png` & `Flask-AppBuilder-4.5.0rc1/docs/images/charts.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/images/contact_list.png` & `Flask-AppBuilder-4.5.0rc1/docs/images/contact_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/images/contacts.png` & `Flask-AppBuilder-4.5.0rc1/docs/images/contacts.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/images/direct_chart.png` & `Flask-AppBuilder-4.5.0rc1/docs/images/direct_chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/images/fab.png` & `Flask-AppBuilder-4.5.0rc1/docs/images/fab.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/images/group_list.png` & `Flask-AppBuilder-4.5.0rc1/docs/images/group_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/images/grouped_chart.png` & `Flask-AppBuilder-4.5.0rc1/docs/images/grouped_chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/images/groups.png` & `Flask-AppBuilder-4.5.0rc1/docs/images/groups.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/images/images_list.png` & `Flask-AppBuilder-4.5.0rc1/docs/images/images_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/images/list_cascade.png` & `Flask-AppBuilder-4.5.0rc1/docs/images/list_cascade.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/images/list_cascade_block.png` & `Flask-AppBuilder-4.5.0rc1/docs/images/list_cascade_block.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/images/list_compact_inline.png` & `Flask-AppBuilder-4.5.0rc1/docs/images/list_compact_inline.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/images/list_master_detail.png` & `Flask-AppBuilder-4.5.0rc1/docs/images/list_master_detail.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/images/login.png` & `Flask-AppBuilder-4.5.0rc1/docs/images/login.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/images/login_db.png` & `Flask-AppBuilder-4.5.0rc1/docs/images/login_db.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/images/login_oid.png` & `Flask-AppBuilder-4.5.0rc1/docs/images/login_oid.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/images/oauth_login.png` & `Flask-AppBuilder-4.5.0rc1/docs/images/oauth_login.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/images/oauth_login_one_provider.png` & `Flask-AppBuilder-4.5.0rc1/docs/images/oauth_login_one_provider.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/images/security.png` & `Flask-AppBuilder-4.5.0rc1/docs/images/security.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/images/simpleview2.png` & `Flask-AppBuilder-4.5.0rc1/docs/images/simpleview2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/images/swagger001.png` & `Flask-AppBuilder-4.5.0rc1/docs/images/swagger001.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/images/swagger002.png` & `Flask-AppBuilder-4.5.0rc1/docs/images/swagger002.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/index.rst` & `Flask-AppBuilder-4.5.0rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/installation.rst` & `Flask-AppBuilder-4.5.0rc1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/intro.rst` & `Flask-AppBuilder-4.5.0rc1/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/make.bat` & `Flask-AppBuilder-4.5.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/multipledbs.rst` & `Flask-AppBuilder-4.5.0rc1/docs/multipledbs.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/quickcharts.rst` & `Flask-AppBuilder-4.5.0rc1/docs/quickcharts.rst`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 Direct Data Charts
 ------------------
 
 These charts can display multiple series, based on columns or methods defined on models.
 You can display multiple charts on the same view.
 
-Let's create a simple model first, the gold is to display a chart showing the unemployment evolution
+Let's create a simple model first, the goal is to display a chart showing the unemployment evolution
 versus the percentage of the population with higher education, our model will be::
 
     class CountryStats(Model):
         id = Column(Integer, primary_key=True)
         stat_date = Column(Date, nullable=True)
         population = Column(Float)
         unemployed_perc = Column(Float)
@@ -122,15 +122,15 @@
 -------------------
 
 These charts can display multiple series, based on columns from models or functions defined on the models.
 You can display multiple charts on the same view. This data can be grouped and aggregated has you like.
 
 Let's create some simple models first, base on the prior example but this time lets make our models
 support has many countries has we like.
-The gold is to display a chart showing the unemployment
+The goal is to display a chart showing the unemployment
 versus the percentage of the population with higher education per country::
 
     from flask_appbuilder import Model
 
     class Country(Model):
         id = Column(Integer, primary_key=True)
         name = Column(String(50), unique = True, nullable=False)
```

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/quickfiles.rst` & `Flask-AppBuilder-4.5.0rc1/docs/quickfiles.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/quickhowto.rst` & `Flask-AppBuilder-4.5.0rc1/docs/quickhowto.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/quickhowto_mongo.rst` & `Flask-AppBuilder-4.5.0rc1/docs/quickhowto_mongo.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/quickminimal.rst` & `Flask-AppBuilder-4.5.0rc1/docs/quickminimal.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/relations.rst` & `Flask-AppBuilder-4.5.0rc1/docs/relations.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/rest_api.rst` & `Flask-AppBuilder-4.5.0rc1/docs/rest_api.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/security.rst` & `Flask-AppBuilder-4.5.0rc1/docs/security.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/templates.rst` & `Flask-AppBuilder-4.5.0rc1/docs/templates.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/user_registration.rst` & `Flask-AppBuilder-4.5.0rc1/docs/user_registration.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/versionmigration.rst` & `Flask-AppBuilder-4.5.0rc1/docs/versionmigration.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/docs/views.rst` & `Flask-AppBuilder-4.5.0rc1/docs/views.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/README.rst` & `Flask-AppBuilder-4.5.0rc1/examples/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/base_api/app/api.py` & `Flask-AppBuilder-4.5.0rc1/examples/base_api/app/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/base_api/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/base_api/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/basefilter/NAMES.DIC` & `Flask-AppBuilder-4.5.0rc1/examples/basefilter/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/basefilter/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/basefilter/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/basefilter/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/basefilter/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/basefilter/babel/messages.pot` & `Flask-AppBuilder-4.5.0rc1/examples/basefilter/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/basefilter/babel/messages.pot~` & `Flask-AppBuilder-4.5.0rc1/examples/basefilter/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/basefilter/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/basefilter/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/basefilter/testdata.py` & `Flask-AppBuilder-4.5.0rc1/examples/basefilter/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/composite_keys/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/composite_keys/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/composite_keys/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/composite_keys/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/composite_keys/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/composite_keys/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/composite_keys/testdata.py` & `Flask-AppBuilder-4.5.0rc1/examples/composite_keys/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/crud_rest_api/NAMES.DIC` & `Flask-AppBuilder-4.5.0rc1/examples/crud_rest_api/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/crud_rest_api/app/api.py` & `Flask-AppBuilder-4.5.0rc1/examples/crud_rest_api/app/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/crud_rest_api/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/crud_rest_api/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/crud_rest_api/babel/messages.pot` & `Flask-AppBuilder-4.5.0rc1/examples/crud_rest_api/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/crud_rest_api/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/crud_rest_api/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/crud_rest_api/testdata.py` & `Flask-AppBuilder-4.5.0rc1/examples/crud_rest_api/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/dash/app/Dashboard/Dash_App1.py` & `Flask-AppBuilder-4.5.0rc1/examples/dash/app/Dashboard/Dash_App1.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/dash/app/Dashboard/Dash_App2.py` & `Flask-AppBuilder-4.5.0rc1/examples/dash/app/Dashboard/Dash_App2.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/dash/app/Dashboard/Dash_fun.py` & `Flask-AppBuilder-4.5.0rc1/examples/dash/app/Dashboard/Dash_fun.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/dash/app/templates/dash.html` & `Flask-AppBuilder-4.5.0rc1/examples/dash/app/templates/dash.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/dash/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/dash/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/dash/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/dash/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/employees/app/__init__.py` & `Flask-AppBuilder-4.5.0rc1/examples/employees/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/employees/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/employees/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/employees/app/security.py` & `Flask-AppBuilder-4.5.0rc1/examples/employees/app/security.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/employees/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/employees/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/employees/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/employees/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/enums/NAMES.DIC` & `Flask-AppBuilder-4.5.0rc1/examples/enums/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/enums/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/enums/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/enums/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/enums/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/enums/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/enums/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/enums/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/enums/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/enums/babel/messages.pot` & `Flask-AppBuilder-4.5.0rc1/examples/enums/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/enums/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/enums/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/enums/testdata.py` & `Flask-AppBuilder-4.5.0rc1/examples/enums/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/NAMES.DIC` & `Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/README.rst` & `Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/app/__init__.py` & `Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/app/sec_forms.py` & `Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/app/sec_forms.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/app/sec_views.py` & `Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/app/sec_views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/babel/messages.pot` & `Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/babel/messages.pot~` & `Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/extendsecurity/testdata.py` & `Flask-AppBuilder-4.5.0rc1/examples/extendsecurity/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/NAMES.DIC` & `Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/README.rst` & `Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/app/sec_forms.py` & `Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/app/sec_forms.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/app/sec_views.py` & `Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/app/sec_views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/babel/messages.pot` & `Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/extendsecurity2/testdata.py` & `Flask-AppBuilder-4.5.0rc1/examples/extendsecurity2/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/factoryapp/NAMES.DIC` & `Flask-AppBuilder-4.5.0rc1/examples/factoryapp/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/factoryapp/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/factoryapp/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/factoryapp/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/factoryapp/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/factoryapp/babel/messages.pot` & `Flask-AppBuilder-4.5.0rc1/examples/factoryapp/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/factoryapp/babel/messages.pot~` & `Flask-AppBuilder-4.5.0rc1/examples/factoryapp/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/factoryapp/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/factoryapp/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/factoryapp/config2.py` & `Flask-AppBuilder-4.5.0rc1/examples/factoryapp/config2.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/factoryapp/testdata.py` & `Flask-AppBuilder-4.5.0rc1/examples/factoryapp/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/issue_789/README.rst` & `Flask-AppBuilder-4.5.0rc1/examples/issue_789/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/issue_789/app.py` & `Flask-AppBuilder-4.5.0rc1/examples/issue_789/app.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/masterdetail/NAMES.DIC` & `Flask-AppBuilder-4.5.0rc1/examples/masterdetail/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/masterdetail/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/masterdetail/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/masterdetail/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/masterdetail/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/masterdetail/babel/messages.pot` & `Flask-AppBuilder-4.5.0rc1/examples/masterdetail/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/masterdetail/babel/messages.pot~` & `Flask-AppBuilder-4.5.0rc1/examples/masterdetail/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/masterdetail/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/masterdetail/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/masterdetail/testdata.py` & `Flask-AppBuilder-4.5.0rc1/examples/masterdetail/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/NAMES.DIC` & `Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/app/__init__.py` & `Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/app/mysecurity.py` & `Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/app/mysecurity.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/babel/messages.pot` & `Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongo_extendedsecurity/testdata.py` & `Flask-AppBuilder-4.5.0rc1/examples/mongo_extendedsecurity/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongoengine/NAMES.DIC` & `Flask-AppBuilder-4.5.0rc1/examples/mongoengine/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongoengine/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/mongoengine/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongoengine/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/mongoengine/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongoengine/babel/messages.pot` & `Flask-AppBuilder-4.5.0rc1/examples/mongoengine/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongoengine/babel/messages.pot~` & `Flask-AppBuilder-4.5.0rc1/examples/mongoengine/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongoengine/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/mongoengine/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongoengine/testdata.py` & `Flask-AppBuilder-4.5.0rc1/examples/mongoengine/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongoimages/NAMES.DIC` & `Flask-AppBuilder-4.5.0rc1/examples/mongoimages/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongoimages/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/mongoimages/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongoimages/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/mongoimages/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongoimages/babel/messages.pot` & `Flask-AppBuilder-4.5.0rc1/examples/mongoimages/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongoimages/babel/messages.pot~` & `Flask-AppBuilder-4.5.0rc1/examples/mongoimages/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongoimages/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/mongoimages/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/mongoimages/testdata.py` & `Flask-AppBuilder-4.5.0rc1/examples/mongoimages/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/oauth/README.rst` & `Flask-AppBuilder-4.5.0rc1/examples/oauth/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/oauth/app/__init__.py` & `Flask-AppBuilder-4.5.0rc1/examples/oauth/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/oauth/app/security.py` & `Flask-AppBuilder-4.5.0rc1/examples/oauth/app/security.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/oauth/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/oauth/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/oauth/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/oauth/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/productsale/app/__init__.py` & `Flask-AppBuilder-4.5.0rc1/examples/productsale/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/productsale/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/productsale/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/productsale/app/translations/es/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/productsale/app/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/productsale/app/translations/es/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/productsale/app/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/productsale/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/productsale/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/productsale/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/productsale/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/productsale/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/productsale/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/productsale/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/productsale/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickactions/app/__init__.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickactions/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickactions/app/translations/es/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/quickactions/app/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickactions/app/translations/es/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/quickactions/app/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickactions/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickactions/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickactions/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickactions/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickcharts/app/data.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickcharts/app/data.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickcharts/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickcharts/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickcharts/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickcharts/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickcharts/babel/messages.pot` & `Flask-AppBuilder-4.5.0rc1/examples/quickcharts/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickcharts/babel/messages.pot~` & `Flask-AppBuilder-4.5.0rc1/examples/quickcharts/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickcharts/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickcharts/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/babel/messages.pot` & `Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/babel/messages.pot~` & `Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/build/bdist.linux-i686/egg/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/build/bdist.linux-i686/egg/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/build/bdist.linux-i686/egg/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/build/bdist.linux-i686/egg/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/build/lib/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/build/lib/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/build/lib/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/build/lib/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickcharts2/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickcharts2/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickfiles/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickfiles/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po~` & `Flask-AppBuilder-4.5.0rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po~` & `Flask-AppBuilder-4.5.0rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickfiles/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickfiles/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickfiles/babel/messages.pot` & `Flask-AppBuilder-4.5.0rc1/examples/quickfiles/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickfiles/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickfiles/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto/NAMES.DIC` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto/babel/messages.pot` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto/babel/messages.pot~` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto/testdata.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/NAMES.DIC` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/__init__.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/forms.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/forms.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/sec_views.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/sec_views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/angularAssets/abModalOkCancel.html` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/angularAssets/abModalOkCancel.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/angularAssets/abModelSearch.html` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/angularAssets/abModelSearch.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/angularAssets/abModelTable.html` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/angularAssets/abModelTable.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/angularAssets/abPagination.html` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/angularAssets/abPagination.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/css/clean-blog.min.css` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/css/clean-blog.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/css/scrolling-nav.css` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/css/scrolling-nav.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/img/brand.jpg` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/img/brand.jpg`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/img/loading.gif` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/img/loading.gif`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/js/Controllers/alertsCtrl.js` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/js/Controllers/alertsCtrl.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/js/Controllers/tableCtrl.js` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/js/Controllers/tableCtrl.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/js/Directives/bigDirectives.js` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/js/Directives/bigDirectives.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/js/Directives/btnDirectives.js` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/js/Directives/btnDirectives.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/js/Services/apiService.js` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/js/Services/apiService.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/js/angular.min.js` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/js/angular.min.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/js/app.js` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/js/app.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/js/clean-blog.min.js` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/js/clean-blog.min.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/static/js/scrolling-nav.js` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/static/js/scrolling-nav.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/templates/list_angulajs.html` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/templates/list_angulajs.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/templates/list_json.html` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/templates/list_json.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/templates/widgets/list.html` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/templates/widgets/list.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/babel/messages.pot` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/babel/messages.pot~` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto2/testdata.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto2/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/.coverage` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/.coverage`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/NAMES.DIC` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/app/__init__.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/babel/messages.pot` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/babel/messages.pot~` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/migrate_db_0.7.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/migrate_db_0.7.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickhowto3/testdata.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickhowto3/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickimages/app/__init__.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickimages/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickimages/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickimages/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickimages/app/translations/es/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/quickimages/app/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickimages/app/translations/es/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/quickimages/app/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickimages/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickimages/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickimages/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickimages/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickmigrate/NAMES.DIC` & `Flask-AppBuilder-4.5.0rc1/examples/quickmigrate/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickmigrate/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickmigrate/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickmigrate/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickmigrate/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickmigrate/babel/messages.pot` & `Flask-AppBuilder-4.5.0rc1/examples/quickmigrate/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickmigrate/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickmigrate/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quickmigrate/testdata.py` & `Flask-AppBuilder-4.5.0rc1/examples/quickmigrate/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/.idea/misc.xml` & `Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/.idea/misc.xml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/.idea/workspace.xml` & `Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/NAMES.DIC` & `Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/babel/messages.pot` & `Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quicksqlviews/testdata.py` & `Flask-AppBuilder-4.5.0rc1/examples/quicksqlviews/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/NAMES.DIC` & `Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/app/static/css/landing-page.css` & `Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/app/static/css/landing-page.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/app/templates/mybase.html` & `Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/app/templates/mybase.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/babel/messages.pot` & `Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/babel/messages.pot~` & `Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/quicktemplates/testdata.py` & `Flask-AppBuilder-4.5.0rc1/examples/quicktemplates/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/NAMES.DIC` & `Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/api.py` & `Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/package-lock.json` & `Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/package-lock.json`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/package.json` & `Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/package.json`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/package.json.react-original` & `Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/package.json.react-original`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/public/favicon.ico` & `Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/src/api/Api.js` & `Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/src/api/Api.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/src/components/CRUDButtons.js` & `Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/src/components/CRUDButtons.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/src/components/Forms.js` & `Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/src/components/Forms.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/static/src/components/Table.js` & `Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/static/src/components/Table.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/templates/base.html` & `Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/templates/base.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/babel/messages.pot` & `Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/react-rest-api/testdata.py` & `Flask-AppBuilder-4.5.0rc1/examples/react-rest-api/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/related_fields/NAMES.DIC` & `Flask-AppBuilder-4.5.0rc1/examples/related_fields/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/related_fields/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/related_fields/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/related_fields/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/related_fields/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/related_fields/babel/messages.pot` & `Flask-AppBuilder-4.5.0rc1/examples/related_fields/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/related_fields/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/related_fields/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/related_fields/testdata.py` & `Flask-AppBuilder-4.5.0rc1/examples/related_fields/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/simpleform/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/simpleform/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/simpleform/babel/messages.pot` & `Flask-AppBuilder-4.5.0rc1/examples/simpleform/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/simpleform/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/simpleform/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/simpleview1/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/simpleview1/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/simpleview1/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/simpleview1/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/simpleview2/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/simpleview2/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/simpleview2/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/simpleview2/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/user_registration/NAMES.DIC` & `Flask-AppBuilder-4.5.0rc1/examples/user_registration/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/user_registration/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/user_registration/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/user_registration/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/user_registration/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/user_registration/babel/messages.pot` & `Flask-AppBuilder-4.5.0rc1/examples/user_registration/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/user_registration/babel/messages.pot~` & `Flask-AppBuilder-4.5.0rc1/examples/user_registration/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/user_registration/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/user_registration/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/user_registration/testdata.py` & `Flask-AppBuilder-4.5.0rc1/examples/user_registration/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/widgets/NAMES.DIC` & `Flask-AppBuilder-4.5.0rc1/examples/widgets/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/widgets/app/models.py` & `Flask-AppBuilder-4.5.0rc1/examples/widgets/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/widgets/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/examples/widgets/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/widgets/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/examples/widgets/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/widgets/app/views.py` & `Flask-AppBuilder-4.5.0rc1/examples/widgets/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/widgets/babel/messages.pot` & `Flask-AppBuilder-4.5.0rc1/examples/widgets/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/widgets/babel/messages.pot~` & `Flask-AppBuilder-4.5.0rc1/examples/widgets/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/widgets/config.py` & `Flask-AppBuilder-4.5.0rc1/examples/widgets/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/examples/widgets/testdata.py` & `Flask-AppBuilder-4.5.0rc1/examples/widgets/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/__init__.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Daniel Vaz Gaspar"
-__version__ = "4.4.1rc2"
+__version__ = "4.5.0rc1"
 
 from .actions import action  # noqa: F401
 from .api import ModelRestApi  # noqa: F401
 from .base import AppBuilder  # noqa: F401
 from .baseviews import BaseView, expose  # noqa: F401
 from .charts.views import DirectByChartView, GroupByChartView  # noqa: F401
 from .models.group import aggregate_avg, aggregate_count, aggregate_sum  # noqa: F401
```

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/_compat.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/_compat.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/actions.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/actions.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/api/__init__.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     API_ORDER_DIRECTION_RIS_KEY,
     API_PAGE_INDEX_RIS_KEY,
     API_PAGE_SIZE_RIS_KEY,
     API_PERMISSIONS_RES_KEY,
     API_PERMISSIONS_RIS_KEY,
     API_RESULT_RES_KEY,
     API_SELECT_COLUMNS_RIS_KEY,
+    API_SELECT_SEL_COLUMNS_RIS_KEY,
     API_SHOW_COLUMNS_RES_KEY,
     API_SHOW_COLUMNS_RIS_KEY,
     API_SHOW_TITLE_RES_KEY,
     API_SHOW_TITLE_RIS_KEY,
     API_URI_RIS_KEY,
     PERMISSION_PREFIX,
 )
@@ -1568,16 +1569,31 @@
     def get_list_headless(self, **kwargs: Any) -> Response:
         """
         Get list of items from Model
         """
         response = dict()
         args = kwargs.get("rison", {})
         # handle select columns
-        select_cols = args.get(API_SELECT_COLUMNS_RIS_KEY, [])
-        pruned_select_cols = [col for col in select_cols if col in self.list_columns]
+        output_select_cols = args.get(API_SELECT_COLUMNS_RIS_KEY, [])
+        select_cols = args.get(API_SELECT_SEL_COLUMNS_RIS_KEY, [])
+        if select_cols and output_select_cols:
+            return self.response_400(message="Cannot use both select and sel columns")
+        list_select_columns = self.list_select_columns
+        pruned_select_cols = []
+        if output_select_cols:
+            pruned_select_cols = [
+                col for col in output_select_cols if col in self.list_columns
+            ]
+        if select_cols:
+            pruned_select_cols = [
+                col for col in select_cols if col in self.list_columns
+            ]
+            list_select_columns = [
+                col for col in select_cols if col in self.list_select_columns
+            ]
         # map decorated metadata
         self.set_response_key_mappings(
             response,
             self.get_list,
             args,
             **{API_SELECT_COLUMNS_RIS_KEY: pruned_select_cols},
         )
@@ -1602,15 +1618,15 @@
         # Make the query
         count, lst = self.datamodel.query(
             joined_filters,
             order_column,
             order_direction,
             page=page_index,
             page_size=page_size,
-            select_columns=self.list_select_columns,
+            select_columns=list_select_columns,
             outer_default_load=self.list_outer_default_load,
         )
         pks = self.datamodel.get_keys(lst)
         response[API_RESULT_RES_KEY] = list_model_schema.dump(lst, many=True)
         response["ids"] = pks
         response["count"] = count
         self.pre_get_list(response)
```

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/api/convert.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/api/convert.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/api/manager.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/api/manager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/api/schemas.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/api/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     API_ORDER_COLUMNS_RIS_KEY,
     API_ORDER_DIRECTION_RIS_KEY,
     API_PAGE_INDEX_RIS_KEY,
     API_PAGE_SIZE_RIS_KEY,
     API_PERMISSIONS_RIS_KEY,
     API_SELECT_COLUMNS_RIS_KEY,
     API_SELECT_KEYS_RIS_KEY,
+    API_SELECT_SEL_COLUMNS_RIS_KEY,
     API_SHOW_COLUMNS_RIS_KEY,
     API_SHOW_TITLE_RIS_KEY,
 )
 
 
 class BaseModelSchema(Schema):
     """
@@ -66,14 +67,15 @@
                     API_DESCRIPTION_COLUMNS_RIS_KEY,
                     API_LIST_TITLE_RIS_KEY,
                     "none",
                 ],
             },
         },
         API_SELECT_COLUMNS_RIS_KEY: {"type": "array", "items": {"type": "string"}},
+        API_SELECT_SEL_COLUMNS_RIS_KEY: {"type": "array", "items": {"type": "string"}},
         API_ORDER_COLUMN_RIS_KEY: {"type": "string"},
         API_ORDER_DIRECTION_RIS_KEY: {"type": "string", "enum": ["asc", "desc"]},
         API_PAGE_INDEX_RIS_KEY: {"type": "integer"},
         API_PAGE_SIZE_RIS_KEY: {"type": "integer"},
         API_FILTERS_RIS_KEY: {
             "type": "array",
             "items": {
```

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/babel/manager.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/babel/manager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/base.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/base.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/baseviews.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/baseviews.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/charts/jsontools.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/charts/jsontools.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/charts/views.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/charts/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/cli.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/cli.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/console.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/console.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/const.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,14 +177,15 @@
 API_SHOW_COLUMNS_RIS_KEY = "show_columns"
 API_ADD_COLUMNS_RIS_KEY = "add_columns"
 API_EDIT_COLUMNS_RIS_KEY = "edit_columns"
 API_DESCRIPTION_COLUMNS_RIS_KEY = "description_columns"
 API_FILTERS_RIS_KEY = "filters"
 API_PERMISSIONS_RIS_KEY = "permissions"
 API_SELECT_COLUMNS_RIS_KEY = "columns"
+API_SELECT_SEL_COLUMNS_RIS_KEY = "select_columns"
 API_SELECT_KEYS_RIS_KEY = "keys"
 API_ORDER_COLUMN_RIS_KEY = "order_column"
 API_ORDER_DIRECTION_RIS_KEY = "order_direction"
 API_PAGE_INDEX_RIS_KEY = "page"
 API_PAGE_SIZE_RIS_KEY = "page_size"
 
 API_LIST_TITLE_RIS_KEY = "list_title"
```

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/exceptions.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/exceptions.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/fields.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/fields.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/fieldwidgets.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/fieldwidgets.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/filemanager.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/filemanager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/filters.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/forms.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/forms.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/hooks.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/hooks.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/menu.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/menu.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/base.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/base.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/decorators.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/decorators.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/filters.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/generic/__init__.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/generic/filters.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/generic/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/generic/interface.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/generic/interface.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/group.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/group.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/mixins.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/mixins.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/mongoengine/fields.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/mongoengine/fields.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/mongoengine/filters.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/mongoengine/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/mongoengine/interface.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/mongoengine/interface.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/sqla/__init__.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/sqla/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/sqla/filters.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/sqla/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/models/sqla/interface.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/models/sqla/interface.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/api.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/decorators.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/decorators.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/forms.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/forms.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/manager.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -656,21 +656,25 @@
             log.debug("User info from OpenShift: %s", data)
             return {"username": "openshift_" + data.get("metadata").get("name")}
         # for Okta
         if provider == "okta":
             me = self.appbuilder.sm.oauth_remotes[provider].get("userinfo")
             data = me.json()
             log.debug("User info from Okta: %s", data)
-            return {
-                "username": f"{provider}_{data['sub']}",
-                "first_name": data.get("given_name", ""),
-                "last_name": data.get("family_name", ""),
-                "email": data["email"],
-                "role_keys": data.get("groups", []),
-            }
+            if "error" not in data:
+                return {
+                    "username": f"{provider}_{data['sub']}",
+                    "first_name": data.get("given_name", ""),
+                    "last_name": data.get("family_name", ""),
+                    "email": data["email"],
+                    "role_keys": data.get("groups", []),
+                }
+            else:
+                log.error(data.get("error_description"))
+                return {}
         # for Auth0
         if provider == "auth0":
             data = self.appbuilder.sm.oauth_remotes[provider].userinfo()
             log.debug("User info from Auth0: %s", data)
             return {
                 "username": f"{provider}_{data['sub']}",
                 "first_name": data.get("given_name", ""),
@@ -687,14 +691,15 @@
             data = me.json()
             log.debug("User info from Keycloak: %s", data)
             return {
                 "username": data.get("preferred_username", ""),
                 "first_name": data.get("given_name", ""),
                 "last_name": data.get("family_name", ""),
                 "email": data.get("email", ""),
+                "role_keys": data.get("groups", []),
             }
         # for Authentik
         if provider == "authentik":
             id_token = resp["id_token"]
             me = self._get_authentik_token_info(id_token)
             log.debug("User info from authentik: %s", me)
             return {
```

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/mongoengine/manager.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/mongoengine/manager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/mongoengine/models.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/mongoengine/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/registerviews.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/registerviews.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/schemas.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/schemas.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/apis/permission/api.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/apis/permission/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/apis/permission_view_menu/api.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/apis/permission_view_menu/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/apis/role/api.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/apis/role/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/apis/user/api.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/apis/user/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/apis/user/schema.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/apis/user/schema.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/apis/user/validator.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/apis/user/validator.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/apis/view_menu/api.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/apis/view_menu/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/manager.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/manager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/sqla/models.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/sqla/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/security/views.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/security/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/.DS_Store` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/.DS_Store`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/.DS_Store` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/.DS_Store`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/ab.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/ab.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/bootstrap-datepicker/bootstrap-datepicker3.min.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/bootstrap-datepicker/bootstrap-datepicker3.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/bootstrap.min.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/bootstrap.min.css.map` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/flags/flags16.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/flags/flags16.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/fontawesome/all.min.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/fontawesome/all.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/fontawesome/brands.min.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/fontawesome/brands.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/fontawesome/fontawesome.min.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/fontawesome/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/fontawesome/regular.min.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/fontawesome/regular.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/fontawesome/solid.min.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/fontawesome/solid.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/fontawesome/svg-with-js.min.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/fontawesome/svg-with-js.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/fontawesome/v4-font-face.min.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/fontawesome/v4-font-face.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/fontawesome/v4-shims.min.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/fontawesome/v4-shims.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/fontawesome/v5-font-face.min.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/fontawesome/v5-font-face.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/images/flags16.png` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/images/flags16.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/select2/select2-bootstrap.min.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/select2/select2-bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/select2/select2.min.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/select2/select2.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/swagger/swagger-ui.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/swagger/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/amelia.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/amelia.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/cerulean.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/cerulean.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/cosmo.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/cosmo.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/cyborg.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/cyborg.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/darkly.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/darkly.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/flatly.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/flatly.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/journal.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/journal.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/lumen.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/lumen.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/paper.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/paper.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/readable.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/readable.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/sandstone.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/sandstone.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/simplex.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/simplex.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/slate.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/slate.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/solar.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/solar.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/spacelab.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/spacelab.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/superhero.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/superhero.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/united.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/united.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/themes/yeti.css` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/themes/yeti.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/webfonts/fa-brands-400.ttf` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/webfonts/fa-brands-400.woff2` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/webfonts/fa-regular-400.ttf` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/webfonts/fa-regular-400.woff2` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/webfonts/fa-solid-900.ttf` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/webfonts/fa-solid-900.woff2` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/webfonts/fa-v4compatibility.ttf` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/css/webfonts/fa-v4compatibility.woff2` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/css/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.eot` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.svg` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.ttf` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff2` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/img/aol.png` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/img/aol.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/img/fab.png` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/img/fab.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/img/flickr.png` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/img/flickr.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/img/glyphicons-halflings-white.png` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/img/glyphicons-halflings.png` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/img/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/img/google.png` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/img/google.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/img/myopenid.png` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/img/myopenid.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/img/yahoo.png` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/img/yahoo.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/js/ab.js` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/js/ab.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/js/ab_actions.js` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/js/ab_actions.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/js/ab_filters.js` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/js/ab_filters.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/js/ab_keep_tab.js` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/js/ab_keep_tab.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/js/bootstrap-datepicker/bootstrap-datepicker.min.js` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/js/bootstrap-datepicker/bootstrap-datepicker.min.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/js/bootstrap.min.js` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/js/google_charts.js` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/js/google_charts.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/js/jquery-latest.js` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/js/jquery-latest.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/js/popper.min.js` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/js/select2/select2.min.js` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/js/select2/select2.min.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/static/appbuilder/js/swagger-ui-bundle.js` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/static/appbuilder/js/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/baselayout.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/baselayout.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/baselib.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/baselib.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/charts/chart.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/charts/chart.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/charts/chart_time.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/charts/chart_time.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/charts/jsonchart.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/charts/jsonchart.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/confirm.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/confirm.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/lib.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/lib.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/model/edit.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/model/edit.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/model/edit_cascade.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/model/edit_cascade.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/model/left_master_detail.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/model/left_master_detail.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/model/multiple_views.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/model/multiple_views.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/model/show.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/model/show.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/model/show_cascade.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/model/show_cascade.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/security/login_db.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/security/login_db.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/security/login_ldap.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/security/login_ldap.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/security/login_oauth.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/security/login_oauth.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/security/login_oid.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/security/login_oid.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/security/register_oauth.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/security/register_oauth.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/base_list.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/base_list.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/chart.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/chart.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/direct_chart.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/direct_chart.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/form.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/form.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/form_horizontal.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/form_horizontal.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/form_inline.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/form_inline.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/form_vertical.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/form_vertical.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/list.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/list.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_block.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_block.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_carousel.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_carousel.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_item.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_item.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_link.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_link.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_master.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_master.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_thumbnail.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_thumbnail.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/multiple_chart.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/multiple_chart.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/roles/list.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/roles/list.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/roles/show.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/roles/show.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/search.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/search.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/show.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/show.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/show_block.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/show_block.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/general/widgets/show_vertical.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/general/widgets/show_vertical.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/init.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/init.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/navbar.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/navbar.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/navbar_menu.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/navbar_menu.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/navbar_right.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/navbar_right.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/templates/appbuilder/swagger/swagger.html` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/templates/appbuilder/swagger/swagger.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/de/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/de/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/el/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/el/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/es/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/es/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/fr/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/fr/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/it/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/it/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/ko/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/ko/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/ko/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/ko/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/nl/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/nl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/nl/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/nl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/pl/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/pl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/pl/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po~` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/ru/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/ru/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/sl/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/sl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/sl/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/sl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/tr/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/tr/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/zh/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/zh/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/zh/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/zh/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/upload.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/upload.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/urltools.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/urltools.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/utils/base.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/utils/base.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/utils/limit.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/utils/limit.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/validators.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/validators.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/views.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/flask_appbuilder/widgets.py` & `Flask-AppBuilder-4.5.0rc1/flask_appbuilder/widgets.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/images/ListThumbnail.png` & `Flask-AppBuilder-4.5.0rc1/images/ListThumbnail.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/images/chart.png` & `Flask-AppBuilder-4.5.0rc1/images/chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/images/chart_time1.png` & `Flask-AppBuilder-4.5.0rc1/images/chart_time1.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/images/chart_time2.png` & `Flask-AppBuilder-4.5.0rc1/images/chart_time2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/images/charts.png` & `Flask-AppBuilder-4.5.0rc1/images/charts.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/images/contact_list.png` & `Flask-AppBuilder-4.5.0rc1/images/contact_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/images/contacts.png` & `Flask-AppBuilder-4.5.0rc1/images/contacts.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/images/direct_chart.png` & `Flask-AppBuilder-4.5.0rc1/images/direct_chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/images/fab.png` & `Flask-AppBuilder-4.5.0rc1/images/fab.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/images/group_list.png` & `Flask-AppBuilder-4.5.0rc1/images/group_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/images/grouped_chart.png` & `Flask-AppBuilder-4.5.0rc1/images/grouped_chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/images/groups.png` & `Flask-AppBuilder-4.5.0rc1/images/groups.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/images/images_list.png` & `Flask-AppBuilder-4.5.0rc1/images/images_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/images/list_cascade.png` & `Flask-AppBuilder-4.5.0rc1/images/list_cascade.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/images/list_cascade_block.png` & `Flask-AppBuilder-4.5.0rc1/images/list_cascade_block.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/images/list_compact_inline.png` & `Flask-AppBuilder-4.5.0rc1/images/list_compact_inline.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/images/list_master_detail.png` & `Flask-AppBuilder-4.5.0rc1/images/list_master_detail.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/images/login.png` & `Flask-AppBuilder-4.5.0rc1/images/login.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/images/login_db.png` & `Flask-AppBuilder-4.5.0rc1/images/login_db.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/images/login_oauth.png` & `Flask-AppBuilder-4.5.0rc1/images/login_oauth.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/images/login_oid.png` & `Flask-AppBuilder-4.5.0rc1/images/login_oid.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/images/security.png` & `Flask-AppBuilder-4.5.0rc1/images/security.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/images/simpleview2.png` & `Flask-AppBuilder-4.5.0rc1/images/simpleview2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/setup.cfg` & `Flask-AppBuilder-4.5.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/setup.py` & `Flask-AppBuilder-4.5.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/tests/base.py` & `Flask-AppBuilder-4.5.0rc1/tests/base.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/tests/config_oauth.py` & `Flask-AppBuilder-4.5.0rc1/tests/config_oauth.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/tests/config_security_api.py` & `Flask-AppBuilder-4.5.0rc1/tests/config_security_api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/tests/fixtures/data_models.py` & `Flask-AppBuilder-4.5.0rc1/tests/fixtures/data_models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/tests/fixtures/users.py` & `Flask-AppBuilder-4.5.0rc1/tests/fixtures/users.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/tests/mongoengine/models.py` & `Flask-AppBuilder-4.5.0rc1/tests/mongoengine/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/tests/security/test_auth_ldap.py` & `Flask-AppBuilder-4.5.0rc1/tests/security/test_auth_ldap.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/tests/security/test_auth_oauth.py` & `Flask-AppBuilder-4.5.0rc1/tests/security/test_auth_oauth.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/tests/security/test_base_security_manager.py` & `Flask-AppBuilder-4.5.0rc1/tests/security/test_base_security_manager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/tests/security/test_mvc_security.py` & `Flask-AppBuilder-4.5.0rc1/tests/security/test_mvc_security.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/tests/security/test_password_complexity.py` & `Flask-AppBuilder-4.5.0rc1/tests/security/test_password_complexity.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/tests/security/test_rate_limiter.py` & `Flask-AppBuilder-4.5.0rc1/tests/security/test_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/tests/sqla/models.py` & `Flask-AppBuilder-4.5.0rc1/tests/sqla/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/tests/test_addon.py` & `Flask-AppBuilder-4.5.0rc1/tests/test_addon.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/tests/test_api.py` & `Flask-AppBuilder-4.5.0rc1/tests/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     API_PERMISSIONS_RES_KEY,
     API_PERMISSIONS_RIS_KEY,
     API_RESULT_RES_KEY,
     API_SECURITY_ACCESS_TOKEN_KEY,
     API_SECURITY_REFRESH_TOKEN_KEY,
     API_SELECT_COLUMNS_RIS_KEY,
     API_SELECT_KEYS_RIS_KEY,
+    API_SELECT_SEL_COLUMNS_RIS_KEY,
     API_SHOW_COLUMNS_RIS_KEY,
     API_SHOW_TITLE_RIS_KEY,
     API_URI_RIS_KEY,
 )
 from flask_appbuilder.hooks import before_request
 from flask_appbuilder.models.sqla.filters import FilterGreater, FilterSmaller
 from flask_appbuilder.models.sqla.interface import SQLAInterface
@@ -866,15 +867,15 @@
                 "field_float": "Field Float",
                 "field_integer": "Field Integer",
                 "field_string": "Field String",
             },
         )
         self.assertEqual(rv.status_code, 200)
 
-    def test_get_item_select_cols(self):
+    def test_get_item_choose_cols(self):
         """
         REST Api: Test get item with select columns
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
         with model1_data(self.appbuilder.session, 1) as models:
             model_id = models[0].id
@@ -1850,15 +1851,15 @@
         self.assertEqual(rv.status_code, 200)
         data = json.loads(rv.data.decode("utf-8"))
         field_string_filters = data["filters"]["field_string"]
         self.assertIn(
             {"name": "Custom Filter", "operator": "custom_filter"}, field_string_filters
         )
 
-    def test_get_list_select_cols(self):
+    def test_get_list_choose_cols(self):
         """
         REST Api: Test get list with select columns
         """
         client = self.app.test_client()
         token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
 
         argument = {
@@ -1866,14 +1867,42 @@
             "order_column": "field_integer",
             "order_direction": "asc",
         }
 
         uri = f"api/v1/model1api/?{API_URI_RIS_KEY}={prison.dumps(argument)}"
         with model1_data(self.appbuilder.session, 5):
             rv = self.auth_client_get(client, token, uri)
+            data = json.loads(rv.data.decode("utf-8"))
+            self.assertEqual(data[API_RESULT_RES_KEY][0], {"field_integer": 0})
+            self.assertEqual(
+                data[API_LABEL_COLUMNS_RES_KEY], {"field_integer": "Field Integer"}
+            )
+            self.assertEqual(
+                data[API_DESCRIPTION_COLUMNS_RES_KEY],
+                {"field_integer": "Field Integer"},
+            )
+            self.assertEqual(data[API_LIST_COLUMNS_RES_KEY], ["field_integer"])
+            self.assertEqual(rv.status_code, 200)
+
+    def test_get_list_choose_select_cols(self):
+        """
+        REST Api: Test get list with select columns
+        """
+        client = self.app.test_client()
+        token = self.login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
+
+        argument = {
+            API_SELECT_SEL_COLUMNS_RIS_KEY: ["field_integer"],
+            "order_column": "field_integer",
+            "order_direction": "asc",
+        }
+
+        uri = f"api/v1/model1api/?{API_URI_RIS_KEY}={prison.dumps(argument)}"
+        with model1_data(self.appbuilder.session, 5):
+            rv = self.auth_client_get(client, token, uri)
             data = json.loads(rv.data.decode("utf-8"))
             self.assertEqual(data[API_RESULT_RES_KEY][0], {"field_integer": 0})
             self.assertEqual(
                 data[API_LABEL_COLUMNS_RES_KEY], {"field_integer": "Field Integer"}
             )
             self.assertEqual(
                 data[API_DESCRIPTION_COLUMNS_RES_KEY],
```

### Comparing `Flask-AppBuilder-4.4.1rc2/tests/test_custom_indexview.py` & `Flask-AppBuilder-4.5.0rc1/tests/test_custom_indexview.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/tests/test_fab_cli.py` & `Flask-AppBuilder-4.5.0rc1/tests/test_fab_cli.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/tests/test_menu.py` & `Flask-AppBuilder-4.5.0rc1/tests/test_menu.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/tests/test_mongoengine.py` & `Flask-AppBuilder-4.5.0rc1/tests/test_mongoengine.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/tests/test_mvc.py` & `Flask-AppBuilder-4.5.0rc1/tests/test_mvc.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/tests/test_mvc_oauth.py` & `Flask-AppBuilder-4.5.0rc1/tests/test_mvc_oauth.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/tests/test_mvc_oid.py` & `Flask-AppBuilder-4.5.0rc1/tests/test_mvc_oid.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/tests/test_security_api.py` & `Flask-AppBuilder-4.5.0rc1/tests/test_security_api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/tests/test_security_permissions.py` & `Flask-AppBuilder-4.5.0rc1/tests/test_security_permissions.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/tests/test_sqlalchemy.py` & `Flask-AppBuilder-4.5.0rc1/tests/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/tests/test_urltools.py` & `Flask-AppBuilder-4.5.0rc1/tests/test_urltools.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.4.1rc2/tox.ini` & `Flask-AppBuilder-4.5.0rc1/tox.ini`

 * *Files identical despite different names*

