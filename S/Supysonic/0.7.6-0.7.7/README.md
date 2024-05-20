# Comparing `tmp/Supysonic-0.7.6.tar.gz` & `tmp/supysonic-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Supysonic-0.7.6.tar", last modified: Fri Jul 14 13:28:33 2023, max compression
+gzip compressed data, was "supysonic-0.7.7.tar", last modified: Sun May 19 15:14:59 2024, max compression
```

## Comparing `Supysonic-0.7.6.tar` & `supysonic-0.7.7.tar`

### file list

```diff
@@ -1,164 +1,170 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 13:28:33.236352 Supysonic-0.7.6/
--rw-rw-rw-   0        0        0    34520 2021-01-23 14:44:54.000000 Supysonic-0.7.6/LICENSE
--rw-rw-rw-   0        0        0      154 2021-12-19 16:15:13.000000 Supysonic-0.7.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1712 2023-07-14 13:28:31.746615 Supysonic-0.7.6/PKG-INFO
--rw-rw-rw-   0        0        0     2738 2023-04-10 13:06:12.000000 Supysonic-0.7.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.676579 Supysonic-0.7.6/Supysonic.egg-info/
--rw-rw-rw-   0        0        0     1712 2023-07-14 13:28:31.000000 Supysonic-0.7.6/Supysonic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4802 2023-07-14 13:28:31.000000 Supysonic-0.7.6/Supysonic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 13:28:31.000000 Supysonic-0.7.6/Supysonic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      135 2023-07-14 13:28:31.000000 Supysonic-0.7.6/Supysonic.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2021-12-31 16:33:42.000000 Supysonic-0.7.6/Supysonic.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      108 2023-07-14 13:28:31.000000 Supysonic-0.7.6/Supysonic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-14 13:28:31.000000 Supysonic-0.7.6/Supysonic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3005 2023-04-10 13:06:12.000000 Supysonic-0.7.6/config.sample
-drwxrwxrwx   0        0        0        0 2023-07-14 13:28:33.646637 Supysonic-0.7.6/man/
--rw-rw-rw-   0        0        0     3675 2023-07-14 13:28:33.586478 Supysonic-0.7.6/man/supysonic-cli-folder.1
--rw-rw-rw-   0        0        0     4128 2023-07-14 13:28:33.586478 Supysonic-0.7.6/man/supysonic-cli-user.1
--rw-rw-rw-   0        0        0     2769 2023-07-14 13:28:33.566552 Supysonic-0.7.6/man/supysonic-cli.1
--rw-rw-rw-   0        0        0     1852 2023-07-14 13:28:33.586478 Supysonic-0.7.6/man/supysonic-daemon.1
--rw-rw-rw-   0        0        0     2984 2023-07-14 13:28:33.586478 Supysonic-0.7.6/man/supysonic-server.1
--rw-rw-rw-   0        0        0      108 2022-04-23 14:58:53.000000 Supysonic-0.7.6/pyproject.toml
--rw-rw-rw-   0        0        0     2175 2023-07-14 13:28:31.746615 Supysonic-0.7.6/setup.cfg
--rw-rw-rw-   0        0        0      744 2023-06-18 13:52:50.000000 Supysonic-0.7.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.686553 Supysonic-0.7.6/supysonic/
--rw-rw-rw-   0        0        0      534 2023-07-14 13:16:51.000000 Supysonic-0.7.6/supysonic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.686553 Supysonic-0.7.6/supysonic/api/
--rw-rw-rw-   0        0        0     4059 2023-07-14 10:03:57.000000 Supysonic-0.7.6/supysonic/api/__init__.py
--rw-rw-rw-   0        0        0     9758 2023-03-18 16:38:26.000000 Supysonic-0.7.6/supysonic/api/albums_songs.py
--rw-rw-rw-   0        0        0     4941 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/api/annotation.py
--rw-rw-rw-   0        0        0     5690 2023-02-11 13:36:47.000000 Supysonic-0.7.6/supysonic/api/browse.py
--rw-rw-rw-   0        0        0      856 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/api/chat.py
--rw-rw-rw-   0        0        0     1035 2023-02-25 16:35:07.000000 Supysonic-0.7.6/supysonic/api/errors.py
--rw-rw-rw-   0        0        0     3585 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/api/exceptions.py
--rw-rw-rw-   0        0        0     5165 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/api/formatters.py
--rw-rw-rw-   0        0        0     2625 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/api/jukebox.py
--rw-rw-rw-   0        0        0    15944 2023-03-18 14:45:11.000000 Supysonic-0.7.6/supysonic/api/media.py
--rw-rw-rw-   0        0        0     3394 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/api/playlists.py
--rw-rw-rw-   0        0        0     1878 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/api/radio.py
--rw-rw-rw-   0        0        0     1367 2021-11-28 15:13:37.000000 Supysonic-0.7.6/supysonic/api/scan.py
--rw-rw-rw-   0        0        0     6948 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/api/search.py
--rw-rw-rw-   0        0        0      434 2021-11-28 15:13:37.000000 Supysonic-0.7.6/supysonic/api/system.py
--rw-rw-rw-   0        0        0      661 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/api/unsupported.py
--rw-rw-rw-   0        0        0     2883 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/api/user.py
--rw-rw-rw-   0        0        0     7911 2021-01-23 14:44:54.000000 Supysonic-0.7.6/supysonic/cache.py
--rw-rw-rw-   0        0        0     9784 2023-04-20 14:50:42.000000 Supysonic-0.7.6/supysonic/cli.py
--rw-rw-rw-   0        0        0     2708 2023-04-10 13:06:12.000000 Supysonic-0.7.6/supysonic/config.py
--rw-rw-rw-   0        0        0     2070 2022-01-30 15:22:37.000000 Supysonic-0.7.6/supysonic/covers.py
-drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.696579 Supysonic-0.7.6/supysonic/daemon/
--rw-rw-rw-   0        0        0     1668 2023-04-20 15:15:30.000000 Supysonic-0.7.6/supysonic/daemon/__init__.py
--rw-rw-rw-   0        0        0      259 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/daemon/__main__.py
--rw-rw-rw-   0        0        0     5313 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/daemon/client.py
--rw-rw-rw-   0        0        0      252 2021-01-23 14:44:54.000000 Supysonic-0.7.6/supysonic/daemon/exceptions.py
--rw-rw-rw-   0        0        0     3744 2023-04-20 15:57:38.000000 Supysonic-0.7.6/supysonic/daemon/server.py
--rw-rw-rw-   0        0        0    20278 2023-05-01 12:09:18.000000 Supysonic-0.7.6/supysonic/db.py
-drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.696579 Supysonic-0.7.6/supysonic/frontend/
--rw-rw-rw-   0        0        0     2382 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/frontend/__init__.py
--rw-rw-rw-   0        0        0     2747 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/frontend/folder.py
--rw-rw-rw-   0        0        0     2627 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/frontend/playlist.py
--rw-rw-rw-   0        0        0     9366 2023-07-14 10:03:57.000000 Supysonic-0.7.6/supysonic/frontend/user.py
--rw-rw-rw-   0        0        0     4204 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/jukebox.py
--rw-rw-rw-   0        0        0     3519 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/lastfm.py
-drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.696579 Supysonic-0.7.6/supysonic/managers/
--rw-rw-rw-   0        0        0      200 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/managers/__init__.py
--rw-rw-rw-   0        0        0     2173 2023-02-11 13:36:47.000000 Supysonic-0.7.6/supysonic/managers/folder.py
--rw-rw-rw-   0        0        0     2528 2023-05-01 12:09:18.000000 Supysonic-0.7.6/supysonic/managers/user.py
--rw-rw-rw-   0        0        0    13097 2023-04-20 15:57:38.000000 Supysonic-0.7.6/supysonic/scanner.py
-drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.696579 Supysonic-0.7.6/supysonic/schema/
-drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.672073 Supysonic-0.7.6/supysonic/schema/migration/
-drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.706673 Supysonic-0.7.6/supysonic/schema/migration/mysql/
--rw-rw-rw-   0        0        0      292 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20161030.sql
--rw-rw-rw-   0        0        0      227 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20171022.sql
--rw-rw-rw-   0        0        0     2758 2023-01-08 15:12:52.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20171230.py
--rw-rw-rw-   0        0        0     3030 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20180221.sql
--rw-rw-rw-   0        0        0      386 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20180317.sql
--rw-rw-rw-   0        0        0      208 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20180521.sql
--rw-rw-rw-   0        0        0       63 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20181010.sql
--rw-rw-rw-   0        0        0     1452 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20190324.sql
--rw-rw-rw-   0        0        0       44 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20190518.sql
--rw-rw-rw-   0        0        0     2767 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20190915.sql
--rw-rw-rw-   0        0        0       73 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20190921.sql
--rw-rw-rw-   0        0        0      266 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20200607.sql
--rw-rw-rw-   0        0        0     2745 2023-02-11 13:36:47.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20230111.py
--rw-rw-rw-   0        0        0      155 2023-02-11 13:36:47.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20230115.sql
--rw-rw-rw-   0        0        0       88 2023-04-10 13:06:12.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/20230331.sql
-drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.706673 Supysonic-0.7.6/supysonic/schema/migration/mysql/__pycache__/
--rw-rw-rw-   0        0        0     2400 2023-01-11 21:50:42.000000 Supysonic-0.7.6/supysonic/schema/migration/mysql/__pycache__/20230111.cpython-38.pyc
-drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.716560 Supysonic-0.7.6/supysonic/schema/migration/postgres/
--rw-rw-rw-   0        0        0      267 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/postgres/20161030.sql
--rw-rw-rw-   0        0        0      232 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/postgres/20171022.sql
--rw-rw-rw-   0        0        0      229 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/postgres/20180311.sql
--rw-rw-rw-   0        0        0     1136 2023-01-08 15:12:52.000000 Supysonic-0.7.6/supysonic/schema/migration/postgres/20180317.py
--rw-rw-rw-   0        0        0      188 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/postgres/20180521.sql
--rw-rw-rw-   0        0        0       63 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/postgres/20181010.sql
--rw-rw-rw-   0        0        0     1748 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/postgres/20190324.sql
--rw-rw-rw-   0        0        0       44 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/postgres/20190518.sql
--rw-rw-rw-   0        0        0     3649 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/postgres/20190915.sql
--rw-rw-rw-   0        0        0       63 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/postgres/20190921.sql
--rw-rw-rw-   0        0        0      204 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/postgres/20200607.sql
--rw-rw-rw-   0        0        0      153 2023-02-11 13:36:47.000000 Supysonic-0.7.6/supysonic/schema/migration/postgres/20230115.sql
--rw-rw-rw-   0        0        0       88 2023-04-10 13:06:12.000000 Supysonic-0.7.6/supysonic/schema/migration/postgres/20230331.sql
-drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.716560 Supysonic-0.7.6/supysonic/schema/migration/sqlite/
--rw-rw-rw-   0        0        0     1176 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20161030.sql
--rw-rw-rw-   0        0        0      882 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20171022.sql
--rw-rw-rw-   0        0        0     2032 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20171230.py
--rw-rw-rw-   0        0        0     1629 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20180311.sql
--rw-rw-rw-   0        0        0      939 2023-01-08 15:12:52.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20180317.py
--rw-rw-rw-   0        0        0      754 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20180521.sql
--rw-rw-rw-   0        0        0       63 2021-01-23 14:44:55.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20181010.sql
--rw-rw-rw-   0        0        0     1746 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20190324.sql
--rw-rw-rw-   0        0        0     1858 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20190518.sql
--rw-rw-rw-   0        0        0     5084 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20190915.sql
--rw-rw-rw-   0        0        0       61 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20190921.sql
--rw-rw-rw-   0        0        0      207 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20200607.sql
--rw-rw-rw-   0        0        0     1924 2023-02-11 13:36:47.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20230111.py
--rw-rw-rw-   0        0        0      499 2023-02-11 13:36:47.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20230115.sql
--rw-rw-rw-   0        0        0       87 2023-04-10 13:06:12.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/20230331.sql
-drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.716560 Supysonic-0.7.6/supysonic/schema/migration/sqlite/__pycache__/
--rw-rw-rw-   0        0        0     1743 2023-02-11 13:37:00.000000 Supysonic-0.7.6/supysonic/schema/migration/sqlite/__pycache__/20230111.cpython-38.pyc
--rw-rw-rw-   0        0        0     6463 2023-04-10 13:06:12.000000 Supysonic-0.7.6/supysonic/schema/mysql.sql
--rw-rw-rw-   0        0        0     5689 2023-04-10 13:06:12.000000 Supysonic-0.7.6/supysonic/schema/postgres.sql
--rw-rw-rw-   0        0        0     5952 2023-04-10 13:06:12.000000 Supysonic-0.7.6/supysonic/schema/sqlite.sql
-drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.726771 Supysonic-0.7.6/supysonic/server/
--rw-rw-rw-   0        0        0     3395 2023-03-25 14:13:16.000000 Supysonic-0.7.6/supysonic/server/__init__.py
--rw-rw-rw-   0        0        0      259 2021-11-01 14:23:27.000000 Supysonic-0.7.6/supysonic/server/__main__.py
--rw-rw-rw-   0        0        0      828 2023-03-25 14:13:16.000000 Supysonic-0.7.6/supysonic/server/_base.py
--rw-rw-rw-   0        0        0      936 2023-02-11 13:36:47.000000 Supysonic-0.7.6/supysonic/server/gevent.py
--rw-rw-rw-   0        0        0     1289 2023-03-25 14:13:16.000000 Supysonic-0.7.6/supysonic/server/gunicorn.py
--rw-rw-rw-   0        0        0      780 2023-03-25 14:13:16.000000 Supysonic-0.7.6/supysonic/server/waitress.py
-drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.672073 Supysonic-0.7.6/supysonic/static/
-drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.726771 Supysonic-0.7.6/supysonic/static/css/
--rw-rw-rw-   0        0        0    23409 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/static/css/bootstrap-theme.min.css
--rw-rw-rw-   0        0        0    25648 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/static/css/bootstrap-theme.min.css.map
--rw-rw-rw-   0        0        0   121200 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/static/css/bootstrap.min.css
--rw-rw-rw-   0        0        0   542194 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/static/css/bootstrap.min.css.map
--rw-rw-rw-   0        0        0      794 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/static/css/supysonic.css
-drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.736752 Supysonic-0.7.6/supysonic/static/fonts/
--rw-rw-rw-   0        0        0    20127 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/static/fonts/glyphicons-halflings-regular.eot
--rw-rw-rw-   0        0        0   108738 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/static/fonts/glyphicons-halflings-regular.svg
--rw-rw-rw-   0        0        0    45404 2021-01-23 14:45:18.000000 Supysonic-0.7.6/supysonic/static/fonts/glyphicons-halflings-regular.ttf
--rw-rw-rw-   0        0        0    23424 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/static/fonts/glyphicons-halflings-regular.woff
--rw-rw-rw-   0        0        0    18028 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/static/fonts/glyphicons-halflings-regular.woff2
-drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.736752 Supysonic-0.7.6/supysonic/static/js/
--rw-rw-rw-   0        0        0    37045 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/static/js/bootstrap.min.js
--rw-rw-rw-   0        0        0      441 2021-04-10 13:49:54.000000 Supysonic-0.7.6/supysonic/static/js/supysonic.js
-drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.746615 Supysonic-0.7.6/supysonic/templates/
--rw-rw-rw-   0        0        0     1336 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/templates/addfolder.html
--rw-rw-rw-   0        0        0     2229 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/templates/adduser.html
--rw-rw-rw-   0        0        0     1346 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/templates/change_mail.html
--rw-rw-rw-   0        0        0     2053 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/templates/change_pass.html
--rw-rw-rw-   0        0        0     1179 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/templates/change_username.html
--rw-rw-rw-   0        0        0     2584 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/templates/folders.html
--rw-rw-rw-   0        0        0     2867 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/templates/home.html
--rw-rw-rw-   0        0        0     4204 2021-11-28 14:09:30.000000 Supysonic-0.7.6/supysonic/templates/layout.html
--rw-rw-rw-   0        0        0     1656 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/templates/login.html
--rw-rw-rw-   0        0        0     1478 2021-04-10 13:49:44.000000 Supysonic-0.7.6/supysonic/templates/playlist.html
--rw-rw-rw-   0        0        0      314 2021-04-10 13:49:54.000000 Supysonic-0.7.6/supysonic/templates/playlist_export.m3u
--rw-rw-rw-   0        0        0     4380 2021-04-10 13:49:54.000000 Supysonic-0.7.6/supysonic/templates/playlists.html
--rw-rw-rw-   0        0        0     6598 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/templates/profile.html
--rw-rw-rw-   0        0        0     2378 2021-01-23 14:44:56.000000 Supysonic-0.7.6/supysonic/templates/users.html
--rw-rw-rw-   0        0        0      640 2023-02-11 13:34:27.000000 Supysonic-0.7.6/supysonic/utils.py
--rw-rw-rw-   0        0        0     9565 2023-04-21 14:53:50.000000 Supysonic-0.7.6/supysonic/watcher.py
--rw-rw-rw-   0        0        0     3067 2023-04-20 16:15:42.000000 Supysonic-0.7.6/supysonic/web.py
-drwxrwxrwx   0        0        0        0 2023-07-14 13:28:31.746615 Supysonic-0.7.6/tests/
--rw-rw-rw-   0        0        0     3386 2023-02-11 13:34:27.000000 Supysonic-0.7.6/tests/testbase.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:14:58.833661 supysonic-0.7.7/
+-rw-rw-rw-   0        0        0    34520 2021-01-23 14:44:54.000000 supysonic-0.7.7/LICENSE
+-rw-rw-rw-   0        0        0      154 2021-12-19 16:15:13.000000 supysonic-0.7.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2000 2024-05-19 15:14:57.378676 supysonic-0.7.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2836 2024-04-01 10:14:48.000000 supysonic-0.7.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 15:14:57.378676 supysonic-0.7.7/Supysonic.egg-info/
+-rw-rw-rw-   0        0        0     2000 2024-05-19 15:14:57.000000 supysonic-0.7.7/Supysonic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5112 2024-05-19 15:14:57.000000 supysonic-0.7.7/Supysonic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 15:14:57.000000 supysonic-0.7.7/Supysonic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2024-05-19 15:14:57.000000 supysonic-0.7.7/Supysonic.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2021-12-31 16:33:42.000000 supysonic-0.7.7/Supysonic.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      108 2024-05-19 15:14:57.000000 supysonic-0.7.7/Supysonic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-19 15:14:57.000000 supysonic-0.7.7/Supysonic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3110 2024-04-01 10:14:48.000000 supysonic-0.7.7/config.sample
+drwxrwxrwx   0        0        0        0 2024-05-19 15:14:59.308660 supysonic-0.7.7/man/
+-rw-rw-rw-   0        0        0     3675 2024-05-19 15:14:59.228533 supysonic-0.7.7/man/supysonic-cli-folder.1
+-rw-rw-rw-   0        0        0     4128 2024-05-19 15:14:59.228533 supysonic-0.7.7/man/supysonic-cli-user.1
+-rw-rw-rw-   0        0        0     2769 2024-05-19 15:14:59.218843 supysonic-0.7.7/man/supysonic-cli.1
+-rw-rw-rw-   0        0        0     1852 2024-05-19 15:14:59.228533 supysonic-0.7.7/man/supysonic-daemon.1
+-rw-rw-rw-   0        0        0     2984 2024-05-19 15:14:59.228533 supysonic-0.7.7/man/supysonic-server.1
+-rw-rw-rw-   0        0        0      108 2022-04-23 14:58:53.000000 supysonic-0.7.7/pyproject.toml
+-rw-rw-rw-   0        0        0     2216 2024-05-19 15:14:57.378676 supysonic-0.7.7/setup.cfg
+-rw-rw-rw-   0        0        0      744 2023-06-18 13:52:50.000000 supysonic-0.7.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:14:57.308684 supysonic-0.7.7/supysonic/
+-rw-rw-rw-   0        0        0      534 2024-05-19 15:13:56.000000 supysonic-0.7.7/supysonic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:14:57.318635 supysonic-0.7.7/supysonic/api/
+-rw-rw-rw-   0        0        0     4059 2024-01-02 14:07:09.000000 supysonic-0.7.7/supysonic/api/__init__.py
+-rw-rw-rw-   0        0        0     9758 2023-03-18 16:38:26.000000 supysonic-0.7.7/supysonic/api/albums_songs.py
+-rw-rw-rw-   0        0        0     5112 2024-04-01 10:14:48.000000 supysonic-0.7.7/supysonic/api/annotation.py
+-rw-rw-rw-   0        0        0     5690 2023-02-11 13:36:47.000000 supysonic-0.7.7/supysonic/api/browse.py
+-rw-rw-rw-   0        0        0      856 2023-02-11 13:34:27.000000 supysonic-0.7.7/supysonic/api/chat.py
+-rw-rw-rw-   0        0        0     1035 2023-02-25 16:35:07.000000 supysonic-0.7.7/supysonic/api/errors.py
+-rw-rw-rw-   0        0        0     3585 2023-02-11 13:34:27.000000 supysonic-0.7.7/supysonic/api/exceptions.py
+-rw-rw-rw-   0        0        0     5229 2024-05-19 14:01:13.000000 supysonic-0.7.7/supysonic/api/formatters.py
+-rw-rw-rw-   0        0        0     2625 2023-02-11 13:34:27.000000 supysonic-0.7.7/supysonic/api/jukebox.py
+-rw-rw-rw-   0        0        0    15944 2023-03-18 14:45:11.000000 supysonic-0.7.7/supysonic/api/media.py
+-rw-rw-rw-   0        0        0     3394 2023-02-11 13:34:27.000000 supysonic-0.7.7/supysonic/api/playlists.py
+-rw-rw-rw-   0        0        0     1878 2023-02-11 13:34:27.000000 supysonic-0.7.7/supysonic/api/radio.py
+-rw-rw-rw-   0        0        0     1367 2021-11-28 15:13:37.000000 supysonic-0.7.7/supysonic/api/scan.py
+-rw-rw-rw-   0        0        0     7052 2024-05-19 14:01:13.000000 supysonic-0.7.7/supysonic/api/search.py
+-rw-rw-rw-   0        0        0      434 2021-11-28 15:13:37.000000 supysonic-0.7.7/supysonic/api/system.py
+-rw-rw-rw-   0        0        0      661 2023-02-11 13:34:27.000000 supysonic-0.7.7/supysonic/api/unsupported.py
+-rw-rw-rw-   0        0        0     2883 2023-02-11 13:34:27.000000 supysonic-0.7.7/supysonic/api/user.py
+-rw-rw-rw-   0        0        0     7911 2021-01-23 14:44:54.000000 supysonic-0.7.7/supysonic/cache.py
+-rw-rw-rw-   0        0        0     9784 2023-04-20 14:50:42.000000 supysonic-0.7.7/supysonic/cli.py
+-rw-rw-rw-   0        0        0     2803 2024-05-19 14:01:13.000000 supysonic-0.7.7/supysonic/config.py
+-rw-rw-rw-   0        0        0     2070 2022-01-30 15:22:37.000000 supysonic-0.7.7/supysonic/covers.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:14:57.318635 supysonic-0.7.7/supysonic/daemon/
+-rw-rw-rw-   0        0        0     1668 2023-04-20 15:15:30.000000 supysonic-0.7.7/supysonic/daemon/__init__.py
+-rw-rw-rw-   0        0        0      259 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/daemon/__main__.py
+-rw-rw-rw-   0        0        0     5313 2023-02-11 13:34:27.000000 supysonic-0.7.7/supysonic/daemon/client.py
+-rw-rw-rw-   0        0        0      252 2021-01-23 14:44:54.000000 supysonic-0.7.7/supysonic/daemon/exceptions.py
+-rw-rw-rw-   0        0        0     3744 2023-04-20 15:57:38.000000 supysonic-0.7.7/supysonic/daemon/server.py
+-rw-rw-rw-   0        0        0    21098 2024-05-19 14:01:13.000000 supysonic-0.7.7/supysonic/db.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:14:57.318635 supysonic-0.7.7/supysonic/frontend/
+-rw-rw-rw-   0        0        0     2382 2023-02-11 13:34:27.000000 supysonic-0.7.7/supysonic/frontend/__init__.py
+-rw-rw-rw-   0        0        0     2747 2023-02-11 13:34:27.000000 supysonic-0.7.7/supysonic/frontend/folder.py
+-rw-rw-rw-   0        0        0     2627 2023-02-11 13:34:27.000000 supysonic-0.7.7/supysonic/frontend/playlist.py
+-rw-rw-rw-   0        0        0    10223 2024-04-01 10:14:48.000000 supysonic-0.7.7/supysonic/frontend/user.py
+-rw-rw-rw-   0        0        0     4204 2023-02-11 13:34:27.000000 supysonic-0.7.7/supysonic/jukebox.py
+-rw-rw-rw-   0        0        0     3519 2023-02-11 13:34:27.000000 supysonic-0.7.7/supysonic/lastfm.py
+-rw-rw-rw-   0        0        0     4259 2024-05-19 14:01:13.000000 supysonic-0.7.7/supysonic/listenbrainz.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:14:57.318635 supysonic-0.7.7/supysonic/managers/
+-rw-rw-rw-   0        0        0      200 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/managers/__init__.py
+-rw-rw-rw-   0        0        0     2173 2023-02-11 13:36:47.000000 supysonic-0.7.7/supysonic/managers/folder.py
+-rw-rw-rw-   0        0        0     2528 2023-05-01 12:09:18.000000 supysonic-0.7.7/supysonic/managers/user.py
+-rw-rw-rw-   0        0        0    13097 2023-04-20 15:57:38.000000 supysonic-0.7.7/supysonic/scanner.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:14:57.318635 supysonic-0.7.7/supysonic/schema/
+drwxrwxrwx   0        0        0        0 2024-05-19 15:14:57.288645 supysonic-0.7.7/supysonic/schema/migration/
+drwxrwxrwx   0        0        0        0 2024-05-19 15:14:57.333696 supysonic-0.7.7/supysonic/schema/migration/mysql/
+-rw-rw-rw-   0        0        0      292 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/schema/migration/mysql/20161030.sql
+-rw-rw-rw-   0        0        0      227 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/schema/migration/mysql/20171022.sql
+-rw-rw-rw-   0        0        0     2758 2023-01-08 15:12:52.000000 supysonic-0.7.7/supysonic/schema/migration/mysql/20171230.py
+-rw-rw-rw-   0        0        0     3030 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/schema/migration/mysql/20180221.sql
+-rw-rw-rw-   0        0        0      386 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/schema/migration/mysql/20180317.sql
+-rw-rw-rw-   0        0        0      208 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/schema/migration/mysql/20180521.sql
+-rw-rw-rw-   0        0        0       63 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/schema/migration/mysql/20181010.sql
+-rw-rw-rw-   0        0        0     1452 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/schema/migration/mysql/20190324.sql
+-rw-rw-rw-   0        0        0       44 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/schema/migration/mysql/20190518.sql
+-rw-rw-rw-   0        0        0     2767 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/schema/migration/mysql/20190915.sql
+-rw-rw-rw-   0        0        0       73 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/schema/migration/mysql/20190921.sql
+-rw-rw-rw-   0        0        0      266 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/schema/migration/mysql/20200607.sql
+-rw-rw-rw-   0        0        0     2745 2023-02-11 13:36:47.000000 supysonic-0.7.7/supysonic/schema/migration/mysql/20230111.py
+-rw-rw-rw-   0        0        0      155 2023-02-11 13:36:47.000000 supysonic-0.7.7/supysonic/schema/migration/mysql/20230115.sql
+-rw-rw-rw-   0        0        0       88 2023-04-10 13:06:12.000000 supysonic-0.7.7/supysonic/schema/migration/mysql/20230331.sql
+-rw-rw-rw-   0        0        0      124 2024-04-01 10:14:48.000000 supysonic-0.7.7/supysonic/schema/migration/mysql/20240318.sql
+drwxrwxrwx   0        0        0        0 2024-05-19 15:14:57.333696 supysonic-0.7.7/supysonic/schema/migration/mysql/__pycache__/
+-rw-rw-rw-   0        0        0     2400 2023-01-11 21:50:42.000000 supysonic-0.7.7/supysonic/schema/migration/mysql/__pycache__/20230111.cpython-38.pyc
+drwxrwxrwx   0        0        0        0 2024-05-19 15:14:57.343706 supysonic-0.7.7/supysonic/schema/migration/postgres/
+-rw-rw-rw-   0        0        0      267 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/schema/migration/postgres/20161030.sql
+-rw-rw-rw-   0        0        0      232 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/schema/migration/postgres/20171022.sql
+-rw-rw-rw-   0        0        0      229 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/schema/migration/postgres/20180311.sql
+-rw-rw-rw-   0        0        0     1136 2023-01-08 15:12:52.000000 supysonic-0.7.7/supysonic/schema/migration/postgres/20180317.py
+-rw-rw-rw-   0        0        0      188 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/schema/migration/postgres/20180521.sql
+-rw-rw-rw-   0        0        0       63 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/schema/migration/postgres/20181010.sql
+-rw-rw-rw-   0        0        0     1748 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/schema/migration/postgres/20190324.sql
+-rw-rw-rw-   0        0        0       44 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/schema/migration/postgres/20190518.sql
+-rw-rw-rw-   0        0        0     3649 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/schema/migration/postgres/20190915.sql
+-rw-rw-rw-   0        0        0       63 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/schema/migration/postgres/20190921.sql
+-rw-rw-rw-   0        0        0      204 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/schema/migration/postgres/20200607.sql
+-rw-rw-rw-   0        0        0      153 2023-02-11 13:36:47.000000 supysonic-0.7.7/supysonic/schema/migration/postgres/20230115.sql
+-rw-rw-rw-   0        0        0       88 2023-04-10 13:06:12.000000 supysonic-0.7.7/supysonic/schema/migration/postgres/20230331.sql
+-rw-rw-rw-   0        0        0      138 2024-04-01 10:14:48.000000 supysonic-0.7.7/supysonic/schema/migration/postgres/20240318.sql
+drwxrwxrwx   0        0        0        0 2024-05-19 15:14:57.348740 supysonic-0.7.7/supysonic/schema/migration/sqlite/
+-rw-rw-rw-   0        0        0     1176 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/schema/migration/sqlite/20161030.sql
+-rw-rw-rw-   0        0        0      882 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/schema/migration/sqlite/20171022.sql
+-rw-rw-rw-   0        0        0     2032 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/schema/migration/sqlite/20171230.py
+-rw-rw-rw-   0        0        0     1629 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/schema/migration/sqlite/20180311.sql
+-rw-rw-rw-   0        0        0      939 2023-01-08 15:12:52.000000 supysonic-0.7.7/supysonic/schema/migration/sqlite/20180317.py
+-rw-rw-rw-   0        0        0      754 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/schema/migration/sqlite/20180521.sql
+-rw-rw-rw-   0        0        0       63 2021-01-23 14:44:55.000000 supysonic-0.7.7/supysonic/schema/migration/sqlite/20181010.sql
+-rw-rw-rw-   0        0        0     1746 2021-01-23 14:44:56.000000 supysonic-0.7.7/supysonic/schema/migration/sqlite/20190324.sql
+-rw-rw-rw-   0        0        0     1858 2021-01-23 14:44:56.000000 supysonic-0.7.7/supysonic/schema/migration/sqlite/20190518.sql
+-rw-rw-rw-   0        0        0     5084 2021-01-23 14:44:56.000000 supysonic-0.7.7/supysonic/schema/migration/sqlite/20190915.sql
+-rw-rw-rw-   0        0        0       61 2021-01-23 14:44:56.000000 supysonic-0.7.7/supysonic/schema/migration/sqlite/20190921.sql
+-rw-rw-rw-   0        0        0      207 2021-01-23 14:44:56.000000 supysonic-0.7.7/supysonic/schema/migration/sqlite/20200607.sql
+-rw-rw-rw-   0        0        0     1924 2023-02-11 13:36:47.000000 supysonic-0.7.7/supysonic/schema/migration/sqlite/20230111.py
+-rw-rw-rw-   0        0        0      499 2023-02-11 13:36:47.000000 supysonic-0.7.7/supysonic/schema/migration/sqlite/20230115.sql
+-rw-rw-rw-   0        0        0       87 2023-04-10 13:06:12.000000 supysonic-0.7.7/supysonic/schema/migration/sqlite/20230331.sql
+-rw-rw-rw-   0        0        0      124 2024-04-01 10:14:48.000000 supysonic-0.7.7/supysonic/schema/migration/sqlite/20240318.sql
+drwxrwxrwx   0        0        0        0 2024-05-19 15:14:57.348740 supysonic-0.7.7/supysonic/schema/migration/sqlite/__pycache__/
+-rw-rw-rw-   0        0        0     1780 2023-11-25 16:15:50.000000 supysonic-0.7.7/supysonic/schema/migration/sqlite/__pycache__/20230111.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1743 2023-02-11 13:37:00.000000 supysonic-0.7.7/supysonic/schema/migration/sqlite/__pycache__/20230111.cpython-38.pyc
+-rw-rw-rw-   0        0        0      302 2024-05-19 13:54:08.000000 supysonic-0.7.7/supysonic/schema/migration/sqlite/__pycache__/20240516.cpython-312.pyc
+-rw-rw-rw-   0        0        0     6540 2024-04-01 10:14:48.000000 supysonic-0.7.7/supysonic/schema/mysql.sql
+-rw-rw-rw-   0        0        0     5766 2024-04-01 10:14:48.000000 supysonic-0.7.7/supysonic/schema/postgres.sql
+-rw-rw-rw-   0        0        0     6029 2024-04-01 10:14:48.000000 supysonic-0.7.7/supysonic/schema/sqlite.sql
+drwxrwxrwx   0        0        0        0 2024-05-19 15:14:57.358645 supysonic-0.7.7/supysonic/server/
+-rw-rw-rw-   0        0        0     3405 2024-05-19 14:01:13.000000 supysonic-0.7.7/supysonic/server/__init__.py
+-rw-rw-rw-   0        0        0      259 2021-11-01 14:23:27.000000 supysonic-0.7.7/supysonic/server/__main__.py
+-rw-rw-rw-   0        0        0      812 2024-05-19 14:01:13.000000 supysonic-0.7.7/supysonic/server/_base.py
+-rw-rw-rw-   0        0        0      936 2023-02-11 13:36:47.000000 supysonic-0.7.7/supysonic/server/gevent.py
+-rw-rw-rw-   0        0        0     1289 2023-03-25 14:13:16.000000 supysonic-0.7.7/supysonic/server/gunicorn.py
+-rw-rw-rw-   0        0        0      780 2023-03-25 14:13:16.000000 supysonic-0.7.7/supysonic/server/waitress.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:14:57.288645 supysonic-0.7.7/supysonic/static/
+drwxrwxrwx   0        0        0        0 2024-05-19 15:14:57.358645 supysonic-0.7.7/supysonic/static/css/
+-rw-rw-rw-   0        0        0    23409 2021-01-23 14:44:56.000000 supysonic-0.7.7/supysonic/static/css/bootstrap-theme.min.css
+-rw-rw-rw-   0        0        0    25648 2021-01-23 14:44:56.000000 supysonic-0.7.7/supysonic/static/css/bootstrap-theme.min.css.map
+-rw-rw-rw-   0        0        0   121200 2021-01-23 14:44:56.000000 supysonic-0.7.7/supysonic/static/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0   542194 2021-01-23 14:44:56.000000 supysonic-0.7.7/supysonic/static/css/bootstrap.min.css.map
+-rw-rw-rw-   0        0        0      794 2021-01-23 14:44:56.000000 supysonic-0.7.7/supysonic/static/css/supysonic.css
+drwxrwxrwx   0        0        0        0 2024-05-19 15:14:57.372167 supysonic-0.7.7/supysonic/static/fonts/
+-rw-rw-rw-   0        0        0    20127 2021-01-23 14:44:56.000000 supysonic-0.7.7/supysonic/static/fonts/glyphicons-halflings-regular.eot
+-rw-rw-rw-   0        0        0   108738 2021-01-23 14:44:56.000000 supysonic-0.7.7/supysonic/static/fonts/glyphicons-halflings-regular.svg
+-rw-rw-rw-   0        0        0    45404 2021-01-23 14:45:18.000000 supysonic-0.7.7/supysonic/static/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-rw-   0        0        0    23424 2021-01-23 14:44:56.000000 supysonic-0.7.7/supysonic/static/fonts/glyphicons-halflings-regular.woff
+-rw-rw-rw-   0        0        0    18028 2021-01-23 14:44:56.000000 supysonic-0.7.7/supysonic/static/fonts/glyphicons-halflings-regular.woff2
+drwxrwxrwx   0        0        0        0 2024-05-19 15:14:57.372167 supysonic-0.7.7/supysonic/static/js/
+-rw-rw-rw-   0        0        0    37045 2021-01-23 14:44:56.000000 supysonic-0.7.7/supysonic/static/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0      441 2021-04-10 13:49:54.000000 supysonic-0.7.7/supysonic/static/js/supysonic.js
+drwxrwxrwx   0        0        0        0 2024-05-19 15:14:57.378676 supysonic-0.7.7/supysonic/templates/
+-rw-rw-rw-   0        0        0     1336 2021-01-23 14:44:56.000000 supysonic-0.7.7/supysonic/templates/addfolder.html
+-rw-rw-rw-   0        0        0     2229 2021-01-23 14:44:56.000000 supysonic-0.7.7/supysonic/templates/adduser.html
+-rw-rw-rw-   0        0        0     1346 2021-01-23 14:44:56.000000 supysonic-0.7.7/supysonic/templates/change_mail.html
+-rw-rw-rw-   0        0        0     2053 2021-01-23 14:44:56.000000 supysonic-0.7.7/supysonic/templates/change_pass.html
+-rw-rw-rw-   0        0        0     1179 2021-01-23 14:44:56.000000 supysonic-0.7.7/supysonic/templates/change_username.html
+-rw-rw-rw-   0        0        0     2584 2021-01-23 14:44:56.000000 supysonic-0.7.7/supysonic/templates/folders.html
+-rw-rw-rw-   0        0        0     2867 2021-01-23 14:44:56.000000 supysonic-0.7.7/supysonic/templates/home.html
+-rw-rw-rw-   0        0        0     4204 2021-11-28 14:09:30.000000 supysonic-0.7.7/supysonic/templates/layout.html
+-rw-rw-rw-   0        0        0     1656 2021-01-23 14:44:56.000000 supysonic-0.7.7/supysonic/templates/login.html
+-rw-rw-rw-   0        0        0     1478 2021-04-10 13:49:44.000000 supysonic-0.7.7/supysonic/templates/playlist.html
+-rw-rw-rw-   0        0        0      314 2021-04-10 13:49:54.000000 supysonic-0.7.7/supysonic/templates/playlist_export.m3u
+-rw-rw-rw-   0        0        0     4380 2021-04-10 13:49:54.000000 supysonic-0.7.7/supysonic/templates/playlists.html
+-rw-rw-rw-   0        0        0     8137 2024-04-01 10:14:48.000000 supysonic-0.7.7/supysonic/templates/profile.html
+-rw-rw-rw-   0        0        0     2378 2021-01-23 14:44:56.000000 supysonic-0.7.7/supysonic/templates/users.html
+-rw-rw-rw-   0        0        0      640 2023-02-11 13:34:27.000000 supysonic-0.7.7/supysonic/utils.py
+-rw-rw-rw-   0        0        0     9727 2024-04-14 13:50:56.000000 supysonic-0.7.7/supysonic/watcher.py
+-rw-rw-rw-   0        0        0     3067 2023-04-20 16:15:42.000000 supysonic-0.7.7/supysonic/web.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:14:57.378676 supysonic-0.7.7/tests/
+-rw-rw-rw-   0        0        0     3386 2023-02-11 13:34:27.000000 supysonic-0.7.7/tests/testbase.py
```

### Comparing `Supysonic-0.7.6/LICENSE` & `supysonic-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/PKG-INFO` & `supysonic-0.7.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Supysonic
-Version: 0.7.6
+Version: 0.7.7
 Summary: Python implementation of the Subsonic server API
 Home-page: https://supysonic.readthedocs.io
 Download-URL: https://github.com/spl0k/supysonic
 Author: Alban Féron
 Author-email: alban.feron@gmail.com
 License: GNU AGPLv3
 Keywords: subsonic,music,server
@@ -17,18 +17,27 @@
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Multimedia :: Sound/Audio
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: click
+Requires-Dist: flask>=0.11
+Requires-Dist: peewee
+Requires-Dist: Pillow>=9.1.0
+Requires-Dist: requests>=1.0.0
+Requires-Dist: mediafile
+Requires-Dist: watchdog>=0.8.0
+Requires-Dist: zipstream-ng<2.0.0,>=1.1.0
 
 
 Supysonic is a Python implementation of the [Subsonic][] server API.
 
 Current supported features are:
 * browsing (by folders or tags)
 * streaming of various audio file formats
```

### Comparing `Supysonic-0.7.6/README.md` & `supysonic-0.7.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 * browsing (by folders or tags)
 * streaming of various audio file formats
 * transcoding
 * user or random playlists
 * cover art
 * starred tracks/albums and ratings
 * [Last.fm][lastfm] scrobbling
+* [ListenBrainz][listenbrainz] scrobbling
 * Jukebox mode
 
 Supysonic currently targets the version 1.12.0 of the Subsonic API. For more
 details, go check the [API implementation status][docs-api].
 
 [subsonic]: http://www.subsonic.org/
 [lastfm]: https://www.last.fm/
+[listenbrainz]: https://listenbrainz.org/
 [docs-api]: https://supysonic.readthedocs.io/en/latest/api.html
 
 ## Documentation
 
 Full documentation is available at https://supysonic.readthedocs.io/
 
 ## Quickstart
@@ -68,10 +70,10 @@
 And there's also the tests (which require `lxml` to run):
 
     $ pip install lxml
     $ python -m unittest
     $ python -m unittest tests.net.suite
 
 The last command runs a few tests that make HTTP requests to remote third-party
-services (namely Last.fm and ChartLyrics).
+services (namely Last.fm, ListenBrainz and ChartLyrics).
 
 [flask]: https://flask.palletsprojects.com/
```

### Comparing `Supysonic-0.7.6/Supysonic.egg-info/PKG-INFO` & `supysonic-0.7.7/Supysonic.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Supysonic
-Version: 0.7.6
+Version: 0.7.7
 Summary: Python implementation of the Subsonic server API
 Home-page: https://supysonic.readthedocs.io
 Download-URL: https://github.com/spl0k/supysonic
 Author: Alban Féron
 Author-email: alban.feron@gmail.com
 License: GNU AGPLv3
 Keywords: subsonic,music,server
@@ -17,18 +17,27 @@
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Multimedia :: Sound/Audio
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: click
+Requires-Dist: flask>=0.11
+Requires-Dist: peewee
+Requires-Dist: Pillow>=9.1.0
+Requires-Dist: requests>=1.0.0
+Requires-Dist: mediafile
+Requires-Dist: watchdog>=0.8.0
+Requires-Dist: zipstream-ng<2.0.0,>=1.1.0
 
 
 Supysonic is a Python implementation of the [Subsonic][] server API.
 
 Current supported features are:
 * browsing (by folders or tags)
 * streaming of various audio file formats
```

### Comparing `Supysonic-0.7.6/Supysonic.egg-info/SOURCES.txt` & `supysonic-0.7.7/Supysonic.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 supysonic/cache.py
 supysonic/cli.py
 supysonic/config.py
 supysonic/covers.py
 supysonic/db.py
 supysonic/jukebox.py
 supysonic/lastfm.py
+supysonic/listenbrainz.py
 supysonic/scanner.py
 supysonic/utils.py
 supysonic/watcher.py
 supysonic/web.py
 supysonic/api/__init__.py
 supysonic/api/albums_songs.py
 supysonic/api/annotation.py
@@ -67,28 +68,30 @@
 supysonic/schema/migration/mysql/20190518.sql
 supysonic/schema/migration/mysql/20190915.sql
 supysonic/schema/migration/mysql/20190921.sql
 supysonic/schema/migration/mysql/20200607.sql
 supysonic/schema/migration/mysql/20230111.py
 supysonic/schema/migration/mysql/20230115.sql
 supysonic/schema/migration/mysql/20230331.sql
+supysonic/schema/migration/mysql/20240318.sql
 supysonic/schema/migration/mysql/__pycache__/20230111.cpython-38.pyc
 supysonic/schema/migration/postgres/20161030.sql
 supysonic/schema/migration/postgres/20171022.sql
 supysonic/schema/migration/postgres/20180311.sql
 supysonic/schema/migration/postgres/20180317.py
 supysonic/schema/migration/postgres/20180521.sql
 supysonic/schema/migration/postgres/20181010.sql
 supysonic/schema/migration/postgres/20190324.sql
 supysonic/schema/migration/postgres/20190518.sql
 supysonic/schema/migration/postgres/20190915.sql
 supysonic/schema/migration/postgres/20190921.sql
 supysonic/schema/migration/postgres/20200607.sql
 supysonic/schema/migration/postgres/20230115.sql
 supysonic/schema/migration/postgres/20230331.sql
+supysonic/schema/migration/postgres/20240318.sql
 supysonic/schema/migration/sqlite/20161030.sql
 supysonic/schema/migration/sqlite/20171022.sql
 supysonic/schema/migration/sqlite/20171230.py
 supysonic/schema/migration/sqlite/20180311.sql
 supysonic/schema/migration/sqlite/20180317.py
 supysonic/schema/migration/sqlite/20180521.sql
 supysonic/schema/migration/sqlite/20181010.sql
@@ -96,15 +99,18 @@
 supysonic/schema/migration/sqlite/20190518.sql
 supysonic/schema/migration/sqlite/20190915.sql
 supysonic/schema/migration/sqlite/20190921.sql
 supysonic/schema/migration/sqlite/20200607.sql
 supysonic/schema/migration/sqlite/20230111.py
 supysonic/schema/migration/sqlite/20230115.sql
 supysonic/schema/migration/sqlite/20230331.sql
+supysonic/schema/migration/sqlite/20240318.sql
+supysonic/schema/migration/sqlite/__pycache__/20230111.cpython-310.pyc
 supysonic/schema/migration/sqlite/__pycache__/20230111.cpython-38.pyc
+supysonic/schema/migration/sqlite/__pycache__/20240516.cpython-312.pyc
 supysonic/server/__init__.py
 supysonic/server/__main__.py
 supysonic/server/_base.py
 supysonic/server/gevent.py
 supysonic/server/gunicorn.py
 supysonic/server/waitress.py
 supysonic/static/css/bootstrap-theme.min.css
```

### Comparing `Supysonic-0.7.6/config.sample` & `supysonic-0.7.7/config.sample`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,19 @@
 
 [lastfm]
 ; API and secret key to enable scrobbling. http://www.last.fm/api/accounts
 ; Defaults: none
 ;api_key =
 ;secret =
 
+[listenbrainz]
+; root URL of the ListenBrainz API.
+; Defaults: https://api.listenbrainz.org/
+;api_url =
+
 [transcoding]
 ; Programs used to convert from one format/bitrate to another. Defaults: none
 transcoder_mp3_mp3 = lame --quiet --mp3input -b %outrate %srcpath -
 transcoder = ffmpeg -i %srcpath -ab %outratek -v 0 -f %outfmt -
 decoder_mp3 = mpg123 --quiet -w - %srcpath
 decoder_ogg = oggdec -o %srcpath
 decoder_flac = flac -d -c -s %srcpath
```

### Comparing `Supysonic-0.7.6/man/supysonic-cli-folder.1` & `supysonic-0.7.7/man/supysonic-cli-folder.1`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "SUPYSONIC-CLI-FOLDER" "1" "Jul 14, 2023" "0.7.6" "Supysonic"
+.TH "SUPYSONIC-CLI-FOLDER" "1" "May 19, 2024" "0.7.7" "Supysonic"
 .SH NAME
 supysonic-cli-folder \- Supysonic folder management commands
 .SH SYNOPSIS
 .sp
 supysonic\-cli folder \fI\-\-help\fP
 .sp
 supysonic\-cli folder \fBlist\fP
```

### Comparing `Supysonic-0.7.6/man/supysonic-cli-user.1` & `supysonic-0.7.7/man/supysonic-cli-user.1`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "SUPYSONIC-CLI-USER" "1" "Jul 14, 2023" "0.7.6" "Supysonic"
+.TH "SUPYSONIC-CLI-USER" "1" "May 19, 2024" "0.7.7" "Supysonic"
 .SH NAME
 supysonic-cli-user \- Supysonic user management commands
 .SH SYNOPSIS
 .sp
 supysonic\-cli user \fI\-\-help\fP
 .sp
 supysonic\-cli user \fBlist\fP
```

### Comparing `Supysonic-0.7.6/man/supysonic-cli.1` & `supysonic-0.7.7/man/supysonic-cli.1`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "SUPYSONIC-CLI" "1" "Jul 14, 2023" "0.7.6" "Supysonic"
+.TH "SUPYSONIC-CLI" "1" "May 19, 2024" "0.7.7" "Supysonic"
 .SH NAME
 supysonic-cli \- Supysonic management command line interface
 .SH SYNOPSIS
 .sp
 supysonic\-cli \fI\-\-help\fP
 .sp
 supysonic\-cli \fBuser\fP [\fIoptions\fP]
```

### Comparing `Supysonic-0.7.6/man/supysonic-daemon.1` & `supysonic-0.7.7/man/supysonic-daemon.1`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "SUPYSONIC-DAEMON" "1" "Jul 14, 2023" "0.7.6" "Supysonic"
+.TH "SUPYSONIC-DAEMON" "1" "May 19, 2024" "0.7.7" "Supysonic"
 .SH NAME
 supysonic-daemon \- Supysonic background daemon
 .SH SYNOPSIS
 .sp
 supysonic\-daemon
 .SH DESCRIPTION
 .sp
```

### Comparing `Supysonic-0.7.6/man/supysonic-server.1` & `supysonic-0.7.7/man/supysonic-server.1`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "SUPYSONIC-SERVER" "1" "Jul 14, 2023" "0.7.6" "Supysonic"
+.TH "SUPYSONIC-SERVER" "1" "May 19, 2024" "0.7.7" "Supysonic"
 .SH NAME
 supysonic-server \- Python implementation of the Subsonic server API
 .SH SYNOPSIS
 .sp
 supysonic\-server [\fB\-\-server\fP \fIgevent\fP | \fIgunicorn\fP | \fIwaitress\fP] [\fB\-\-host\fP <\fIhostname\fP>] [\fB\-\-port\fP <\fIport\fP>] [\fB\-\-socket\fP <\fIpath\fP>] [\fB\-\-processes\fP <\fIn\fP>] [\fB\-\-threads\fP <\fIn\fP>]
 .SH DESCRIPTION
 .sp
```

### Comparing `Supysonic-0.7.6/setup.cfg` & `supysonic-0.7.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 	License :: OSI Approved :: GNU Affero General Public License v3
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Multimedia :: Sound/Audio
 
 [options]
 python_requires = >=3.7
 install_requires = 
 	click
 	flask >=0.11
```

### Comparing `Supysonic-0.7.6/setup.py` & `supysonic-0.7.7/setup.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/__init__.py` & `supysonic-0.7.7/supysonic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 #
 # Copyright (C) 2013-2018 Alban 'spl0k' Féron
 #                    2017 Óscar García Amor
 #
 # Distributed under terms of the GNU AGPLv3 license.
 
 NAME = "Supysonic"
-VERSION = "0.7.6"
+VERSION = "0.7.7"
 DESCRIPTION = "Python implementation of the Subsonic server API"
 AUTHOR = "Alban Féron"
 AUTHOR_EMAIL = "alban.feron@gmail.com"
 URL = "https://supysonic.readthedocs.io/"
 DOWNLOAD_URL = "https://github.com/spl0k/supysonic"
 LICENSE = "GNU AGPLv3"
```

### Comparing `Supysonic-0.7.6/supysonic/api/__init__.py` & `supysonic-0.7.7/supysonic/api/__init__.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/api/albums_songs.py` & `supysonic-0.7.7/supysonic/api/albums_songs.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/api/annotation.py` & `supysonic-0.7.7/supysonic/api/annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from flask import current_app, request
 
 from ..db import Track, Album, Artist, Folder
 from ..db import StarredTrack, StarredAlbum, StarredArtist, StarredFolder
 from ..db import RatingTrack, RatingFolder
 from ..lastfm import LastFm
+from ..listenbrainz import ListenBrainz
 
 from . import get_entity, get_entity_id, api_routing
 from .exceptions import AggregateException, GenericError, MissingParameter, NotFound
 
 
 def star_single(cls, starcls, eid):
     """Stars an entity
@@ -171,14 +172,17 @@
 @api_routing("/scrobble")
 def scrobble():
     res = get_entity(Track)
     t, submission = map(request.values.get, ("time", "submission"))
     t = int(t) / 1000 if t else int(time.time())
 
     lfm = LastFm(current_app.config["LASTFM"], request.user)
+    lbz = ListenBrainz(current_app.config["LISTENBRAINZ"], request.user)
 
     if submission in (None, "", True, "true", "True", 1, "1"):
         lfm.scrobble(res, t)
+        lbz.scrobble(res, t)
     else:
         lfm.now_playing(res)
+        lbz.now_playing(res)
 
     return request.formatter.empty
```

### Comparing `Supysonic-0.7.6/supysonic/api/browse.py` & `supysonic-0.7.7/supysonic/api/browse.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/api/chat.py` & `supysonic-0.7.7/supysonic/api/chat.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/api/errors.py` & `supysonic-0.7.7/supysonic/api/errors.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/api/exceptions.py` & `supysonic-0.7.7/supysonic/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/api/formatters.py` & `supysonic-0.7.7/supysonic/api/formatters.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,17 +38,19 @@
             if isinstance(value, dict):
                 d[key] = self.__remove_empty_lists(value)
             elif isinstance(value, list):
                 if len(value) == 0:
                     keys_to_remove.append(key)
                 else:
                     d[key] = [
-                        self.__remove_empty_lists(item)
-                        if isinstance(item, dict)
-                        else item
+                        (
+                            self.__remove_empty_lists(item)
+                            if isinstance(item, dict)
+                            else item
+                        )
                         for item in value
                     ]
 
         for key in keys_to_remove:
             del d[key]
 
         return d
```

### Comparing `Supysonic-0.7.6/supysonic/api/jukebox.py` & `supysonic-0.7.7/supysonic/api/jukebox.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/api/media.py` & `supysonic-0.7.7/supysonic/api/media.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/api/playlists.py` & `supysonic-0.7.7/supysonic/api/playlists.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/api/radio.py` & `supysonic-0.7.7/supysonic/api/radio.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/api/scan.py` & `supysonic-0.7.7/supysonic/api/scan.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/api/search.py` & `supysonic-0.7.7/supysonic/api/search.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,33 +63,37 @@
 
         return request.formatter(
             "searchResult",
             {
                 "totalHits": folders.count() + tracks.count(),
                 "offset": offset,
                 "match": [
-                    r.as_subsonic_child(request.user)
-                    if isinstance(r, Folder)
-                    else r.as_subsonic_child(request.user, request.client)
+                    (
+                        r.as_subsonic_child(request.user)
+                        if isinstance(r, Folder)
+                        else r.as_subsonic_child(request.user, request.client)
+                    )
                     for r in res
                 ],
             },
         )
     else:
         raise MissingParameter("search")
 
     return request.formatter(
         "searchResult",
         {
             "totalHits": query.count(),
             "offset": offset,
             "match": [
-                r.as_subsonic_child(request.user)
-                if isinstance(r, Folder)
-                else r.as_subsonic_child(request.user, request.client)
+                (
+                    r.as_subsonic_child(request.user)
+                    if isinstance(r, Folder)
+                    else r.as_subsonic_child(request.user, request.client)
+                )
                 for r in query[offset : offset + count]
             ],
         },
     )
 
 
 @api_routing("/search2")
```

### Comparing `Supysonic-0.7.6/supysonic/api/unsupported.py` & `supysonic-0.7.7/supysonic/api/unsupported.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/api/user.py` & `supysonic-0.7.7/supysonic/api/user.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/cache.py` & `supysonic-0.7.7/supysonic/cache.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/cli.py` & `supysonic-0.7.7/supysonic/cli.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/config.py` & `supysonic-0.7.7/supysonic/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,25 +37,28 @@
         "log_rotate": True,
         "mount_webui": True,
         "mount_api": True,
         "index_ignored_prefixes": "El La Le Las Les Los The",
         "online_lyrics": False,
     }
     DAEMON = {
-        "socket": r"\\.\pipe\supysonic"
-        if sys.platform == "win32"
-        else os.path.join(tempdir, "supysonic.sock"),
+        "socket": (
+            r"\\.\pipe\supysonic"
+            if sys.platform == "win32"
+            else os.path.join(tempdir, "supysonic.sock")
+        ),
         "run_watcher": True,
         "wait_delay": 5,
         "jukebox_command": None,
         "log_file": None,
         "log_level": "WARNING",
         "log_rotate": True,
     }
     LASTFM = {"api_key": None, "secret": None}
+    LISTENBRAINZ = {"api_url": "https://api.listenbrainz.org"}
     TRANSCODING = {}
     MIMETYPES = {}
 
     def __init__(self):
         current_config = self
```

### Comparing `Supysonic-0.7.6/supysonic/covers.py` & `supysonic-0.7.7/supysonic/covers.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/daemon/__init__.py` & `supysonic-0.7.7/supysonic/daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/daemon/client.py` & `supysonic-0.7.7/supysonic/daemon/client.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/daemon/server.py` & `supysonic-0.7.7/supysonic/daemon/server.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/db.py` & `supysonic-0.7.7/supysonic/db.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # This file is part of Supysonic.
 # Supysonic is a Python implementation of the Subsonic server API.
 #
-# Copyright (C) 2013-2023 Alban 'spl0k' Féron
+# Copyright (C) 2013-2024 Alban 'spl0k' Féron
 #
 # Distributed under terms of the GNU AGPLv3 license.
 
 import importlib
 import mimetypes
 import os.path
-import pkg_resources
+import sys
 import time
 
 from datetime import datetime
 from hashlib import sha1
 from peewee import (
     AutoField,
     BlobField,
@@ -27,15 +27,15 @@
 )
 from peewee import CompositeKey, DatabaseProxy, Model, MySQLDatabase
 from peewee import fn
 from playhouse.db_url import parseresult_to_dict, schemes
 from urllib.parse import urlparse
 from uuid import UUID, uuid4
 
-SCHEMA_VERSION = "20230331"
+SCHEMA_VERSION = "20240318"
 
 
 def now():
     return datetime.now().replace(microsecond=0)
 
 
 def random():
@@ -435,14 +435,19 @@
     jukebox = BooleanField(default=False)
 
     lastfm_session = FixedCharField(32, null=True)
     lastfm_status = BooleanField(
         default=True
     )  # True: ok/unlinked, False: invalid session
 
+    listenbrainz_session = FixedCharField(36, null=True)
+    listenbrainz_status = BooleanField(
+        default=True
+    )  # True: ok/unlinked, False: invalid token
+
     last_play = ForeignKeyField(Track, null=True, backref="+")
     last_play_date = DateTimeField(null=True)
 
     def as_subsonic_user(self):
         return {
             "username": self.name,
             "email": self.mail or "",
@@ -530,17 +535,19 @@
     created = DateTimeField(default=now)
     tracks = TextField(null=True)
 
     def as_subsonic_playlist(self, user):
         tracks = self.get_tracks()
         info = {
             "id": str(self.id),
-            "name": self.name
-            if self.user.id == user.id
-            else f"[{self.user.name}] {self.name}",
+            "name": (
+                self.name
+                if self.user.id == user.id
+                else f"[{self.user.name}] {self.name}"
+            ),
             "owner": self.user.name,
             "public": self.public,
             "songCount": len(tracks),
             "duration": sum(t.duration for t in tracks),
             "created": self.created.isoformat(),
         }
         if self.comment:
@@ -607,16 +614,44 @@
             "streamUrl": self.stream_url,
             "name": self.name,
             "homePageUrl": self.homepage_url,
         }
         return info
 
 
+if sys.version_info < (3, 9):
+    import pkg_resources
+
+    def get_resource_text(respath):
+        return pkg_resources.resource_string(__package__, respath).decode("utf-8")
+
+    def list_migrations(provider):
+        return pkg_resources.resource_listdir(
+            __package__, f"schema/migration/{provider}"
+        )
+
+else:
+    import importlib.resources
+
+    def get_resource_text(respath):
+        return (
+            importlib.resources.files(__package__).joinpath(respath).read_text("utf-8")
+        )
+
+    def list_migrations(provider):
+        return (
+            e.name
+            for e in importlib.resources.files(__package__)
+            .joinpath(f"schema/migration/{provider}")
+            .iterdir()
+        )
+
+
 def execute_sql_resource_script(respath):
-    sql = pkg_resources.resource_string(__package__, respath).decode("utf-8")
+    sql = get_resource_text(respath)
     for statement in sql.split(";"):
         statement = statement.strip()
         if statement and not statement.startswith("--"):
             db.execute_sql(statement)
 
 
 def init_database(database_uri):
@@ -646,17 +681,15 @@
             execute_sql_resource_script(f"schema/{provider}.sql")
             Meta.create(key="schema_version", value=SCHEMA_VERSION)
 
     # Check for schema changes
     version = Meta["schema_version"]
     if version.value < SCHEMA_VERSION:
         args.pop("pragmas", ())
-        migrations = sorted(
-            pkg_resources.resource_listdir(__package__, f"schema/migration/{provider}")
-        )
+        migrations = sorted(list_migrations(provider))
         for migration in migrations:
             if migration[0] in ("_", "."):
                 continue
 
             date, ext = os.path.splitext(migration)
             if date <= version.value:
                 continue
```

### Comparing `Supysonic-0.7.6/supysonic/frontend/__init__.py` & `supysonic-0.7.7/supysonic/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/frontend/folder.py` & `supysonic-0.7.7/supysonic/frontend/folder.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/frontend/playlist.py` & `supysonic-0.7.7/supysonic/frontend/playlist.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/frontend/user.py` & `supysonic-0.7.7/supysonic/frontend/user.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from flask import flash, redirect, render_template, request, session, url_for
 from flask import current_app
 from functools import wraps
 
 from ..db import ClientPrefs, User
 from ..lastfm import LastFm
+from ..listenbrainz import ListenBrainz
 from ..managers.user import UserManager
 
 from . import admin_only, frontend
 
 logger = logging.getLogger(__name__)
 
 
@@ -293,14 +294,38 @@
 def lastfm_unreg(uid, user):
     lfm = LastFm(current_app.config["LASTFM"], user)
     lfm.unlink_account()
     flash("Unlinked LastFM account")
     return redirect(url_for("frontend.user_profile", uid=uid))
 
 
+@frontend.route("/user/<uid>/listenbrainz/link")
+@me_or_uuid
+def listenbrainz_reg(uid, user):
+    token = request.args.get("token")
+    if not token:
+        flash("Missing ListenBrainz auth token")
+        return redirect(url_for("frontend.user_profile", uid=uid))
+
+    lbz = ListenBrainz(current_app.config["LISTENBRAINZ"], user)
+    status, error = lbz.link_account(token)
+    flash(error if not status else "Successfully linked ListenBrainz account")
+
+    return redirect(url_for("frontend.user_profile", uid=uid))
+
+
+@frontend.route("/user/<uid>/listenbrainz/unlink")
+@me_or_uuid
+def listenbrainz_unreg(uid, user):
+    lbz = ListenBrainz(current_app.config["LISTENBRAINZ"], user)
+    lbz.unlink_account()
+    flash("Unlinked ListenBrainz account")
+    return redirect(url_for("frontend.user_profile", uid=uid))
+
+
 @frontend.route("/user/login", methods=["GET", "POST"])
 def login():
     return_url = request.args.get("returnUrl") or url_for("frontend.index")
     if request.user:
         flash("Already logged in")
         return redirect(return_url)
```

### Comparing `Supysonic-0.7.6/supysonic/jukebox.py` & `supysonic-0.7.7/supysonic/jukebox.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/lastfm.py` & `supysonic-0.7.7/supysonic/lastfm.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/managers/folder.py` & `supysonic-0.7.7/supysonic/managers/folder.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/managers/user.py` & `supysonic-0.7.7/supysonic/managers/user.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/scanner.py` & `supysonic-0.7.7/supysonic/scanner.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/schema/migration/mysql/20171230.py` & `supysonic-0.7.7/supysonic/schema/migration/mysql/20171230.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/schema/migration/mysql/20180221.sql` & `supysonic-0.7.7/supysonic/schema/migration/mysql/20180221.sql`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/schema/migration/mysql/20190324.sql` & `supysonic-0.7.7/supysonic/schema/migration/mysql/20190324.sql`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/schema/migration/mysql/20190915.sql` & `supysonic-0.7.7/supysonic/schema/migration/mysql/20190915.sql`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/schema/migration/mysql/20230111.py` & `supysonic-0.7.7/supysonic/schema/migration/mysql/20230111.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/schema/migration/mysql/__pycache__/20230111.cpython-38.pyc` & `supysonic-0.7.7/supysonic/schema/migration/mysql/__pycache__/20230111.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/schema/migration/postgres/20180317.py` & `supysonic-0.7.7/supysonic/schema/migration/postgres/20180317.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/schema/migration/postgres/20190324.sql` & `supysonic-0.7.7/supysonic/schema/migration/postgres/20190324.sql`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/schema/migration/postgres/20190915.sql` & `supysonic-0.7.7/supysonic/schema/migration/postgres/20190915.sql`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/schema/migration/sqlite/20161030.sql` & `supysonic-0.7.7/supysonic/schema/migration/sqlite/20161030.sql`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/schema/migration/sqlite/20171022.sql` & `supysonic-0.7.7/supysonic/schema/migration/sqlite/20171022.sql`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/schema/migration/sqlite/20171230.py` & `supysonic-0.7.7/supysonic/schema/migration/sqlite/20171230.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/schema/migration/sqlite/20180311.sql` & `supysonic-0.7.7/supysonic/schema/migration/sqlite/20180311.sql`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/schema/migration/sqlite/20180317.py` & `supysonic-0.7.7/supysonic/schema/migration/sqlite/20180317.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/schema/migration/sqlite/20180521.sql` & `supysonic-0.7.7/supysonic/schema/migration/sqlite/20180521.sql`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/schema/migration/sqlite/20190324.sql` & `supysonic-0.7.7/supysonic/schema/migration/sqlite/20190324.sql`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/schema/migration/sqlite/20190518.sql` & `supysonic-0.7.7/supysonic/schema/migration/sqlite/20190518.sql`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/schema/migration/sqlite/20190915.sql` & `supysonic-0.7.7/supysonic/schema/migration/sqlite/20190915.sql`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/schema/migration/sqlite/20230111.py` & `supysonic-0.7.7/supysonic/schema/migration/sqlite/20230111.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/schema/migration/sqlite/__pycache__/20230111.cpython-38.pyc` & `supysonic-0.7.7/supysonic/schema/migration/sqlite/__pycache__/20230111.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/schema/mysql.sql` & `supysonic-0.7.7/supysonic/schema/mysql.sql`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,16 @@
     id CHAR(32) PRIMARY KEY,
     name VARCHAR(64) NOT NULL,
     mail VARCHAR(256),
     password CHAR(40) NOT NULL,
     salt CHAR(6) NOT NULL,
     admin BOOLEAN NOT NULL,
     jukebox BOOLEAN NOT NULL,
+    listenbrainz_session CHAR(36),
+    listenbrainz_status BOOLEAN NOT NULL,
     lastfm_session CHAR(32),
     lastfm_status BOOLEAN NOT NULL,
     last_play_id CHAR(32) REFERENCES track(id),
     last_play_date DATETIME
 ) DEFAULT CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
 CREATE INDEX index_user_last_play_id_fk ON user(last_play_id);
```

### Comparing `Supysonic-0.7.6/supysonic/schema/postgres.sql` & `supysonic-0.7.7/supysonic/schema/postgres.sql`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,16 @@
     id UUID PRIMARY KEY,
     name VARCHAR(64) NOT NULL,
     mail VARCHAR(256),
     password CHAR(40) NOT NULL,
     salt CHAR(6) NOT NULL,
     admin BOOLEAN NOT NULL,
     jukebox BOOLEAN NOT NULL,
+    listenbrainz_session CHAR(36),
+    listenbrainz_status BOOLEAN NOT NULL,
     lastfm_session CHAR(32),
     lastfm_status BOOLEAN NOT NULL,
     last_play_id UUID REFERENCES track,
     last_play_date TIMESTAMP
 );
 CREATE INDEX IF NOT EXISTS index_user_last_play_id_fk ON "user"(last_play_id);
```

### Comparing `Supysonic-0.7.6/supysonic/schema/sqlite.sql` & `supysonic-0.7.7/supysonic/schema/sqlite.sql`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,16 @@
     id CHAR(36) PRIMARY KEY,
     name VARCHAR(64) NOT NULL,
     mail VARCHAR(256),
     password CHAR(40) NOT NULL,
     salt CHAR(6) NOT NULL,
     admin BOOLEAN NOT NULL,
     jukebox BOOLEAN NOT NULL,
+    listenbrainz_session CHAR(36),
+    listenbrainz_status BOOLEAN NOT NULL,
     lastfm_session CHAR(32),
     lastfm_status BOOLEAN NOT NULL,
     last_play_id CHAR(36) REFERENCES track,
     last_play_date DATETIME
 );
 CREATE INDEX IF NOT EXISTS index_user_last_play_id_fk ON user(last_play_id);
```

### Comparing `Supysonic-0.7.6/supysonic/server/__init__.py` & `supysonic-0.7.7/supysonic/server/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,18 @@
 
 class MutuallyExclusiveOption(Option):
     def __init__(self, *args, **kwargs):
         self.mutually_exclusive = set(kwargs.pop("mutually_exclusive", []))
         help = kwargs.get("help", "")
         if self.mutually_exclusive:
             ex_str = ", ".join(self.mutually_exclusive)
-            kwargs[
-                "help"
-            ] = "{}  NOTE: This argument is mutually exclusive with arguments: [{}].".format(
-                help, ex_str
+            kwargs["help"] = (
+                "{}  NOTE: This argument is mutually exclusive with arguments: [{}].".format(
+                    help, ex_str
+                )
             )
         super().__init__(*args, **kwargs)
 
     def handle_parse_result(self, ctx, opts, args):
         if self.mutually_exclusive.intersection(opts) and self.name in opts:
             raise UsageError(
                 "Illegal usage: `{}` is mutually exclusive with arguments `{}`.".format(
```

### Comparing `Supysonic-0.7.6/supysonic/server/_base.py` & `supysonic-0.7.7/supysonic/server/_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,19 +17,17 @@
         self._host = host
         self._port = port
         self._socket = socket
         self._processes = processes
         self._threads = threads
 
     @abstractmethod
-    def _build_kwargs(self):
-        ...
+    def _build_kwargs(self): ...
 
     @abstractmethod
-    def _run(self, **kwargs):
-        ...
+    def _run(self, **kwargs): ...
 
     def _load_app(self):
         return create_application()
 
     def run(self):
         self._run(**self._build_kwargs())
```

### Comparing `Supysonic-0.7.6/supysonic/server/gevent.py` & `supysonic-0.7.7/supysonic/server/gevent.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/server/gunicorn.py` & `supysonic-0.7.7/supysonic/server/gunicorn.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/server/waitress.py` & `supysonic-0.7.7/supysonic/server/waitress.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/static/css/bootstrap-theme.min.css` & `supysonic-0.7.7/supysonic/static/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/static/css/bootstrap-theme.min.css.map` & `supysonic-0.7.7/supysonic/static/css/bootstrap-theme.min.css.map`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/static/css/bootstrap.min.css` & `supysonic-0.7.7/supysonic/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/static/css/bootstrap.min.css.map` & `supysonic-0.7.7/supysonic/static/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/static/css/supysonic.css` & `supysonic-0.7.7/supysonic/static/css/supysonic.css`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/static/fonts/glyphicons-halflings-regular.eot` & `supysonic-0.7.7/supysonic/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/static/fonts/glyphicons-halflings-regular.svg` & `supysonic-0.7.7/supysonic/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/static/fonts/glyphicons-halflings-regular.ttf` & `supysonic-0.7.7/supysonic/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/static/fonts/glyphicons-halflings-regular.woff` & `supysonic-0.7.7/supysonic/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/static/fonts/glyphicons-halflings-regular.woff2` & `supysonic-0.7.7/supysonic/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/static/js/bootstrap.min.js` & `supysonic-0.7.7/supysonic/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/templates/addfolder.html` & `supysonic-0.7.7/supysonic/templates/addfolder.html`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/templates/adduser.html` & `supysonic-0.7.7/supysonic/templates/adduser.html`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/templates/change_mail.html` & `supysonic-0.7.7/supysonic/templates/change_mail.html`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/templates/change_pass.html` & `supysonic-0.7.7/supysonic/templates/change_pass.html`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/templates/change_username.html` & `supysonic-0.7.7/supysonic/templates/change_username.html`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/templates/folders.html` & `supysonic-0.7.7/supysonic/templates/folders.html`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/templates/home.html` & `supysonic-0.7.7/supysonic/templates/home.html`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/templates/layout.html` & `supysonic-0.7.7/supysonic/templates/layout.html`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/templates/login.html` & `supysonic-0.7.7/supysonic/templates/login.html`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/templates/playlist.html` & `supysonic-0.7.7/supysonic/templates/playlist.html`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/templates/playlists.html` & `supysonic-0.7.7/supysonic/templates/playlists.html`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/templates/profile.html` & `supysonic-0.7.7/supysonic/templates/profile.html`

 * *Files 13% similar despite different names*

```diff
@@ -77,14 +77,44 @@
           {% else %}
           <input type="text" class="form-control" id="lastfm" placeholder="Unavailable" readonly>
           {% endif %}
         </div>
       </div>
     </form>
   </div>
+  <div class="col-md-6">
+    <form>
+      <div class="form_group">
+        <label class="sr-only" for="listenbrainz">ListenBrainz status</label>
+        <div class="input-group">
+          <div class="input-group-addon">ListenBrainz status</div>
+          {% if user.listenbrainz_session %}
+            <input class="form-control" type="text" id="listenbrainz" placeholder="{% if user.listenbrainz_status %}Linked{% else %}Invalid token{% endif %}" readonly>
+            <div class="input-group-btn">
+              {% if request.user.id == user.id %}
+              <a class="btn btn-default" href="{{ url_for('frontend.listenbrainz_unreg', uid = 'me') }}">Unlink</a>
+              {% else %}
+              <a class="btn btn-default" href="{{ url_for('frontend.listenbrainz_unreg', uid = user.id) }}">Unlink</a>
+              {% endif %}
+            </div>
+          {% else %}
+            <input class="form-control" type="text" name="token" id="listenbrainz" placeholder="Insert auth token" maxlength="36" />
+            <div class="input-group-btn">
+              {% if request.user.id == user.id %}
+              <button class="btn btn-default" type="submit" formaction="{{ url_for('frontend.listenbrainz_reg', uid = 'me') }}">Link</button>
+              {% else %}
+              <button class="btn btn-default" type="submit" formaction="{{ url_for('frontend.listenbrainz_reg', uid = user.id) }}">Link</button>
+              {% endif %}
+            </div>
+          {% endif %}
+        </div>
+      </div>
+    </form>
+    <br>
+  </div>
 </div>
 {% if request.user.id == user.id %}
 <a href="{{ url_for('frontend.change_password_form', uid = 'me') }}" class="btn btn-default">Change password</a></li>
 {% else %}
 <a href="{{ url_for('frontend.change_username_form', uid = user.id) }}" class="btn btn-default">Change username or admin status</a></li>
 <a href="{{ url_for('frontend.change_password_form', uid = user.id) }}" class="btn btn-default">Change password</a></li>
 {% endif %}
```

#### html2text {}

```diff
@@ -16,14 +16,22 @@
 LastFM status
 LastFM status
 {% if api_key != None %} {% if user.lastfm_session %}[                    ]
 {% if request.user.id == user.id %} _U_n_l_i_n_k {% else %} _U_n_l_i_n_k {% endif %}
 {% else %}[                    ]
 {% if request.user.id == user.id %} _L_i_n_k {% else %} _L_i_n_k {% endif %}
 {% endif %} {% else %} [                    ]{% endif %}
+ListenBrainz status
+ListenBrainz status
+{% if user.listenbrainz_session %}[                    ]
+{% if request.user.id == user.id %} _U_n_l_i_n_k {% else %} _U_n_l_i_n_k {% endif %}
+{% else %}[token               ]
+{% if request.user.id == user.id %} Link {% else %} Link {% endif %}
+{% endif %}
+
 {% if request.user.id == user.id %} _C_h_a_n_g_e_ _p_a_s_s_w_o_r_d
 {% else %} _C_h_a_n_g_e_ _u_s_e_r_n_a_m_e_ _o_r_ _a_d_m_i_n_ _s_t_a_t_u_s
 _C_h_a_n_g_e_ _p_a_s_s_w_o_r_d
 {% endif %} {% if clients.count() %}
 ********** CClliieennttss **********
 Here's a list of clients you used to stream music. If you want to use
 transcoding or downsampling with one of them (for instance using a low bitrate
```

### Comparing `Supysonic-0.7.6/supysonic/templates/users.html` & `supysonic-0.7.7/supysonic/templates/users.html`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/utils.py` & `supysonic-0.7.7/supysonic/utils.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/supysonic/watcher.py` & `supysonic-0.7.7/supysonic/watcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,18 @@
             raise e
 
     def __run(self):
         while self.__running:
             time.sleep(0.1)
 
             with self.__cond:
-                self.__cond.wait()
+                # Flag might have flipped during sleep. Check it again before waiting
+                # See issue #263
+                if self.__running:
+                    self.__cond.wait()
 
                 if not self.__queue:
                     continue
 
             logger.debug("Instantiating scanner")
             open_connection()
             scanner = Scanner()
@@ -191,16 +194,16 @@
 
         if item.operation & OP_MOVE:
             logger.info("Moving cover: '%s' -> '%s'", item.src_path, item.path)
             scanner.find_cover(os.path.dirname(item.src_path))
             scanner.add_cover(item.path)
 
     def stop(self):
-        self.__running = False
         with self.__cond:
+            self.__running = False
             self.__cond.notify()
 
     def put(self, path, operation, **kwargs):
         if not self.__running:
             raise RuntimeError("Trying to put an item in a stopped queue")
 
         with self.__cond:
```

### Comparing `Supysonic-0.7.6/supysonic/web.py` & `supysonic-0.7.7/supysonic/web.py`

 * *Files identical despite different names*

### Comparing `Supysonic-0.7.6/tests/testbase.py` & `supysonic-0.7.7/tests/testbase.py`

 * *Files identical despite different names*

