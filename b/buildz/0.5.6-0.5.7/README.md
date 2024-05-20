# Comparing `tmp/buildz-0.5.6.tar.gz` & `tmp/buildz-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildz-0.5.6.tar", last modified: Thu May 16 08:02:56 2024, max compression
+gzip compressed data, was "buildz-0.5.7.tar", last modified: Mon May 20 16:42:50 2024, max compression
```

## Comparing `buildz-0.5.6.tar` & `buildz-0.5.7.tar`

### file list

```diff
@@ -1,163 +1,164 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:56.824154 buildz-0.5.6/
--rw-rw-rw-   0        0        0    11558 2023-10-16 14:40:02.000000 buildz-0.5.6/LICENSE
--rw-rw-rw-   0        0        0       45 2024-02-27 01:25:41.000000 buildz-0.5.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2823 2024-05-16 08:02:56.824154 buildz-0.5.6/PKG-INFO
--rw-rw-rw-   0        0        0     2342 2024-05-08 03:05:06.000000 buildz-0.5.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:56.398876 buildz-0.5.6/buildz/
--rw-rw-rw-   0        0        0      153 2024-04-16 14:04:54.000000 buildz-0.5.6/buildz/__init__.py
--rw-rw-rw-   0        0        0       90 2024-04-01 15:59:48.000000 buildz-0.5.6/buildz/__main__.py
--rw-rw-rw-   0        0        0     2944 2024-05-07 11:40:11.000000 buildz-0.5.6/buildz/argx.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:56.420628 buildz-0.5.6/buildz/demo/
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:56.420628 buildz-0.5.6/buildz/demo/ioc/
--rw-rw-rw-   0        0        0      548 2024-04-02 17:19:41.000000 buildz-0.5.6/buildz/demo/ioc/deal.py
--rw-rw-rw-   0        0        0     1401 2024-04-02 17:34:58.000000 buildz-0.5.6/buildz/demo/ioc/help.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:56.430138 buildz-0.5.6/buildz/demo/myers/
--rw-rw-rw-   0        0        0     2060 2024-05-03 05:05:39.000000 buildz-0.5.6/buildz/demo/myers/deal.py
--rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.6/buildz/demo/myers/help.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:56.438861 buildz-0.5.6/buildz/demo/res/
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:56.452751 buildz-0.5.6/buildz/demo/res/conf/
--rw-rw-rw-   0        0        0      432 2024-04-01 16:28:22.000000 buildz-0.5.6/buildz/demo/res/conf/ioc.js
--rw-rw-rw-   0        0        0     1930 2024-04-07 16:29:22.000000 buildz-0.5.6/buildz/demo/res/conf/main.js
--rw-rw-rw-   0        0        0      461 2024-04-07 16:06:55.000000 buildz-0.5.6/buildz/demo/res/conf/myers.js
--rw-rw-rw-   0        0        0      466 2024-04-02 16:29:25.000000 buildz-0.5.6/buildz/demo/res/conf/search.js
--rw-rw-rw-   0        0        0      446 2024-04-01 16:28:28.000000 buildz-0.5.6/buildz/demo/res/conf/xf.js
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:56.461963 buildz-0.5.6/buildz/demo/res/help/
--rw-rw-rw-   0        0        0      419 2024-04-07 16:31:32.000000 buildz-0.5.6/buildz/demo/res/help/default.js
--rw-rw-rw-   0        0        0     1117 2024-04-02 17:27:33.000000 buildz-0.5.6/buildz/demo/res/help/ioc.js
--rw-rw-rw-   0        0        0     1234 2024-04-07 18:48:53.000000 buildz-0.5.6/buildz/demo/res/help/myers.js
--rw-rw-rw-   0        0        0      871 2024-04-02 17:27:41.000000 buildz-0.5.6/buildz/demo/res/help/search.js
--rw-rw-rw-   0        0        0     1547 2024-04-02 17:12:29.000000 buildz-0.5.6/buildz/demo/res/help/xf.js
--rw-rw-rw-   0        0        0      572 2024-05-16 07:51:44.000000 buildz-0.5.6/buildz/demo/res/test.js
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:56.461963 buildz-0.5.6/buildz/demo/search/
--rw-rw-rw-   0        0        0      907 2024-04-02 17:19:49.000000 buildz-0.5.6/buildz/demo/search/deal.py
--rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.6/buildz/demo/search/help.py
--rw-rw-rw-   0        0        0     1664 2024-04-02 17:36:05.000000 buildz-0.5.6/buildz/demo/test.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:56.478191 buildz-0.5.6/buildz/demo/xf/
--rw-rw-rw-   0        0        0      368 2024-04-02 17:20:04.000000 buildz-0.5.6/buildz/demo/xf/deal.py
--rw-rw-rw-   0        0        0      502 2024-04-02 17:20:15.000000 buildz-0.5.6/buildz/demo/xf/help.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:56.487423 buildz-0.5.6/buildz/fz/
--rw-rw-rw-   0        0        0      243 2024-05-11 09:00:08.000000 buildz-0.5.6/buildz/fz/__init__.py
--rw-rw-rw-   0        0        0     1387 2024-04-01 14:39:23.000000 buildz-0.5.6/buildz/fz/dirz.py
--rw-rw-rw-   0        0        0      795 2024-05-11 08:59:27.000000 buildz-0.5.6/buildz/fz/fio.py
--rw-rw-rw-   0        0        0     1729 2024-04-02 16:31:56.000000 buildz-0.5.6/buildz/fz/lsf.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:56.493319 buildz-0.5.6/buildz/ioc/
--rw-rw-rw-   0        0        0      124 2024-04-02 15:52:39.000000 buildz-0.5.6/buildz/ioc/__init__.py
--rw-rw-rw-   0        0        0       89 2024-04-25 13:59:49.000000 buildz-0.5.6/buildz/ioc/base.py
--rw-rw-rw-   0        0        0      297 2024-03-31 08:12:36.000000 buildz-0.5.6/buildz/ioc/init.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:56.508525 buildz-0.5.6/buildz/ioc/ioc/
--rw-rw-rw-   0        0        0     2390 2024-04-25 13:41:08.000000 buildz-0.5.6/buildz/ioc/ioc/base.py
--rw-rw-rw-   0        0        0     6918 2024-04-25 16:44:39.000000 buildz-0.5.6/buildz/ioc/ioc/conf.py
--rw-rw-rw-   0        0        0    13518 2024-04-25 16:45:58.000000 buildz-0.5.6/buildz/ioc/ioc/confs.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:56.571609 buildz-0.5.6/buildz/ioc/ioc_deal/
--rw-rw-rw-   0        0        0     5966 2024-04-25 13:56:41.000000 buildz-0.5.6/buildz/ioc/ioc_deal/base.py
--rw-rw-rw-   0        0        0     1465 2024-04-25 13:54:58.000000 buildz-0.5.6/buildz/ioc/ioc_deal/call.py
--rw-rw-rw-   0        0        0     1243 2024-04-25 13:54:58.000000 buildz-0.5.6/buildz/ioc/ioc_deal/calls.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:56.618965 buildz-0.5.6/buildz/ioc/ioc_deal/conf/
--rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.5.6/buildz/ioc/ioc_deal/conf/call_defaults.js
--rw-rw-rw-   0        0        0      416 2024-03-31 09:53:23.000000 buildz-0.5.6/buildz/ioc/ioc_deal/conf/call_lists.js
--rw-rw-rw-   0        0        0       19 2024-04-01 14:21:19.000000 buildz-0.5.6/buildz/ioc/ioc_deal/conf/calls_defaults.js
--rw-rw-rw-   0        0        0      376 2024-04-01 14:21:18.000000 buildz-0.5.6/buildz/ioc/ioc_deal/conf/calls_lists.js
--rw-rw-rw-   0        0        0      412 2024-04-23 19:15:09.000000 buildz-0.5.6/buildz/ioc/ioc_deal/conf/deal_lists.js
--rw-rw-rw-   0        0        0     2341 2024-05-08 19:55:33.000000 buildz-0.5.6/buildz/ioc/ioc_deal/conf/deals.js
--rw-rw-rw-   0        0        0      389 2024-05-08 02:56:58.000000 buildz-0.5.6/buildz/ioc/ioc_deal/conf/env_lists.js
--rw-rw-rw-   0        0        0      444 2024-04-01 11:09:33.000000 buildz-0.5.6/buildz/ioc/ioc_deal/conf/ioc_lists.js
--rw-rw-rw-   0        0        0      421 2024-05-08 19:53:08.000000 buildz-0.5.6/buildz/ioc/ioc_deal/conf/iocf_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.6/buildz/ioc/ioc_deal/conf/join_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.6/buildz/ioc/ioc_deal/conf/list_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:46.000000 buildz-0.5.6/buildz/ioc/ioc_deal/conf/map_lists.js
--rw-rw-rw-   0        0        0       66 2024-04-02 15:18:35.000000 buildz-0.5.6/buildz/ioc/ioc_deal/conf/mcall_defaults.js
--rw-rw-rw-   0        0        0      509 2024-04-02 15:19:12.000000 buildz-0.5.6/buildz/ioc/ioc_deal/conf/mcall_lists.js
--rw-rw-rw-   0        0        0      159 2024-03-31 08:48:51.000000 buildz-0.5.6/buildz/ioc/ioc_deal/conf/obj_cst_lists.js
--rw-rw-rw-   0        0        0      173 2024-04-02 14:50:55.000000 buildz-0.5.6/buildz/ioc/ioc_deal/conf/obj_defaults.js
--rw-rw-rw-   0        0        0      627 2024-04-02 14:51:11.000000 buildz-0.5.6/buildz/ioc/ioc_deal/conf/obj_lists.js
--rw-rw-rw-   0        0        0      113 2024-03-31 08:45:47.000000 buildz-0.5.6/buildz/ioc/ioc_deal/conf/obj_set_lists.js
--rw-rw-rw-   0        0        0      443 2024-04-02 15:23:34.000000 buildz-0.5.6/buildz/ioc/ioc_deal/conf/ovar_lists.js
--rw-rw-rw-   0        0        0      615 2024-05-13 09:04:25.000000 buildz-0.5.6/buildz/ioc/ioc_deal/conf/ref_lists.js
--rw-rw-rw-   0        0        0      351 2024-03-31 10:05:46.000000 buildz-0.5.6/buildz/ioc/ioc_deal/conf/var_lists.js
--rw-rw-rw-   0        0        0        4 2024-04-23 10:50:44.000000 buildz-0.5.6/buildz/ioc/ioc_deal/conf/xfile_defaults.js
--rw-rw-rw-   0        0        0      410 2024-04-23 10:50:04.000000 buildz-0.5.6/buildz/ioc/ioc_deal/conf/xfile_lists.js
--rw-rw-rw-   0        0        0     2713 2024-04-25 13:54:58.000000 buildz-0.5.6/buildz/ioc/ioc_deal/deal.py
--rw-rw-rw-   0        0        0      365 2024-03-31 09:08:35.000000 buildz-0.5.6/buildz/ioc/ioc_deal/demo.py
--rw-rw-rw-   0        0        0     1038 2024-05-06 14:06:01.000000 buildz-0.5.6/buildz/ioc/ioc_deal/env.py
--rw-rw-rw-   0        0        0      954 2024-04-25 13:54:58.000000 buildz-0.5.6/buildz/ioc/ioc_deal/ioc.py
--rw-rw-rw-   0        0        0     1798 2024-05-09 01:32:23.000000 buildz-0.5.6/buildz/ioc/ioc_deal/iocf.py
--rw-rw-rw-   0        0        0      932 2024-05-07 08:29:26.000000 buildz-0.5.6/buildz/ioc/ioc_deal/join.py
--rw-rw-rw-   0        0        0     1090 2024-04-25 13:54:58.000000 buildz-0.5.6/buildz/ioc/ioc_deal/list.py
--rw-rw-rw-   0        0        0     1022 2024-05-13 09:26:45.000000 buildz-0.5.6/buildz/ioc/ioc_deal/map.py
--rw-rw-rw-   0        0        0     1976 2024-04-25 13:54:58.000000 buildz-0.5.6/buildz/ioc/ioc_deal/mcall.py
--rw-rw-rw-   0        0        0     6322 2024-05-15 08:22:26.000000 buildz-0.5.6/buildz/ioc/ioc_deal/obj.py
--rw-rw-rw-   0        0        0     1562 2024-04-25 13:54:58.000000 buildz-0.5.6/buildz/ioc/ioc_deal/ovar.py
--rw-rw-rw-   0        0        0     1255 2024-05-14 03:17:05.000000 buildz-0.5.6/buildz/ioc/ioc_deal/ref.py
--rw-rw-rw-   0        0        0      702 2024-05-13 09:30:29.000000 buildz-0.5.6/buildz/ioc/ioc_deal/val.py
--rw-rw-rw-   0        0        0     1004 2024-04-25 13:54:58.000000 buildz-0.5.6/buildz/ioc/ioc_deal/var.py
--rw-rw-rw-   0        0        0     1174 2024-05-07 08:28:27.000000 buildz-0.5.6/buildz/ioc/ioc_deal/xfile.py
--rw-rw-rw-   0        0        0     2295 2024-05-13 02:27:31.000000 buildz-0.5.6/buildz/pyz.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:56.639345 buildz-0.5.6/buildz/tz/
--rw-rw-rw-   0        0        0      324 2024-04-16 14:03:17.000000 buildz-0.5.6/buildz/tz/__init__.py
--rw-rw-rw-   0        0        0     7543 2024-04-07 19:00:58.000000 buildz-0.5.6/buildz/tz/myers_diff.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:56.666425 buildz-0.5.6/buildz/xf/
--rw-rw-rw-   0        0        0      224 2024-04-25 14:33:04.000000 buildz-0.5.6/buildz/xf/__init__.py
--rw-rw-rw-   0        0        0       86 2024-04-13 11:53:05.000000 buildz-0.5.6/buildz/xf/__main__.py
--rw-rw-rw-   0        0        0     1082 2024-05-13 07:36:04.000000 buildz-0.5.6/buildz/xf/file.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:56.698194 buildz-0.5.6/buildz/xf/loader/
--rw-rw-rw-   0        0        0     1782 2024-04-14 12:14:09.000000 buildz-0.5.6/buildz/xf/loader/base.py
--rw-rw-rw-   0        0        0     3647 2024-04-14 14:34:15.000000 buildz-0.5.6/buildz/xf/loader/buffer.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:56.746322 buildz-0.5.6/buildz/xf/loader/deal/
--rw-rw-rw-   0        0        0      613 2024-02-22 13:04:58.000000 buildz-0.5.6/buildz/xf/loader/deal/listz.py
--rw-rw-rw-   0        0        0     2647 2024-04-14 14:34:45.000000 buildz-0.5.6/buildz/xf/loader/deal/lr.py
--rw-rw-rw-   0        0        0     1583 2024-03-01 16:44:58.000000 buildz-0.5.6/buildz/xf/loader/deal/lrval.py
--rw-rw-rw-   0        0        0      734 2024-02-22 13:18:57.000000 buildz-0.5.6/buildz/xf/loader/deal/mapz.py
--rw-rw-rw-   0        0        0      517 2024-02-22 16:24:13.000000 buildz-0.5.6/buildz/xf/loader/deal/nextz.py
--rw-rw-rw-   0        0        0     1242 2024-04-14 12:03:17.000000 buildz-0.5.6/buildz/xf/loader/deal/reval.py
--rw-rw-rw-   0        0        0     1134 2024-04-14 12:09:59.000000 buildz-0.5.6/buildz/xf/loader/deal/setz.py
--rw-rw-rw-   0        0        0      504 2024-04-14 14:10:33.000000 buildz-0.5.6/buildz/xf/loader/deal/spc.py
--rw-rw-rw-   0        0        0     1358 2024-02-28 03:19:27.000000 buildz-0.5.6/buildz/xf/loader/deal/spt.py
--rw-rw-rw-   0        0        0     3180 2024-04-14 14:16:55.000000 buildz-0.5.6/buildz/xf/loader/deal/strz.py
--rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.6/buildz/xf/loader/exp.py
--rw-rw-rw-   0        0        0     1490 2024-04-12 12:01:04.000000 buildz-0.5.6/buildz/xf/loader/item.py
--rw-rw-rw-   0        0        0     2502 2024-04-16 13:18:40.000000 buildz-0.5.6/buildz/xf/loader/mg.py
--rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.6/buildz/xf/loader/pos.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:56.770756 buildz-0.5.6/buildz/xf/loaderz/
--rw-rw-rw-   0        0        0      746 2024-04-26 07:15:39.000000 buildz-0.5.6/buildz/xf/loaderz/base.py
--rw-rw-rw-   0        0        0     3126 2024-04-16 13:11:00.000000 buildz-0.5.6/buildz/xf/loaderz/buffer.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:56.792898 buildz-0.5.6/buildz/xf/loaderz/deal/
--rw-rw-rw-   0        0        0      963 2024-04-26 07:40:02.000000 buildz-0.5.6/buildz/xf/loaderz/deal/listz.py
--rw-rw-rw-   0        0        0     2056 2024-05-16 07:51:17.000000 buildz-0.5.6/buildz/xf/loaderz/deal/lr.py
--rw-rw-rw-   0        0        0     1156 2024-05-16 07:57:06.000000 buildz-0.5.6/buildz/xf/loaderz/deal/lrval.py
--rw-rw-rw-   0        0        0     1143 2024-04-26 07:39:58.000000 buildz-0.5.6/buildz/xf/loaderz/deal/mapz.py
--rw-rw-rw-   0        0        0      740 2024-04-26 07:40:46.000000 buildz-0.5.6/buildz/xf/loaderz/deal/nextz.py
--rw-rw-rw-   0        0        0      781 2024-04-26 07:04:45.000000 buildz-0.5.6/buildz/xf/loaderz/deal/reval.py
--rw-rw-rw-   0        0        0      287 2024-04-16 10:07:28.000000 buildz-0.5.6/buildz/xf/loaderz/deal/setz.py
--rw-rw-rw-   0        0        0      418 2024-04-25 17:42:03.000000 buildz-0.5.6/buildz/xf/loaderz/deal/spc.py
--rw-rw-rw-   0        0        0     1147 2024-04-16 12:27:46.000000 buildz-0.5.6/buildz/xf/loaderz/deal/spt.py
--rw-rw-rw-   0        0        0     3295 2024-05-14 07:15:35.000000 buildz-0.5.6/buildz/xf/loaderz/deal/strz.py
--rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.6/buildz/xf/loaderz/exp.py
--rw-rw-rw-   0        0        0     1911 2024-04-16 10:34:17.000000 buildz-0.5.6/buildz/xf/loaderz/item.py
--rw-rw-rw-   0        0        0     3517 2024-05-14 07:12:19.000000 buildz-0.5.6/buildz/xf/loaderz/mg.py
--rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.6/buildz/xf/loaderz/pos.py
--rw-rw-rw-   0        0        0     1753 2024-04-26 07:24:25.000000 buildz-0.5.6/buildz/xf/loaderz/test.py
--rw-rw-rw-   0        0        0       97 2024-04-26 07:42:38.000000 buildz-0.5.6/buildz/xf/loaderz/test1.py
--rw-rw-rw-   0        0        0     2940 2024-05-15 09:18:22.000000 buildz-0.5.6/buildz/xf/mapz.py
--rw-rw-rw-   0        0        0     2587 2024-04-16 13:17:27.000000 buildz-0.5.6/buildz/xf/read.py
--rw-rw-rw-   0        0        0     2746 2024-05-07 11:58:30.000000 buildz-0.5.6/buildz/xf/readz.py
--rw-rw-rw-   0        0        0     1999 2024-04-15 04:06:48.000000 buildz-0.5.6/buildz/xf/stack.py
--rw-rw-rw-   0        0        0     1477 2024-05-07 11:34:30.000000 buildz-0.5.6/buildz/xf/write.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:56.808530 buildz-0.5.6/buildz/xf/writer/
--rw-rw-rw-   0        0        0     1108 2024-02-23 14:38:49.000000 buildz-0.5.6/buildz/xf/writer/base.py
--rw-rw-rw-   0        0        0     1519 2024-02-23 14:41:57.000000 buildz-0.5.6/buildz/xf/writer/conf.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:56.808530 buildz-0.5.6/buildz/xf/writer/deal/
--rw-rw-rw-   0        0        0      461 2024-02-24 09:45:45.000000 buildz-0.5.6/buildz/xf/writer/deal/jsonval.py
--rw-rw-rw-   0        0        0     1105 2024-02-24 09:40:04.000000 buildz-0.5.6/buildz/xf/writer/deal/listz.py
--rw-rw-rw-   0        0        0     1252 2024-02-24 09:40:12.000000 buildz-0.5.6/buildz/xf/writer/deal/mapz.py
--rw-rw-rw-   0        0        0      504 2024-02-24 09:41:59.000000 buildz-0.5.6/buildz/xf/writer/deal/reval.py
--rw-rw-rw-   0        0        0     1429 2024-04-07 12:04:50.000000 buildz-0.5.6/buildz/xf/writer/deal/strz.py
--rw-rw-rw-   0        0        0     1152 2024-02-23 09:09:41.000000 buildz-0.5.6/buildz/xf/writer/itemz.py
--rw-rw-rw-   0        0        0     2038 2024-02-24 09:36:48.000000 buildz-0.5.6/buildz/xf/writer/mg.py
--rw-rw-rw-   0        0        0      597 2024-04-13 11:53:25.000000 buildz-0.5.6/buildz/xf/xargs.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:56.414106 buildz-0.5.6/buildz.egg-info/
--rw-rw-rw-   0        0        0     2823 2024-05-16 08:02:56.000000 buildz-0.5.6/buildz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3818 2024-05-16 08:02:56.000000 buildz-0.5.6/buildz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 08:02:56.000000 buildz-0.5.6/buildz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-16 08:02:56.000000 buildz-0.5.6/buildz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 08:02:56.824154 buildz-0.5.6/setup.cfg
--rw-rw-rw-   0        0        0      836 2024-05-16 07:58:46.000000 buildz-0.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:42:50.193680 buildz-0.5.7/
+-rw-rw-rw-   0        0        0    11558 2023-10-16 14:40:02.000000 buildz-0.5.7/LICENSE
+-rw-rw-rw-   0        0        0       45 2024-02-27 01:25:41.000000 buildz-0.5.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2823 2024-05-20 16:42:50.193680 buildz-0.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2342 2024-05-08 03:05:06.000000 buildz-0.5.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.535085 buildz-0.5.7/buildz/
+-rw-rw-rw-   0        0        0      153 2024-04-16 14:04:54.000000 buildz-0.5.7/buildz/__init__.py
+-rw-rw-rw-   0        0        0       90 2024-04-01 15:59:48.000000 buildz-0.5.7/buildz/__main__.py
+-rw-rw-rw-   0        0        0     2944 2024-05-07 11:40:11.000000 buildz-0.5.7/buildz/argx.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.546087 buildz-0.5.7/buildz/demo/
+drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.553416 buildz-0.5.7/buildz/demo/ioc/
+-rw-rw-rw-   0        0        0      548 2024-04-02 17:19:41.000000 buildz-0.5.7/buildz/demo/ioc/deal.py
+-rw-rw-rw-   0        0        0     1401 2024-04-02 17:34:58.000000 buildz-0.5.7/buildz/demo/ioc/help.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.562518 buildz-0.5.7/buildz/demo/myers/
+-rw-rw-rw-   0        0        0     2060 2024-05-03 05:05:39.000000 buildz-0.5.7/buildz/demo/myers/deal.py
+-rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.7/buildz/demo/myers/help.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.562518 buildz-0.5.7/buildz/demo/res/
+drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.593651 buildz-0.5.7/buildz/demo/res/conf/
+-rw-rw-rw-   0        0        0      432 2024-04-01 16:28:22.000000 buildz-0.5.7/buildz/demo/res/conf/ioc.js
+-rw-rw-rw-   0        0        0     1930 2024-04-07 16:29:22.000000 buildz-0.5.7/buildz/demo/res/conf/main.js
+-rw-rw-rw-   0        0        0      461 2024-04-07 16:06:55.000000 buildz-0.5.7/buildz/demo/res/conf/myers.js
+-rw-rw-rw-   0        0        0      466 2024-04-02 16:29:25.000000 buildz-0.5.7/buildz/demo/res/conf/search.js
+-rw-rw-rw-   0        0        0      446 2024-04-01 16:28:28.000000 buildz-0.5.7/buildz/demo/res/conf/xf.js
+drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.625147 buildz-0.5.7/buildz/demo/res/help/
+-rw-rw-rw-   0        0        0      419 2024-04-07 16:31:32.000000 buildz-0.5.7/buildz/demo/res/help/default.js
+-rw-rw-rw-   0        0        0     1117 2024-04-02 17:27:33.000000 buildz-0.5.7/buildz/demo/res/help/ioc.js
+-rw-rw-rw-   0        0        0     1234 2024-04-07 18:48:53.000000 buildz-0.5.7/buildz/demo/res/help/myers.js
+-rw-rw-rw-   0        0        0      871 2024-04-02 17:27:41.000000 buildz-0.5.7/buildz/demo/res/help/search.js
+-rw-rw-rw-   0        0        0     1547 2024-04-02 17:12:29.000000 buildz-0.5.7/buildz/demo/res/help/xf.js
+-rw-rw-rw-   0        0        0      572 2024-05-16 07:51:44.000000 buildz-0.5.7/buildz/demo/res/test.js
+drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.635345 buildz-0.5.7/buildz/demo/search/
+-rw-rw-rw-   0        0        0      907 2024-04-02 17:19:49.000000 buildz-0.5.7/buildz/demo/search/deal.py
+-rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.7/buildz/demo/search/help.py
+-rw-rw-rw-   0        0        0     1664 2024-04-02 17:36:05.000000 buildz-0.5.7/buildz/demo/test.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.640932 buildz-0.5.7/buildz/demo/xf/
+-rw-rw-rw-   0        0        0      368 2024-04-02 17:20:04.000000 buildz-0.5.7/buildz/demo/xf/deal.py
+-rw-rw-rw-   0        0        0      502 2024-04-02 17:20:15.000000 buildz-0.5.7/buildz/demo/xf/help.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.650139 buildz-0.5.7/buildz/fz/
+-rw-rw-rw-   0        0        0      285 2024-05-20 14:01:14.000000 buildz-0.5.7/buildz/fz/__init__.py
+-rw-rw-rw-   0        0        0     2293 2024-05-20 08:56:56.000000 buildz-0.5.7/buildz/fz/dirz.py
+-rw-rw-rw-   0        0        0      959 2024-05-20 09:16:37.000000 buildz-0.5.7/buildz/fz/fio.py
+-rw-rw-rw-   0        0        0     3425 2024-05-20 14:01:07.000000 buildz-0.5.7/buildz/fz/lsf.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.656891 buildz-0.5.7/buildz/ioc/
+-rw-rw-rw-   0        0        0      124 2024-04-02 15:52:39.000000 buildz-0.5.7/buildz/ioc/__init__.py
+-rw-rw-rw-   0        0        0      121 2024-05-16 11:49:03.000000 buildz-0.5.7/buildz/ioc/base.py
+-rw-rw-rw-   0        0        0      297 2024-03-31 08:12:36.000000 buildz-0.5.7/buildz/ioc/init.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.674153 buildz-0.5.7/buildz/ioc/ioc/
+-rw-rw-rw-   0        0        0     2554 2024-05-16 14:21:57.000000 buildz-0.5.7/buildz/ioc/ioc/base.py
+-rw-rw-rw-   0        0        0     6918 2024-04-25 16:44:39.000000 buildz-0.5.7/buildz/ioc/ioc/conf.py
+-rw-rw-rw-   0        0        0    13518 2024-04-25 16:45:58.000000 buildz-0.5.7/buildz/ioc/ioc/confs.py
+-rw-rw-rw-   0        0        0     1521 2024-05-16 15:35:31.000000 buildz-0.5.7/buildz/ioc/ioc/single.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.752259 buildz-0.5.7/buildz/ioc/ioc_deal/
+-rw-rw-rw-   0        0        0     5966 2024-04-25 13:56:41.000000 buildz-0.5.7/buildz/ioc/ioc_deal/base.py
+-rw-rw-rw-   0        0        0     1465 2024-04-25 13:54:58.000000 buildz-0.5.7/buildz/ioc/ioc_deal/call.py
+-rw-rw-rw-   0        0        0     1255 2024-05-16 14:17:26.000000 buildz-0.5.7/buildz/ioc/ioc_deal/calls.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.942593 buildz-0.5.7/buildz/ioc/ioc_deal/conf/
+-rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/call_defaults.js
+-rw-rw-rw-   0        0        0      416 2024-03-31 09:53:23.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/call_lists.js
+-rw-rw-rw-   0        0        0       19 2024-04-01 14:21:19.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/calls_defaults.js
+-rw-rw-rw-   0        0        0      376 2024-04-01 14:21:18.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/calls_lists.js
+-rw-rw-rw-   0        0        0      412 2024-04-23 19:15:09.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/deal_lists.js
+-rw-rw-rw-   0        0        0     2341 2024-05-08 19:55:33.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/deals.js
+-rw-rw-rw-   0        0        0      389 2024-05-08 02:56:58.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/env_lists.js
+-rw-rw-rw-   0        0        0      444 2024-04-01 11:09:33.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/ioc_lists.js
+-rw-rw-rw-   0        0        0      421 2024-05-08 19:53:08.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/iocf_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/join_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/list_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:46.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/map_lists.js
+-rw-rw-rw-   0        0        0       66 2024-04-02 15:18:35.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/mcall_defaults.js
+-rw-rw-rw-   0        0        0      509 2024-04-02 15:19:12.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/mcall_lists.js
+-rw-rw-rw-   0        0        0      159 2024-03-31 08:48:51.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/obj_cst_lists.js
+-rw-rw-rw-   0        0        0      173 2024-04-02 14:50:55.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/obj_defaults.js
+-rw-rw-rw-   0        0        0      627 2024-04-02 14:51:11.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/obj_lists.js
+-rw-rw-rw-   0        0        0      113 2024-03-31 08:45:47.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/obj_set_lists.js
+-rw-rw-rw-   0        0        0      443 2024-04-02 15:23:34.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/ovar_lists.js
+-rw-rw-rw-   0        0        0      615 2024-05-13 09:04:25.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/ref_lists.js
+-rw-rw-rw-   0        0        0      351 2024-03-31 10:05:46.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/var_lists.js
+-rw-rw-rw-   0        0        0        4 2024-04-23 10:50:44.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/xfile_defaults.js
+-rw-rw-rw-   0        0        0      410 2024-04-23 10:50:04.000000 buildz-0.5.7/buildz/ioc/ioc_deal/conf/xfile_lists.js
+-rw-rw-rw-   0        0        0     2713 2024-04-25 13:54:58.000000 buildz-0.5.7/buildz/ioc/ioc_deal/deal.py
+-rw-rw-rw-   0        0        0      365 2024-03-31 09:08:35.000000 buildz-0.5.7/buildz/ioc/ioc_deal/demo.py
+-rw-rw-rw-   0        0        0     1059 2024-05-16 14:13:56.000000 buildz-0.5.7/buildz/ioc/ioc_deal/env.py
+-rw-rw-rw-   0        0        0      975 2024-05-16 14:13:36.000000 buildz-0.5.7/buildz/ioc/ioc_deal/ioc.py
+-rw-rw-rw-   0        0        0     1798 2024-05-09 01:32:23.000000 buildz-0.5.7/buildz/ioc/ioc_deal/iocf.py
+-rw-rw-rw-   0        0        0      944 2024-05-16 14:13:13.000000 buildz-0.5.7/buildz/ioc/ioc_deal/join.py
+-rw-rw-rw-   0        0        0     1102 2024-05-16 14:12:34.000000 buildz-0.5.7/buildz/ioc/ioc_deal/list.py
+-rw-rw-rw-   0        0        0     1033 2024-05-16 14:17:05.000000 buildz-0.5.7/buildz/ioc/ioc_deal/map.py
+-rw-rw-rw-   0        0        0     1976 2024-04-25 13:54:58.000000 buildz-0.5.7/buildz/ioc/ioc_deal/mcall.py
+-rw-rw-rw-   0        0        0     6546 2024-05-16 15:31:49.000000 buildz-0.5.7/buildz/ioc/ioc_deal/obj.py
+-rw-rw-rw-   0        0        0     1562 2024-04-25 13:54:58.000000 buildz-0.5.7/buildz/ioc/ioc_deal/ovar.py
+-rw-rw-rw-   0        0        0     1276 2024-05-16 14:15:31.000000 buildz-0.5.7/buildz/ioc/ioc_deal/ref.py
+-rw-rw-rw-   0        0        0      744 2024-05-16 14:45:17.000000 buildz-0.5.7/buildz/ioc/ioc_deal/val.py
+-rw-rw-rw-   0        0        0     1004 2024-04-25 13:54:58.000000 buildz-0.5.7/buildz/ioc/ioc_deal/var.py
+-rw-rw-rw-   0        0        0     1174 2024-05-07 08:28:27.000000 buildz-0.5.7/buildz/ioc/ioc_deal/xfile.py
+-rw-rw-rw-   0        0        0     2295 2024-05-16 11:50:23.000000 buildz-0.5.7/buildz/pyz.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.944244 buildz-0.5.7/buildz/tz/
+-rw-rw-rw-   0        0        0      324 2024-04-16 14:03:17.000000 buildz-0.5.7/buildz/tz/__init__.py
+-rw-rw-rw-   0        0        0     7543 2024-04-07 19:00:58.000000 buildz-0.5.7/buildz/tz/myers_diff.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.978280 buildz-0.5.7/buildz/xf/
+-rw-rw-rw-   0        0        0      224 2024-04-25 14:33:04.000000 buildz-0.5.7/buildz/xf/__init__.py
+-rw-rw-rw-   0        0        0       86 2024-04-13 11:53:05.000000 buildz-0.5.7/buildz/xf/__main__.py
+-rw-rw-rw-   0        0        0     1082 2024-05-13 07:36:04.000000 buildz-0.5.7/buildz/xf/file.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:42:50.006118 buildz-0.5.7/buildz/xf/loader/
+-rw-rw-rw-   0        0        0     1782 2024-04-14 12:14:09.000000 buildz-0.5.7/buildz/xf/loader/base.py
+-rw-rw-rw-   0        0        0     3647 2024-04-14 14:34:15.000000 buildz-0.5.7/buildz/xf/loader/buffer.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:42:50.068699 buildz-0.5.7/buildz/xf/loader/deal/
+-rw-rw-rw-   0        0        0      613 2024-02-22 13:04:58.000000 buildz-0.5.7/buildz/xf/loader/deal/listz.py
+-rw-rw-rw-   0        0        0     2647 2024-04-14 14:34:45.000000 buildz-0.5.7/buildz/xf/loader/deal/lr.py
+-rw-rw-rw-   0        0        0     1583 2024-03-01 16:44:58.000000 buildz-0.5.7/buildz/xf/loader/deal/lrval.py
+-rw-rw-rw-   0        0        0      734 2024-02-22 13:18:57.000000 buildz-0.5.7/buildz/xf/loader/deal/mapz.py
+-rw-rw-rw-   0        0        0      517 2024-02-22 16:24:13.000000 buildz-0.5.7/buildz/xf/loader/deal/nextz.py
+-rw-rw-rw-   0        0        0     1242 2024-04-14 12:03:17.000000 buildz-0.5.7/buildz/xf/loader/deal/reval.py
+-rw-rw-rw-   0        0        0     1134 2024-04-14 12:09:59.000000 buildz-0.5.7/buildz/xf/loader/deal/setz.py
+-rw-rw-rw-   0        0        0      504 2024-04-14 14:10:33.000000 buildz-0.5.7/buildz/xf/loader/deal/spc.py
+-rw-rw-rw-   0        0        0     1358 2024-02-28 03:19:27.000000 buildz-0.5.7/buildz/xf/loader/deal/spt.py
+-rw-rw-rw-   0        0        0     3180 2024-04-14 14:16:55.000000 buildz-0.5.7/buildz/xf/loader/deal/strz.py
+-rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.7/buildz/xf/loader/exp.py
+-rw-rw-rw-   0        0        0     1490 2024-04-12 12:01:04.000000 buildz-0.5.7/buildz/xf/loader/item.py
+-rw-rw-rw-   0        0        0     2502 2024-04-16 13:18:40.000000 buildz-0.5.7/buildz/xf/loader/mg.py
+-rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.7/buildz/xf/loader/pos.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:42:50.099973 buildz-0.5.7/buildz/xf/loaderz/
+-rw-rw-rw-   0        0        0      746 2024-04-26 07:15:39.000000 buildz-0.5.7/buildz/xf/loaderz/base.py
+-rw-rw-rw-   0        0        0     3126 2024-04-16 13:11:00.000000 buildz-0.5.7/buildz/xf/loaderz/buffer.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:42:50.146745 buildz-0.5.7/buildz/xf/loaderz/deal/
+-rw-rw-rw-   0        0        0      963 2024-04-26 07:40:02.000000 buildz-0.5.7/buildz/xf/loaderz/deal/listz.py
+-rw-rw-rw-   0        0        0     2056 2024-05-16 07:51:17.000000 buildz-0.5.7/buildz/xf/loaderz/deal/lr.py
+-rw-rw-rw-   0        0        0     1156 2024-05-16 07:57:06.000000 buildz-0.5.7/buildz/xf/loaderz/deal/lrval.py
+-rw-rw-rw-   0        0        0     1143 2024-04-26 07:39:58.000000 buildz-0.5.7/buildz/xf/loaderz/deal/mapz.py
+-rw-rw-rw-   0        0        0      740 2024-04-26 07:40:46.000000 buildz-0.5.7/buildz/xf/loaderz/deal/nextz.py
+-rw-rw-rw-   0        0        0      781 2024-04-26 07:04:45.000000 buildz-0.5.7/buildz/xf/loaderz/deal/reval.py
+-rw-rw-rw-   0        0        0      287 2024-04-16 10:07:28.000000 buildz-0.5.7/buildz/xf/loaderz/deal/setz.py
+-rw-rw-rw-   0        0        0      418 2024-04-25 17:42:03.000000 buildz-0.5.7/buildz/xf/loaderz/deal/spc.py
+-rw-rw-rw-   0        0        0     1147 2024-04-16 12:27:46.000000 buildz-0.5.7/buildz/xf/loaderz/deal/spt.py
+-rw-rw-rw-   0        0        0     3295 2024-05-14 07:15:35.000000 buildz-0.5.7/buildz/xf/loaderz/deal/strz.py
+-rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.7/buildz/xf/loaderz/exp.py
+-rw-rw-rw-   0        0        0     1911 2024-04-16 10:34:17.000000 buildz-0.5.7/buildz/xf/loaderz/item.py
+-rw-rw-rw-   0        0        0     3517 2024-05-14 07:12:19.000000 buildz-0.5.7/buildz/xf/loaderz/mg.py
+-rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.7/buildz/xf/loaderz/pos.py
+-rw-rw-rw-   0        0        0     1753 2024-04-26 07:24:25.000000 buildz-0.5.7/buildz/xf/loaderz/test.py
+-rw-rw-rw-   0        0        0       97 2024-04-26 07:42:38.000000 buildz-0.5.7/buildz/xf/loaderz/test1.py
+-rw-rw-rw-   0        0        0     3379 2024-05-16 14:12:15.000000 buildz-0.5.7/buildz/xf/mapz.py
+-rw-rw-rw-   0        0        0     2587 2024-04-16 13:17:27.000000 buildz-0.5.7/buildz/xf/read.py
+-rw-rw-rw-   0        0        0     2746 2024-05-07 11:58:30.000000 buildz-0.5.7/buildz/xf/readz.py
+-rw-rw-rw-   0        0        0     1999 2024-04-15 04:06:48.000000 buildz-0.5.7/buildz/xf/stack.py
+-rw-rw-rw-   0        0        0     1477 2024-05-07 11:34:30.000000 buildz-0.5.7/buildz/xf/write.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:42:50.162439 buildz-0.5.7/buildz/xf/writer/
+-rw-rw-rw-   0        0        0     1108 2024-02-23 14:38:49.000000 buildz-0.5.7/buildz/xf/writer/base.py
+-rw-rw-rw-   0        0        0     1519 2024-02-23 14:41:57.000000 buildz-0.5.7/buildz/xf/writer/conf.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:42:50.178068 buildz-0.5.7/buildz/xf/writer/deal/
+-rw-rw-rw-   0        0        0      461 2024-02-24 09:45:45.000000 buildz-0.5.7/buildz/xf/writer/deal/jsonval.py
+-rw-rw-rw-   0        0        0     1105 2024-02-24 09:40:04.000000 buildz-0.5.7/buildz/xf/writer/deal/listz.py
+-rw-rw-rw-   0        0        0     1252 2024-02-24 09:40:12.000000 buildz-0.5.7/buildz/xf/writer/deal/mapz.py
+-rw-rw-rw-   0        0        0      504 2024-02-24 09:41:59.000000 buildz-0.5.7/buildz/xf/writer/deal/reval.py
+-rw-rw-rw-   0        0        0     1429 2024-04-07 12:04:50.000000 buildz-0.5.7/buildz/xf/writer/deal/strz.py
+-rw-rw-rw-   0        0        0     1152 2024-02-23 09:09:41.000000 buildz-0.5.7/buildz/xf/writer/itemz.py
+-rw-rw-rw-   0        0        0     2038 2024-02-24 09:36:48.000000 buildz-0.5.7/buildz/xf/writer/mg.py
+-rw-rw-rw-   0        0        0      597 2024-04-13 11:53:25.000000 buildz-0.5.7/buildz/xf/xargs.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:42:49.535085 buildz-0.5.7/buildz.egg-info/
+-rw-rw-rw-   0        0        0     2823 2024-05-20 16:42:49.000000 buildz-0.5.7/buildz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3843 2024-05-20 16:42:49.000000 buildz-0.5.7/buildz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 16:42:49.000000 buildz-0.5.7/buildz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-20 16:42:49.000000 buildz-0.5.7/buildz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 16:42:50.193680 buildz-0.5.7/setup.cfg
+-rw-rw-rw-   0        0        0      836 2024-05-20 16:41:30.000000 buildz-0.5.7/setup.py
```

### Comparing `buildz-0.5.6/LICENSE` & `buildz-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/PKG-INFO` & `buildz-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.5.6
+Version: 0.5.7
 Summary: 配置读写（基于json格式进行简化），以及ioc。a json-base file format's read and write code by python, and codes to read and product object from configure file in such format(ioc)
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
```

### Comparing `buildz-0.5.6/README.md` & `buildz-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/argx.py` & `buildz-0.5.7/buildz/argx.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/demo/ioc/deal.py` & `buildz-0.5.7/buildz/demo/ioc/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/demo/ioc/help.py` & `buildz-0.5.7/buildz/demo/ioc/help.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/demo/myers/deal.py` & `buildz-0.5.7/buildz/demo/myers/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/demo/res/conf/main.js` & `buildz-0.5.7/buildz/demo/res/conf/main.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/demo/res/help/ioc.js` & `buildz-0.5.7/buildz/demo/res/help/ioc.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/demo/res/help/myers.js` & `buildz-0.5.7/buildz/demo/res/help/myers.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/demo/res/help/search.js` & `buildz-0.5.7/buildz/demo/res/help/search.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/demo/res/help/xf.js` & `buildz-0.5.7/buildz/demo/res/help/xf.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/demo/res/test.js` & `buildz-0.5.7/buildz/demo/res/test.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/demo/search/deal.py` & `buildz-0.5.7/buildz/demo/search/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/demo/test.py` & `buildz-0.5.7/buildz/demo/test.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/fz/fio.py` & `buildz-0.5.7/buildz/fz/fio.py`

 * *Files 27% similar despite different names*

```diff
@@ -30,16 +30,27 @@
     with open(fp, mode) as f:
         for ct in cts:
             f.write(ct)
 
 pass
 writes = fwrites
 
-def makefdir(fp):
-    fp = os.path.abspath(fp)
-    dp = os.path.dirname(fp)
+def makedir(dp):
     if os.path.isdir(dp):
         return
     os.makedirs(dp)
 
 pass
+def makefdir(fp):
+    fp = os.path.abspath(fp)
+    dp = os.path.dirname(fp)
+    makedir(dp)
+
+pass
 
+def dirpath(fp, n=1):
+    for i in range(n):
+        fp = os.path.dirname(fp)
+    return fp
+
+pass
+dirname = dirpath
```

### Comparing `buildz-0.5.6/buildz/ioc/ioc/base.py` & `buildz-0.5.7/buildz/ioc/ioc/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,25 +33,29 @@
             conf: 配置数据对应的配置文件的管理器
             local: 是否是locals的数据（配置文件局部数据）
             type: 配置数据的type字段
             src: 源对象，配置数据生成的对象调用conf获取对象，会有这个字段，目前只有object会放这个字段，其他要么透传要么不传
             info: 额外的调用信息，目前只有object会用到里面的id字段，作为单例额外输入
         """
         if typez(data)==dict:
-            pid = xf.g(data, parent=None)
+            pid = xf.g1(data, parent=None)
             if pid is not None:
-                pedt = conf.get_data(pid, local=True, search_confs = True,src = src, info = info)
-                if pedt is None:
-                    raise IOCError("unfind parend: "+pid)
-                pdt = pedt.data
-                if typez(pdt)!=dict:
-                    raise IOCError("only dict can be a parent: "+pid)
                 data = dict(data)
-                self.update_maps(data, pdt, replace=0)
                 del data['parent']
+                pids = pid
+                if typez(pids)!=list:
+                    pids = [pid]
+                for pid in pids:
+                    pedt = conf.get_data(pid, local=True, search_confs = True,src = src, info = info)
+                    if pedt is None:
+                        raise IOCError("unfind parend: "+pid)
+                    pdt = pedt.data
+                    if typez(pdt)!=dict:
+                        raise IOCError("only dict can be a parent: "+pid)
+                    self.update_maps(data, pdt, replace=0)
         self.data = data
         self.sid = conf.id
         self.src = src
         self.conf = conf
         self.confs = conf.confs
         self.local = local
         if type is None:
```

### Comparing `buildz-0.5.6/buildz/ioc/ioc/conf.py` & `buildz-0.5.7/buildz/ioc/ioc/conf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/ioc/ioc/confs.py` & `buildz-0.5.7/buildz/ioc/ioc/confs.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/ioc/ioc_deal/base.py` & `buildz-0.5.7/buildz/ioc/ioc_deal/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/ioc/ioc_deal/call.py` & `buildz-0.5.7/buildz/ioc/ioc_deal/call.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/ioc/ioc_deal/calls.py` & `buildz-0.5.7/buildz/ioc/ioc_deal/calls.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,14 @@
             join(dp, "conf", "calls_defaults.js"))
     def deal(self, edata:EncapeData):
         sid = edata.sid
         data = edata.data
         conf = edata.conf
         data = self.format(data)
         src = edata.src
-        calls = xf.g(data, calls=[])
+        calls = xf.g1(data, calls=[], data = [])
         rst = None
         for call in calls:
             rst = self.get_obj(call, conf, src)
         return rst
 
 pass
```

### Comparing `buildz-0.5.6/buildz/ioc/ioc_deal/conf/deals.js` & `buildz-0.5.7/buildz/ioc/ioc_deal/conf/deals.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/ioc/ioc_deal/conf/obj_lists.js` & `buildz-0.5.7/buildz/ioc/ioc_deal/conf/obj_lists.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/ioc/ioc_deal/conf/ref_lists.js` & `buildz-0.5.7/buildz/ioc/ioc_deal/conf/ref_lists.js`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/ioc/ioc_deal/deal.py` & `buildz-0.5.7/buildz/ioc/ioc_deal/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/ioc/ioc_deal/env.py` & `buildz-0.5.7/buildz/ioc/ioc_deal/env.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             [env, path] //读取环境变量path
     """
     def init(self, fp_lists=None, fp_defaults=None):
         super().init("EnvDeal", fp_lists, fp_defaults, join(dp, "conf", "env_lists.js"), None)
     def deal(self, edata:EncapeData):
         data = edata.data
         data = self.fill(data)
-        key = data['key']
+        key = xf.get_first(data, 'env', 'key')
         val = edata.conf.get_env(key)
         default = xf.g(data, default=None)
         if val is None and default is not None:
             val = self.get_obj(default, edata.conf)
         return val
 
 pass
```

### Comparing `buildz-0.5.6/buildz/ioc/ioc_deal/ioc.py` & `buildz-0.5.7/buildz/ioc/ioc_deal/ioc.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,13 +21,13 @@
             [ioc, conf] //返回ioc内部数据的conf字段
     """
     def init(self, fp_lists=None, fp_defaults=None):
         super().init("IOCObjectDeal", fp_lists, fp_defaults, join(dp, "conf", "ioc_lists.js"), None)
     def deal(self, edata:EncapeData):
         data = edata.data
         data = self.fill(data)
-        key = data['key']
+        key = xf.get_first(data, 'ioc', 'key')
         if not hasattr(edata, key):
             return None
         return getattr(edata, key)
 
 pass
```

### Comparing `buildz-0.5.6/buildz/ioc/ioc_deal/iocf.py` & `buildz-0.5.7/buildz/ioc/ioc_deal/iocf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/ioc/ioc_deal/join.py` & `buildz-0.5.7/buildz/ioc/ioc_deal/join.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,13 +20,13 @@
         [join, [[val, home], [val, buildz]]] //返回字符串 "home/buildz"
     """
     def init(self, fp_lists=None, fp_defaults=None):
         super().init("JoinDeal", fp_lists, fp_defaults, join(dp, "conf", "join_lists.js"), None)
     def deal(self, edata:EncapeData):
         data = edata.data
         data = self.fill(data)
-        lists = xf.g(data, data=[])
+        lists = xf.g1(data, join = [], data=[])
         conf = edata.conf
         rst = [self.get_obj(k, conf, edata.src, edata.info) for k in lists]
         return join(*rst)
 
 pass
```

### Comparing `buildz-0.5.6/buildz/ioc/ioc_deal/list.py` & `buildz-0.5.7/buildz/ioc/ioc_deal/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,13 +23,13 @@
             [list, [[ref, obj.test], [env, path]]] // 返回列表,第0个元素是对数据obj.test的索引，第二个是环境变量path的值
     """
     def init(self, fp_lists=None, fp_defaults=None):
         super().init("ListDeal", fp_lists, fp_defaults, join(dp, "conf", "list_lists.js"), None)
     def deal(self, edata:EncapeData):
         data = edata.data
         data = self.fill(data)
-        lists = xf.g(data, data=[])
+        lists = xf.g1(data, list = [], data=[])
         conf = edata.conf
         rst = [self.get_obj(k, conf, edata.src, edata.info) for k in lists]
         return rst
 
 pass
```

### Comparing `buildz-0.5.6/buildz/ioc/ioc_deal/map.py` & `buildz-0.5.7/buildz/ioc/ioc_deal/map.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,12 +24,12 @@
     """
     def init(self, fp_lists=None, fp_defaults=None):
         super().init("MapDeal", fp_lists, fp_defaults, join(dp, "conf", "map_lists.js"), None)
     def deal(self, edata:EncapeData):
         data = edata.data
         conf = edata.conf
         data = self.fill(data)
-        maps = xf.g(data, data={})
+        maps = xf.g1(data, map = {}, data={})
         rst = {k:self.get_obj(maps[k], conf, edata.src, edata.info) for k in maps}
         return rst
 
 pass
```

### Comparing `buildz-0.5.6/buildz/ioc/ioc_deal/mcall.py` & `buildz-0.5.7/buildz/ioc/ioc_deal/mcall.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/ioc/ioc_deal/obj.py` & `buildz-0.5.7/buildz/ioc/ioc_deal/obj.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,20 +132,25 @@
         if ids is not None:
             xf.sets(self.singles, ids, obj)
         prev_call = xf.g(data, prev_call=None)
         if prev_call is not None:
             # TODO: 这边info透传好像会有问题
             self.get_obj(prev_call, conf, obj, edata.info)
         sets = xf.g(data, sets=[])
-        for kv in sets:
-            kv = self.fmt_set(kv)
-            k = kv['key']
-            v = kv['data']
-            v = self.get_obj(v, conf, obj, edata.info)
-            setattr(obj, k, v)
+        if type(sets)==list:
+            for kv in sets:
+                kv = self.fmt_set(kv)
+                k = kv['key']
+                v = xf.get_first(kv, "val", "data")
+                v = self.get_obj(v, conf, obj, edata.info)
+                setattr(obj, k, v)
+        else:
+            for k,v in sets.items():
+                v = self.get_obj(v, conf, obj, edata.info)
+                setattr(obj, k, v)
         call = xf.g(data, call=None)
         if call is not None:
             self.get_obj(call, conf, obj, edata.info)
         return obj
     def remove(self, edata:EncapeData):
         sid = edata.sid
         data = edata.data
```

### Comparing `buildz-0.5.6/buildz/ioc/ioc_deal/ovar.py` & `buildz-0.5.7/buildz/ioc/ioc_deal/ovar.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/ioc/ioc_deal/ref.py` & `buildz-0.5.7/buildz/ioc/ioc_deal/ref.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             [ref, obj.test] // 数据项"obj.test"的引用
     """
     def init(self, fp_lists=None, fp_defaults=None):
         super().init("RefDeal", fp_lists, fp_defaults, join(dp, "conf", "ref_lists.js"), None)
     def deal(self, edata:EncapeData):
         data = edata.data
         data = self.fill(data)
-        key = data['key']
+        key = xf.get_first(data, 'ref', 'key')
         info = xf.g(data, info=None)
         if info is not None and type(info)==dict:
             #info = {k:self.get_obj(info, edata.conf, src = edata.src) for k in info}
             info = {'type':'map', 'data':info}
             info = self.get_obj(info, edata.conf, src = edata.src)
         return edata.conf.get_obj(key, info = info, src = edata.src)
```

### Comparing `buildz-0.5.6/buildz/ioc/ioc_deal/val.py` & `buildz-0.5.7/buildz/ioc/ioc_deal/val.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #
 from ..ioc.base import Base, EncapeData
-
+from buildz import xf
 class ValDeal(Base):
     """
         数据val:
             {
                 // 查找id，可选
                 id: id
                 type: val
@@ -20,10 +20,10 @@
         注: val是默认数据项的类型，如果data不是list或map，可以直接只写data：
             100元
     """
     def deal(self, edata:EncapeData):
         data = edata.data
         if type(data)==list:
             return data[-1]
-        return data['data']
+        return xf.get_first(data, "val", "data")
 
 pass
```

### Comparing `buildz-0.5.6/buildz/ioc/ioc_deal/var.py` & `buildz-0.5.7/buildz/ioc/ioc_deal/var.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/ioc/ioc_deal/xfile.py` & `buildz-0.5.7/buildz/ioc/ioc_deal/xfile.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/pyz.py` & `buildz-0.5.7/buildz/pyz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/tz/myers_diff.py` & `buildz-0.5.7/buildz/tz/myers_diff.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/file.py` & `buildz-0.5.7/buildz/xf/file.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loader/base.py` & `buildz-0.5.7/buildz/xf/loader/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loader/buffer.py` & `buildz-0.5.7/buildz/xf/loader/buffer.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loader/deal/listz.py` & `buildz-0.5.7/buildz/xf/loader/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loader/deal/lr.py` & `buildz-0.5.7/buildz/xf/loader/deal/lr.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loader/deal/lrval.py` & `buildz-0.5.7/buildz/xf/loader/deal/lrval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loader/deal/mapz.py` & `buildz-0.5.7/buildz/xf/loader/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loader/deal/nextz.py` & `buildz-0.5.7/buildz/xf/loader/deal/nextz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loader/deal/reval.py` & `buildz-0.5.7/buildz/xf/loader/deal/reval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loader/deal/setz.py` & `buildz-0.5.7/buildz/xf/loader/deal/setz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loader/deal/spt.py` & `buildz-0.5.7/buildz/xf/loader/deal/spt.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loader/deal/strz.py` & `buildz-0.5.7/buildz/xf/loader/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loader/item.py` & `buildz-0.5.7/buildz/xf/loader/item.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loader/mg.py` & `buildz-0.5.7/buildz/xf/loader/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loader/pos.py` & `buildz-0.5.7/buildz/xf/loader/pos.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loaderz/base.py` & `buildz-0.5.7/buildz/xf/loaderz/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loaderz/buffer.py` & `buildz-0.5.7/buildz/xf/loaderz/buffer.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loaderz/deal/listz.py` & `buildz-0.5.7/buildz/xf/loaderz/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loaderz/deal/lr.py` & `buildz-0.5.7/buildz/xf/loaderz/deal/lr.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loaderz/deal/lrval.py` & `buildz-0.5.7/buildz/xf/loaderz/deal/lrval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loaderz/deal/mapz.py` & `buildz-0.5.7/buildz/xf/loaderz/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loaderz/deal/nextz.py` & `buildz-0.5.7/buildz/xf/loaderz/deal/nextz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loaderz/deal/reval.py` & `buildz-0.5.7/buildz/xf/loaderz/deal/reval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loaderz/deal/spt.py` & `buildz-0.5.7/buildz/xf/loaderz/deal/spt.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loaderz/deal/strz.py` & `buildz-0.5.7/buildz/xf/loaderz/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loaderz/item.py` & `buildz-0.5.7/buildz/xf/loaderz/item.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loaderz/mg.py` & `buildz-0.5.7/buildz/xf/loaderz/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loaderz/pos.py` & `buildz-0.5.7/buildz/xf/loaderz/pos.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/loaderz/test.py` & `buildz-0.5.7/buildz/xf/loaderz/test.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/mapz.py` & `buildz-0.5.7/buildz/xf/mapz.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,143 +42,171 @@
 00000290: 2020 2020 2076 203d 206d 6170 735b 6b5d       v = maps[k]
 000002a0: 2829 0d0a 2020 2020 2020 2020 7273 742e  ()..        rst.
 000002b0: 6170 7065 6e64 2876 290d 0a20 2020 2069  append(v)..    i
 000002c0: 6620 6c65 6e28 7273 7429 3d3d 313a 0d0a  f len(rst)==1:..
 000002d0: 2020 2020 2020 2020 7273 7420 3d20 7273          rst = rs
 000002e0: 745b 305d 0d0a 2020 2020 7265 7475 726e  t[0]..    return
 000002f0: 2072 7374 0d0a 0d0a 7061 7373 0d0a 6465   rst....pass..de
-00000300: 6620 6728 6f62 6a2c 202a 2a6d 6170 7329  f g(obj, **maps)
-00000310: 3a0d 0a20 2020 2072 7374 203d 205b 5d0d  :..    rst = [].
-00000320: 0a20 2020 2066 6f72 206b 2069 6e20 6d61  .    for k in ma
-00000330: 7073 3a0d 0a20 2020 2020 2020 2076 203d  ps:..        v =
-00000340: 206d 6170 735b 6b5d 0d0a 2020 2020 2020   maps[k]..      
-00000350: 2020 6966 206b 2069 6e20 6f62 6a3a 0d0a    if k in obj:..
-00000360: 2020 2020 2020 2020 2020 2020 7620 3d20              v = 
-00000370: 6f62 6a5b 6b5d 0d0a 2020 2020 2020 2020  obj[k]..        
-00000380: 7273 742e 6170 7065 6e64 2876 290d 0a20  rst.append(v).. 
-00000390: 2020 2069 6620 6c65 6e28 7273 7429 3d3d     if len(rst)==
-000003a0: 313a 0d0a 2020 2020 2020 2020 7273 7420  1:..        rst 
-000003b0: 3d20 7273 745b 305d 0d0a 2020 2020 7265  = rst[0]..    re
-000003c0: 7475 726e 2072 7374 0d0a 0d0a 7061 7373  turn rst....pass
-000003d0: 0d0a 6465 6620 6773 286f 626a 2c20 2a2a  ..def gs(obj, **
-000003e0: 6d61 7073 293a 0d0a 2020 2020 7273 7420  maps):..    rst 
-000003f0: 3d20 5b5d 0d0a 2020 2020 666f 7220 6b20  = []..    for k 
-00000400: 696e 206d 6170 733a 0d0a 2020 2020 2020  in maps:..      
-00000410: 2020 7620 3d20 6d61 7073 5b6b 5d0d 0a20    v = maps[k].. 
-00000420: 2020 2020 2020 2069 6620 6b20 696e 206f         if k in o
-00000430: 626a 3a0d 0a20 2020 2020 2020 2020 2020  bj:..           
-00000440: 2076 203d 206f 626a 5b6b 5d0d 0a20 2020   v = obj[k]..   
-00000450: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00000460: 2020 2020 2020 2020 6f62 6a5b 6b5d 203d          obj[k] =
-00000470: 2076 0d0a 2020 2020 2020 2020 7273 742e   v..        rst.
-00000480: 6170 7065 6e64 2876 290d 0a20 2020 2069  append(v)..    i
-00000490: 6620 6c65 6e28 7273 7429 3d3d 313a 0d0a  f len(rst)==1:..
-000004a0: 2020 2020 2020 2020 7273 7420 3d20 7273          rst = rs
-000004b0: 745b 305d 0d0a 2020 2020 7265 7475 726e  t[0]..    return
-000004c0: 2072 7374 0d0a 0d0a 7061 7373 0d0a 6465   rst....pass..de
-000004d0: 6620 7328 6f62 6a2c 202a 2a6d 6170 7329  f s(obj, **maps)
-000004e0: 3a0d 0a20 2020 2066 6f72 206b 2069 6e20  :..    for k in 
-000004f0: 6d61 7073 3a0d 0a20 2020 2020 2020 2076  maps:..        v
-00000500: 203d 206d 6170 735b 6b5d 0d0a 2020 2020   = maps[k]..    
-00000510: 2020 2020 6f62 6a5b 6b5d 203d 2076 0d0a      obj[k] = v..
-00000520: 0d0a 7061 7373 0d0a 6465 6620 7365 7473  ..pass..def sets
-00000530: 286d 6170 732c 206b 6579 732c 2076 616c  (maps, keys, val
-00000540: 293a 0d0a 2020 2020 6966 2074 7970 6528  ):..    if type(
-00000550: 6b65 7973 2920 213d 206c 6973 743a 0d0a  keys) != list:..
-00000560: 2020 2020 2020 2020 6b65 7973 203d 205b          keys = [
-00000570: 6b65 7973 5d0d 0a20 2020 2066 6f72 206b  keys]..    for k
-00000580: 6579 2069 6e20 6b65 7973 5b3a 2d31 5d3a  ey in keys[:-1]:
-00000590: 0d0a 2020 2020 2020 2020 6966 206b 6579  ..        if key
-000005a0: 206e 6f74 2069 6e20 6d61 7073 3a0d 0a20   not in maps:.. 
-000005b0: 2020 2020 2020 2020 2020 206d 6170 735b             maps[
-000005c0: 6b65 795d 203d 207b 7d0d 0a20 2020 2020  key] = {}..     
-000005d0: 2020 206d 6170 7320 3d20 6d61 7073 5b6b     maps = maps[k
-000005e0: 6579 5d0d 0a20 2020 206d 6170 735b 6b65  ey]..    maps[ke
-000005f0: 7973 5b2d 315d 5d20 3d20 7661 6c0d 0a0d  ys[-1]] = val...
-00000600: 0a70 6173 730d 0a64 6566 2067 6574 7328  .pass..def gets(
-00000610: 6d61 7073 2c20 6b65 7973 2c20 6465 6661  maps, keys, defa
-00000620: 756c 7420 3d20 4e6f 6e65 293a 0d0a 2020  ult = None):..  
-00000630: 2020 6966 2074 7970 6528 6b65 7973 2920    if type(keys) 
-00000640: 213d 206c 6973 743a 0d0a 2020 2020 2020  != list:..      
-00000650: 2020 6b65 7973 203d 205b 6b65 7973 5d0d    keys = [keys].
-00000660: 0a20 2020 2066 6f72 206b 6579 2069 6e20  .    for key in 
-00000670: 6b65 7973 3a0d 0a20 2020 2020 2020 2069  keys:..        i
-00000680: 6620 6b65 7920 6e6f 7420 696e 206d 6170  f key not in map
-00000690: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-000006a0: 7265 7475 726e 2064 6566 6175 6c74 0d0a  return default..
-000006b0: 2020 2020 2020 2020 6d61 7073 203d 206d          maps = m
-000006c0: 6170 735b 6b65 795d 0d0a 2020 2020 7265  aps[key]..    re
-000006d0: 7475 726e 206d 6170 730d 0a0d 0a70 6173  turn maps....pas
-000006e0: 730d 0a64 6566 2072 656d 6f76 6573 286d  s..def removes(m
-000006f0: 6170 732c 206b 6579 7329 3a0d 0a20 2020  aps, keys):..   
-00000700: 2069 6620 7479 7065 286b 6579 7329 2021   if type(keys) !
-00000710: 3d20 6c69 7374 3a0d 0a20 2020 2020 2020  = list:..       
-00000720: 206b 6579 7320 3d20 5b6b 6579 735d 0d0a   keys = [keys]..
-00000730: 2020 2020 6172 7220 3d20 5b5d 0d0a 2020      arr = []..  
-00000740: 2020 666f 7220 6b65 7920 696e 206b 6579    for key in key
-00000750: 733a 0d0a 2020 2020 2020 2020 6966 206b  s:..        if k
-00000760: 6579 206e 6f74 2069 6e20 6d61 7073 3a0d  ey not in maps:.
-00000770: 0a20 2020 2020 2020 2020 2020 2062 7265  .            bre
-00000780: 616b 0d0a 2020 2020 2020 2020 6172 722e  ak..        arr.
-00000790: 6170 7065 6e64 285b 6d61 7073 2c20 6b65  append([maps, ke
-000007a0: 795d 290d 0a20 2020 2020 2020 206d 6170  y])..        map
-000007b0: 7320 3d20 6d61 7073 5b6b 6579 5d0d 0a20  s = maps[key].. 
-000007c0: 2020 2061 7272 2e72 6576 6572 7365 2829     arr.reverse()
-000007d0: 0d0a 2020 2020 6669 7273 743d 310d 0a20  ..    first=1.. 
-000007e0: 2020 2066 6f72 206d 6170 732c 6b65 7920     for maps,key 
-000007f0: 696e 2061 7272 3a0d 0a20 2020 2020 2020  in arr:..       
-00000800: 2069 6620 6669 7273 7420 6f72 206c 656e   if first or len
-00000810: 286d 6170 735b 6b65 795d 293d 3d30 3a0d  (maps[key])==0:.
-00000820: 0a20 2020 2020 2020 2020 2020 2064 656c  .            del
-00000830: 206d 6170 735b 6b65 795d 0d0a 2020 2020   maps[key]..    
-00000840: 2020 2020 6669 7273 743d 300d 0a20 2020      first=0..   
-00000850: 2072 6574 7572 6e20 4e6f 6e65 0d0a 0d0a   return None....
-00000860: 7061 7373 0d0a 6465 6620 6c32 6d28 6172  pass..def l2m(ar
-00000870: 722c 202a 2a6d 6170 7329 3a0d 0a20 2020  r, **maps):..   
-00000880: 2072 7374 203d 207b 7d0d 0a20 2020 2069   rst = {}..    i
-00000890: 203d 2030 0d0a 2020 2020 666f 7220 6b20   = 0..    for k 
-000008a0: 696e 206d 6170 733a 0d0a 2020 2020 2020  in maps:..      
-000008b0: 2020 6966 2069 3c6c 656e 2861 7272 293a    if i<len(arr):
-000008c0: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
-000008d0: 6c20 3d20 6172 725b 695d 0d0a 2020 2020  l = arr[i]..    
-000008e0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-000008f0: 2020 2020 2020 2076 616c 203d 206d 6170         val = map
-00000900: 735b 6b5d 0d0a 2020 2020 2020 2020 7273  s[k]..        rs
-00000910: 745b 6b5d 203d 2076 616c 0d0a 2020 2020  t[k] = val..    
-00000920: 2020 2020 692b 3d31 0d0a 2020 2020 7265      i+=1..    re
-00000930: 7475 726e 2072 7374 0d0a 0d0a 7061 7373  turn rst....pass
-00000940: 0d0a 0d0a 6465 6620 6465 6570 5f75 7064  ....def deep_upd
-00000950: 6174 6528 7461 7267 6574 2c20 7372 632c  ate(target, src,
-00000960: 2072 6570 6c61 6365 3d31 293a 0d0a 2020   replace=1):..  
-00000970: 2020 2222 220d 0a20 2020 2020 2020 2064    """..        d
-00000980: 6963 74e6 b7b1 e5b1 82e6 9bb4 e696 b0ef  ict.............
-00000990: bc8c 7372 635b 6b65 795d e698 af64 6963  ..src[key]...dic
-000009a0: 74e5 b0b1 e6b7 b1e5 85a5 e69b b4e6 96b0  t...............
-000009b0: efbc 8ce5 90a6 e588 993a 0d0a 2020 2020  .........:..    
-000009c0: 2020 2020 2020 2020 7372 63e6 9c89 e880          src.....
-000009d0: 8c74 6172 6765 74e6 b2a1 e69c 89e5 b0b1  .target.........
-000009e0: e69b bfe6 8da2 efbc 8ce5 90a6 e588 99ef  ................
-000009f0: bc9a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00000a00: 2020 2020 7265 706c 6163 653d 31e5 b0b1      replace=1...
-00000a10: e69b bfe6 8da2 0d0a 2020 2020 2222 220d  ........    """.
-00000a20: 0a20 2020 2066 6f72 206b 2069 6e20 7372  .    for k in sr
-00000a30: 633a 0d0a 2020 2020 2020 2020 7661 6c20  c:..        val 
-00000a40: 3d20 7372 635b 6b5d 0d0a 2020 2020 2020  = src[k]..      
-00000a50: 2020 6966 206b 206e 6f74 2069 6e20 7461    if k not in ta
-00000a60: 7267 6574 3a0d 0a20 2020 2020 2020 2020  rget:..         
-00000a70: 2020 2074 6172 6765 745b 6b5d 203d 2076     target[k] = v
-00000a80: 616c 0d0a 2020 2020 2020 2020 2020 2020  al..            
-00000a90: 636f 6e74 696e 7565 0d0a 2020 2020 2020  continue..      
-00000aa0: 2020 6d76 616c 203d 2074 6172 6765 745b    mval = target[
-00000ab0: 6b5d 0d0a 2020 2020 2020 2020 6966 2074  k]..        if t
-00000ac0: 7970 6528 6d76 616c 2920 3d3d 2064 6963  ype(mval) == dic
-00000ad0: 7420 616e 6420 7479 7065 2876 616c 293d  t and type(val)=
-00000ae0: 3d64 6963 743a 0d0a 2020 2020 2020 2020  =dict:..        
-00000af0: 2020 2020 6465 6570 5f75 7064 6174 6528      deep_update(
-00000b00: 6d76 616c 2c20 7661 6c2c 2072 6570 6c61  mval, val, repla
-00000b10: 6365 290d 0a20 2020 2020 2020 2065 6c73  ce)..        els
-00000b20: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00000b30: 6966 2072 6570 6c61 6365 3a0d 0a20 2020  if replace:..   
-00000b40: 2020 2020 2020 2020 2020 2020 2074 6172               tar
-00000b50: 6765 745b 6b5d 203d 2076 616c 0d0a 0d0a  get[k] = val....
-00000b60: 7061 7373 0d0a 7570 6461 7465 203d 2064  pass..update = d
-00000b70: 6565 705f 7570 6461 7465 0d0a            eep_update..
+00000300: 6620 6765 745f 6669 7273 7428 6f62 6a2c  f get_first(obj,
+00000310: 202a 6b65 7973 293a 0d0a 2020 2020 666f   *keys):..    fo
+00000320: 7220 6b20 696e 206b 6579 733a 0d0a 2020  r k in keys:..  
+00000330: 2020 2020 2020 6966 206b 2069 6e20 6f62        if k in ob
+00000340: 6a3a 0d0a 2020 2020 2020 2020 2020 2020  j:..            
+00000350: 7265 7475 726e 206f 626a 5b6b 5d0d 0a20  return obj[k].. 
+00000360: 2020 2072 6169 7365 204b 6579 4572 726f     raise KeyErro
+00000370: 7228 6b65 7973 5b30 5d29 0d0a 0d0a 7061  r(keys[0])....pa
+00000380: 7373 0d0a 6465 6620 6765 745f 6f6e 6528  ss..def get_one(
+00000390: 6f62 6a2c 206b 6579 732c 2064 6566 6175  obj, keys, defau
+000003a0: 6c74 203d 204e 6f6e 6529 3a0d 0a20 2020  lt = None):..   
+000003b0: 2066 6f72 206b 2069 6e20 6b65 7973 3a0d   for k in keys:.
+000003c0: 0a20 2020 2020 2020 2069 6620 6b20 696e  .        if k in
+000003d0: 206f 626a 3a0d 0a20 2020 2020 2020 2020   obj:..         
+000003e0: 2020 2072 6574 7572 6e20 6f62 6a5b 6b5d     return obj[k]
+000003f0: 0d0a 2020 2020 7265 7475 726e 2064 6566  ..    return def
+00000400: 6175 6c74 0d0a 0d0a 7061 7373 0d0a 6465  ault....pass..de
+00000410: 6620 6731 286f 626a 2c20 2a2a 6d61 7073  f g1(obj, **maps
+00000420: 293a 0d0a 2020 2020 7620 3d20 4e6f 6e65  ):..    v = None
+00000430: 0d0a 2020 2020 666f 7220 6b20 696e 206d  ..    for k in m
+00000440: 6170 733a 0d0a 2020 2020 2020 2020 7620  aps:..        v 
+00000450: 3d20 6d61 7073 5b6b 5d0d 0a20 2020 2020  = maps[k]..     
+00000460: 2020 2069 6620 6b20 696e 206f 626a 3a0d     if k in obj:.
+00000470: 0a20 2020 2020 2020 2020 2020 2076 203d  .            v =
+00000480: 206f 626a 5b6b 5d0d 0a20 2020 2020 2020   obj[k]..       
+00000490: 2020 2020 2072 6574 7572 6e20 760d 0a20       return v.. 
+000004a0: 2020 2072 6574 7572 6e20 760d 0a0d 0a70     return v....p
+000004b0: 6173 730d 0a64 6566 2067 286f 626a 2c20  ass..def g(obj, 
+000004c0: 2a2a 6d61 7073 293a 0d0a 2020 2020 7273  **maps):..    rs
+000004d0: 7420 3d20 5b5d 0d0a 2020 2020 666f 7220  t = []..    for 
+000004e0: 6b20 696e 206d 6170 733a 0d0a 2020 2020  k in maps:..    
+000004f0: 2020 2020 7620 3d20 6d61 7073 5b6b 5d0d      v = maps[k].
+00000500: 0a20 2020 2020 2020 2069 6620 6b20 696e  .        if k in
+00000510: 206f 626a 3a0d 0a20 2020 2020 2020 2020   obj:..         
+00000520: 2020 2076 203d 206f 626a 5b6b 5d0d 0a20     v = obj[k].. 
+00000530: 2020 2020 2020 2072 7374 2e61 7070 656e         rst.appen
+00000540: 6428 7629 0d0a 2020 2020 6966 206c 656e  d(v)..    if len
+00000550: 2872 7374 293d 3d31 3a0d 0a20 2020 2020  (rst)==1:..     
+00000560: 2020 2072 7374 203d 2072 7374 5b30 5d0d     rst = rst[0].
+00000570: 0a20 2020 2072 6574 7572 6e20 7273 740d  .    return rst.
+00000580: 0a0d 0a70 6173 730d 0a64 6566 2067 7328  ...pass..def gs(
+00000590: 6f62 6a2c 202a 2a6d 6170 7329 3a0d 0a20  obj, **maps):.. 
+000005a0: 2020 2072 7374 203d 205b 5d0d 0a20 2020     rst = []..   
+000005b0: 2066 6f72 206b 2069 6e20 6d61 7073 3a0d   for k in maps:.
+000005c0: 0a20 2020 2020 2020 2076 203d 206d 6170  .        v = map
+000005d0: 735b 6b5d 0d0a 2020 2020 2020 2020 6966  s[k]..        if
+000005e0: 206b 2069 6e20 6f62 6a3a 0d0a 2020 2020   k in obj:..    
+000005f0: 2020 2020 2020 2020 7620 3d20 6f62 6a5b          v = obj[
+00000600: 6b5d 0d0a 2020 2020 2020 2020 656c 7365  k]..        else
+00000610: 3a0d 0a20 2020 2020 2020 2020 2020 206f  :..            o
+00000620: 626a 5b6b 5d20 3d20 760d 0a20 2020 2020  bj[k] = v..     
+00000630: 2020 2072 7374 2e61 7070 656e 6428 7629     rst.append(v)
+00000640: 0d0a 2020 2020 6966 206c 656e 2872 7374  ..    if len(rst
+00000650: 293d 3d31 3a0d 0a20 2020 2020 2020 2072  )==1:..        r
+00000660: 7374 203d 2072 7374 5b30 5d0d 0a20 2020  st = rst[0]..   
+00000670: 2072 6574 7572 6e20 7273 740d 0a0d 0a70   return rst....p
+00000680: 6173 730d 0a64 6566 2073 286f 626a 2c20  ass..def s(obj, 
+00000690: 2a2a 6d61 7073 293a 0d0a 2020 2020 666f  **maps):..    fo
+000006a0: 7220 6b20 696e 206d 6170 733a 0d0a 2020  r k in maps:..  
+000006b0: 2020 2020 2020 7620 3d20 6d61 7073 5b6b        v = maps[k
+000006c0: 5d0d 0a20 2020 2020 2020 206f 626a 5b6b  ]..        obj[k
+000006d0: 5d20 3d20 760d 0a0d 0a70 6173 730d 0a64  ] = v....pass..d
+000006e0: 6566 2073 6574 7328 6d61 7073 2c20 6b65  ef sets(maps, ke
+000006f0: 7973 2c20 7661 6c29 3a0d 0a20 2020 2069  ys, val):..    i
+00000700: 6620 7479 7065 286b 6579 7329 2021 3d20  f type(keys) != 
+00000710: 6c69 7374 3a0d 0a20 2020 2020 2020 206b  list:..        k
+00000720: 6579 7320 3d20 5b6b 6579 735d 0d0a 2020  eys = [keys]..  
+00000730: 2020 666f 7220 6b65 7920 696e 206b 6579    for key in key
+00000740: 735b 3a2d 315d 3a0d 0a20 2020 2020 2020  s[:-1]:..       
+00000750: 2069 6620 6b65 7920 6e6f 7420 696e 206d   if key not in m
+00000760: 6170 733a 0d0a 2020 2020 2020 2020 2020  aps:..          
+00000770: 2020 6d61 7073 5b6b 6579 5d20 3d20 7b7d    maps[key] = {}
+00000780: 0d0a 2020 2020 2020 2020 6d61 7073 203d  ..        maps =
+00000790: 206d 6170 735b 6b65 795d 0d0a 2020 2020   maps[key]..    
+000007a0: 6d61 7073 5b6b 6579 735b 2d31 5d5d 203d  maps[keys[-1]] =
+000007b0: 2076 616c 0d0a 0d0a 7061 7373 0d0a 6465   val....pass..de
+000007c0: 6620 6765 7473 286d 6170 732c 206b 6579  f gets(maps, key
+000007d0: 732c 2064 6566 6175 6c74 203d 204e 6f6e  s, default = Non
+000007e0: 6529 3a0d 0a20 2020 2069 6620 7479 7065  e):..    if type
+000007f0: 286b 6579 7329 2021 3d20 6c69 7374 3a0d  (keys) != list:.
+00000800: 0a20 2020 2020 2020 206b 6579 7320 3d20  .        keys = 
+00000810: 5b6b 6579 735d 0d0a 2020 2020 666f 7220  [keys]..    for 
+00000820: 6b65 7920 696e 206b 6579 733a 0d0a 2020  key in keys:..  
+00000830: 2020 2020 2020 6966 206b 6579 206e 6f74        if key not
+00000840: 2069 6e20 6d61 7073 3a0d 0a20 2020 2020   in maps:..     
+00000850: 2020 2020 2020 2072 6574 7572 6e20 6465         return de
+00000860: 6661 756c 740d 0a20 2020 2020 2020 206d  fault..        m
+00000870: 6170 7320 3d20 6d61 7073 5b6b 6579 5d0d  aps = maps[key].
+00000880: 0a20 2020 2072 6574 7572 6e20 6d61 7073  .    return maps
+00000890: 0d0a 0d0a 7061 7373 0d0a 6465 6620 7265  ....pass..def re
+000008a0: 6d6f 7665 7328 6d61 7073 2c20 6b65 7973  moves(maps, keys
+000008b0: 293a 0d0a 2020 2020 6966 2074 7970 6528  ):..    if type(
+000008c0: 6b65 7973 2920 213d 206c 6973 743a 0d0a  keys) != list:..
+000008d0: 2020 2020 2020 2020 6b65 7973 203d 205b          keys = [
+000008e0: 6b65 7973 5d0d 0a20 2020 2061 7272 203d  keys]..    arr =
+000008f0: 205b 5d0d 0a20 2020 2066 6f72 206b 6579   []..    for key
+00000900: 2069 6e20 6b65 7973 3a0d 0a20 2020 2020   in keys:..     
+00000910: 2020 2069 6620 6b65 7920 6e6f 7420 696e     if key not in
+00000920: 206d 6170 733a 0d0a 2020 2020 2020 2020   maps:..        
+00000930: 2020 2020 6272 6561 6b0d 0a20 2020 2020      break..     
+00000940: 2020 2061 7272 2e61 7070 656e 6428 5b6d     arr.append([m
+00000950: 6170 732c 206b 6579 5d29 0d0a 2020 2020  aps, key])..    
+00000960: 2020 2020 6d61 7073 203d 206d 6170 735b      maps = maps[
+00000970: 6b65 795d 0d0a 2020 2020 6172 722e 7265  key]..    arr.re
+00000980: 7665 7273 6528 290d 0a20 2020 2066 6972  verse()..    fir
+00000990: 7374 3d31 0d0a 2020 2020 666f 7220 6d61  st=1..    for ma
+000009a0: 7073 2c6b 6579 2069 6e20 6172 723a 0d0a  ps,key in arr:..
+000009b0: 2020 2020 2020 2020 6966 2066 6972 7374          if first
+000009c0: 206f 7220 6c65 6e28 6d61 7073 5b6b 6579   or len(maps[key
+000009d0: 5d29 3d3d 303a 0d0a 2020 2020 2020 2020  ])==0:..        
+000009e0: 2020 2020 6465 6c20 6d61 7073 5b6b 6579      del maps[key
+000009f0: 5d0d 0a20 2020 2020 2020 2066 6972 7374  ]..        first
+00000a00: 3d30 0d0a 2020 2020 7265 7475 726e 204e  =0..    return N
+00000a10: 6f6e 650d 0a0d 0a70 6173 730d 0a64 6566  one....pass..def
+00000a20: 206c 326d 2861 7272 2c20 2a2a 6d61 7073   l2m(arr, **maps
+00000a30: 293a 0d0a 2020 2020 7273 7420 3d20 7b7d  ):..    rst = {}
+00000a40: 0d0a 2020 2020 6920 3d20 300d 0a20 2020  ..    i = 0..   
+00000a50: 2066 6f72 206b 2069 6e20 6d61 7073 3a0d   for k in maps:.
+00000a60: 0a20 2020 2020 2020 2069 6620 693c 6c65  .        if i<le
+00000a70: 6e28 6172 7229 3a0d 0a20 2020 2020 2020  n(arr):..       
+00000a80: 2020 2020 2076 616c 203d 2061 7272 5b69       val = arr[i
+00000a90: 5d0d 0a20 2020 2020 2020 2065 6c73 653a  ]..        else:
+00000aa0: 0d0a 2020 2020 2020 2020 2020 2020 7661  ..            va
+00000ab0: 6c20 3d20 6d61 7073 5b6b 5d0d 0a20 2020  l = maps[k]..   
+00000ac0: 2020 2020 2072 7374 5b6b 5d20 3d20 7661       rst[k] = va
+00000ad0: 6c0d 0a20 2020 2020 2020 2069 2b3d 310d  l..        i+=1.
+00000ae0: 0a20 2020 2072 6574 7572 6e20 7273 740d  .    return rst.
+00000af0: 0a0d 0a70 6173 730d 0a0d 0a64 6566 2064  ...pass....def d
+00000b00: 6565 705f 7570 6461 7465 2874 6172 6765  eep_update(targe
+00000b10: 742c 2073 7263 2c20 7265 706c 6163 653d  t, src, replace=
+00000b20: 3129 3a0d 0a20 2020 2022 2222 0d0a 2020  1):..    """..  
+00000b30: 2020 2020 2020 6469 6374 e6b7 b1e5 b182        dict......
+00000b40: e69b b4e6 96b0 efbc 8c73 7263 5b6b 6579  .........src[key
+00000b50: 5de6 98af 6469 6374 e5b0 b1e6 b7b1 e585  ]...dict........
+00000b60: a5e6 9bb4 e696 b0ef bc8c e590 a6e5 8899  ................
+00000b70: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00000b80: 7263 e69c 89e8 808c 7461 7267 6574 e6b2  rc......target..
+00000b90: a1e6 9c89 e5b0 b1e6 9bbf e68d a2ef bc8c  ................
+00000ba0: e590 a6e5 8899 efbc 9a0d 0a20 2020 2020  ...........     
+00000bb0: 2020 2020 2020 2020 2020 2072 6570 6c61             repla
+00000bc0: 6365 3d31 e5b0 b1e6 9bbf e68d a20d 0a20  ce=1........... 
+00000bd0: 2020 2022 2222 0d0a 2020 2020 666f 7220     """..    for 
+00000be0: 6b20 696e 2073 7263 3a0d 0a20 2020 2020  k in src:..     
+00000bf0: 2020 2076 616c 203d 2073 7263 5b6b 5d0d     val = src[k].
+00000c00: 0a20 2020 2020 2020 2069 6620 6b20 6e6f  .        if k no
+00000c10: 7420 696e 2074 6172 6765 743a 0d0a 2020  t in target:..  
+00000c20: 2020 2020 2020 2020 2020 7461 7267 6574            target
+00000c30: 5b6b 5d20 3d20 7661 6c0d 0a20 2020 2020  [k] = val..     
+00000c40: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
+00000c50: 0a20 2020 2020 2020 206d 7661 6c20 3d20  .        mval = 
+00000c60: 7461 7267 6574 5b6b 5d0d 0a20 2020 2020  target[k]..     
+00000c70: 2020 2069 6620 7479 7065 286d 7661 6c29     if type(mval)
+00000c80: 203d 3d20 6469 6374 2061 6e64 2074 7970   == dict and typ
+00000c90: 6528 7661 6c29 3d3d 6469 6374 3a0d 0a20  e(val)==dict:.. 
+00000ca0: 2020 2020 2020 2020 2020 2064 6565 705f             deep_
+00000cb0: 7570 6461 7465 286d 7661 6c2c 2076 616c  update(mval, val
+00000cc0: 2c20 7265 706c 6163 6529 0d0a 2020 2020  , replace)..    
+00000cd0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00000ce0: 2020 2020 2020 2069 6620 7265 706c 6163         if replac
+00000cf0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00000d00: 2020 2020 7461 7267 6574 5b6b 5d20 3d20      target[k] = 
+00000d10: 7661 6c0d 0a0d 0a70 6173 730d 0a75 7064  val....pass..upd
+00000d20: 6174 6520 3d20 6465 6570 5f75 7064 6174  ate = deep_updat
+00000d30: 650d 0a                                  e..
```

### Comparing `buildz-0.5.6/buildz/xf/read.py` & `buildz-0.5.7/buildz/xf/read.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/readz.py` & `buildz-0.5.7/buildz/xf/readz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/stack.py` & `buildz-0.5.7/buildz/xf/stack.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/write.py` & `buildz-0.5.7/buildz/xf/write.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/writer/base.py` & `buildz-0.5.7/buildz/xf/writer/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/writer/conf.py` & `buildz-0.5.7/buildz/xf/writer/conf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/writer/deal/listz.py` & `buildz-0.5.7/buildz/xf/writer/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/writer/deal/mapz.py` & `buildz-0.5.7/buildz/xf/writer/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/writer/deal/strz.py` & `buildz-0.5.7/buildz/xf/writer/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/writer/itemz.py` & `buildz-0.5.7/buildz/xf/writer/itemz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/writer/mg.py` & `buildz-0.5.7/buildz/xf/writer/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz/xf/xargs.py` & `buildz-0.5.7/buildz/xf/xargs.py`

 * *Files identical despite different names*

### Comparing `buildz-0.5.6/buildz.egg-info/PKG-INFO` & `buildz-0.5.7/buildz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.5.6
+Version: 0.5.7
 Summary: 配置读写（基于json格式进行简化），以及ioc。a json-base file format's read and write code by python, and codes to read and product object from configure file in such format(ioc)
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
```

### Comparing `buildz-0.5.6/buildz.egg-info/SOURCES.txt` & `buildz-0.5.7/buildz.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 buildz/fz/lsf.py
 buildz/ioc/__init__.py
 buildz/ioc/base.py
 buildz/ioc/init.py
 buildz/ioc/ioc/base.py
 buildz/ioc/ioc/conf.py
 buildz/ioc/ioc/confs.py
+buildz/ioc/ioc/single.py
 buildz/ioc/ioc_deal/base.py
 buildz/ioc/ioc_deal/call.py
 buildz/ioc/ioc_deal/calls.py
 buildz/ioc/ioc_deal/deal.py
 buildz/ioc/ioc_deal/demo.py
 buildz/ioc/ioc_deal/env.py
 buildz/ioc/ioc_deal/ioc.py
```

### Comparing `buildz-0.5.6/setup.py` & `buildz-0.5.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Author: Zzz(1309458652@qq.com)
 # Description:
 
 from setuptools import setup, find_packages
 
 setup(
     name = 'buildz',
-    version = '0.5.6',
+    version = '0.5.7',
     keywords='buildz',
     long_description=open('README.md', 'r', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     description = "配置读写（基于json格式进行简化），以及ioc。a json-base file format's read and write code by python, and codes to read and product object from configure file in such format(ioc)",
     license = 'Apache License 2.0',
     url = 'https://github.com/buildCodeZ/buildz',
     author = 'Zzz',
```

