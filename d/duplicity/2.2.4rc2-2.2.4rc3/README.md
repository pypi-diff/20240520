# Comparing `tmp/duplicity-2.2.4rc2.tar.gz` & `tmp/duplicity-2.2.4rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duplicity-2.2.4rc2.tar", last modified: Sat May 18 17:01:06 2024, max compression
+gzip compressed data, was "duplicity-2.2.4rc3.tar", last modified: Sun May 19 17:40:58 2024, max compression
```

## Comparing `duplicity-2.2.4rc2.tar` & `duplicity-2.2.4rc3.tar`

### file list

```diff
@@ -1,398 +1,398 @@
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.828805 duplicity-2.2.4rc2/
--rw-r--r--   0 ken       (1000) ken       (1000)    10366 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/.gitchangelog.rc
--rw-r--r--   0 ken       (1000) ken       (1000)      529 2024-03-19 15:05:23.000000 duplicity-2.2.4rc2/.gitignore
--rw-r--r--   0 ken       (1000) ken       (1000)     6266 2024-05-18 16:48:38.000000 duplicity-2.2.4rc2/.gitlab-ci.yml
--rw-r--r--   0 ken       (1000) ken       (1000)     1390 2024-01-29 17:23:01.000000 duplicity-2.2.4rc2/AUTHORS.md
--rw-r--r--   0 ken       (1000) ken       (1000)   592972 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/CHANGELOG.md
--rw-r--r--   0 ken       (1000) ken       (1000)    18028 2022-12-27 19:32:15.000000 duplicity-2.2.4rc2/COPYING
--rw-r--r--   0 ken       (1000) ken       (1000)     1124 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/Makefile
--rw-r--r--   0 ken       (1000) ken       (1000)      918 2024-05-18 17:01:06.828805 duplicity-2.2.4rc2/PKG-INFO
--rw-r--r--   0 ken       (1000) ken       (1000)     1284 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/README-LOG.md
--rw-r--r--   0 ken       (1000) ken       (1000)      618 2024-04-30 19:30:15.000000 duplicity-2.2.4rc2/README-REPO.md
--rw-r--r--   0 ken       (1000) ken       (1000)     3250 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/README-SNAP.md
--rw-r--r--   0 ken       (1000) ken       (1000)     5364 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/README-TESTING.md
--rw-r--r--   0 ken       (1000) ken       (1000)     3484 2024-05-16 20:53:05.000000 duplicity-2.2.4rc2/README.md
--rw-r--r--   0 ken       (1000) ken       (1000)      164 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/crowdin.yml
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.792723 duplicity-2.2.4rc2/debian/
--rw-r--r--   0 ken       (1000) ken       (1000)      189 2022-12-27 19:32:15.000000 duplicity-2.2.4rc2/debian/changelog
--rw-r--r--   0 ken       (1000) ken       (1000)        3 2024-02-02 16:10:07.000000 duplicity-2.2.4rc2/debian/compat
--rw-r--r--   0 ken       (1000) ken       (1000)     1510 2024-05-02 15:20:27.000000 duplicity-2.2.4rc2/debian/control
--rw-r--r--   0 ken       (1000) ken       (1000)     1546 2024-01-29 17:35:45.000000 duplicity-2.2.4rc2/debian/copyright
--rw-r--r--   0 ken       (1000) ken       (1000)      223 2024-02-02 16:10:07.000000 duplicity-2.2.4rc2/debian/duplicity.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      629 2024-02-02 16:10:07.000000 duplicity-2.2.4rc2/debian/rules
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.792723 duplicity-2.2.4rc2/debian/source/
--rw-r--r--   0 ken       (1000) ken       (1000)       13 2022-12-27 19:32:15.000000 duplicity-2.2.4rc2/debian/source/format
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.792723 duplicity-2.2.4rc2/docs/
--rw-r--r--   0 ken       (1000) ken       (1000)      787 2024-05-14 14:50:00.000000 duplicity-2.2.4rc2/docs/Makefile
--rw-r--r--   0 ken       (1000) ken       (1000)      372 2024-03-25 15:18:48.000000 duplicity-2.2.4rc2/docs/README.md
--rw-r--r--   0 ken       (1000) ken       (1000)     3436 2024-03-25 15:20:00.000000 duplicity-2.2.4rc2/docs/conf.py
--rw-r--r--   0 ken       (1000) ken       (1000)      915 2023-03-19 16:45:14.000000 duplicity-2.2.4rc2/docs/index.rst
--rw-r--r--   0 ken       (1000) ken       (1000)       75 2023-03-19 16:45:14.000000 duplicity-2.2.4rc2/docs/modules.rst
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.796732 duplicity-2.2.4rc2/duplicity/
--rw-r--r--   0 ken       (1000) ken       (1000)     1034 2024-05-18 16:27:33.000000 duplicity-2.2.4rc2/duplicity/__init__.py
--rwxr-xr-x   0 ken       (1000) ken       (1000)     3896 2024-01-29 17:23:01.000000 duplicity-2.2.4rc2/duplicity/__main__.py
--rw-r--r--   0 ken       (1000) ken       (1000)    14510 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/_librsyncmodule.c
--rw-r--r--   0 ken       (1000) ken       (1000)    96777 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/argparse311.py
--rw-r--r--   0 ken       (1000) ken       (1000)    10243 2024-05-03 17:58:22.000000 duplicity-2.2.4rc2/duplicity/asyncscheduler.py
--rw-r--r--   0 ken       (1000) ken       (1000)    28309 2024-05-14 14:50:00.000000 duplicity-2.2.4rc2/duplicity/backend.py
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.804751 duplicity-2.2.4rc2/duplicity/backends/
--rw-r--r--   0 ken       (1000) ken       (1000)     3158 2024-03-19 15:05:23.000000 duplicity-2.2.4rc2/duplicity/backends/README
--rw-r--r--   0 ken       (1000) ken       (1000)     1115 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/__init__.py
--rw-r--r--   0 ken       (1000) ken       (1000)     3920 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/_cf_cloudfiles.py
--rw-r--r--   0 ken       (1000) ken       (1000)     5138 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/_cf_pyrax.py
--rw-r--r--   0 ken       (1000) ken       (1000)     9388 2024-05-14 14:50:00.000000 duplicity-2.2.4rc2/duplicity/backends/_testbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    16562 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/adbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     5536 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/azurebackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     9214 2024-03-19 15:05:23.000000 duplicity-2.2.4rc2/duplicity/backends/b2backend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     6784 2024-01-29 16:41:36.000000 duplicity-2.2.4rc2/duplicity/backends/boxbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     1142 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/cfbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    19552 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/dpbxbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     9115 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/gdocsbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    16667 2024-02-03 16:19:07.000000 duplicity-2.2.4rc2/duplicity/backends/gdrivebackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     7889 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/giobackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2604 2024-01-29 17:23:01.000000 duplicity-2.2.4rc2/duplicity/backends/hsibackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2426 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/hubicbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    19313 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/idrivedbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     9761 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/imapbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     5753 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/jottacloudbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     9183 2024-01-29 17:23:01.000000 duplicity-2.2.4rc2/duplicity/backends/lftpbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     3040 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/localbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     4634 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/mediafirebackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     7097 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/megabackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     8623 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/megav2backend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     9862 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/megav3backend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    15763 2023-12-04 21:05:42.000000 duplicity-2.2.4rc2/duplicity/backends/multibackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     5450 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/ncftpbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    16318 2024-05-18 14:59:19.000000 duplicity-2.2.4rc2/duplicity/backends/onedrivebackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     8989 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/par2backend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    12471 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/pcabackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    13026 2024-01-29 16:41:36.000000 duplicity-2.2.4rc2/duplicity/backends/pydrivebackend.py
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.804751 duplicity-2.2.4rc2/duplicity/backends/pyrax_identity/
--rw-r--r--   0 ken       (1000) ken       (1000)      903 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/pyrax_identity/__init__.py
--rw-r--r--   0 ken       (1000) ken       (1000)     9745 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/pyrax_identity/hubic.py
--rw-r--r--   0 ken       (1000) ken       (1000)     4284 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/rclonebackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     6455 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/rsyncbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    10498 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/s3_boto3_backend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     6520 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/slatebackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    19675 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/ssh_paramiko_backend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    12942 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/ssh_pexpect_backend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    10143 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/swiftbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2317 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/sxbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2564 2024-01-29 17:23:01.000000 duplicity-2.2.4rc2/duplicity/backends/tahoebackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    18682 2024-05-14 14:50:00.000000 duplicity-2.2.4rc2/duplicity/backends/webdavbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    12248 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/backends/xorrisobackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     1668 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/cached_ops.py
--rw-r--r--   0 ken       (1000) ken       (1000)    34088 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/duplicity/cli_data.py
--rw-r--r--   0 ken       (1000) ken       (1000)    11716 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/duplicity/cli_main.py
--rw-r--r--   0 ken       (1000) ken       (1000)    14078 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/duplicity/cli_util.py
--rw-r--r--   0 ken       (1000) ken       (1000)    11185 2024-05-03 17:58:22.000000 duplicity-2.2.4rc2/duplicity/config.py
--rw-r--r--   0 ken       (1000) ken       (1000)    25936 2024-01-29 17:23:01.000000 duplicity-2.2.4rc2/duplicity/diffdir.py
--rw-r--r--   0 ken       (1000) ken       (1000)    49699 2024-05-03 17:58:22.000000 duplicity-2.2.4rc2/duplicity/dup_collections.py
--rw-r--r--   0 ken       (1000) ken       (1000)    62946 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/duplicity/dup_main.py
--rw-r--r--   0 ken       (1000) ken       (1000)     1262 2024-01-29 17:23:01.000000 duplicity-2.2.4rc2/duplicity/dup_tarfile.py
--rw-r--r--   0 ken       (1000) ken       (1000)     8369 2023-12-12 19:20:24.000000 duplicity-2.2.4rc2/duplicity/dup_temp.py
--rw-r--r--   0 ken       (1000) ken       (1000)     7198 2024-05-03 17:58:22.000000 duplicity-2.2.4rc2/duplicity/dup_threading.py
--rw-r--r--   0 ken       (1000) ken       (1000)    10380 2024-01-29 17:23:01.000000 duplicity-2.2.4rc2/duplicity/dup_time.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2723 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/errors.py
--rw-r--r--   0 ken       (1000) ken       (1000)    16727 2024-01-20 17:46:53.000000 duplicity-2.2.4rc2/duplicity/file_naming.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2625 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/filechunkio.py
--rw-r--r--   0 ken       (1000) ken       (1000)     7537 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/globmatch.py
--rw-r--r--   0 ken       (1000) ken       (1000)    17768 2024-05-14 14:50:00.000000 duplicity-2.2.4rc2/duplicity/gpg.py
--rw-r--r--   0 ken       (1000) ken       (1000)    22946 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/gpginterface.py
--rw-r--r--   0 ken       (1000) ken       (1000)    14947 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/lazy.py
--rw-r--r--   0 ken       (1000) ken       (1000)     8502 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/librsync.py
--rw-r--r--   0 ken       (1000) ken       (1000)    15983 2024-05-03 17:58:22.000000 duplicity-2.2.4rc2/duplicity/log.py
--rw-r--r--   0 ken       (1000) ken       (1000)    17964 2024-01-29 17:23:01.000000 duplicity-2.2.4rc2/duplicity/manifest.py
--rw-r--r--   0 ken       (1000) ken       (1000)    21774 2024-01-29 17:23:01.000000 duplicity-2.2.4rc2/duplicity/patchdir.py
--rw-r--r--   0 ken       (1000) ken       (1000)    28589 2024-03-19 15:05:23.000000 duplicity-2.2.4rc2/duplicity/path.py
--rw-r--r--   0 ken       (1000) ken       (1000)    13824 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/progress.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2730 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/duplicity/robust.py
--rw-r--r--   0 ken       (1000) ken       (1000)    29428 2024-01-29 16:41:36.000000 duplicity-2.2.4rc2/duplicity/selection.py
--rw-r--r--   0 ken       (1000) ken       (1000)    15619 2023-12-20 17:08:29.000000 duplicity-2.2.4rc2/duplicity/statistics.py
--rw-r--r--   0 ken       (1000) ken       (1000)    10716 2024-01-29 17:23:01.000000 duplicity-2.2.4rc2/duplicity/tempdir.py
--rw-r--r--   0 ken       (1000) ken       (1000)    11030 2024-01-29 17:23:01.000000 duplicity-2.2.4rc2/duplicity/util.py
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.828805 duplicity-2.2.4rc2/duplicity.egg-info/
--rw-r--r--   0 ken       (1000) ken       (1000)      918 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/duplicity.egg-info/PKG-INFO
--rw-r--r--   0 ken       (1000) ken       (1000)     7811 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/duplicity.egg-info/SOURCES.txt
--rw-r--r--   0 ken       (1000) ken       (1000)        1 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/duplicity.egg-info/dependency_links.txt
--rw-r--r--   0 ken       (1000) ken       (1000)       57 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/duplicity.egg-info/entry_points.txt
--rw-r--r--   0 ken       (1000) ken       (1000)      365 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/duplicity.egg-info/requires.txt
--rw-r--r--   0 ken       (1000) ken       (1000)       10 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/duplicity.egg-info/top_level.txt
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.804751 duplicity-2.2.4rc2/man/
--rw-r--r--   0 ken       (1000) ken       (1000)    94191 2024-05-18 16:27:33.000000 duplicity-2.2.4rc2/man/duplicity.1
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.812769 duplicity-2.2.4rc2/po/
--rw-r--r--   0 ken       (1000) ken       (1000)      276 2024-05-14 15:33:39.000000 duplicity-2.2.4rc2/po/LINGUAS
--rw-r--r--   0 ken       (1000) ken       (1000)     1174 2022-12-27 19:32:15.000000 duplicity-2.2.4rc2/po/Makevars
--rw-r--r--   0 ken       (1000) ken       (1000)     2315 2024-05-14 15:33:39.000000 duplicity-2.2.4rc2/po/POTFILES.in
--rw-r--r--   0 ken       (1000) ken       (1000)     1074 2024-05-14 15:33:39.000000 duplicity-2.2.4rc2/po/POTFILES.skip
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.812769 duplicity-2.2.4rc2/po/af_ZA/
--rw-rw-r--   0 ken       (1000) ken       (1000)      516 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/af_ZA/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    45456 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/af_ZA.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.812769 duplicity-2.2.4rc2/po/ar_SA/
--rw-rw-r--   0 ken       (1000) ken       (1000)    47467 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/ar_SA/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    69886 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/ar_SA.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.812769 duplicity-2.2.4rc2/po/ca_ES/
--rw-rw-r--   0 ken       (1000) ken       (1000)      514 2024-05-18 17:01:05.000000 duplicity-2.2.4rc2/po/ca_ES/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    45454 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/ca_ES.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.812769 duplicity-2.2.4rc2/po/cs_CZ/
--rw-rw-r--   0 ken       (1000) ken       (1000)    42586 2024-05-18 17:01:05.000000 duplicity-2.2.4rc2/po/cs_CZ/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    64046 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/cs_CZ.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.812769 duplicity-2.2.4rc2/po/da_DK/
--rw-rw-r--   0 ken       (1000) ken       (1000)    40754 2024-05-18 17:01:05.000000 duplicity-2.2.4rc2/po/da_DK/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    62115 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/da_DK.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.812769 duplicity-2.2.4rc2/po/de_AT/
--rw-rw-r--   0 ken       (1000) ken       (1000)    43792 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/de_AT/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    65263 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/de_AT.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.812769 duplicity-2.2.4rc2/po/de_DE/
--rw-rw-r--   0 ken       (1000) ken       (1000)    43780 2024-05-18 17:01:05.000000 duplicity-2.2.4rc2/po/de_DE/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    65251 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/de_DE.po
--rw-r--r--   0 ken       (1000) ken       (1000)    45784 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/duplicity.pot
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.812769 duplicity-2.2.4rc2/po/el_GR/
--rw-rw-r--   0 ken       (1000) ken       (1000)    52055 2024-05-18 17:01:05.000000 duplicity-2.2.4rc2/po/el_GR/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    75344 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/el_GR.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.812769 duplicity-2.2.4rc2/po/en_AU/
--rw-rw-r--   0 ken       (1000) ken       (1000)      944 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/en_AU/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    45632 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/en_AU.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.812769 duplicity-2.2.4rc2/po/en_GB/
--rw-rw-r--   0 ken       (1000) ken       (1000)     2745 2024-05-18 17:01:05.000000 duplicity-2.2.4rc2/po/en_GB/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    46469 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/en_GB.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.812769 duplicity-2.2.4rc2/po/en_PR/
--rw-rw-r--   0 ken       (1000) ken       (1000)      530 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/en_PR/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    45470 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/en_PR.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.812769 duplicity-2.2.4rc2/po/en_US/
--rw-rw-r--   0 ken       (1000) ken       (1000)      532 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/en_US/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    45472 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/en_US.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.812769 duplicity-2.2.4rc2/po/es_EM/
--rw-rw-r--   0 ken       (1000) ken       (1000)    42408 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/es_EM/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    64161 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/es_EM.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.812769 duplicity-2.2.4rc2/po/es_ES/
--rw-rw-r--   0 ken       (1000) ken       (1000)    42399 2024-05-18 17:01:05.000000 duplicity-2.2.4rc2/po/es_ES/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    64152 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/es_ES.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.812769 duplicity-2.2.4rc2/po/es_MX/
--rw-rw-r--   0 ken       (1000) ken       (1000)    42407 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/es_MX/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    64160 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/es_MX.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.812769 duplicity-2.2.4rc2/po/es_PR/
--rw-rw-r--   0 ken       (1000) ken       (1000)    42412 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/es_PR/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    64165 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/es_PR.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.812769 duplicity-2.2.4rc2/po/es_US/
--rw-rw-r--   0 ken       (1000) ken       (1000)    42414 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/es_US/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    64167 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/es_US.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.812769 duplicity-2.2.4rc2/po/fi_FI/
--rw-rw-r--   0 ken       (1000) ken       (1000)    40182 2024-05-18 17:01:05.000000 duplicity-2.2.4rc2/po/fi_FI/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    62727 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/fi_FI.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.812769 duplicity-2.2.4rc2/po/fr_FR/
--rw-rw-r--   0 ken       (1000) ken       (1000)    42577 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/fr_FR/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    64995 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/fr_FR.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.812769 duplicity-2.2.4rc2/po/he_IL/
--rw-rw-r--   0 ken       (1000) ken       (1000)      964 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/he_IL/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    45741 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/he_IL.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.812769 duplicity-2.2.4rc2/po/hu_HU/
--rw-rw-r--   0 ken       (1000) ken       (1000)    20731 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/hu_HU/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    54662 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/hu_HU.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.816778 duplicity-2.2.4rc2/po/it_IT/
--rw-rw-r--   0 ken       (1000) ken       (1000)    42374 2024-05-18 17:01:05.000000 duplicity-2.2.4rc2/po/it_IT/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    64000 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/it_IT.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.816778 duplicity-2.2.4rc2/po/ja_JP/
--rw-rw-r--   0 ken       (1000) ken       (1000)    43260 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/ja_JP/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    66545 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/ja_JP.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.816778 duplicity-2.2.4rc2/po/ko_KR/
--rw-rw-r--   0 ken       (1000) ken       (1000)     5451 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/ko_KR/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    47463 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/ko_KR.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.816778 duplicity-2.2.4rc2/po/nl_BE/
--rw-rw-r--   0 ken       (1000) ken       (1000)    41940 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/nl_BE/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    63301 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/nl_BE.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.816778 duplicity-2.2.4rc2/po/nl_NL/
--rw-rw-r--   0 ken       (1000) ken       (1000)    41928 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/nl_NL/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    63289 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/nl_NL.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.816778 duplicity-2.2.4rc2/po/nl_SR/
--rw-rw-r--   0 ken       (1000) ken       (1000)    41941 2024-05-18 17:01:05.000000 duplicity-2.2.4rc2/po/nl_SR/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    63302 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/nl_SR.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.816778 duplicity-2.2.4rc2/po/no_NO/
--rw-rw-r--   0 ken       (1000) ken       (1000)    38960 2024-05-18 17:01:05.000000 duplicity-2.2.4rc2/po/no_NO/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    61387 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/no_NO.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.816778 duplicity-2.2.4rc2/po/pl_PL/
--rw-rw-r--   0 ken       (1000) ken       (1000)    42510 2024-05-18 17:01:05.000000 duplicity-2.2.4rc2/po/pl_PL/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    64376 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/pl_PL.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.816778 duplicity-2.2.4rc2/po/pt_BR/
--rw-rw-r--   0 ken       (1000) ken       (1000)    42538 2024-05-18 17:01:05.000000 duplicity-2.2.4rc2/po/pt_BR/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    64283 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/pt_BR.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.816778 duplicity-2.2.4rc2/po/pt_PT/
--rw-rw-r--   0 ken       (1000) ken       (1000)    41404 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/pt_PT/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    63328 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/pt_PT.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.816778 duplicity-2.2.4rc2/po/ro_RO/
--rw-rw-r--   0 ken       (1000) ken       (1000)    42217 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/ro_RO/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    63905 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/ro_RO.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.816778 duplicity-2.2.4rc2/po/ru_BY/
--rw-rw-r--   0 ken       (1000) ken       (1000)    54999 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/ru_BY/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    76691 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/ru_BY.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.816778 duplicity-2.2.4rc2/po/ru_MD/
--rw-rw-r--   0 ken       (1000) ken       (1000)    54999 2024-05-18 17:01:05.000000 duplicity-2.2.4rc2/po/ru_MD/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    76691 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/ru_MD.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.816778 duplicity-2.2.4rc2/po/ru_RU/
--rw-rw-r--   0 ken       (1000) ken       (1000)    54987 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/ru_RU/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    76679 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/ru_RU.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.816778 duplicity-2.2.4rc2/po/ru_UA/
--rw-rw-r--   0 ken       (1000) ken       (1000)    55001 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/ru_UA/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    76693 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/ru_UA.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.816778 duplicity-2.2.4rc2/po/sr_SP/
--rw-rw-r--   0 ken       (1000) ken       (1000)      599 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/sr_SP/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    45565 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/sr_SP.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.816778 duplicity-2.2.4rc2/po/sv_SE/
--rw-rw-r--   0 ken       (1000) ken       (1000)    42037 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/sv_SE/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    63416 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/sv_SE.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.816778 duplicity-2.2.4rc2/po/tr_TR/
--rw-rw-r--   0 ken       (1000) ken       (1000)     3629 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/tr_TR/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    46575 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/tr_TR.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.816778 duplicity-2.2.4rc2/po/uk_UA/
--rw-rw-r--   0 ken       (1000) ken       (1000)    47951 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/uk_UA/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    72573 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/uk_UA.po
--rwxr-xr-x   0 ken       (1000) ken       (1000)     1140 2024-02-03 16:20:49.000000 duplicity-2.2.4rc2/po/update-pot
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.816778 duplicity-2.2.4rc2/po/vi_VN/
--rw-rw-r--   0 ken       (1000) ken       (1000)      510 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/vi_VN/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    45424 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/vi_VN.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.816778 duplicity-2.2.4rc2/po/zh_CN/
--rw-rw-r--   0 ken       (1000) ken       (1000)    35542 2024-05-18 17:01:05.000000 duplicity-2.2.4rc2/po/zh_CN/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    58854 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/zh_CN.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.816778 duplicity-2.2.4rc2/po/zh_HK/
--rw-rw-r--   0 ken       (1000) ken       (1000)      533 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/zh_HK/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    45447 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/zh_HK.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.816778 duplicity-2.2.4rc2/po/zh_MO/
--rw-rw-r--   0 ken       (1000) ken       (1000)      529 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/zh_MO/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    45443 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/zh_MO.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.816778 duplicity-2.2.4rc2/po/zh_SG/
--rw-rw-r--   0 ken       (1000) ken       (1000)      533 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/zh_SG/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    45447 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/zh_SG.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.816778 duplicity-2.2.4rc2/po/zh_TW/
--rw-rw-r--   0 ken       (1000) ken       (1000)      522 2024-05-18 17:01:06.000000 duplicity-2.2.4rc2/po/zh_TW/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    45436 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/po/zh_TW.po
--rw-r--r--   0 ken       (1000) ken       (1000)     2689 2024-05-18 16:27:33.000000 duplicity-2.2.4rc2/pyproject.toml
--rw-r--r--   0 ken       (1000) ken       (1000)      497 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/readthedocs.yaml
--rw-r--r--   0 ken       (1000) ken       (1000)      479 2024-05-18 15:49:51.000000 duplicity-2.2.4rc2/requirements.txt
--rw-r--r--   0 ken       (1000) ken       (1000)      695 2024-05-18 17:01:06.828805 duplicity-2.2.4rc2/setup.cfg
--rwxr-xr-x   0 ken       (1000) ken       (1000)     9840 2024-05-18 16:59:04.000000 duplicity-2.2.4rc2/setup.py
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.816778 duplicity-2.2.4rc2/snap/
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.816778 duplicity-2.2.4rc2/snap/local/
--rwxr-xr-x   0 ken       (1000) ken       (1000)      186 2022-12-27 19:32:15.000000 duplicity-2.2.4rc2/snap/local/debug.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      110 2022-12-27 19:32:15.000000 duplicity-2.2.4rc2/snap/local/launcher.sh
--rw-r--r--   0 ken       (1000) ken       (1000)     4684 2024-05-18 16:27:33.000000 duplicity-2.2.4rc2/snap/snapcraft.yaml
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.820787 duplicity-2.2.4rc2/testing/
--rw-r--r--   0 ken       (1000) ken       (1000)     4611 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/testing/__init__.py
--rw-r--r--   0 ken       (1000) ken       (1000)      941 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/conftest.py
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.820787 duplicity-2.2.4rc2/testing/docker/
--rw-r--r--   0 ken       (1000) ken       (1000)     1151 2022-12-27 19:32:15.000000 duplicity-2.2.4rc2/testing/docker/.env
--rw-r--r--   0 ken       (1000) ken       (1000)       37 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/docker/.gitignore
--rwxr-xr-x   0 ken       (1000) ken       (1000)     1272 2024-05-16 14:18:05.000000 duplicity-2.2.4rc2/testing/docker/build.sh
--rw-r--r--   0 ken       (1000) ken       (1000)     2361 2022-12-27 19:32:15.000000 duplicity-2.2.4rc2/testing/docker/docker-compose.yml
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.820787 duplicity-2.2.4rc2/testing/docker/duplicity_test/
--rw-r--r--   0 ken       (1000) ken       (1000)     3618 2024-05-16 14:18:05.000000 duplicity-2.2.4rc2/testing/docker/duplicity_test/Dockerfile
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.820787 duplicity-2.2.4rc2/testing/docker/ftp_server/
--rw-r--r--   0 ken       (1000) ken       (1000)     1234 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/docker/ftp_server/Dockerfile
--rw-r--r--   0 ken       (1000) ken       (1000)       94 2022-12-27 19:32:15.000000 duplicity-2.2.4rc2/testing/docker/ftp_server/pureftpd.passwd
--rw-r--r--   0 ken       (1000) ken       (1000)     4199 2022-12-27 19:32:15.000000 duplicity-2.2.4rc2/testing/docker/hello-world-master.zip
--rw-r--r--   0 ken       (1000) ken       (1000)     1675 2022-12-27 19:32:15.000000 duplicity-2.2.4rc2/testing/docker/id_rsa
--rw-r--r--   0 ken       (1000) ken       (1000)      406 2022-12-27 19:32:15.000000 duplicity-2.2.4rc2/testing/docker/id_rsa.pub
--rwxr-xr-x   0 ken       (1000) ken       (1000)     1320 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/docker/push.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)     1151 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/docker/setup.sh
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.820787 duplicity-2.2.4rc2/testing/docker/ssh_server/
--rw-r--r--   0 ken       (1000) ken       (1000)     2352 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/docker/ssh_server/Dockerfile
--rwxr-xr-x   0 ken       (1000) ken       (1000)     1105 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/docker/teardown.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)     1188 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/docker/testit.sh
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.820787 duplicity-2.2.4rc2/testing/functional/
--rw-r--r--   0 ken       (1000) ken       (1000)    10498 2024-05-03 17:58:22.000000 duplicity-2.2.4rc2/testing/functional/__init__.py
--rw-r--r--   0 ken       (1000) ken       (1000)     3303 2024-05-03 17:58:22.000000 duplicity-2.2.4rc2/testing/functional/test_badupload.py
--rw-r--r--   0 ken       (1000) ken       (1000)     3825 2024-05-03 17:58:22.000000 duplicity-2.2.4rc2/testing/functional/test_cleanup.py
--rw-r--r--   0 ken       (1000) ken       (1000)    11215 2024-01-29 17:23:01.000000 duplicity-2.2.4rc2/testing/functional/test_final.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2401 2024-03-19 15:05:23.000000 duplicity-2.2.4rc2/testing/functional/test_log.py
--rw-r--r--   0 ken       (1000) ken       (1000)    18836 2024-05-03 17:58:22.000000 duplicity-2.2.4rc2/testing/functional/test_restart.py
--rw-r--r--   0 ken       (1000) ken       (1000)    99174 2024-01-29 17:23:01.000000 duplicity-2.2.4rc2/testing/functional/test_selection.py
--rw-r--r--   0 ken       (1000) ken       (1000)     8664 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/functional/test_verify.py
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.820787 duplicity-2.2.4rc2/testing/gnupg/
--rw-r--r--   0 ken       (1000) ken       (1000)      255 2022-12-27 19:32:15.000000 duplicity-2.2.4rc2/testing/gnupg/README
--rw-r--r--   0 ken       (1000) ken       (1000)      145 2022-12-27 19:32:15.000000 duplicity-2.2.4rc2/testing/gnupg/gpg-agent.conf
--rw-r--r--   0 ken       (1000) ken       (1000)      425 2022-12-27 19:32:15.000000 duplicity-2.2.4rc2/testing/gnupg/gpg.conf
--rw-r--r--   0 ken       (1000) ken       (1000)     3567 2022-12-27 19:32:15.000000 duplicity-2.2.4rc2/testing/gnupg/pubring.gpg
--rw-r--r--   0 ken       (1000) ken       (1000)     7549 2022-12-27 19:32:15.000000 duplicity-2.2.4rc2/testing/gnupg/secring.gpg
--rw-r--r--   0 ken       (1000) ken       (1000)     1440 2022-12-27 19:32:15.000000 duplicity-2.2.4rc2/testing/gnupg/trustdb.gpg
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.824796 duplicity-2.2.4rc2/testing/manual/
--rw-r--r--   0 ken       (1000) ken       (1000)      903 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/manual/__init__.py
--rwxr-xr-x   0 ken       (1000) ken       (1000)     1411 2022-12-27 19:32:15.000000 duplicity-2.2.4rc2/testing/manual/auto-ctrl-c-test.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)     8583 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/manual/backendtest.py
--rwxr-xr-x   0 ken       (1000) ken       (1000)     1834 2022-12-27 19:32:15.000000 duplicity-2.2.4rc2/testing/manual/manual-ctrl-c-test.sh
--rw-r--r--   0 ken       (1000) ken       (1000)      738 2022-12-27 19:32:15.000000 duplicity-2.2.4rc2/testing/manual/rootfiles.tar.gz
--rwxr-xr-x   0 ken       (1000) ken       (1000)     4765 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/manual/roottest.py
--rwxr-xr-x   0 ken       (1000) ken       (1000)     1727 2022-12-27 19:32:15.000000 duplicity-2.2.4rc2/testing/manual/run-coverage.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      446 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/testing/manual/test-prefix-install.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      542 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/testing/manual/test-venv-install.sh
--rw-r--r--   0 ken       (1000) ken       (1000)     1612 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/manual/test_config.py.tmpl
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.824796 duplicity-2.2.4rc2/testing/overrides/
--rw-r--r--   0 ken       (1000) ken       (1000)       75 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/overrides/__init__.py
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.824796 duplicity-2.2.4rc2/testing/overrides/bin/
--rwxr-xr-x   0 ken       (1000) ken       (1000)      423 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/overrides/bin/hsi
--rwxr-xr-x   0 ken       (1000) ken       (1000)      512 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/overrides/bin/lftp
--rwxr-xr-x   0 ken       (1000) ken       (1000)      155 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/overrides/bin/ncftpget
--rwxr-xr-x   0 ken       (1000) ken       (1000)      558 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/overrides/bin/ncftpls
--rwxr-xr-x   0 ken       (1000) ken       (1000)      155 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/overrides/bin/ncftpput
--rwxr-xr-x   0 ken       (1000) ken       (1000)      416 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/overrides/bin/tahoe
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.824796 duplicity-2.2.4rc2/testing/regression/
--rwxr-xr-x   0 ken       (1000) ken       (1000)      503 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/regression/bug1526557.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      192 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/regression/bug1846678.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      680 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/regression/bug1860200.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      905 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/regression/bug487720.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      457 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/regression/bug930151.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      417 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/regression/issue100.sh
--rw-r--r--   0 ken       (1000) ken       (1000)      295 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/regression/issue103.json
--rwxr-xr-x   0 ken       (1000) ken       (1000)     1621 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/regression/issue103.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      554 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/regression/issue110-setup.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      278 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/regression/issue110-test.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)     1312 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/regression/issue125.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      280 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/regression/issue147.sh
--rw-r--r--   0 ken       (1000) ken       (1000)      189 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/regression/issue25.json
--rwxr-xr-x   0 ken       (1000) ken       (1000)      685 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/regression/issue25.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      466 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/regression/issue26.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      464 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/regression/issue683.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      794 2024-03-19 15:05:23.000000 duplicity-2.2.4rc2/testing/regression/issue725.sh
--rw-r--r--   0 ken       (1000) ken       (1000)      144 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/regression/issue73.env
--rwxr-xr-x   0 ken       (1000) ken       (1000)      418 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/regression/issue73.sh
--rw-r--r--   0 ken       (1000) ken       (1000)      189 2023-12-04 21:05:42.000000 duplicity-2.2.4rc2/testing/regression/issue781.json
--rwxr-xr-x   0 ken       (1000) ken       (1000)      630 2023-12-04 21:05:42.000000 duplicity-2.2.4rc2/testing/regression/issue781.sh
--rw-r--r--   0 ken       (1000) ken       (1000)      189 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/regression/issue79.json
--rwxr-xr-x   0 ken       (1000) ken       (1000)     1087 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/regression/issue79.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)     1001 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/regression/issue98.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      878 2022-12-27 19:32:15.000000 duplicity-2.2.4rc2/testing/run-tests
--rw-r--r--   0 ken       (1000) ken       (1000)     3287 2024-05-14 14:50:00.000000 duplicity-2.2.4rc2/testing/test_code.py
--rw-r--r--   0 ken       (1000) ken       (1000)   319661 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/testfiles.tar.gz
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.828805 duplicity-2.2.4rc2/testing/unit/
--rw-r--r--   0 ken       (1000) ken       (1000)      918 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/unit/__init__.py
--rw-r--r--   0 ken       (1000) ken       (1000)    15341 2024-03-19 15:05:23.000000 duplicity-2.2.4rc2/testing/unit/test_backend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    10384 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/unit/test_backend_instance.py
--rwxr-xr-x   0 ken       (1000) ken       (1000)    24240 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/testing/unit/test_cli_main.py
--rw-r--r--   0 ken       (1000) ken       (1000)    11337 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/unit/test_collections.py
--rw-r--r--   0 ken       (1000) ken       (1000)    12290 2024-01-29 17:23:01.000000 duplicity-2.2.4rc2/testing/unit/test_diffdir.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2371 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/unit/test_dup_temp.py
--rw-r--r--   0 ken       (1000) ken       (1000)     6012 2024-01-29 17:23:01.000000 duplicity-2.2.4rc2/testing/unit/test_dup_time.py
--rw-r--r--   0 ken       (1000) ken       (1000)     6084 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/unit/test_file_naming.py
--rw-r--r--   0 ken       (1000) ken       (1000)    13683 2024-01-29 17:20:11.000000 duplicity-2.2.4rc2/testing/unit/test_globmatch.py
--rw-r--r--   0 ken       (1000) ken       (1000)     8219 2024-01-29 17:23:01.000000 duplicity-2.2.4rc2/testing/unit/test_gpg.py
--rw-r--r--   0 ken       (1000) ken       (1000)     7891 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/unit/test_gpginterface.py
--rw-r--r--   0 ken       (1000) ken       (1000)    11380 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/unit/test_lazy.py
--rw-r--r--   0 ken       (1000) ken       (1000)     5722 2024-01-29 17:23:01.000000 duplicity-2.2.4rc2/testing/unit/test_manifest.py
--rw-r--r--   0 ken       (1000) ken       (1000)    11361 2024-03-19 15:05:23.000000 duplicity-2.2.4rc2/testing/unit/test_patchdir.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2888 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/unit/test_path.py
--rw-r--r--   0 ken       (1000) ken       (1000)    63194 2024-01-29 17:23:01.000000 duplicity-2.2.4rc2/testing/unit/test_selection.py
--rw-r--r--   0 ken       (1000) ken       (1000)     5549 2023-12-20 17:08:29.000000 duplicity-2.2.4rc2/testing/unit/test_statistics.py
--rw-r--r--   0 ken       (1000) ken       (1000)     1190 2024-01-29 17:23:01.000000 duplicity-2.2.4rc2/testing/unit/test_tarfile.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2483 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/unit/test_tempdir.py
--rw-r--r--   0 ken       (1000) ken       (1000)     1430 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/testing/unit/test_util.py
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2024-05-18 17:01:06.828805 duplicity-2.2.4rc2/tools/
--rwxr-xr-x   0 ken       (1000) ken       (1000)     1514 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/tools/installpyenv
--rwxr-xr-x   0 ken       (1000) ken       (1000)     2481 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/tools/installpythons
--rwxr-xr-x   0 ken       (1000) ken       (1000)     1936 2022-12-27 19:32:15.000000 duplicity-2.2.4rc2/tools/installsnap
--rwxr-xr-x   0 ken       (1000) ken       (1000)     1374 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/tools/makechangelog
--rwxr-xr-x   0 ken       (1000) ken       (1000)     1117 2024-03-19 15:05:23.000000 duplicity-2.2.4rc2/tools/makepip
--rwxr-xr-x   0 ken       (1000) ken       (1000)     1795 2024-03-19 15:05:23.000000 duplicity-2.2.4rc2/tools/makesnap
--rwxr-xr-x   0 ken       (1000) ken       (1000)     1243 2024-03-19 15:05:23.000000 duplicity-2.2.4rc2/tools/pushpip
--rwxr-xr-x   0 ken       (1000) ken       (1000)     1423 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/tools/pushsnap
--rwxr-xr-x   0 ken       (1000) ken       (1000)     2083 2024-03-20 16:49:45.000000 duplicity-2.2.4rc2/tools/release-prep
--rwxr-xr-x   0 ken       (1000) ken       (1000)     2856 2024-05-15 14:42:05.000000 duplicity-2.2.4rc2/tools/testpip
--rwxr-xr-x   0 ken       (1000) ken       (1000)     2114 2023-11-23 16:54:07.000000 duplicity-2.2.4rc2/tools/testsnap
--rw-r--r--   0 ken       (1000) ken       (1000)     2339 2024-03-19 15:05:23.000000 duplicity-2.2.4rc2/tox.ini
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.952723 duplicity-2.2.4rc3/
+-rw-r--r--   0 ken        (501) staff       (20)    10366 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/.gitchangelog.rc
+-rw-r--r--   0 ken        (501) staff       (20)      529 2024-03-19 15:05:23.000000 duplicity-2.2.4rc3/.gitignore
+-rw-r--r--   0 ken        (501) staff       (20)     6266 2024-05-18 18:19:59.000000 duplicity-2.2.4rc3/.gitlab-ci.yml
+-rw-r--r--   0 ken        (501) staff       (20)     1390 2024-01-29 17:23:01.000000 duplicity-2.2.4rc3/AUTHORS.md
+-rw-r--r--   0 ken        (501) staff       (20)   594229 2024-05-19 17:40:55.000000 duplicity-2.2.4rc3/CHANGELOG.md
+-rw-r--r--   0 ken        (501) staff       (20)    18028 2022-12-27 19:32:15.000000 duplicity-2.2.4rc3/COPYING
+-rw-r--r--   0 ken        (501) staff       (20)     1124 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/Makefile
+-rw-r--r--   0 ken        (501) staff       (20)     3848 2024-05-19 17:40:58.952574 duplicity-2.2.4rc3/PKG-INFO
+-rw-r--r--   0 ken        (501) staff       (20)     1284 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/README-LOG.md
+-rw-r--r--   0 ken        (501) staff       (20)      618 2024-04-30 19:30:15.000000 duplicity-2.2.4rc3/README-REPO.md
+-rw-r--r--   0 ken        (501) staff       (20)     3250 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/README-SNAP.md
+-rw-r--r--   0 ken        (501) staff       (20)     5364 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/README-TESTING.md
+-rw-r--r--   0 ken        (501) staff       (20)     3484 2024-05-18 18:19:59.000000 duplicity-2.2.4rc3/README.md
+-rw-r--r--   0 ken        (501) staff       (20)      164 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/crowdin.yml
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.798519 duplicity-2.2.4rc3/debian/
+-rw-r--r--   0 ken        (501) staff       (20)      189 2022-12-27 19:32:15.000000 duplicity-2.2.4rc3/debian/changelog
+-rw-r--r--   0 ken        (501) staff       (20)        3 2024-02-02 16:10:07.000000 duplicity-2.2.4rc3/debian/compat
+-rw-r--r--   0 ken        (501) staff       (20)     1510 2024-05-02 15:20:27.000000 duplicity-2.2.4rc3/debian/control
+-rw-r--r--   0 ken        (501) staff       (20)     1546 2024-01-29 17:35:45.000000 duplicity-2.2.4rc3/debian/copyright
+-rw-r--r--   0 ken        (501) staff       (20)      223 2024-02-02 16:10:07.000000 duplicity-2.2.4rc3/debian/duplicity.sh
+-rwxr-xr-x   0 ken        (501) staff       (20)      629 2024-02-02 16:10:07.000000 duplicity-2.2.4rc3/debian/rules
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.799095 duplicity-2.2.4rc3/debian/source/
+-rw-r--r--   0 ken        (501) staff       (20)       13 2022-12-27 19:32:15.000000 duplicity-2.2.4rc3/debian/source/format
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.802549 duplicity-2.2.4rc3/docs/
+-rw-r--r--   0 ken        (501) staff       (20)      787 2024-05-14 14:50:00.000000 duplicity-2.2.4rc3/docs/Makefile
+-rw-r--r--   0 ken        (501) staff       (20)      372 2024-03-25 15:18:48.000000 duplicity-2.2.4rc3/docs/README.md
+-rw-r--r--   0 ken        (501) staff       (20)     3436 2024-03-25 15:20:00.000000 duplicity-2.2.4rc3/docs/conf.py
+-rw-r--r--   0 ken        (501) staff       (20)      915 2023-03-19 16:45:14.000000 duplicity-2.2.4rc3/docs/index.rst
+-rw-r--r--   0 ken        (501) staff       (20)       75 2023-03-19 16:45:14.000000 duplicity-2.2.4rc3/docs/modules.rst
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.827064 duplicity-2.2.4rc3/duplicity/
+-rw-r--r--   0 ken        (501) staff       (20)     1034 2024-05-19 17:40:47.000000 duplicity-2.2.4rc3/duplicity/__init__.py
+-rwxr-xr-x   0 ken        (501) staff       (20)     3896 2024-01-29 17:23:01.000000 duplicity-2.2.4rc3/duplicity/__main__.py
+-rw-r--r--   0 ken        (501) staff       (20)    14510 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/_librsyncmodule.c
+-rw-r--r--   0 ken        (501) staff       (20)    96777 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/argparse311.py
+-rw-r--r--   0 ken        (501) staff       (20)    10243 2024-05-03 17:58:22.000000 duplicity-2.2.4rc3/duplicity/asyncscheduler.py
+-rw-r--r--   0 ken        (501) staff       (20)    28309 2024-05-14 14:50:00.000000 duplicity-2.2.4rc3/duplicity/backend.py
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.850148 duplicity-2.2.4rc3/duplicity/backends/
+-rw-r--r--   0 ken        (501) staff       (20)     3158 2024-03-19 15:05:23.000000 duplicity-2.2.4rc3/duplicity/backends/README
+-rw-r--r--   0 ken        (501) staff       (20)     1115 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/__init__.py
+-rw-r--r--   0 ken        (501) staff       (20)     3920 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/_cf_cloudfiles.py
+-rw-r--r--   0 ken        (501) staff       (20)     5138 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/_cf_pyrax.py
+-rw-r--r--   0 ken        (501) staff       (20)     9388 2024-05-14 14:50:00.000000 duplicity-2.2.4rc3/duplicity/backends/_testbackend.py
+-rw-r--r--   0 ken        (501) staff       (20)    16562 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/adbackend.py
+-rw-r--r--   0 ken        (501) staff       (20)     5536 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/azurebackend.py
+-rw-r--r--   0 ken        (501) staff       (20)     9214 2024-03-19 15:05:23.000000 duplicity-2.2.4rc3/duplicity/backends/b2backend.py
+-rw-r--r--   0 ken        (501) staff       (20)     6784 2024-01-29 16:41:36.000000 duplicity-2.2.4rc3/duplicity/backends/boxbackend.py
+-rw-r--r--   0 ken        (501) staff       (20)     1142 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/cfbackend.py
+-rw-r--r--   0 ken        (501) staff       (20)    19552 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/dpbxbackend.py
+-rw-r--r--   0 ken        (501) staff       (20)     9115 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/gdocsbackend.py
+-rw-r--r--   0 ken        (501) staff       (20)    16667 2024-02-03 16:19:07.000000 duplicity-2.2.4rc3/duplicity/backends/gdrivebackend.py
+-rw-r--r--   0 ken        (501) staff       (20)     7889 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/giobackend.py
+-rw-r--r--   0 ken        (501) staff       (20)     2604 2024-01-29 17:23:01.000000 duplicity-2.2.4rc3/duplicity/backends/hsibackend.py
+-rw-r--r--   0 ken        (501) staff       (20)     2426 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/hubicbackend.py
+-rw-r--r--   0 ken        (501) staff       (20)    19313 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/idrivedbackend.py
+-rw-r--r--   0 ken        (501) staff       (20)     9761 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/imapbackend.py
+-rw-r--r--   0 ken        (501) staff       (20)     5753 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/jottacloudbackend.py
+-rw-r--r--   0 ken        (501) staff       (20)     9183 2024-01-29 17:23:01.000000 duplicity-2.2.4rc3/duplicity/backends/lftpbackend.py
+-rw-r--r--   0 ken        (501) staff       (20)     3040 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/localbackend.py
+-rw-r--r--   0 ken        (501) staff       (20)     4634 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/mediafirebackend.py
+-rw-r--r--   0 ken        (501) staff       (20)     7097 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/megabackend.py
+-rw-r--r--   0 ken        (501) staff       (20)     8623 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/megav2backend.py
+-rw-r--r--   0 ken        (501) staff       (20)     9862 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/megav3backend.py
+-rw-r--r--   0 ken        (501) staff       (20)    15763 2023-12-04 21:05:42.000000 duplicity-2.2.4rc3/duplicity/backends/multibackend.py
+-rw-r--r--   0 ken        (501) staff       (20)     5450 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/ncftpbackend.py
+-rw-r--r--   0 ken        (501) staff       (20)    16318 2024-05-18 18:19:59.000000 duplicity-2.2.4rc3/duplicity/backends/onedrivebackend.py
+-rw-r--r--   0 ken        (501) staff       (20)     8989 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/par2backend.py
+-rw-r--r--   0 ken        (501) staff       (20)    12471 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/pcabackend.py
+-rw-r--r--   0 ken        (501) staff       (20)    13026 2024-01-29 16:41:36.000000 duplicity-2.2.4rc3/duplicity/backends/pydrivebackend.py
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.851594 duplicity-2.2.4rc3/duplicity/backends/pyrax_identity/
+-rw-r--r--   0 ken        (501) staff       (20)      903 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/pyrax_identity/__init__.py
+-rw-r--r--   0 ken        (501) staff       (20)     9745 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/pyrax_identity/hubic.py
+-rw-r--r--   0 ken        (501) staff       (20)     4284 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/rclonebackend.py
+-rw-r--r--   0 ken        (501) staff       (20)     6455 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/rsyncbackend.py
+-rw-r--r--   0 ken        (501) staff       (20)    10498 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/s3_boto3_backend.py
+-rw-r--r--   0 ken        (501) staff       (20)     6520 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/slatebackend.py
+-rw-r--r--   0 ken        (501) staff       (20)    19675 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/ssh_paramiko_backend.py
+-rw-r--r--   0 ken        (501) staff       (20)    12942 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/ssh_pexpect_backend.py
+-rw-r--r--   0 ken        (501) staff       (20)    10143 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/swiftbackend.py
+-rw-r--r--   0 ken        (501) staff       (20)     2317 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/sxbackend.py
+-rw-r--r--   0 ken        (501) staff       (20)     2564 2024-01-29 17:23:01.000000 duplicity-2.2.4rc3/duplicity/backends/tahoebackend.py
+-rw-r--r--   0 ken        (501) staff       (20)    18682 2024-05-14 14:50:00.000000 duplicity-2.2.4rc3/duplicity/backends/webdavbackend.py
+-rw-r--r--   0 ken        (501) staff       (20)    12248 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/backends/xorrisobackend.py
+-rw-r--r--   0 ken        (501) staff       (20)     1668 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/cached_ops.py
+-rw-r--r--   0 ken        (501) staff       (20)    34088 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/duplicity/cli_data.py
+-rw-r--r--   0 ken        (501) staff       (20)    11716 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/duplicity/cli_main.py
+-rw-r--r--   0 ken        (501) staff       (20)    14078 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/duplicity/cli_util.py
+-rw-r--r--   0 ken        (501) staff       (20)    11185 2024-05-03 17:58:22.000000 duplicity-2.2.4rc3/duplicity/config.py
+-rw-r--r--   0 ken        (501) staff       (20)    25936 2024-01-29 17:23:01.000000 duplicity-2.2.4rc3/duplicity/diffdir.py
+-rw-r--r--   0 ken        (501) staff       (20)    49699 2024-05-03 17:58:22.000000 duplicity-2.2.4rc3/duplicity/dup_collections.py
+-rw-r--r--   0 ken        (501) staff       (20)    62946 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/duplicity/dup_main.py
+-rw-r--r--   0 ken        (501) staff       (20)     1262 2024-01-29 17:23:01.000000 duplicity-2.2.4rc3/duplicity/dup_tarfile.py
+-rw-r--r--   0 ken        (501) staff       (20)     8369 2023-12-12 19:20:24.000000 duplicity-2.2.4rc3/duplicity/dup_temp.py
+-rw-r--r--   0 ken        (501) staff       (20)     7198 2024-05-03 17:58:22.000000 duplicity-2.2.4rc3/duplicity/dup_threading.py
+-rw-r--r--   0 ken        (501) staff       (20)    10380 2024-01-29 17:23:01.000000 duplicity-2.2.4rc3/duplicity/dup_time.py
+-rw-r--r--   0 ken        (501) staff       (20)     2723 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/errors.py
+-rw-r--r--   0 ken        (501) staff       (20)    16727 2024-01-20 17:46:53.000000 duplicity-2.2.4rc3/duplicity/file_naming.py
+-rw-r--r--   0 ken        (501) staff       (20)     2625 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/filechunkio.py
+-rw-r--r--   0 ken        (501) staff       (20)     7537 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/globmatch.py
+-rw-r--r--   0 ken        (501) staff       (20)    17768 2024-05-14 14:50:00.000000 duplicity-2.2.4rc3/duplicity/gpg.py
+-rw-r--r--   0 ken        (501) staff       (20)    22946 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/gpginterface.py
+-rw-r--r--   0 ken        (501) staff       (20)    14947 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/lazy.py
+-rw-r--r--   0 ken        (501) staff       (20)     8502 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/librsync.py
+-rw-r--r--   0 ken        (501) staff       (20)    15983 2024-05-03 17:58:22.000000 duplicity-2.2.4rc3/duplicity/log.py
+-rw-r--r--   0 ken        (501) staff       (20)    17964 2024-01-29 17:23:01.000000 duplicity-2.2.4rc3/duplicity/manifest.py
+-rw-r--r--   0 ken        (501) staff       (20)    21774 2024-01-29 17:23:01.000000 duplicity-2.2.4rc3/duplicity/patchdir.py
+-rw-r--r--   0 ken        (501) staff       (20)    28589 2024-03-19 15:05:23.000000 duplicity-2.2.4rc3/duplicity/path.py
+-rw-r--r--   0 ken        (501) staff       (20)    13824 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/progress.py
+-rw-r--r--   0 ken        (501) staff       (20)     2730 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/duplicity/robust.py
+-rw-r--r--   0 ken        (501) staff       (20)    29428 2024-01-29 16:41:36.000000 duplicity-2.2.4rc3/duplicity/selection.py
+-rw-r--r--   0 ken        (501) staff       (20)    15619 2023-12-20 17:08:29.000000 duplicity-2.2.4rc3/duplicity/statistics.py
+-rw-r--r--   0 ken        (501) staff       (20)    10716 2024-01-29 17:23:01.000000 duplicity-2.2.4rc3/duplicity/tempdir.py
+-rw-r--r--   0 ken        (501) staff       (20)    11030 2024-01-29 17:23:01.000000 duplicity-2.2.4rc3/duplicity/util.py
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.951226 duplicity-2.2.4rc3/duplicity.egg-info/
+-rw-r--r--   0 ken        (501) staff       (20)     3848 2024-05-19 17:40:58.000000 duplicity-2.2.4rc3/duplicity.egg-info/PKG-INFO
+-rw-r--r--   0 ken        (501) staff       (20)     7811 2024-05-19 17:40:58.000000 duplicity-2.2.4rc3/duplicity.egg-info/SOURCES.txt
+-rw-r--r--   0 ken        (501) staff       (20)        1 2024-05-19 17:40:58.000000 duplicity-2.2.4rc3/duplicity.egg-info/dependency_links.txt
+-rw-r--r--   0 ken        (501) staff       (20)       57 2024-05-19 17:40:58.000000 duplicity-2.2.4rc3/duplicity.egg-info/entry_points.txt
+-rw-r--r--   0 ken        (501) staff       (20)     2140 2024-05-19 17:40:58.000000 duplicity-2.2.4rc3/duplicity.egg-info/requires.txt
+-rw-r--r--   0 ken        (501) staff       (20)       10 2024-05-19 17:40:58.000000 duplicity-2.2.4rc3/duplicity.egg-info/top_level.txt
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.852309 duplicity-2.2.4rc3/man/
+-rw-r--r--   0 ken        (501) staff       (20)    94191 2024-05-19 17:40:47.000000 duplicity-2.2.4rc3/man/duplicity.1
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.875866 duplicity-2.2.4rc3/po/
+-rw-r--r--   0 ken        (501) staff       (20)      276 2024-05-14 15:33:39.000000 duplicity-2.2.4rc3/po/LINGUAS
+-rw-r--r--   0 ken        (501) staff       (20)     1174 2022-12-27 19:32:15.000000 duplicity-2.2.4rc3/po/Makevars
+-rw-r--r--   0 ken        (501) staff       (20)     2315 2024-05-14 15:33:39.000000 duplicity-2.2.4rc3/po/POTFILES.in
+-rw-r--r--   0 ken        (501) staff       (20)     1074 2024-05-14 15:33:39.000000 duplicity-2.2.4rc3/po/POTFILES.skip
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.876261 duplicity-2.2.4rc3/po/af_ZA/
+-rw-r--r--   0 ken        (501) staff       (20)      516 2024-05-19 17:40:58.000000 duplicity-2.2.4rc3/po/af_ZA/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    45456 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/af_ZA.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.876536 duplicity-2.2.4rc3/po/ar_SA/
+-rw-r--r--   0 ken        (501) staff       (20)    47467 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/ar_SA/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    69886 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/ar_SA.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.876860 duplicity-2.2.4rc3/po/ca_ES/
+-rw-r--r--   0 ken        (501) staff       (20)      514 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/ca_ES/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    45454 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/ca_ES.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.877119 duplicity-2.2.4rc3/po/cs_CZ/
+-rw-r--r--   0 ken        (501) staff       (20)    42586 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/cs_CZ/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    64046 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/cs_CZ.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.877541 duplicity-2.2.4rc3/po/da_DK/
+-rw-r--r--   0 ken        (501) staff       (20)    40754 2024-05-19 17:40:58.000000 duplicity-2.2.4rc3/po/da_DK/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    62115 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/da_DK.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.877881 duplicity-2.2.4rc3/po/de_AT/
+-rw-r--r--   0 ken        (501) staff       (20)    43792 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/de_AT/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    65263 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/de_AT.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.878204 duplicity-2.2.4rc3/po/de_DE/
+-rw-r--r--   0 ken        (501) staff       (20)    43780 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/de_DE/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    65251 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/de_DE.po
+-rw-r--r--   0 ken        (501) staff       (20)    45784 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/duplicity.pot
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.878625 duplicity-2.2.4rc3/po/el_GR/
+-rw-r--r--   0 ken        (501) staff       (20)    52055 2024-05-19 17:40:58.000000 duplicity-2.2.4rc3/po/el_GR/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    75344 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/el_GR.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.879014 duplicity-2.2.4rc3/po/en_AU/
+-rw-r--r--   0 ken        (501) staff       (20)      944 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/en_AU/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    45632 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/en_AU.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.879399 duplicity-2.2.4rc3/po/en_GB/
+-rw-r--r--   0 ken        (501) staff       (20)     2745 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/en_GB/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    46469 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/en_GB.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.879668 duplicity-2.2.4rc3/po/en_PR/
+-rw-r--r--   0 ken        (501) staff       (20)      530 2024-05-19 17:40:58.000000 duplicity-2.2.4rc3/po/en_PR/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    45470 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/en_PR.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.879909 duplicity-2.2.4rc3/po/en_US/
+-rw-r--r--   0 ken        (501) staff       (20)      532 2024-05-19 17:40:58.000000 duplicity-2.2.4rc3/po/en_US/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    45472 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/en_US.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.880161 duplicity-2.2.4rc3/po/es_EM/
+-rw-r--r--   0 ken        (501) staff       (20)    42408 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/es_EM/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    64161 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/es_EM.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.880483 duplicity-2.2.4rc3/po/es_ES/
+-rw-r--r--   0 ken        (501) staff       (20)    42399 2024-05-19 17:40:58.000000 duplicity-2.2.4rc3/po/es_ES/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    64152 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/es_ES.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.880802 duplicity-2.2.4rc3/po/es_MX/
+-rw-r--r--   0 ken        (501) staff       (20)    42407 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/es_MX/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    64160 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/es_MX.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.881110 duplicity-2.2.4rc3/po/es_PR/
+-rw-r--r--   0 ken        (501) staff       (20)    42412 2024-05-19 17:40:58.000000 duplicity-2.2.4rc3/po/es_PR/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    64165 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/es_PR.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.881413 duplicity-2.2.4rc3/po/es_US/
+-rw-r--r--   0 ken        (501) staff       (20)    42414 2024-05-19 17:40:58.000000 duplicity-2.2.4rc3/po/es_US/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    64167 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/es_US.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.881772 duplicity-2.2.4rc3/po/fi_FI/
+-rw-r--r--   0 ken        (501) staff       (20)    40182 2024-05-19 17:40:58.000000 duplicity-2.2.4rc3/po/fi_FI/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    62727 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/fi_FI.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.882085 duplicity-2.2.4rc3/po/fr_FR/
+-rw-r--r--   0 ken        (501) staff       (20)    42577 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/fr_FR/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    64995 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/fr_FR.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.882395 duplicity-2.2.4rc3/po/he_IL/
+-rw-r--r--   0 ken        (501) staff       (20)      964 2024-05-19 17:40:58.000000 duplicity-2.2.4rc3/po/he_IL/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    45741 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/he_IL.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.882642 duplicity-2.2.4rc3/po/hu_HU/
+-rw-r--r--   0 ken        (501) staff       (20)    20731 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/hu_HU/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    54662 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/hu_HU.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.882942 duplicity-2.2.4rc3/po/it_IT/
+-rw-r--r--   0 ken        (501) staff       (20)    42374 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/it_IT/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    64000 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/it_IT.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.883248 duplicity-2.2.4rc3/po/ja_JP/
+-rw-r--r--   0 ken        (501) staff       (20)    43260 2024-05-19 17:40:58.000000 duplicity-2.2.4rc3/po/ja_JP/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    66545 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/ja_JP.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.883556 duplicity-2.2.4rc3/po/ko_KR/
+-rw-r--r--   0 ken        (501) staff       (20)     5451 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/ko_KR/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    47463 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/ko_KR.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.883798 duplicity-2.2.4rc3/po/nl_BE/
+-rw-r--r--   0 ken        (501) staff       (20)    41940 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/nl_BE/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    63301 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/nl_BE.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.884120 duplicity-2.2.4rc3/po/nl_NL/
+-rw-r--r--   0 ken        (501) staff       (20)    41928 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/nl_NL/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    63289 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/nl_NL.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.884430 duplicity-2.2.4rc3/po/nl_SR/
+-rw-r--r--   0 ken        (501) staff       (20)    41941 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/nl_SR/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    63302 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/nl_SR.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.884728 duplicity-2.2.4rc3/po/no_NO/
+-rw-r--r--   0 ken        (501) staff       (20)    38960 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/no_NO/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    61387 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/no_NO.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.885042 duplicity-2.2.4rc3/po/pl_PL/
+-rw-r--r--   0 ken        (501) staff       (20)    42510 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/pl_PL/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    64376 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/pl_PL.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.885363 duplicity-2.2.4rc3/po/pt_BR/
+-rw-r--r--   0 ken        (501) staff       (20)    42538 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/pt_BR/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    64283 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/pt_BR.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.885674 duplicity-2.2.4rc3/po/pt_PT/
+-rw-r--r--   0 ken        (501) staff       (20)    41404 2024-05-19 17:40:58.000000 duplicity-2.2.4rc3/po/pt_PT/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    63328 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/pt_PT.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.885981 duplicity-2.2.4rc3/po/ro_RO/
+-rw-r--r--   0 ken        (501) staff       (20)    42217 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/ro_RO/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    63905 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/ro_RO.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.886296 duplicity-2.2.4rc3/po/ru_BY/
+-rw-r--r--   0 ken        (501) staff       (20)    54999 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/ru_BY/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    76691 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/ru_BY.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.886613 duplicity-2.2.4rc3/po/ru_MD/
+-rw-r--r--   0 ken        (501) staff       (20)    54999 2024-05-19 17:40:58.000000 duplicity-2.2.4rc3/po/ru_MD/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    76691 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/ru_MD.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.886942 duplicity-2.2.4rc3/po/ru_RU/
+-rw-r--r--   0 ken        (501) staff       (20)    54987 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/ru_RU/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    76679 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/ru_RU.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.887259 duplicity-2.2.4rc3/po/ru_UA/
+-rw-r--r--   0 ken        (501) staff       (20)    55001 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/ru_UA/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    76693 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/ru_UA.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.887576 duplicity-2.2.4rc3/po/sr_SP/
+-rw-r--r--   0 ken        (501) staff       (20)      599 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/sr_SP/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    45565 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/sr_SP.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.887815 duplicity-2.2.4rc3/po/sv_SE/
+-rw-r--r--   0 ken        (501) staff       (20)    42037 2024-05-19 17:40:58.000000 duplicity-2.2.4rc3/po/sv_SE/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    63416 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/sv_SE.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.888117 duplicity-2.2.4rc3/po/tr_TR/
+-rw-r--r--   0 ken        (501) staff       (20)     3629 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/tr_TR/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    46575 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/tr_TR.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.888376 duplicity-2.2.4rc3/po/uk_UA/
+-rw-r--r--   0 ken        (501) staff       (20)    47951 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/uk_UA/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    72573 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/uk_UA.po
+-rwxr-xr-x   0 ken        (501) staff       (20)     1140 2024-02-03 16:20:49.000000 duplicity-2.2.4rc3/po/update-pot
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.888676 duplicity-2.2.4rc3/po/vi_VN/
+-rw-r--r--   0 ken        (501) staff       (20)      510 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/vi_VN/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    45424 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/vi_VN.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.888931 duplicity-2.2.4rc3/po/zh_CN/
+-rw-r--r--   0 ken        (501) staff       (20)    35542 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/zh_CN/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    58854 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/zh_CN.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.889250 duplicity-2.2.4rc3/po/zh_HK/
+-rw-r--r--   0 ken        (501) staff       (20)      533 2024-05-19 17:40:58.000000 duplicity-2.2.4rc3/po/zh_HK/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    45447 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/zh_HK.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.889524 duplicity-2.2.4rc3/po/zh_MO/
+-rw-r--r--   0 ken        (501) staff       (20)      529 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/zh_MO/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    45443 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/zh_MO.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.889780 duplicity-2.2.4rc3/po/zh_SG/
+-rw-r--r--   0 ken        (501) staff       (20)      533 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/zh_SG/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    45447 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/zh_SG.po
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.890026 duplicity-2.2.4rc3/po/zh_TW/
+-rw-r--r--   0 ken        (501) staff       (20)      522 2024-05-19 17:40:57.000000 duplicity-2.2.4rc3/po/zh_TW/duplicity.mo
+-rw-r--r--   0 ken        (501) staff       (20)    45436 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/po/zh_TW.po
+-rw-r--r--   0 ken        (501) staff       (20)     2689 2024-05-19 17:40:47.000000 duplicity-2.2.4rc3/pyproject.toml
+-rw-r--r--   0 ken        (501) staff       (20)      497 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/readthedocs.yaml
+-rw-r--r--   0 ken        (501) staff       (20)     7662 2024-05-19 17:19:15.000000 duplicity-2.2.4rc3/requirements.txt
+-rw-r--r--   0 ken        (501) staff       (20)      695 2024-05-19 17:40:58.953710 duplicity-2.2.4rc3/setup.cfg
+-rwxr-xr-x   0 ken        (501) staff       (20)     9840 2024-05-19 17:40:47.000000 duplicity-2.2.4rc3/setup.py
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.890272 duplicity-2.2.4rc3/snap/
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.891103 duplicity-2.2.4rc3/snap/local/
+-rwxr-xr-x   0 ken        (501) staff       (20)      186 2022-12-27 19:32:15.000000 duplicity-2.2.4rc3/snap/local/debug.sh
+-rwxr-xr-x   0 ken        (501) staff       (20)      110 2022-12-27 19:32:15.000000 duplicity-2.2.4rc3/snap/local/launcher.sh
+-rw-r--r--   0 ken        (501) staff       (20)     4684 2024-05-19 17:40:47.000000 duplicity-2.2.4rc3/snap/snapcraft.yaml
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.894027 duplicity-2.2.4rc3/testing/
+-rw-r--r--   0 ken        (501) staff       (20)     4611 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/testing/__init__.py
+-rw-r--r--   0 ken        (501) staff       (20)      941 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/conftest.py
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.902130 duplicity-2.2.4rc3/testing/docker/
+-rw-r--r--   0 ken        (501) staff       (20)     1151 2022-12-27 19:32:15.000000 duplicity-2.2.4rc3/testing/docker/.env
+-rw-r--r--   0 ken        (501) staff       (20)       37 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/docker/.gitignore
+-rwxr-xr-x   0 ken        (501) staff       (20)     1272 2024-05-16 14:18:05.000000 duplicity-2.2.4rc3/testing/docker/build.sh
+-rw-r--r--   0 ken        (501) staff       (20)     2361 2022-12-27 19:32:15.000000 duplicity-2.2.4rc3/testing/docker/docker-compose.yml
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.902651 duplicity-2.2.4rc3/testing/docker/duplicity_test/
+-rw-r--r--   0 ken        (501) staff       (20)     3618 2024-05-16 14:18:05.000000 duplicity-2.2.4rc3/testing/docker/duplicity_test/Dockerfile
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.903758 duplicity-2.2.4rc3/testing/docker/ftp_server/
+-rw-r--r--   0 ken        (501) staff       (20)     1234 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/docker/ftp_server/Dockerfile
+-rw-r--r--   0 ken        (501) staff       (20)       94 2022-12-27 19:32:15.000000 duplicity-2.2.4rc3/testing/docker/ftp_server/pureftpd.passwd
+-rw-r--r--   0 ken        (501) staff       (20)     4199 2022-12-27 19:32:15.000000 duplicity-2.2.4rc3/testing/docker/hello-world-master.zip
+-rw-r--r--   0 ken        (501) staff       (20)     1675 2022-12-27 19:32:15.000000 duplicity-2.2.4rc3/testing/docker/id_rsa
+-rw-r--r--   0 ken        (501) staff       (20)      406 2022-12-27 19:32:15.000000 duplicity-2.2.4rc3/testing/docker/id_rsa.pub
+-rwxr-xr-x   0 ken        (501) staff       (20)     1320 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/docker/push.sh
+-rwxr-xr-x   0 ken        (501) staff       (20)     1151 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/docker/setup.sh
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.905410 duplicity-2.2.4rc3/testing/docker/ssh_server/
+-rw-r--r--   0 ken        (501) staff       (20)     2352 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/docker/ssh_server/Dockerfile
+-rwxr-xr-x   0 ken        (501) staff       (20)     1105 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/docker/teardown.sh
+-rwxr-xr-x   0 ken        (501) staff       (20)     1188 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/docker/testit.sh
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.911936 duplicity-2.2.4rc3/testing/functional/
+-rw-r--r--   0 ken        (501) staff       (20)    10498 2024-05-03 17:58:22.000000 duplicity-2.2.4rc3/testing/functional/__init__.py
+-rw-r--r--   0 ken        (501) staff       (20)     3303 2024-05-03 17:58:22.000000 duplicity-2.2.4rc3/testing/functional/test_badupload.py
+-rw-r--r--   0 ken        (501) staff       (20)     3825 2024-05-03 17:58:22.000000 duplicity-2.2.4rc3/testing/functional/test_cleanup.py
+-rw-r--r--   0 ken        (501) staff       (20)    11215 2024-01-29 17:23:01.000000 duplicity-2.2.4rc3/testing/functional/test_final.py
+-rw-r--r--   0 ken        (501) staff       (20)     2401 2024-03-19 15:05:23.000000 duplicity-2.2.4rc3/testing/functional/test_log.py
+-rw-r--r--   0 ken        (501) staff       (20)    18836 2024-05-03 17:58:22.000000 duplicity-2.2.4rc3/testing/functional/test_restart.py
+-rw-r--r--   0 ken        (501) staff       (20)    99174 2024-01-29 17:23:01.000000 duplicity-2.2.4rc3/testing/functional/test_selection.py
+-rw-r--r--   0 ken        (501) staff       (20)     8664 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/functional/test_verify.py
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.915172 duplicity-2.2.4rc3/testing/gnupg/
+-rw-r--r--   0 ken        (501) staff       (20)      255 2022-12-27 19:32:15.000000 duplicity-2.2.4rc3/testing/gnupg/README
+-rw-r--r--   0 ken        (501) staff       (20)      145 2022-12-27 19:32:15.000000 duplicity-2.2.4rc3/testing/gnupg/gpg-agent.conf
+-rw-r--r--   0 ken        (501) staff       (20)      425 2022-12-27 19:32:15.000000 duplicity-2.2.4rc3/testing/gnupg/gpg.conf
+-rw-r--r--   0 ken        (501) staff       (20)     3567 2022-12-27 19:32:15.000000 duplicity-2.2.4rc3/testing/gnupg/pubring.gpg
+-rw-r--r--   0 ken        (501) staff       (20)     7549 2022-12-27 19:32:15.000000 duplicity-2.2.4rc3/testing/gnupg/secring.gpg
+-rw-r--r--   0 ken        (501) staff       (20)     1440 2022-12-27 19:32:15.000000 duplicity-2.2.4rc3/testing/gnupg/trustdb.gpg
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.920250 duplicity-2.2.4rc3/testing/manual/
+-rw-r--r--   0 ken        (501) staff       (20)      903 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/manual/__init__.py
+-rwxr-xr-x   0 ken        (501) staff       (20)     1411 2022-12-27 19:32:15.000000 duplicity-2.2.4rc3/testing/manual/auto-ctrl-c-test.sh
+-rwxr-xr-x   0 ken        (501) staff       (20)     8583 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/manual/backendtest.py
+-rwxr-xr-x   0 ken        (501) staff       (20)     1834 2022-12-27 19:32:15.000000 duplicity-2.2.4rc3/testing/manual/manual-ctrl-c-test.sh
+-rw-r--r--   0 ken        (501) staff       (20)      738 2022-12-27 19:32:15.000000 duplicity-2.2.4rc3/testing/manual/rootfiles.tar.gz
+-rwxr-xr-x   0 ken        (501) staff       (20)     4765 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/manual/roottest.py
+-rwxr-xr-x   0 ken        (501) staff       (20)     1727 2022-12-27 19:32:15.000000 duplicity-2.2.4rc3/testing/manual/run-coverage.sh
+-rwxr-xr-x   0 ken        (501) staff       (20)      446 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/testing/manual/test-prefix-install.sh
+-rwxr-xr-x   0 ken        (501) staff       (20)      542 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/testing/manual/test-venv-install.sh
+-rw-r--r--   0 ken        (501) staff       (20)     1612 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/manual/test_config.py.tmpl
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.920660 duplicity-2.2.4rc3/testing/overrides/
+-rw-r--r--   0 ken        (501) staff       (20)       75 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/overrides/__init__.py
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.923029 duplicity-2.2.4rc3/testing/overrides/bin/
+-rwxr-xr-x   0 ken        (501) staff       (20)      423 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/overrides/bin/hsi
+-rwxr-xr-x   0 ken        (501) staff       (20)      512 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/overrides/bin/lftp
+-rwxr-xr-x   0 ken        (501) staff       (20)      155 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/overrides/bin/ncftpget
+-rwxr-xr-x   0 ken        (501) staff       (20)      558 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/overrides/bin/ncftpls
+-rwxr-xr-x   0 ken        (501) staff       (20)      155 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/overrides/bin/ncftpput
+-rwxr-xr-x   0 ken        (501) staff       (20)      416 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/overrides/bin/tahoe
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.933773 duplicity-2.2.4rc3/testing/regression/
+-rwxr-xr-x   0 ken        (501) staff       (20)      503 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/regression/bug1526557.sh
+-rwxr-xr-x   0 ken        (501) staff       (20)      192 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/regression/bug1846678.sh
+-rwxr-xr-x   0 ken        (501) staff       (20)      680 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/regression/bug1860200.sh
+-rwxr-xr-x   0 ken        (501) staff       (20)      905 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/regression/bug487720.sh
+-rwxr-xr-x   0 ken        (501) staff       (20)      457 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/regression/bug930151.sh
+-rwxr-xr-x   0 ken        (501) staff       (20)      417 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/regression/issue100.sh
+-rw-r--r--   0 ken        (501) staff       (20)      295 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/regression/issue103.json
+-rwxr-xr-x   0 ken        (501) staff       (20)     1621 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/regression/issue103.sh
+-rwxr-xr-x   0 ken        (501) staff       (20)      554 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/regression/issue110-setup.sh
+-rwxr-xr-x   0 ken        (501) staff       (20)      278 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/regression/issue110-test.sh
+-rwxr-xr-x   0 ken        (501) staff       (20)     1312 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/regression/issue125.sh
+-rwxr-xr-x   0 ken        (501) staff       (20)      280 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/regression/issue147.sh
+-rw-r--r--   0 ken        (501) staff       (20)      189 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/regression/issue25.json
+-rwxr-xr-x   0 ken        (501) staff       (20)      685 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/regression/issue25.sh
+-rwxr-xr-x   0 ken        (501) staff       (20)      466 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/regression/issue26.sh
+-rwxr-xr-x   0 ken        (501) staff       (20)      464 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/regression/issue683.sh
+-rwxr-xr-x   0 ken        (501) staff       (20)      794 2024-03-19 15:05:23.000000 duplicity-2.2.4rc3/testing/regression/issue725.sh
+-rw-r--r--   0 ken        (501) staff       (20)      144 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/regression/issue73.env
+-rwxr-xr-x   0 ken        (501) staff       (20)      418 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/regression/issue73.sh
+-rw-r--r--   0 ken        (501) staff       (20)      189 2023-12-04 21:05:42.000000 duplicity-2.2.4rc3/testing/regression/issue781.json
+-rwxr-xr-x   0 ken        (501) staff       (20)      630 2023-12-04 21:05:42.000000 duplicity-2.2.4rc3/testing/regression/issue781.sh
+-rw-r--r--   0 ken        (501) staff       (20)      189 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/regression/issue79.json
+-rwxr-xr-x   0 ken        (501) staff       (20)     1087 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/regression/issue79.sh
+-rwxr-xr-x   0 ken        (501) staff       (20)     1001 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/regression/issue98.sh
+-rwxr-xr-x   0 ken        (501) staff       (20)      878 2022-12-27 19:32:15.000000 duplicity-2.2.4rc3/testing/run-tests
+-rw-r--r--   0 ken        (501) staff       (20)     3287 2024-05-14 14:50:00.000000 duplicity-2.2.4rc3/testing/test_code.py
+-rw-r--r--   0 ken        (501) staff       (20)   319661 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/testfiles.tar.gz
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.944667 duplicity-2.2.4rc3/testing/unit/
+-rw-r--r--   0 ken        (501) staff       (20)      918 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/unit/__init__.py
+-rw-r--r--   0 ken        (501) staff       (20)    15341 2024-03-19 15:05:23.000000 duplicity-2.2.4rc3/testing/unit/test_backend.py
+-rw-r--r--   0 ken        (501) staff       (20)    10384 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/unit/test_backend_instance.py
+-rwxr-xr-x   0 ken        (501) staff       (20)    24240 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/testing/unit/test_cli_main.py
+-rw-r--r--   0 ken        (501) staff       (20)    11337 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/unit/test_collections.py
+-rw-r--r--   0 ken        (501) staff       (20)    12290 2024-01-29 17:23:01.000000 duplicity-2.2.4rc3/testing/unit/test_diffdir.py
+-rw-r--r--   0 ken        (501) staff       (20)     2371 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/unit/test_dup_temp.py
+-rw-r--r--   0 ken        (501) staff       (20)     6012 2024-01-29 17:23:01.000000 duplicity-2.2.4rc3/testing/unit/test_dup_time.py
+-rw-r--r--   0 ken        (501) staff       (20)     6084 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/unit/test_file_naming.py
+-rw-r--r--   0 ken        (501) staff       (20)    13683 2024-01-29 17:20:11.000000 duplicity-2.2.4rc3/testing/unit/test_globmatch.py
+-rw-r--r--   0 ken        (501) staff       (20)     8219 2024-01-29 17:23:01.000000 duplicity-2.2.4rc3/testing/unit/test_gpg.py
+-rw-r--r--   0 ken        (501) staff       (20)     7891 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/unit/test_gpginterface.py
+-rw-r--r--   0 ken        (501) staff       (20)    11380 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/unit/test_lazy.py
+-rw-r--r--   0 ken        (501) staff       (20)     5722 2024-01-29 17:23:01.000000 duplicity-2.2.4rc3/testing/unit/test_manifest.py
+-rw-r--r--   0 ken        (501) staff       (20)    11361 2024-03-19 15:05:23.000000 duplicity-2.2.4rc3/testing/unit/test_patchdir.py
+-rw-r--r--   0 ken        (501) staff       (20)     2888 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/unit/test_path.py
+-rw-r--r--   0 ken        (501) staff       (20)    63194 2024-01-29 17:23:01.000000 duplicity-2.2.4rc3/testing/unit/test_selection.py
+-rw-r--r--   0 ken        (501) staff       (20)     5549 2023-12-20 17:08:29.000000 duplicity-2.2.4rc3/testing/unit/test_statistics.py
+-rw-r--r--   0 ken        (501) staff       (20)     1190 2024-01-29 17:23:01.000000 duplicity-2.2.4rc3/testing/unit/test_tarfile.py
+-rw-r--r--   0 ken        (501) staff       (20)     2483 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/unit/test_tempdir.py
+-rw-r--r--   0 ken        (501) staff       (20)     1430 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/testing/unit/test_util.py
+drwxr-xr-x   0 ken        (501) staff       (20)        0 2024-05-19 17:40:58.950216 duplicity-2.2.4rc3/tools/
+-rwxr-xr-x   0 ken        (501) staff       (20)     1514 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/tools/installpyenv
+-rwxr-xr-x   0 ken        (501) staff       (20)     2481 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/tools/installpythons
+-rwxr-xr-x   0 ken        (501) staff       (20)     1936 2022-12-27 19:32:15.000000 duplicity-2.2.4rc3/tools/installsnap
+-rwxr-xr-x   0 ken        (501) staff       (20)     1374 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/tools/makechangelog
+-rwxr-xr-x   0 ken        (501) staff       (20)     1117 2024-03-19 15:05:23.000000 duplicity-2.2.4rc3/tools/makepip
+-rwxr-xr-x   0 ken        (501) staff       (20)     1795 2024-03-19 15:05:23.000000 duplicity-2.2.4rc3/tools/makesnap
+-rwxr-xr-x   0 ken        (501) staff       (20)     1267 2024-05-18 18:19:59.000000 duplicity-2.2.4rc3/tools/pushpip
+-rwxr-xr-x   0 ken        (501) staff       (20)     1423 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/tools/pushsnap
+-rwxr-xr-x   0 ken        (501) staff       (20)     2083 2024-03-20 16:49:45.000000 duplicity-2.2.4rc3/tools/release-prep
+-rwxr-xr-x   0 ken        (501) staff       (20)     2856 2024-05-15 14:42:05.000000 duplicity-2.2.4rc3/tools/testpip
+-rwxr-xr-x   0 ken        (501) staff       (20)     2114 2023-11-23 16:54:07.000000 duplicity-2.2.4rc3/tools/testsnap
+-rw-r--r--   0 ken        (501) staff       (20)     2339 2024-03-19 15:05:23.000000 duplicity-2.2.4rc3/tox.ini
```

### Comparing `duplicity-2.2.4rc2/.gitchangelog.rc` & `duplicity-2.2.4rc3/.gitchangelog.rc`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/.gitignore` & `duplicity-2.2.4rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/.gitlab-ci.yml` & `duplicity-2.2.4rc3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/AUTHORS.md` & `duplicity-2.2.4rc3/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/CHANGELOG.md` & `duplicity-2.2.4rc3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,54 @@
 # Changelog
 
 
+## rel.2.2.4rc3 (2024-05-19)
+
+### Changes
+
+* Bump version to 2.2.4.rc3. [Kenneth Loafman]
+
+* Use pip-compile to build requirements.txt. [Kenneth Loafman]
+
+
+## rel.2.2.4rc2 (2024-05-18)
+
+### Changes
+
+* Adjust since twine does not do wildcards. [Kenneth Loafman]
+
+* Revert "chg:pkg: Add missing fasteners install dependency" [Kenneth Loafman]
+
+    This reverts commit ce3baa9a86ed6734dc7b013b6aaa1b873a2ba481.
+
+* Add requirements.dev to tests. [Kenneth Loafman]
+
+* Bump version to 2.2.4.rc2. [Kenneth Loafman]
+
+* Split requirements.txt into .txt and .dev. [Kenneth Loafman]
+
+* Add missing fasteners install dependency. [Michael Terry]
+
+* Run po/update-pot. [Kenneth Loafman]
+
+* Fix typo in ignore new pylint warning. [Kenneth Loafman]
+
+* Ignore new pylint warning E0606 (possibly-used-before-assignment). [Kenneth Loafman]
+
+### Fix
+
+* Onedrive: fix "unauthorized" upload error by not passing auth. [Michael Terry]
+
+    After the initial createUploadSession, apparently OneDrive actively dislikes it if you send Authorization headers on the subsequent PUT calls.
+
+    See their docs: https://learn.microsoft.com/en-us/graph/api/driveitem-createuploadsession?view=graph-rest-1.0#remarks
+
+    If you do include the Authorization header, you get 401 responses.
+
+
 ## rel.2.2.4rc1 (2024-05-15)
 
 ### Changes
 
 * Run po/update-pot. [Kenneth Loafman]
 
 * Fix typo in ignore new pylint warning. [Kenneth Loafman]
```

### Comparing `duplicity-2.2.4rc2/COPYING` & `duplicity-2.2.4rc3/COPYING`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/Makefile` & `duplicity-2.2.4rc3/Makefile`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/README-LOG.md` & `duplicity-2.2.4rc3/README-LOG.md`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/README-REPO.md` & `duplicity-2.2.4rc3/README-REPO.md`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/README-SNAP.md` & `duplicity-2.2.4rc3/README-SNAP.md`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/README-TESTING.md` & `duplicity-2.2.4rc3/README-TESTING.md`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/README.md` & `duplicity-2.2.4rc3/README.md`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/debian/control` & `duplicity-2.2.4rc3/debian/control`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/debian/copyright` & `duplicity-2.2.4rc3/debian/copyright`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/debian/rules` & `duplicity-2.2.4rc3/debian/rules`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/docs/Makefile` & `duplicity-2.2.4rc3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/docs/conf.py` & `duplicity-2.2.4rc3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/docs/index.rst` & `duplicity-2.2.4rc3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/__init__.py` & `duplicity-2.2.4rc3/duplicity/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,11 +17,11 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with duplicity; if not, write to the Free Software Foundation,
 # Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307 USA
 
 import gettext
 
-__version__: str = "2.2.4rc2"
-__reldate__: str = "May 18, 2024"
+__version__: str = "2.2.4rc3"
+__reldate__: str = "May 19, 2024"
 
 gettext.install("duplicity", names=["ngettext"])
```

### Comparing `duplicity-2.2.4rc2/duplicity/__main__.py` & `duplicity-2.2.4rc3/duplicity/__main__.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/_librsyncmodule.c` & `duplicity-2.2.4rc3/duplicity/_librsyncmodule.c`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/argparse311.py` & `duplicity-2.2.4rc3/duplicity/argparse311.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/asyncscheduler.py` & `duplicity-2.2.4rc3/duplicity/asyncscheduler.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backend.py` & `duplicity-2.2.4rc3/duplicity/backend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/README` & `duplicity-2.2.4rc3/duplicity/backends/README`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/__init__.py` & `duplicity-2.2.4rc3/duplicity/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/_cf_cloudfiles.py` & `duplicity-2.2.4rc3/duplicity/backends/_cf_cloudfiles.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/_cf_pyrax.py` & `duplicity-2.2.4rc3/duplicity/backends/_cf_pyrax.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/_testbackend.py` & `duplicity-2.2.4rc3/duplicity/backends/_testbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/adbackend.py` & `duplicity-2.2.4rc3/duplicity/backends/adbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/azurebackend.py` & `duplicity-2.2.4rc3/duplicity/backends/azurebackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/b2backend.py` & `duplicity-2.2.4rc3/duplicity/backends/b2backend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/boxbackend.py` & `duplicity-2.2.4rc3/duplicity/backends/boxbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/cfbackend.py` & `duplicity-2.2.4rc3/duplicity/backends/cfbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/dpbxbackend.py` & `duplicity-2.2.4rc3/duplicity/backends/dpbxbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/gdocsbackend.py` & `duplicity-2.2.4rc3/duplicity/backends/gdocsbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/gdrivebackend.py` & `duplicity-2.2.4rc3/duplicity/backends/gdrivebackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/giobackend.py` & `duplicity-2.2.4rc3/duplicity/backends/giobackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/hsibackend.py` & `duplicity-2.2.4rc3/duplicity/backends/hsibackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/hubicbackend.py` & `duplicity-2.2.4rc3/duplicity/backends/hubicbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/idrivedbackend.py` & `duplicity-2.2.4rc3/duplicity/backends/idrivedbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/imapbackend.py` & `duplicity-2.2.4rc3/duplicity/backends/imapbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/jottacloudbackend.py` & `duplicity-2.2.4rc3/duplicity/backends/jottacloudbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/lftpbackend.py` & `duplicity-2.2.4rc3/duplicity/backends/lftpbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/localbackend.py` & `duplicity-2.2.4rc3/duplicity/backends/localbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/mediafirebackend.py` & `duplicity-2.2.4rc3/duplicity/backends/mediafirebackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/megabackend.py` & `duplicity-2.2.4rc3/duplicity/backends/megabackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/megav2backend.py` & `duplicity-2.2.4rc3/duplicity/backends/megav2backend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/megav3backend.py` & `duplicity-2.2.4rc3/duplicity/backends/megav3backend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/multibackend.py` & `duplicity-2.2.4rc3/duplicity/backends/multibackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/ncftpbackend.py` & `duplicity-2.2.4rc3/duplicity/backends/ncftpbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/onedrivebackend.py` & `duplicity-2.2.4rc3/duplicity/backends/onedrivebackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/par2backend.py` & `duplicity-2.2.4rc3/duplicity/backends/par2backend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/pcabackend.py` & `duplicity-2.2.4rc3/duplicity/backends/pcabackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/pydrivebackend.py` & `duplicity-2.2.4rc3/duplicity/backends/pydrivebackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/pyrax_identity/__init__.py` & `duplicity-2.2.4rc3/duplicity/backends/pyrax_identity/__init__.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/pyrax_identity/hubic.py` & `duplicity-2.2.4rc3/duplicity/backends/pyrax_identity/hubic.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/rclonebackend.py` & `duplicity-2.2.4rc3/duplicity/backends/rclonebackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/rsyncbackend.py` & `duplicity-2.2.4rc3/duplicity/backends/rsyncbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/s3_boto3_backend.py` & `duplicity-2.2.4rc3/duplicity/backends/s3_boto3_backend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/slatebackend.py` & `duplicity-2.2.4rc3/duplicity/backends/slatebackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/ssh_paramiko_backend.py` & `duplicity-2.2.4rc3/duplicity/backends/ssh_paramiko_backend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/ssh_pexpect_backend.py` & `duplicity-2.2.4rc3/duplicity/backends/ssh_pexpect_backend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/swiftbackend.py` & `duplicity-2.2.4rc3/duplicity/backends/swiftbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/sxbackend.py` & `duplicity-2.2.4rc3/duplicity/backends/sxbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/tahoebackend.py` & `duplicity-2.2.4rc3/duplicity/backends/tahoebackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/webdavbackend.py` & `duplicity-2.2.4rc3/duplicity/backends/webdavbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/backends/xorrisobackend.py` & `duplicity-2.2.4rc3/duplicity/backends/xorrisobackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/cached_ops.py` & `duplicity-2.2.4rc3/duplicity/cached_ops.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/cli_data.py` & `duplicity-2.2.4rc3/duplicity/cli_data.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/cli_main.py` & `duplicity-2.2.4rc3/duplicity/cli_main.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/cli_util.py` & `duplicity-2.2.4rc3/duplicity/cli_util.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/config.py` & `duplicity-2.2.4rc3/duplicity/config.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/diffdir.py` & `duplicity-2.2.4rc3/duplicity/diffdir.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/dup_collections.py` & `duplicity-2.2.4rc3/duplicity/dup_collections.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/dup_main.py` & `duplicity-2.2.4rc3/duplicity/dup_main.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/dup_tarfile.py` & `duplicity-2.2.4rc3/duplicity/dup_tarfile.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/dup_temp.py` & `duplicity-2.2.4rc3/duplicity/dup_temp.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/dup_threading.py` & `duplicity-2.2.4rc3/duplicity/dup_threading.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/dup_time.py` & `duplicity-2.2.4rc3/duplicity/dup_time.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/errors.py` & `duplicity-2.2.4rc3/duplicity/errors.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/file_naming.py` & `duplicity-2.2.4rc3/duplicity/file_naming.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/filechunkio.py` & `duplicity-2.2.4rc3/duplicity/filechunkio.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/globmatch.py` & `duplicity-2.2.4rc3/duplicity/globmatch.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/gpg.py` & `duplicity-2.2.4rc3/duplicity/gpg.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/gpginterface.py` & `duplicity-2.2.4rc3/duplicity/gpginterface.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/lazy.py` & `duplicity-2.2.4rc3/duplicity/lazy.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/librsync.py` & `duplicity-2.2.4rc3/duplicity/librsync.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/log.py` & `duplicity-2.2.4rc3/duplicity/log.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/manifest.py` & `duplicity-2.2.4rc3/duplicity/manifest.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/patchdir.py` & `duplicity-2.2.4rc3/duplicity/patchdir.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/path.py` & `duplicity-2.2.4rc3/duplicity/path.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/progress.py` & `duplicity-2.2.4rc3/duplicity/progress.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/robust.py` & `duplicity-2.2.4rc3/duplicity/robust.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/selection.py` & `duplicity-2.2.4rc3/duplicity/selection.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/statistics.py` & `duplicity-2.2.4rc3/duplicity/statistics.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/tempdir.py` & `duplicity-2.2.4rc3/duplicity/tempdir.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity/util.py` & `duplicity-2.2.4rc3/duplicity/util.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/duplicity.egg-info/SOURCES.txt` & `duplicity-2.2.4rc3/duplicity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/man/duplicity.1` & `duplicity-2.2.4rc3/man/duplicity.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH DUPLICITY 1 "May 18, 2024" "Version 2.2.4rc2" "User Manuals" \"  -*- nroff -*-
+.TH DUPLICITY 1 "May 19, 2024" "Version 2.2.4rc3" "User Manuals" \"  -*- nroff -*-
 .\" disable justification (adjust text to left margin only)
 .\" command line examples stay readable through that
 .ad l
 .\" disable hyphenation
 .nh
 
 .SH NAME
```

### Comparing `duplicity-2.2.4rc2/po/Makevars` & `duplicity-2.2.4rc3/po/Makevars`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/POTFILES.in` & `duplicity-2.2.4rc3/po/POTFILES.in`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/POTFILES.skip` & `duplicity-2.2.4rc3/po/POTFILES.skip`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/af_ZA/duplicity.mo` & `duplicity-2.2.4rc3/po/af_ZA/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/af_ZA.po` & `duplicity-2.2.4rc3/po/af_ZA.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/ar_SA/duplicity.mo` & `duplicity-2.2.4rc3/po/ar_SA/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/ar_SA.po` & `duplicity-2.2.4rc3/po/ar_SA.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/ca_ES/duplicity.mo` & `duplicity-2.2.4rc3/po/ca_ES/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/ca_ES.po` & `duplicity-2.2.4rc3/po/ca_ES.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/cs_CZ/duplicity.mo` & `duplicity-2.2.4rc3/po/cs_CZ/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/cs_CZ.po` & `duplicity-2.2.4rc3/po/cs_CZ.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/da_DK/duplicity.mo` & `duplicity-2.2.4rc3/po/da_DK/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/da_DK.po` & `duplicity-2.2.4rc3/po/da_DK.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/de_AT/duplicity.mo` & `duplicity-2.2.4rc3/po/de_AT/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/de_AT.po` & `duplicity-2.2.4rc3/po/de_AT.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/de_DE/duplicity.mo` & `duplicity-2.2.4rc3/po/de_DE/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/de_DE.po` & `duplicity-2.2.4rc3/po/de_DE.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/duplicity.pot` & `duplicity-2.2.4rc3/po/duplicity.pot`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/el_GR/duplicity.mo` & `duplicity-2.2.4rc3/po/el_GR/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/el_GR.po` & `duplicity-2.2.4rc3/po/el_GR.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/en_AU/duplicity.mo` & `duplicity-2.2.4rc3/po/en_AU/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/en_AU.po` & `duplicity-2.2.4rc3/po/en_AU.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/en_GB/duplicity.mo` & `duplicity-2.2.4rc3/po/en_GB/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/en_GB.po` & `duplicity-2.2.4rc3/po/en_GB.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/en_PR/duplicity.mo` & `duplicity-2.2.4rc3/po/en_PR/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/en_PR.po` & `duplicity-2.2.4rc3/po/en_PR.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/en_US/duplicity.mo` & `duplicity-2.2.4rc3/po/en_US/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/en_US.po` & `duplicity-2.2.4rc3/po/en_US.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/es_EM/duplicity.mo` & `duplicity-2.2.4rc3/po/es_EM/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/es_EM.po` & `duplicity-2.2.4rc3/po/es_EM.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/es_ES/duplicity.mo` & `duplicity-2.2.4rc3/po/es_ES/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/es_ES.po` & `duplicity-2.2.4rc3/po/es_ES.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/es_MX/duplicity.mo` & `duplicity-2.2.4rc3/po/es_MX/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/es_MX.po` & `duplicity-2.2.4rc3/po/es_MX.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/es_PR/duplicity.mo` & `duplicity-2.2.4rc3/po/es_PR/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/es_PR.po` & `duplicity-2.2.4rc3/po/es_PR.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/es_US/duplicity.mo` & `duplicity-2.2.4rc3/po/es_US/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/es_US.po` & `duplicity-2.2.4rc3/po/es_US.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/fi_FI/duplicity.mo` & `duplicity-2.2.4rc3/po/fi_FI/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/fi_FI.po` & `duplicity-2.2.4rc3/po/fi_FI.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/fr_FR/duplicity.mo` & `duplicity-2.2.4rc3/po/fr_FR/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/fr_FR.po` & `duplicity-2.2.4rc3/po/fr_FR.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/he_IL/duplicity.mo` & `duplicity-2.2.4rc3/po/he_IL/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/he_IL.po` & `duplicity-2.2.4rc3/po/he_IL.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/hu_HU/duplicity.mo` & `duplicity-2.2.4rc3/po/hu_HU/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/hu_HU.po` & `duplicity-2.2.4rc3/po/hu_HU.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/it_IT/duplicity.mo` & `duplicity-2.2.4rc3/po/it_IT/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/it_IT.po` & `duplicity-2.2.4rc3/po/it_IT.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/ja_JP/duplicity.mo` & `duplicity-2.2.4rc3/po/ja_JP/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/ja_JP.po` & `duplicity-2.2.4rc3/po/ja_JP.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/ko_KR/duplicity.mo` & `duplicity-2.2.4rc3/po/ko_KR/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/ko_KR.po` & `duplicity-2.2.4rc3/po/ko_KR.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/nl_BE/duplicity.mo` & `duplicity-2.2.4rc3/po/nl_BE/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/nl_BE.po` & `duplicity-2.2.4rc3/po/nl_BE.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/nl_NL/duplicity.mo` & `duplicity-2.2.4rc3/po/nl_NL/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/nl_NL.po` & `duplicity-2.2.4rc3/po/nl_NL.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/nl_SR/duplicity.mo` & `duplicity-2.2.4rc3/po/nl_SR/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/nl_SR.po` & `duplicity-2.2.4rc3/po/nl_SR.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/no_NO/duplicity.mo` & `duplicity-2.2.4rc3/po/no_NO/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/no_NO.po` & `duplicity-2.2.4rc3/po/no_NO.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/pl_PL/duplicity.mo` & `duplicity-2.2.4rc3/po/pl_PL/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/pl_PL.po` & `duplicity-2.2.4rc3/po/pl_PL.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/pt_BR/duplicity.mo` & `duplicity-2.2.4rc3/po/pt_BR/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/pt_BR.po` & `duplicity-2.2.4rc3/po/pt_BR.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/pt_PT/duplicity.mo` & `duplicity-2.2.4rc3/po/pt_PT/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/pt_PT.po` & `duplicity-2.2.4rc3/po/pt_PT.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/ro_RO/duplicity.mo` & `duplicity-2.2.4rc3/po/ro_RO/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/ro_RO.po` & `duplicity-2.2.4rc3/po/ro_RO.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/ru_BY/duplicity.mo` & `duplicity-2.2.4rc3/po/ru_BY/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/ru_BY.po` & `duplicity-2.2.4rc3/po/ru_BY.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/ru_MD/duplicity.mo` & `duplicity-2.2.4rc3/po/ru_MD/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/ru_MD.po` & `duplicity-2.2.4rc3/po/ru_MD.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/ru_RU/duplicity.mo` & `duplicity-2.2.4rc3/po/ru_RU/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/ru_RU.po` & `duplicity-2.2.4rc3/po/ru_RU.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/ru_UA/duplicity.mo` & `duplicity-2.2.4rc3/po/ru_UA/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/ru_UA.po` & `duplicity-2.2.4rc3/po/ru_UA.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/sr_SP/duplicity.mo` & `duplicity-2.2.4rc3/po/sr_SP/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/sr_SP.po` & `duplicity-2.2.4rc3/po/sr_SP.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/sv_SE/duplicity.mo` & `duplicity-2.2.4rc3/po/sv_SE/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/sv_SE.po` & `duplicity-2.2.4rc3/po/sv_SE.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/tr_TR/duplicity.mo` & `duplicity-2.2.4rc3/po/tr_TR/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/tr_TR.po` & `duplicity-2.2.4rc3/po/tr_TR.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/uk_UA/duplicity.mo` & `duplicity-2.2.4rc3/po/uk_UA/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/uk_UA.po` & `duplicity-2.2.4rc3/po/uk_UA.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/update-pot` & `duplicity-2.2.4rc3/po/update-pot`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/vi_VN.po` & `duplicity-2.2.4rc3/po/vi_VN.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/zh_CN/duplicity.mo` & `duplicity-2.2.4rc3/po/zh_CN/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/zh_CN.po` & `duplicity-2.2.4rc3/po/zh_CN.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/zh_HK/duplicity.mo` & `duplicity-2.2.4rc3/po/zh_HK/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/zh_HK.po` & `duplicity-2.2.4rc3/po/zh_HK.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/zh_MO/duplicity.mo` & `duplicity-2.2.4rc3/po/zh_MO/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/zh_MO.po` & `duplicity-2.2.4rc3/po/zh_MO.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/zh_SG/duplicity.mo` & `duplicity-2.2.4rc3/po/zh_SG/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/zh_SG.po` & `duplicity-2.2.4rc3/po/zh_SG.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/zh_TW/duplicity.mo` & `duplicity-2.2.4rc3/po/zh_TW/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/po/zh_TW.po` & `duplicity-2.2.4rc3/po/zh_TW.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/pyproject.toml` & `duplicity-2.2.4rc3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "duplicity"
-version = "2.2.4rc2"
+version = "2.2.4rc3"
 dynamic = ["dependencies"]
 
 
 [build-system]
 requires = [
     "build>=1.1",
     "pip>=24.0",
```

### Comparing `duplicity-2.2.4rc2/setup.cfg` & `duplicity-2.2.4rc3/setup.cfg`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/setup.py` & `duplicity-2.2.4rc3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 from setuptools.command.build_ext import build_ext
 
 # check that we can function here
 if not ((3, 8) <= sys.version_info[:2] <= (3, 12)):
     print("Sorry, duplicity requires version 3.8 thru 3.12 of Python.")
     sys.exit(1)
 
-Version: str = "2.2.4rc2"
+Version: str = "2.2.4rc3"
 reldate: str = time.strftime("%B %d, %Y", time.gmtime(int(os.environ.get("SOURCE_DATE_EPOCH", time.time()))))
 
 # READTHEDOCS uses setup.py sdist but can't handle extensions
 ext_modules = list()
 incdir_list = list()
 libdir_list = list()
 if os.environ.get("READTHEDOCS", None) is None:
```

### Comparing `duplicity-2.2.4rc2/snap/snapcraft.yaml` & `duplicity-2.2.4rc3/snap/snapcraft.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 name: duplicity
-version: 2.2.4rc2
+version: 2.2.4rc3
 license: GPL-2.0
 summary: Efficient, encrypted backup to local or remote hosts
 description: |
   Duplicity backs directories by producing encrypted tar-format volumes and uploading
   them to a remote or local file server. Because duplicity uses librsync, the incremental
   archives are space efficient and only record the parts of files that have changed since
   the last backup. Because duplicity uses GnuPG to encrypt and/or sign these archives,
```

### Comparing `duplicity-2.2.4rc2/testing/__init__.py` & `duplicity-2.2.4rc3/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/conftest.py` & `duplicity-2.2.4rc3/testing/conftest.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/docker/.env` & `duplicity-2.2.4rc3/testing/docker/.env`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/docker/build.sh` & `duplicity-2.2.4rc3/testing/docker/build.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/docker/docker-compose.yml` & `duplicity-2.2.4rc3/testing/docker/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/docker/duplicity_test/Dockerfile` & `duplicity-2.2.4rc3/testing/docker/duplicity_test/Dockerfile`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/docker/ftp_server/Dockerfile` & `duplicity-2.2.4rc3/testing/docker/ftp_server/Dockerfile`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/docker/hello-world-master.zip` & `duplicity-2.2.4rc3/testing/docker/hello-world-master.zip`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/docker/id_rsa` & `duplicity-2.2.4rc3/testing/docker/id_rsa`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/docker/push.sh` & `duplicity-2.2.4rc3/testing/docker/push.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/docker/setup.sh` & `duplicity-2.2.4rc3/testing/docker/setup.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/docker/ssh_server/Dockerfile` & `duplicity-2.2.4rc3/testing/docker/ssh_server/Dockerfile`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/docker/teardown.sh` & `duplicity-2.2.4rc3/testing/docker/teardown.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/docker/testit.sh` & `duplicity-2.2.4rc3/testing/docker/testit.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/functional/__init__.py` & `duplicity-2.2.4rc3/testing/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/functional/test_badupload.py` & `duplicity-2.2.4rc3/testing/functional/test_badupload.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/functional/test_cleanup.py` & `duplicity-2.2.4rc3/testing/functional/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/functional/test_final.py` & `duplicity-2.2.4rc3/testing/functional/test_final.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/functional/test_log.py` & `duplicity-2.2.4rc3/testing/functional/test_log.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/functional/test_restart.py` & `duplicity-2.2.4rc3/testing/functional/test_restart.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/functional/test_selection.py` & `duplicity-2.2.4rc3/testing/functional/test_selection.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/functional/test_verify.py` & `duplicity-2.2.4rc3/testing/functional/test_verify.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/gnupg/pubring.gpg` & `duplicity-2.2.4rc3/testing/gnupg/pubring.gpg`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/gnupg/secring.gpg` & `duplicity-2.2.4rc3/testing/gnupg/secring.gpg`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/gnupg/trustdb.gpg` & `duplicity-2.2.4rc3/testing/gnupg/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/manual/__init__.py` & `duplicity-2.2.4rc3/testing/manual/__init__.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/manual/auto-ctrl-c-test.sh` & `duplicity-2.2.4rc3/testing/manual/auto-ctrl-c-test.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/manual/backendtest.py` & `duplicity-2.2.4rc3/testing/manual/backendtest.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/manual/manual-ctrl-c-test.sh` & `duplicity-2.2.4rc3/testing/manual/manual-ctrl-c-test.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/manual/rootfiles.tar.gz` & `duplicity-2.2.4rc3/testing/manual/rootfiles.tar.gz`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/manual/roottest.py` & `duplicity-2.2.4rc3/testing/manual/roottest.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/manual/run-coverage.sh` & `duplicity-2.2.4rc3/testing/manual/run-coverage.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/manual/test-venv-install.sh` & `duplicity-2.2.4rc3/testing/manual/test-venv-install.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/manual/test_config.py.tmpl` & `duplicity-2.2.4rc3/testing/manual/test_config.py.tmpl`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/overrides/bin/lftp` & `duplicity-2.2.4rc3/testing/overrides/bin/lftp`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/overrides/bin/ncftpls` & `duplicity-2.2.4rc3/testing/overrides/bin/ncftpls`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/regression/bug1860200.sh` & `duplicity-2.2.4rc3/testing/regression/bug1860200.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/regression/bug487720.sh` & `duplicity-2.2.4rc3/testing/regression/bug487720.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/regression/issue103.sh` & `duplicity-2.2.4rc3/testing/regression/issue103.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/regression/issue110-setup.sh` & `duplicity-2.2.4rc3/testing/regression/issue110-setup.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/regression/issue125.sh` & `duplicity-2.2.4rc3/testing/regression/issue125.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/regression/issue25.sh` & `duplicity-2.2.4rc3/testing/regression/issue25.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/regression/issue725.sh` & `duplicity-2.2.4rc3/testing/regression/issue725.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/regression/issue781.sh` & `duplicity-2.2.4rc3/testing/regression/issue781.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/regression/issue79.sh` & `duplicity-2.2.4rc3/testing/regression/issue79.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/regression/issue98.sh` & `duplicity-2.2.4rc3/testing/regression/issue98.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/run-tests` & `duplicity-2.2.4rc3/testing/run-tests`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/test_code.py` & `duplicity-2.2.4rc3/testing/test_code.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/testfiles.tar.gz` & `duplicity-2.2.4rc3/testing/testfiles.tar.gz`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/unit/__init__.py` & `duplicity-2.2.4rc3/testing/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/unit/test_backend.py` & `duplicity-2.2.4rc3/testing/unit/test_backend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/unit/test_backend_instance.py` & `duplicity-2.2.4rc3/testing/unit/test_backend_instance.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/unit/test_cli_main.py` & `duplicity-2.2.4rc3/testing/unit/test_cli_main.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/unit/test_collections.py` & `duplicity-2.2.4rc3/testing/unit/test_collections.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/unit/test_diffdir.py` & `duplicity-2.2.4rc3/testing/unit/test_diffdir.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/unit/test_dup_temp.py` & `duplicity-2.2.4rc3/testing/unit/test_dup_temp.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/unit/test_dup_time.py` & `duplicity-2.2.4rc3/testing/unit/test_dup_time.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/unit/test_file_naming.py` & `duplicity-2.2.4rc3/testing/unit/test_file_naming.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/unit/test_globmatch.py` & `duplicity-2.2.4rc3/testing/unit/test_globmatch.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/unit/test_gpg.py` & `duplicity-2.2.4rc3/testing/unit/test_gpg.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/unit/test_gpginterface.py` & `duplicity-2.2.4rc3/testing/unit/test_gpginterface.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/unit/test_lazy.py` & `duplicity-2.2.4rc3/testing/unit/test_lazy.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/unit/test_manifest.py` & `duplicity-2.2.4rc3/testing/unit/test_manifest.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/unit/test_patchdir.py` & `duplicity-2.2.4rc3/testing/unit/test_patchdir.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/unit/test_path.py` & `duplicity-2.2.4rc3/testing/unit/test_path.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/unit/test_selection.py` & `duplicity-2.2.4rc3/testing/unit/test_selection.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/unit/test_statistics.py` & `duplicity-2.2.4rc3/testing/unit/test_statistics.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/unit/test_tarfile.py` & `duplicity-2.2.4rc3/testing/unit/test_tarfile.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/unit/test_tempdir.py` & `duplicity-2.2.4rc3/testing/unit/test_tempdir.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/testing/unit/test_util.py` & `duplicity-2.2.4rc3/testing/unit/test_util.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/tools/installpyenv` & `duplicity-2.2.4rc3/tools/installpyenv`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/tools/installpythons` & `duplicity-2.2.4rc3/tools/installpythons`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/tools/installsnap` & `duplicity-2.2.4rc3/tools/installsnap`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/tools/makechangelog` & `duplicity-2.2.4rc3/tools/makechangelog`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/tools/makepip` & `duplicity-2.2.4rc3/tools/makepip`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/tools/makesnap` & `duplicity-2.2.4rc3/tools/makesnap`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/tools/pushpip` & `duplicity-2.2.4rc3/tools/pushpip`

 * *Files 8% similar despite different names*

```diff
@@ -36,8 +36,10 @@
 
 if [ -e "wheelhouse" ]; then
     mv wheelhouse/duplicity-${VERSION}-*.whl dist
     rmdir wheelhouse
 fi
 
 ## upload to pypi
-twine upload --non-interactive dist/duplicity-${VERSION}-*
+for f in dist/duplicity-${VERSION}*; do
+    twine upload --non-interactive $f
+done
```

### Comparing `duplicity-2.2.4rc2/tools/pushsnap` & `duplicity-2.2.4rc3/tools/pushsnap`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/tools/release-prep` & `duplicity-2.2.4rc3/tools/release-prep`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/tools/testpip` & `duplicity-2.2.4rc3/tools/testpip`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/tools/testsnap` & `duplicity-2.2.4rc3/tools/testsnap`

 * *Files identical despite different names*

### Comparing `duplicity-2.2.4rc2/tox.ini` & `duplicity-2.2.4rc3/tox.ini`

 * *Files identical despite different names*

